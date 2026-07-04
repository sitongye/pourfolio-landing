# Cloudflare Pages Setup

Tamped should be hosted as a single Cloudflare Pages project at `tamped.coffee`.

## Recommended Project

- Project name: `tamped-coffee`
- Repository: `sitongye/pourfolio-landing`
- Production branch: `main`
- Framework preset: `None`
- Build command: `exit 0`
- Build output directory: `.`
- Custom domains: `tamped.coffee`, `www.tamped.coffee`

## DNS Cutover

Do not remove the existing GitHub Pages records until Cloudflare Pages has a successful production deployment and the custom domains are active.

Current GitHub Pages records to remove during cutover:

- Apex `A` records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `www` CNAME pointing to `sitongye.github.io`

Keep MX and TXT records for email/Firebase.

## SEO Pages

SEO pages live under the same domain:

- `/coffee-ratio-calculator/`
- `/brew-guides/espresso-dial-in/`
- `/brew-guides/v60-pour-over/`
- `/cities/tokyo/`
- `/cities/london/`
- `/cities/berlin/`

`robots.txt` points search engines to `sitemap.xml`.
