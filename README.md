# joshaho.com

Personal website of [Josha Ho](https://joshaho.com) — a link-in-bio style home
page with hosted articles, built with [Astro](https://astro.build) and deployed
on [Render](https://render.com).

## Development

```sh
pnpm install
pnpm dev      # local dev server at http://localhost:4321
pnpm build    # production build to dist/
```

## Structure

| Path                      | Purpose                                          |
| ------------------------- | ------------------------------------------------ |
| `index.json`              | Site config: links, socials, featured content    |
| `src/components/`         | Page sections (header, socials, links, articles) |
| `src/content/articles/`   | Articles — add a `.md` file to publish           |
| `src/pages/articles/`     | Article listing + article template               |

## Writing an article

Add a markdown file to `src/content/articles/`:

```md
---
title: "My Article"
description: "A short summary shown on cards."
pubDate: 2026-01-15
tags: ["tag"]
---

Your content here.
```

It automatically appears in the Writing section on the home page and at
`/articles/`.

## License

MIT — see [LICENSE](LICENSE).
