# jonnochoo.com

Source for my personal blog, built with [Astro](https://astro.build). It's a space for writing about technology and whatever else — mainly for me, but you're welcome to read along.

Live at [jonnochoo.com](https://jonnochoo.com).

## Project Structure

```text
├── public/              # Static assets (favicon, etc.)
├── src/
│   ├── assets/           # Images and fonts processed by Astro
│   ├── components/        # Header, Footer, BaseHead, etc.
│   ├── content/blog/       # Blog posts (Markdown & MDX)
│   ├── layouts/            # BlogPost layout
│   └── pages/
│       ├── index.astro       # Blog listing (home page)
│       ├── about.astro        # About page
│       ├── blog/[...slug].astro  # Individual post pages
│       └── rss.xml.js          # RSS feed
├── astro.config.mjs
└── package.json
```

The blog listing currently lives at `/` — there's no separate landing page yet. Posts are Markdown/MDX files in `src/content/blog/`, and `getCollection()` pulls them into the listing and RSS feed.

## Commands

| Command             | Action                                       |
| :------------------- | :-------------------------------------------- |
| `npm install`         | Install dependencies                          |
| `npm run dev`          | Start local dev server at `localhost:4321`    |
| `npm run build`        | Build the production site to `./dist/`        |
| `npm run preview`      | Preview the production build locally          |
| `npm run astro ...`    | Run Astro CLI commands (`astro add`, `astro check`, etc.) |

When working with an agent in this repo, prefer `astro dev --background` so the dev server runs detached (see `CLAUDE.md`).

## Stack

- [Astro](https://astro.build) with the MDX and Sitemap integrations
- Content Collections for blog posts, with schema-checked frontmatter
- RSS feed via `@astrojs/rss`

## Credit

Originally scaffolded from Astro's official blog starter theme, itself based on [Bear Blog](https://github.com/HermanMartinus/bearblog/).
