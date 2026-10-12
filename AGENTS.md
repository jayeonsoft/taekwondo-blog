## Project

Devlog for Seoul Nights (taekwondo.jayeonsoft.com). Static Astro site, deployed as a Cloudflare
Worker serving static assets (`wrangler.jsonc`, custom domain `blog.taekwondo.jayeonsoft.com`).
Posts live in `src/content/blog/*.md`. Ships by merge: Cloudflare Workers Builds deploys `main` on
every push — never run `wrangler deploy` by hand except to bootstrap a brand-new deploy.

## Development

When starting the dev server, use background mode:

```
astro dev --background
```

Manage the background server with `astro dev stop`, `astro dev status`, and `astro dev logs`.

## Documentation

Full documentation: https://docs.astro.build

Consult these guides before working on related tasks:

- [Adding pages, dynamic routes, or middleware](https://docs.astro.build/en/guides/routing/)
- [Working with Astro components](https://docs.astro.build/en/basics/astro-components/)
- [Using React, Vue, Svelte, or other framework components](https://docs.astro.build/en/guides/framework-components/)
- [Adding or managing content](https://docs.astro.build/en/guides/content-collections/)
- [Adding styles or using Tailwind](https://docs.astro.build/en/guides/styling/)
- [Supporting multiple languages](https://docs.astro.build/en/guides/internationalization/)
