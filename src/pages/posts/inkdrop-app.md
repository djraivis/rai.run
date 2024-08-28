---
description: to use it as a CMS for my blog posts
slug: inkdrop-app
public: true
URL: inkdrop
layout: ../../layouts/BlogPost.astro
title: Integrating Inkdrop
createdAt: 1696446320561
updatedAt: 1724859060899
tags: []
heroImage: /posts/inkdrop-app_thumbnail.jpg
---

Connecting this was a bit challenging, but I received excellent support from the developer, Takuya Matsuyama, who is the owner of this app. Find out more on [Inkdrops forum support.](https://forum.inkdrop.app/t/impossible-to-connect-live-export/4147/3)

![thumbnail](/posts/inkdrop-app_thumbnail.png)

![CleanShot 2024-03-10 at 10 .14.59@2x](/posts/inkdrop-app_clean-shot-2024-03-10-at-10-14-59-2-x.jpg)


I've compiled a list of valuable notes for initiating and enabling logging, helpful tips to address similar challenges should you encounter them.

### Start localhost:3000
```zsh
yarn start 
```

### To link inkdrop db
```zsh
yarn run live-import
```

![123](/posts/inkdrop-app_123.gif)


Before setting up anything I was running into an errors

## Local HTTP server not working
![not-iterable](/posts/inkdrop-app_not-iterable.png)

## --enable-logging 
```zsh
/Applications/Inkdrop.app/Contents/MacOS/Inkdrop --enable-logging
```

![CleanShot 2023-10-04 at 8 .55.28@2x](/posts/inkdrop-app_clean-shot-2023-10-04-at-8-55-28-2-x.png)
Enable debug logs: [https://github.com/inkdropapp/inkdrop-live-export#debugging 2](https://github.com/inkdropapp/inkdrop-live-export#debugging)


### Connect/Test
```zsh
curl -v http://<USERNAME>:<PASSWORD>@localhost:19840
```

![username](/posts/inkdrop-app_username.png)
How to specify book ID: [GitHub - inkdropapp/inkdrop-live-export: A library for programmatically exporting notes to local filesystem from Inkdrop 1](https://github.com/inkdropapp/inkdrop-live-export#install-dev-tools-plugin)


### Live Export installation
```zsh
npm i -D @inkdropapp/live-export
yarn add -D @inkdropapp/live-export dotenv
```

### ipm-beta
```zsh
ipm-beta install dev-tools
```

### What is [CSON](https://github.com/bevry/cson#what-is-cson)
```zsh
~/Library/Application Support/inkdrop/
```

### Inkdrop Desktop [v5.6.0 beta.3](https://forum.inkdrop.app/t/inkdrop-desktop-v5-6-0-beta-3/4195) is released.


Installation on Inkdrop
This needs to included in .env file in the project

```js
DEBUG="inkdrop:export:info,inkdrop:export:error"
DEBUG='*'
INKDROP_USERNAME="username"
INKDROP_PASSWORD="password"
INKDROP_PORT=19840
INKDROP_BOOKID="book:bookID"
```

This needs to be added in the below file
```json
   "server": {
        "auth": {
          "password": "password",
          "username": "username"
        },
        "bindAddress": "127.0.0.1",
        "enabled": true,
        "port": 19840
      }
```

### Inkdrop Application Support Json File
```json
{
  "*": {
    "core": {
      "db": {
         "machineId": "machineID"
      },
      "lastNavigationState": {
        "editingNoteId": "note:noteID",
        "queryContext": {
          "bookId": "book:bookID",
          "filterKeyword": "",
          "includeChildren": false,
          "mode": "book",
          "sort": [
            {
              "pinned": "desc"
            },
            {
              "updatedAt": "desc"
            }
          ]
        },
        "sidebar": {
          "workspace": {
            "visible": false
          }
        }
      },
      "mainWindow": {
        "fullscreen": false,
        "maximized": false,
        "position": {
          "x": 193,
          "y": -1232
        },
        "sideBar": {
          "collapsedBooks": [
            "book:4ulSioEn-"
          ]
        },
        "size": {
          "h": 964,
          "w": 1372
        }
      },
      "server": {
        "auth": {
          "password": "password",
          "username": "username"
        },
        "bindAddress": "127.0.0.1",
        "enabled": true,
        "port": 19840
      }
    },
    "editor": {
      "fontSize": 11,
      "viewMode": "edit"
    }
  }
}

```

### [Configurations](https://developers.inkdrop.app/guides/access-the-local-database#configurations)

- `core.server.enabled` - Specify `true` to enable the HTTP server. Default is `false`.
- `core.server.port` - Defines the port number to listen. Default is `19840`.
- `core.server.bindAddress` - Defines the IP address to listen. Default is `127.0.0.1`.
- `core.server.auth.{username,password}` - Defines Basic auth credentials.

###

1. <https://github.com/inkdropapp/inkdrop-live-export#install-dev-tools-plugin>
2. <https://developers.inkdrop.app/guides/access-the-local-database#accessing-via-http-advanced>
3. <https://docs.inkdrop.app/reference/user-data-directory>
4. <https://my.inkdrop.app/plugins/dev-tools>
