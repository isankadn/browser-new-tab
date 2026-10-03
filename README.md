# Quiet Tab

A calm, local-first new tab dashboard: your daily tools without the clutter.

This overview describes the active development checkout. Public source may lag ongoing application changes; there is no advertised store release.

- Clock/time zones, search, shortcuts, notes, todos, and opt-in weather.
- Full-width responsive layout, light/dark modes, five color templates, and local or automatic photo backgrounds.
- Customize from the bottom-right icon; editing controls stay hidden during normal use.
- Local notes work offline. Google Drive sync/sharing is opt-in and requires publisher OAuth setup.

## Try the development build

1. Use a development checkout containing `app.js` and `widgets.js`, then open `chrome://extensions`.
2. Enable **Developer mode**, choose **Load unpacked**, and select this repository's folder.
3. Open a new tab. Use **Customize** to add widgets or change the appearance.

No dependencies or build step are needed to run the extension. After editing files, reload it from the extensions page.

## Browser packages

Run `node scripts/package.mjs chromium` (or `firefox` / `safari`) to create `dist/<browser>`.
Firefox distribution requires Mozilla signing. Safari requires Apple conversion/signing and explicit new-tab selection; Drive also needs a native OAuth bridge. Packages are not proof of verified browser support.

Weather's keyless Open-Meteo service is for permitted non-commercial use. Online wallpapers and weather request provider access only when enabled; the local dashboard needs no account.

## More

- [Website](https://isankadn.github.io/browser-new-tab/) — overview and installation.
- Requirements and architecture: `REQUIREMENTS.md` in the development checkout.
- Optional widget candidates: `requirements/OPTIONAL_WIDGETS.md` in the development checkout.

The website is static HTML/CSS in `docs/`, published through GitHub Pages from `main` → `/docs`. It is an informational site, not the extension itself.
