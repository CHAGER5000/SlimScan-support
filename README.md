# SlimScan-support

Public website for SlimScan, live at https://chager5000.github.io/SlimScan-support/ (GitHub Pages, deployed from `main`).
Plain static HTML and one stylesheet: no scripts, no cookies, no web fonts, no trackers.

## Pages
| File | What it is |
|---|---|
| `index.html` | Home (English) + Support/FAQ and contact. This is the App Store **Support URL**: keep the FAQ and the email on it. |
| `privacy.html` | Privacy policy (iPhone, Android, common). This URL is given to Apple and Google: keep it. |
| `de/index.html`, `fr/index.html`, `it/index.html` | Short home pages in German, French, Italian. FAQ and privacy link to the English pages. |
| `style.css` | All styles, light and dark mode. |

## Images (all in `assets/`, replace in place when the new screenshot set is ready)
| File | Shown | Current source |
|---|---|---|
| `assets/screen-1.jpg` | Hero, all languages | iOS simulator, Swiss look, home screen |
| `assets/screen-2.jpg` | "What it does", all languages | iOS simulator, Swiss look, page grid |
| `assets/screen-3.jpg` | "What it does", all languages | iOS simulator, Retro look, PDF preview with size |
| `assets/icon.svg` | Favicon (Swiss cross) | drawn by hand |

Screenshots: 600 px wide JPEG (quality ~82, under 110 KB each), phone ratio 1320 × 2868. If a new image has another
ratio, update the `width`/`height` attributes in the pages. Alt texts and captions describe each image: update them too.

## To do before publishing (merging into `main`)
- App Store link: every page has `https://apps.apple.com/app/idXXXXXXXXXX` (marked `TODO(owner)`); put in the real id.
- The site describes iOS 1.2 features (ID photo, Remove hidden data, Copy text): publish together with 1.2.
