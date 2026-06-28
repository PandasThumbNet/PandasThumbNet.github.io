# Static GitHub Pages mirror for pandasthumb.net

- Expected GitHub user: `PandasThumbNet`
- Expected GitHub email: `github@pandasthumb.net`
- Expected user Pages repo: `PandasThumbNet.github.io`
- Custom domain: `pandasthumb.net`
- Local source: `/home/netuser/dev/sites/pandasthumb.net/public_html`

## Provisioning Notes

This directory is intended to be pushed as the GitHub Pages repository for the domain.
It was generated from the local static `public_html` snapshot and includes `CNAME` and `.nojekyll`.

Server-side scripts, CGI directories, logs, and private web-server files are excluded from the publish copy.
Review `PAGES_STATIC_RISK_REPORT.md` before DNS cutover.

## Static Search

Search is provided by Pagefind. Build the browser-only search bundle before publishing:

```bash
npm install
npm run build:search
```

Commit the generated `_pagefind/` directory with the site. GitHub Pages then serves search as static files; no backend service is required.
