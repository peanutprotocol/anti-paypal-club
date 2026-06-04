# antipaypal.club

A static, single-page cypherpunk shrine to PayPal's fees, holds and frozen funds — with a
soft, UTM-tagged path to Peanut. No build step, no framework. Deployed on **GitHub Pages**.

## Files
- `index.html` — the whole site (Y2K/Milady cypherpunk: matrix rain, sparkle cursor, marquees,
  wall of fact-checked quotes, the Frozen Tamagotchi, the Peanut escape).
- `assets/` — `hero.jpg`, the `mila-*.png` mascots + pet evolution sprites, and `quotes.js`
  (the 26 verified quotes, generated from `paypal_horror_quotes.html`).
- `CNAME` — custom domain for GitHub Pages (`antipaypal.club`).
- `.nojekyll` — tells Pages to serve files as-is (no Jekyll processing).

## Local preview
```bash
python3 -m http.server 8787   # then open http://127.0.0.1:8787/
```

## Deploy (GitHub Pages)
Push to `main`, then Settings → Pages → Deploy from branch → `main` / root. See repo notes for
the custom-domain DNS records.

## The Frozen Tamagotchi
Adopt a chibi, **tap to mine ❄shards** (combo multiplier), idle/offline mining, a shop
(Tap Power / Mining Rig / Thermal Coat), bond levels, random events, daily streak. PayPal freezes
it at random (mining stops); the free skip is **Defrost with Peanut**. The pet **evolves** with your
shard high-water-mark: Frozen Egg → Frostling → Ice Cadet → Cyber Maiden → Cryo Goddess.
All state is `localStorage` — no server.

## Content / legal
All 26 wall quotes are real and sourced (links on each). Figures are illustrative. Nominative use
of the "PayPal" trademark for comparison/criticism; FTC affiliation disclosure in the footer.

## Local-only tooling (gitignored)
`gen-*.mjs` (Gemini image gen) and `extract-verified.mjs` (quote extraction) are dev scripts and
are not deployed.
