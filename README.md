# switchsuite.io

The website for Switch Suite, a family of Android utilities: a landing page, the privacy policy and support.

Plain static HTML and CSS: no framework, no build step, no JavaScript, no cookies, analytics or third-party requests. It's served by GitHub Pages from the `main` branch root, with the custom domain in `CNAME`.

| Path | Page |
|---|---|
| `/` | `index.html` |
| `/privacy/` | `privacy/index.html`: the Switch Suite app's privacy policy (source: `docs/privacy-policy.md` in the app repo) |
| `/support/` | `support/index.html` |
| any other path | `404.html` (uses root-absolute links, so it works at any depth) |

Pages use relative links, so the site also works under `https://ciderguyms.github.io/switchsuite-site/`.

## Look

Same tokens as the Android app: Inter (self-hosted in `assets/fonts/`, SIL Open Font License 1.1, see `assets/fonts/OFL.txt`), accent `#007AFF` (`#0A84FF` in dark mode), grouped backgrounds `#F2F2F7` / `#000000`, and light/dark from `prefers-color-scheme`. The favicon (`favicon.svg`, `favicon-32.png`, `assets/icon-*.png`) is the app's placeholder "S" mark. Module glyphs are Material Design icon paths (Apache 2.0).

## Editing

Edit the HTML directly and push to `main`; Pages redeploys within a minute or two. Keep the brand rules: describe the apps neutrally and don't name other platforms' products.
