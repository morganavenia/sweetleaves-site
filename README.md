# sweetleavesmn.com

Production marketing site for Sweetleaves (North Loop, Minneapolis). Static site plus one serverless function.

## Pages
- Homepage: / (index.html)
- Rewards / Garden Club landing: /rewards (rewards/index.html)
- Assets: assets/ (homepage), rewards/assets/ (rewards page)

## Serverless
- api/track.js: first-party attribution relay (sl_attr / sl_vid). No-op 204 by default, add forwarding as needed.

## Hosting
Deploy on Vercel. Framework preset: Other, no build command. Homepage at /, rewards at /rewards, api/track runs as a function.

## Tracking
Client-side, baked into the HTML: GTM-KPKJKT5G and GA4 G-N126LC5ZYF, G-3M9FSQWF9T, G-CSL7L78N6C. Plus the first-party relay at /api/track.

## Notes
Fully off Netlify: RUM script removed, attribution relay moved from /.netlify/functions/track to /api/track.
