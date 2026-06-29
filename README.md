# sweetleavesmn.com

Production marketing site for Sweetleaves (North Loop, Minneapolis). Static, no build step.

## Pages
- Homepage: `/` (`index.html`)
- Rewards / Garden Club landing: `/rewards` (`rewards/index.html`)
- Assets: `assets/` (homepage), `rewards/assets/` (rewards page)

## Hosting
Deploy as a static site on Vercel. Framework preset: Other. No build command. Homepage serves at `/`, rewards at `/rewards`.

## Tracking
All client-side, baked into the HTML:
- Google Tag Manager: GTM-KPKJKT5G
- GA4: G-N126LC5ZYF, G-3M9FSQWF9T, G-CSL7L78N6C

## Notes
Captured from the original Netlify deploy. Two Netlify-only references remain (the RUM script and a /.netlify/functions/track beacon). They 404 off Netlify but do not affect the GTM/GA4 tracking above, so they can be left as-is or removed later.
