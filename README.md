# New Tab Boilerplate

A minimal Chrome extension that shows a custom page whenever you open a new tab.

## Get started

1. Clone this repository and open `chrome://extensions` in Google Chrome.
2. Turn on **Developer mode** in the top-right corner.
3. Click **Load unpacked** and select this repository's folder (the one containing `manifest.json`).
4. Open a new tab to see **Hello, world!**

Edit `newtab.html` to customize the page. After changing a file, click the extension's **Reload** button on `chrome://extensions`, then open or refresh a new tab.

## Files

- `manifest.json` declares a Manifest V3 extension and points Chrome's new tab override to `newtab.html`.
- `newtab.html` contains the page's HTML and CSS.

No dependencies or build step are required.
