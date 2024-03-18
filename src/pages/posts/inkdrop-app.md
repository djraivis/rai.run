---
description: to use it as a CMS for my blog posts
slug: inkdrop-app
public: true
URL: inkdrop
layout: ../../layouts/BlogPost.astro
title: Integrating Inkdrop
createdAt: 1696446320561
updatedAt: 1710370603862
tags: []
heroImage: /posts/inkdrop-app_thumbnail.jpg
---

Connecting this was a bit challenging, but I received excellent support from the developer, Takuya Matsuyama, who is the owner of this app. Find out more on [Inkdrops forum support.](https://forum.inkdrop.app/t/impossible-to-connect-live-export/4147/3)

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