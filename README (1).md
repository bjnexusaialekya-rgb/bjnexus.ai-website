# BJNEXUS.AI — Website

Single-page marketing site for BJNEXUS.AI, an AI automation agency building
AI automation systems, SaaS platforms, and n8n workflows for B2B clients.

**Live site:** https://bjnexus.ai (once custom domain is connected)

## Stack

Plain static HTML/CSS/JS — no build step, no framework, no dependencies.

- `index.html` — the entire site (markup, styles, and scripts inline)
- Google Fonts loaded via CDN (Fraunces, DM Sans, JetBrains Mono, Inter)
- JSON-LD structured data for SEO
- Lead capture form with [Web3Forms](https://web3forms.com) + WhatsApp fallback

## Local development

No build tools needed. Just open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

Deployed via **Cloudflare Pages**, connected directly to this repo's `main`
branch. Every push to `main` triggers an automatic redeploy.

- Framework preset: `None`
- Build command: *(none)*
- Build output directory: `/`

## Before going fully live

- [ ] Replace the placeholder `YOUR_WEB3FORMS_ACCESS_KEY` in `index.html` with
      a real key from web3forms.com so form submissions route by email/CRM
      instead of only falling back to WhatsApp
- [ ] Connect the production custom domain in Cloudflare Pages
- [ ] Add privacy policy / terms pages if collecting lead data
- [ ] Verify all proof/stat claims on the page are accurate before publishing

## Contact

- Email: bjnexus.ai@gmail.com
- WhatsApp: via the link in the site footer
