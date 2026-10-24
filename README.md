# The Inside Story of Electricity

>Drag, pinch, scroll, slide, press, click, and peel your way through the hidden world deep within computers 🔎 ✨ 🖥️

An interactive, offline 3D primer on what electrons and atoms are doing inside wires, diodes, capacitors, transistors, logic gates, adders, an ALU and a small CPU. Fourteen plates, one self-contained HTML file, no build step, no dependencies.

Made by AirplaneBug using Anthropic's Claude.

(Editor's note: Made by Claude using AirplaneBug?)

## Run it

Open `index.html` in any modern browser. To host it, upload the whole folder to any static host (Netlify, GitHub Pages, and so on). The page itself makes no network requests unless you turn on the optional Google Fonts setting.

## Install it as an app

Served over HTTPS, the page is installable: it ships a web app manifest, regular and maskable icons, screenshots for install dialogs, and a service worker that keeps it working offline. In Chrome and Edge, use the install icon in the address bar. On iPhone and iPad, use Share, then Add to Home Screen. The settings menu also has an Install button where the browser allows one.

## What is in the folder

- `index.html`: the whole page.
- `sw.js`: offline support. Bump the `CACHE` name in it to make every visitor drop old copies.
- `site.webmanifest`, `favicon.*`, `apple-touch-icon.png`, `icon-*.png`, `screenshots/`: install and icon files.
- `og-image.png`: 1200 by 630 preview image for link sharing and search.
- `robots.txt`, `sitemap.xml`: for search engines.
- `_headers`: Netlify caching and content-type rules.

If you host the page at a different address than `https://inside-electricity.airplanebug.io/`, update that address in `index.html` (canonical link, `og:` and `twitter:` tags, structured data), `robots.txt` and `sitemap.xml`.

## Features

- Pseudo-3D canvas engine written from scratch: rotate, zoom, cutaway, see-through, peel the onion.
- A working gate-level simulator behind the Blinky, logic gate, adder, ALU and CPU plates.
- Settings menu: light, dark and three print-inspired colour themes; optional high-contrast and colour-blind-safe palettes; font choices (system fonts by default, Google Fonts only if you allow them); calm readout; panning; reduced motion.
- Program the 8-bit computer (Plate XIV): stop the clock, open "Compose a program" in the Experiment card, and edit the sixteen bytes as instructions or hex. Save, rename and delete programs (kept in your browser), download one as a plain text file, or open one back in. Saved programs are not touched by the settings Reset. A tutorial for ages 13 and up ("Program it yourself") sits under "Under the hood" on that plate, with two example programs that load into the desk.
- Keyboard operation: Alt+Shift+S opens settings, Alt+Shift+K turns on page-wide viewport keys, and the full list is in the settings menu.

## A note on the facts

Facts and sources (Editor's note: and code) have been assembled by Claude and are not yet human-verified. Use them at your own discretion, and please open an issue or pull request if you find a mistake.

## License

Copyright (C) 2026 AirplaneBug.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. See [LICENSE](LICENSE) for the full text.

If you run a modified version of this page on a public website, the AGPL asks you to offer your visitors the source of your modified version, for example with a "Source" link in the page.

Fonts are not bundled. If you enable Google Fonts in the settings, your browser fetches them from Google under their own licenses.
