# easyglenn.de

Static site for EasyGlenn (Glenn Reichardt) — BioLink page and coaching checkout.

## Structure

| Path | URL | Purpose |
|---|---|---|
| `index.html` | `easyglenn.de/` | BioLink page (Coaching, Instagram, TikTok, Anfragen) |
| `coaching/index.html` | `easyglenn.de/coaching/` | Coaching checkout page with PayPal |

## Deployment

Deployed via Cloudflare Pages with GitHub integration.
Every push to `main` triggers automatic build & deploy.

## Tech

- Pure HTML / CSS / vanilla JS — no build step
- PayPal Hosted Button SDK loaded from PayPal CDN
- Coaching form submits to Supabase project `jvdozdzvoqzvacqpyynd` (table `glenn_anfragen`)
- Legal documents (AGB, Datenschutz, Widerruf) loaded as iframes from itrk.legal
- Images hosted in Supabase Storage (project `bzejndghppuipnedasuv`, bucket `Glenn`)
