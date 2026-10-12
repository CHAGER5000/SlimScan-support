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
Screenshots: iPhone 6.9" captures (12 Oct 2026), Swiss look, English UI, demo documents only. Each is 580 px wide, as
WebP (served first) plus a JPEG fallback in `<picture>`. If a replacement has another ratio than 1320 × 2868, update its
`width`/`height` attributes (580 × 1260). Never use a paywall shot (it shows a price).

| File (.webp + .jpg) | Where | Caption (EN) | Source |
|---|---|---|---|
| `assets/01-swiss-start` | Hero, all languages | none | `screenshots/01-swiss-start.png` |
| `assets/04-swiss-export` | Screens row, 1st | See the size before you send | `screenshots/04-swiss-export.png` |
| `assets/09-swiss-idphoto-chooser` | Screens row, 2nd | ID and visa photos for online forms (iPhone) | `screenshots/09-swiss-idphoto-chooser.png` |
| `assets/02-swiss-pages` | Screens row, 3rd | Tap a page to leave it out | `screenshots/02-swiss-pages.png` |
| `assets/og.png` | Social preview (1200 × 630) | text only: cross, SlimScan, headline | built from HTML |
| `assets/apple-touch-icon.png` | Home-screen icon (180 × 180) | Swiss cross | built from HTML |
| `assets/icon.svg` | Favicon | Swiss cross | hand-drawn |

Alt texts describe what each screenshot shows; update them on all 4 home pages if an image changes.
Dark-mode screenshots (optional): save as `NAME-dark.webp` next to the light one and un-comment the
`<source … media="(prefers-color-scheme: dark)">` line inside that image's `<picture>`.

## To do before publishing (merging into `main`)
- App Store id: replace `XXXXXXXXXX` in the App Store link (`?ct=website`) and in the `apple-itunes-app` meta on the 4 home
  pages (both marked `TODO(owner)`). For campaign stats in App Store Connect also add `&pt=PROVIDER_TOKEN`.
- The site describes iOS 1.2 features (ID photo, Remove hidden data, Copy text): publish together with 1.2.
- DE/FR/IT texts: native check.
