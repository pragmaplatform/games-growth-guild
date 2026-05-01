# Games Growth Guild

The largest network of marketing professionals in the games industry, from indie to AAA.

This is the static marketing site for [gamesgrowth.com](https://gamesgrowth.com).

## Stack

Plain HTML, CSS, and a sprinkle of JavaScript. No framework, no build step. Hosted on Vercel.

Fonts: Inter and Cal Sans (matching the player.gg type system) plus JetBrains Mono for technical labels.

## Project structure

```
.
├── index.html                                 Homepage
├── blog/
│   └── introducing-the-games-growth-guild.html  Blog post
├── assets/
│   ├── logo-mark.svg                          GGG mark
│   └── logo-lockup.svg                        GGG lockup
├── vercel.json                                Vercel config (clean URLs, headers)
└── README.md                                  This file
```

## Adding a new blog post

1. Duplicate `blog/introducing-the-games-growth-guild.html` and rename to your slug
2. Update the title, meta, post-meta, post-title, post-deck, post-cover, and prose blocks
3. Add a new `.blog-card` to `index.html` inside the `.blog-grid` container, pointing at `/blog/your-slug`
4. Commit and push. Vercel will redeploy on push to main.

## Local preview

Open `index.html` directly in a browser, or run any static file server:

```sh
npx serve .
```

## Deploy

The site auto deploys to Vercel on push to `main`. Manual deploy:

```sh
vercel deploy --prod
```
