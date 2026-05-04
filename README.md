# WeTrade SEO Operations — Dashboard Demo

A static HTML mockup of the SEO automation dashboard for wetrademarketing.com.

This is a **visual demo / showcase** — it loads instantly, has realistic data baked in, and shows what the system will look like when running against real GSC data. Use this for boss demos and stakeholder presentations while the backend (the Node.js SEO automation system) connects to live data later.

## Deploy to Vercel — 60 seconds

### Option A: Drag and drop (easiest)
1. Go to https://vercel.com/new
2. Drag the entire `wetrade-seo-dashboard` folder onto the page
3. Click Deploy
4. Get a URL like `wetrade-seo-dashboard-xxxx.vercel.app`

### Option B: Vercel CLI
```bash
npm i -g vercel
cd wetrade-seo-dashboard
vercel
```
Follow prompts. Free tier is plenty.

### Option C: GitHub auto-deploy
1. Push this folder to a GitHub repo
2. Connect repo to Vercel
3. Auto-deploys on every push

## Custom domain (optional, $0)

In Vercel project settings → Domains → add `seo.wetrademarketing.com` (or whatever subdomain you want). Vercel gives you DNS instructions; usually it's a CNAME record. SSL is automatic and free.

## What's included

- **`index.html`** — the entire dashboard, single file, no build step
- **`vercel.json`** — config telling Vercel this is a static site

That's it. No npm install, no dependencies, no API keys. Just static HTML + CSS + a tiny bit of JS for click feedback.

## What it shows in the demo

- **Topbar** with live-style metrics: 2 urgent · 12 pending · 8 auto-safe · +1,247 est. monthly clicks
- **Urgent section** with 2 examples (5xx error, ranking drop)
- **Auto-safe section** with one-click batch apply banner
- **Review queue** with detailed proposal cards (title rewrite, meta description, new article)
- **Executed section** with rollback option

The interactive bits work for the demo (clicking Apply turns the button green, etc.) but no real backend calls happen.

## Pairing with the live system

When the Node.js SEO automation system from earlier runs against real wetrademarketing.com data (after ~2 months of GSC data accumulation), this dashboard layout becomes the live frontend. The visual identity is identical — same fonts, same colors, same components — so the transition from "demo" to "production" is seamless.
