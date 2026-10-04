# rafaeltovar-tumblr-theme

A personal Tumblr theme: minimal, type-focused, with light and dark modes.

Live at **[rafaeltovar.tumblr.com](https://rafaeltovar.tumblr.com)**.

The whole theme lives in a single file: [`theme/theme.html`](theme/theme.html).

## Features

- Serif type (Libre Baskerville) for content and sans-serif (Roboto) for navigation and tags.
- Light and dark modes with a toggle button. The visitor's choice is remembered in their browser.
- Optional automatic dark mode that follows the operating system preference.
- The theme is applied before the page is painted, so there is no flash of the wrong colors on load.
- Every post reads in a single 820px column. Photosets are laid out natively in rows that follow Tumblr's photoset layout, instead of the fixed-width Tumblr iframe.
- Support for every Tumblr post type: text, photo, photoset, panorama, quote, link, chat, audio, video and answers.
- Navigation with home, ask, submit, custom pages, archive and likes. On mobile it scrolls horizontally.
- Responsive layout.

## Installation

1. In Tumblr, open your blog and go to **Edit appearance → Edit theme**.
2. If needed, turn on **Custom theme** in the blog settings.
3. Click **Edit HTML**, delete the existing code and paste the contents of [`theme/theme.html`](theme/theme.html).
4. Click **Update preview**, check that everything looks right, and save.

## Customization options

These can be changed from Tumblr's **Edit theme** panel:

| Option | Type | Default |
|---|---|---|
| Logo | Image | — |
| Show avatar | Toggle | On |
| Show navigation | Toggle | On |
| Enable theme switcher | Toggle | On |
| Auto dark mode | Toggle | On |
| Default theme | Select | Light |
| Light background / text / link | Color | `#ffffff` / `#232323` / `#6b6b6b` |
| Dark background / text / link | Color | `#181818` / `#eaeaea` / `#bdbdbd` |
| Card border light / dark | Color | `#e9e9e9` / `#2b2b2b` |

**Default theme** only applies when **Auto dark mode** is off.

Anything added under **Custom CSS** is inserted at the end of the theme's styles, so it takes precedence over them.

## Development

The theme is written in [Tumblr's template language](https://www.tumblr.com/docs/en/custom_themes) (`{block:...}`, `{Variable}`, `{lang:...}`). There are no dependencies and no build step, and the file can't be opened directly in a browser. To test a change, paste it into **Edit HTML** and use **Update preview** before saving.

Branch and commit conventions are in [`AGENTS.md`](AGENTS.md).
