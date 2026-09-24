# skolefinder.dk

The public site for the Skolefinder app, served by GitHub Pages from `main`
(custom domain `skolefinder.dk`, HTTPS enforced). Plain HTML, no build step.

| Path | Purpose |
|---|---|
| `index.html` | The front page: the app, what it shows, and the App Store link |
| `support/` | Support page (Danish first, English under `#english`) — the store listings' Support URL |
| `privatlivspolitik/` | Privacy policy, Danish (authoritative) — the store listings' Privacy Policy URL |
| `privacy-policy/` | Privacy policy, English |

## Assets

Everything under `assets/` is derived from the app repo (`school-ranking-app-dk`);
nothing here is hand-drawn.

- `assets/fonts/` — Libre Caslon Text and Hanken Grotesk, the app's two faces
  (SIL OFL 1.1, licences alongside), subset to Latin plus Danish and converted to
  woff2 from the app's static instances in `assets/fonts/`. Self-hosted so the site
  makes no third-party request — the privacy policy promises no tracking.
- `assets/img/glass.png` — the icon's magnifier, composited from the app's iOS 26
  icon layers (`assets/brand/AppIcon.icon/Assets/`) on the icon's own blue
  (`#5C7C97`), with the handle continued along its measured taper far past the
  frame so it always leaves the hero band through an edge.
- `assets/img/app-icon-*.png`, `apple-touch-icon.png`, `favicon-*.png` — the tile
  master `assets/brand/skolefinder-icon.png`, resized.
- `assets/img/screen.png` — the app's own App Store screenshot (the "Skolen ved
  Dybbølsbro" detail page), cropped to the screen inside the phone frame.
- `assets/img/app-store-badge-*.svg` — Apple's official badge artwork from the
  App Store marketing tools, Danish and English, black and white.

The front page's copy is the audited store-listing copy (`docs/store-listing.md`
in the app repo): no price, no exclamation mark, no composite score, and every
figure as the ministry states it.
