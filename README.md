# Sparkrail — website & legal pages

Static GitHub Pages site for the Android game **Sparkrail** (developer: Manfred Uschan).
Bilingual (English / German, auto-detected from the browser, switchable via EN/DE).

| Page | URL (after enabling Pages) |
|---|---|
| Start | https://onvexalabs-dev.github.io/sparkrail-site/ |
| Privacy policy (Play Console "Privacy policy") | https://onvexalabs-dev.github.io/sparkrail-site/privacy.html |
| Terms of use | https://onvexalabs-dev.github.io/sparkrail-site/terms.html |
| Imprint / Impressum | https://onvexalabs-dev.github.io/sparkrail-site/imprint.html |
| Data deletion | https://onvexalabs-dev.github.io/sparkrail-site/delete-data.html |
| app-ads.txt | https://onvexalabs-dev.github.io/sparkrail-site/app-ads.txt (see note!) |

## Before going live
1. Replace the highlighted address placeholder (`[Street and number…]`) in `privacy.html`, `terms.html`, `imprint.html`
   (search for `class="todo"`; 3 files × EN + DE). Austrian law (§ 5 ECG, § 25 MedienG) requires a postal address in the imprint.
2. Replace `pub-0000000000000000` in `app-ads.txt` with your AdMob publisher ID.
3. Repo ▸ Settings ▸ Pages ▸ Source: *Deploy from a branch* ▸ `main` / root.

## Important: app-ads.txt must be at the domain ROOT
AdMob only crawls `https://<developer-website-domain>/app-ads.txt`. A project page lives in a sub-path
(`/sparkrail-site/`), so the copy in this repo is **not** crawled on its own. Use one of:
- **Option A (free, recommended):** create the repo `onvexalabs-dev/onvexalabs-dev.github.io` containing the same
  `app-ads.txt` at its root, and enter `https://onvexalabs-dev.github.io/` as *Developer website* in Play Console.
- **Option B:** attach a custom domain to this repo (Settings ▸ Pages ▸ Custom domain); then `app-ads.txt` is served at
  that domain's root.

© 2026 Manfred Uschan. All rights reserved.
