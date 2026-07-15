# CleanPro — Commercial Cleaning Website Template

A premium, fully responsive commercial-cleaning website with light/dark themes, RTL support, a services catalogue, and client + admin dashboards.

## Quick start
Just open `index.html` — everything (CSS, JS, fonts, runtime) is inlined, so it works offline with no build step.

## Deploy to Vercel
1. Push this folder to a Git repo (or drag-drop into the Vercel dashboard).
2. Framework preset: **Other** (no build command, output dir = project root).
3. Deploy. `vercel.json` is already configured (clean URLs, root rewrite, caching).

Or with the CLI:
```
npm i -g vercel
vercel        # preview
vercel --prod # production
```

## Structure
```
cleanpro-template/
├── index.html              # the complete, self-contained app
├── vercel.json             # Vercel hosting config
├── pages/                  # deep-link entry points (redirect into the SPA via #hash)
│   ├── index.html
│   ├── about.html · services.html · contact.html
│   ├── home2.html · login.html · signup.html · forgot.html
│   ├── client-dashboard.html · admin-dashboard.html
├── assets/
│   ├── css/  (rtl.css reference + notes)
│   ├── js/   ├── images/ ├── fonts/
├── documentation/
└── README.md
```

## Pages / screens
Home · Home 2 (editorial) · Services (+ service detail) · Contact · About · Login · Sign up · Forgot password · Client dashboard · Admin dashboard · 404 · Coming soon.

Navigation is hash-based, so `index.html#services`, `index.html#admin`, etc. open directly.

## Features
- Light / dark theme toggle (system-aware tokens)
- RTL ⇄ LTR toggle on every screen
- Fully responsive (mobile, tablet, desktop) with off-canvas dashboard drawer
- Sticky navigation, hover mega-menus, animated marquee
- Client dashboard: requests, scheduling, invoices, notifications, profile
- Admin dashboard: analytics, customers, services, staff, reports, settings

## Customising
The source of truth is `CleanPro.dc.html` (+ `responsive.css`) in the design project; `index.html` here is the compiled output. Re-export after edits.

## Credits
Fonts: Google Fonts (Spectral, Schibsted Grotesk, JetBrains Mono). Icons: Lucide. Demo imagery: Unsplash.


## Support
Replace Unsplash imagery and Formspree/Stripe placeholders before production use.