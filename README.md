# Tamped Landing Page

Static landing and SEO pages for **Tamped** — your personal coffee journal app.

## Preview

Open `index.html` in a browser, or run a local static server:

```sh
python3 -m http.server 8090
```

## Hosting

The site is prepared for Cloudflare Pages.

- Project name: `tamped-coffee`
- Build command: `exit 0`
- Build output directory: `.`
- Production branch: `main`

See `docs/cloudflare-pages.md` for the DNS cutover checklist.

## Stack

- Static HTML
- Tailwind CDN on the landing page
- Shared CSS for SEO pages in `marketing.css`
- Cloudflare Pages `_headers` and `_redirects`
