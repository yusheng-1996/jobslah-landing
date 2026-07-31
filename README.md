# Jobs Lah — Landing Page

A clean, jobseeker-focused job portal landing page for **Singapore & Brunei**. No employer side, no account sign-up, no courses, no AI messaging — just search, browse and apply.

## Features

- Hero search with keyword + location (Singapore / Brunei) filtering
- 50 varied job listings loaded from [`jobs.json`](jobs.json) — edit that file to manage jobs
- Job categories, trending tags, employer chips — all filter the listings
- Clickable job cards that open full detail modals
- Working **Career Tools**: Salary Calculator (computes from listing data), Interview Guide, Resume Builder (fill → preview → print/PDF)
- **Career Tips** with full article content
- Info modals for About / Privacy / Terms / Contact
- Fully responsive, light-mode, self-contained (only Google Fonts + Unsplash images are external)

## Run locally

Because the page loads `jobs.json` via `fetch()`, open it through a web server (not `file://`):

```bash
npx serve .
# or
python -m http.server 8099
```

Then visit the printed URL.

## Deploy

Static site — no build step. On Netlify, connect this repo and it deploys the root directory as-is (see [`netlify.toml`](netlify.toml)).
