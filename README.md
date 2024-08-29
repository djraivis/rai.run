# Inkdrop App User - Raivis

Welcome to my corner of the coding universe! I’ve taken inspiration from Craftzdog’s brilliant framework, adding my own touch to create this blog where I share the tech notes and insights I gather along my coding journey. This space is my digital notebook, where every post is a reflection of the challenges I tackle and the discoveries I make. Dive in to explore the evolving landscape of tech through my eyes, as I document and discuss the nuances of programming and development.

## Tutorial

Watch how craftzdog built this website on YouTube:

[![tutorial thumbnail](./docs/cover-thumb.jpg)]


## Link – originally created by Craftzdog
<https://youtu.be/3_JE76PKBWE>

## Stack

- [Astro](https://astro.build/) - Static Website Framework
- [Tailwind CSS](https://tailwindui.com/) - CSS Framework
- [React](https://reactjs.org/) - Component-based UI framework for JS
- [Headless UI](https://headlessui.com/) - Unstyled interactive components
- [React Icons](https://react-icons.github.io/react-icons/) - Icon set
- [Inkdrop](https://www.inkdrop.app/) - Markdown note-taking app, for writing the blog content (optional)

## Project Structure

Inside of your Astro project, you'll see the following folders and files:

```
PROJECT_ROOT
├── public              # static assets
│   └── posts           # images of posts
├── src
│   ├── components      # Astro & React components
│   │   └── icons
│   ├── layouts         # page layouts
│   ├── pages           # page files
│   │   ├── categories  # category pages
│   │   └── posts       # .md files
│   └── styles          # global stylesheets
└── tools               # Inkdrop integration
```

## How to import notes from your Inkdrop local server

First, please check out the [live-export](https://github.com/inkdropapp/inkdrop-live-export) documentation.

Create `.env` file as following:

```
DEBUG='inkdrop:export:info,inkdrop:export:error'
INKDROP_USERNAME='***'
INKDROP_PASSWORD='***'
INKDROP_PORT=***
INKDROP_BOOKID='***'
```

Then, run the following command:

```sh
npm run live-import
```

0r

```sh
yarn run live-import
```

## License

MIT License.

You can create your own homepage for free without notifying me by forking this project under the following conditions:

- Delete my blog content and assets
- Add a link to [my homepage](https://www.craftz.dog/)

---

Looking for a Markdown note-taking app? Check out my app called Inkdrop:

[![Inkdrop](https://github.com/craftzdog/dotfiles-public/raw/master/images/inkdrop.png)](https://www.inkdrop.app/)

[![Netlify Status](https://api.netlify.com/api/v1/badges/87aa8712-b37a-449e-a25c-bc7075074f06/deploy-status)](https://app.netlify.com/sites/rai-run-tech-notes/deploys)
