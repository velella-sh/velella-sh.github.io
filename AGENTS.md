# velella-sh.github.io

The Velella root site, served by GitHub Pages at https://velella.sh. It is built with Mizzen and the Lateen theme from `site/`; each project (`/ebb`, `/mizzen`, `/lateen`, `/offing`) publishes its own site below its path from its own repository.

- Pages are Markdown in `site/` (`index.md`, `skills.md`); configuration is `site/mizzen.yml`.
- `site/network.lock.json` is the pinned copy of the shared network list. Refresh it with `mizzen network update site`, never by hand.
- The deploy workflow builds the site, then `mizzen network sitemap` writes the root `sitemap.xml` index and `robots.txt` over the output. Do not add a root `sitemap.xml` or `robots.txt` by hand.
- Analytics is Cloudflare Web Analytics through the `analytics` key in `site/mizzen.yml`; add no other third-party scripts.
- Keep `CNAME` and `.nojekyll`. Pages' source is "GitHub Actions".

Check locally (Node 24 or later):

```bash
npm install --no-save @velella/mizzen@0.2.7 @velella/lateen@0.2.5
npx mizzen check site --theme node_modules/@velella/lateen
npx mizzen dev site --theme node_modules/@velella/lateen
```

One change per commit. No secrets.
