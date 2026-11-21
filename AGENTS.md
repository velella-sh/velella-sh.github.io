# velella-sh.github.io

The Velella landing site, served by GitHub Pages at https://velella.sh. Static HTML and inline CSS; no build step and no dependencies.

- Start with the affected page: `index.html` for the landing page or `skills/index.html` for Agent Skills. Check both when changing shared styles or theme behavior.
- Keep `CNAME` and `.nojekyll`; Pages needs both.
- Styles are inline in each page. The design tokens are in `:root` and the `[data-theme="day"]` block; reuse the existing token names instead of adding colors.
- The only script is the inline theme toggle. Keep it inline, dependency-free, and safe when `localStorage` throws.
- External requests are limited to Google Fonts. Do not add analytics or other third-party scripts.
- Keep both pages working at narrow widths, keyboard accessible, and readable without the theme script.

Check locally:

```bash
python3 -m http.server 8000
```

One change per commit. No secrets.
