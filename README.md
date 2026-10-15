# Discount Foam — Google Ads landing page

Static page, no build step. Deploy the folder as-is (Vercel, Netlify, any static host).

## Files
- `index.html` — the page (all CSS/JS inline)
- `images/` — logo (green + white PNG) and compressed WebP photos

## Before launch
1. **GTM:** replace `GTM-XXXXXXX` (2 places in `index.html`) with the real container ID.
2. **Form:** replace `REPLACE_ME` in the form `action` with a Formspree form ID (or swap to another endpoint that returns JSON).
3. Page is `noindex, nofollow` on purpose (ads-only page).

## GTM events pushed to dataLayer
- `call-click` — any tel: link tapped
- `directions-click` — Google Maps link
- `form-submit` — successful form submission

## Ad-group headline variants
Append `?s=` to the final URL to swap the hero headline + intro:
`mattress`, `cushions` (`couch`, `sofa`), `boat` (`rv`, `marine`), `outdoor`, `upholstery`.
No param = default headline. Edit copy in the `V` object in the inline script after the hero.

## Brand
- Dark `#1C1C1C`, green `#63AF47`, lime `#D7E35A`, tint `#EEF5EA`
- Headings: League Spartan; body: Archivo (Google Fonts)
