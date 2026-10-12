# SlimScan-support

Public website for SlimScan, live at https://chager5000.github.io/SlimScan-support/ (GitHub Pages, deployed from `main`).
Plain static HTML and one stylesheet: no scripts, no cookies, no web fonts, no trackers.

## Pages
| File | What it is |
|---|---|
| `index.html` | Home (English) + Support/FAQ and contact. This is the App Store **Support URL**: keep the FAQ and the email on it. |
| `privacy.html` | Privacy policy (iPhone, Android, common). This URL is given to Apple and Google: keep it. |
| `de/index.html`, `fr/index.html`, `it/index.html` | Short home pages in German, French, Italian, with the 3 most-needed FAQ answers. Full FAQ and privacy policy are in English. |
| `style.css` | All styles, light and dark mode. |
| `sitemap.xml` | The 5 public URLs. |

## Images (all in `assets/`)
Screenshots: iPhone, Swiss look, unlocked, demo documents only. 600 px wide JPEG (quality ~82), ratio 1320 × 2868.
If a new image has another ratio, update its `width`/`height` attributes. Never use the paywall shot (it shows a price).

| File | Where | Caption (EN) | Status |
|---|---|---|---|
| `assets/01-swiss-start.jpg` | Hero, all languages | none | placeholder (older simulator shot); replace with the new capture |
| `assets/04-swiss-export.jpg` | Screens row, 1st | See the size before you send | **missing**: add the file, then remove the `<!-- ENABLE … -->` wrapper around its `<li>` on all 4 home pages |
| `assets/08-swiss-idphoto.jpg` | Screens row, 2nd | ID and visa photos, checked (iPhone) | **missing**: same as above |
| `assets/02-swiss-pages.jpg` | Screens row, 3rd | Tap a page to leave it out | placeholder (older simulator shot); replace with the new capture |
| `assets/og.png` | Social preview (1200 × 630) | text only: cross, SlimScan, headline | done |
| `assets/apple-touch-icon.png` | Home-screen icon (180 × 180) | Swiss cross | done |
| `assets/icon.svg` | Favicon | Swiss cross | done |

Dark-mode screenshots (optional): save as `NAME-dark.jpg` next to the light one and un-comment the
`<source … media="(prefers-color-scheme: dark)">` line inside that image's `<picture>`.

## To do before publishing (merging into `main`)
- App Store id: replace `XXXXXXXXXX` in the App Store link (`?ct=website`) and in the `apple-itunes-app` meta on the 4 home
  pages (both marked `TODO(owner)`). For campaign stats in App Store Connect also add `&pt=PROVIDER_TOKEN`.
- The site describes iOS 1.2 features (ID photo, Remove hidden data, Copy text): publish together with 1.2.
- DE/FR/IT texts: native check.
