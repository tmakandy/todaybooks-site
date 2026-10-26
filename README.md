# TodayBooks — website

Public marketing and legal pages for the **TodayBooks** iOS app, served by GitHub Pages.
The app's source lives in a separate private repository; this repo holds static content
only, so it can be public without exposing the code.

| Page | Purpose |
|---|---|
| `index.html` | Landing page and FAQ — the SEO surface |
| `privacy.html` | Privacy policy — **required** by App Store Connect |
| `support.html` | Support page — **required** by App Store Connect |
| `sitemap.xml`, `robots.txt` | Search indexing |
| `.nojekyll` | Stops Jekyll from processing the folder |

No build step: plain HTML and one stylesheet.

## Published at

- https://tmakandy.github.io/todaybooks-site/
- https://tmakandy.github.io/todaybooks-site/privacy.html
- https://tmakandy.github.io/todaybooks-site/support.html

## Setup

Settings → Pages → Deploy from a branch → `main` / `(root)`.

## Keeping it honest

`privacy.html` describes what the app actually collects, derived from an audit of the
source: name, email, phone, physical address, user ID and purchase history — with no
tracking and no analytics SDK. **If the app's data collection changes, update this page
and the App Privacy answers in App Store Connect together.** Apple compares them, and
the app ships a `PrivacyInfo.xcprivacy` manifest that must agree as well.
