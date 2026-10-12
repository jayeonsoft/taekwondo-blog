# Seoul Nights Devlog

Devlog for [Seoul Nights](https://taekwondo.jayeonsoft.com), a browser 3D taekwondo action game — built with [Astro](https://astro.build).

Static site, deployed as a Cloudflare Worker (static assets) at `blog.taekwondo.jayeonsoft.com`.

## Commands

All commands run from the repo root:

| Command           | Action                                      |
| :---------------- | :------------------------------------------- |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start local dev server at `localhost:4321`  |
| `npm run build`   | Build the production site to `./dist/`      |
| `npm run preview` | Preview the build locally                   |

## Posts

New posts go in `src/content/blog/` as `.md` or `.mdx` files with `title`, `description` and `pubDate` frontmatter.

## Deploy

Ships by merge: pushing to `main` triggers Cloudflare Workers Builds, which runs `npm run build` and deploys `dist/` via `npx wrangler deploy`. Never deploy by hand.
