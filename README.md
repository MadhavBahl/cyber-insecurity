# Cyber ~~Security~~ Insecurity: lecture deck

Open `index.html` in Chrome or Edge. Everything (styles, script, images) is inside that one file.

## Presenting
- `→` / `Space`: next slide, or reveal the answer on quiz slides
- `←`: back (on a quiz slide, hides the answer first)
- `N`: speaker notes · `F`: fullscreen · `?`: help · `Home` / `End`: first / last slide
- Jump to a slide: add `#s12` to the end of the URL

## Editing
- Each slide is one `<section class="slide">…</section>` block, in order. A comment like `<!-- 4 WHO AM I -->` sits above each one (the numbers in these comments are old labels, not current positions).
- To add a slide, copy an existing `<section>` and edit it. The counter and progress bar update by themselves.
- Speaker notes live in the `<div class="notes-src">` inside each slide.
- Click-to-reveal: give any element `class="reveal"`. It stays hidden until you press `→`. Don't also give it `class="anim"`.
- Entrance animation: `class="anim"` on direct children of a slide's wrapper.
- Colors and fonts are set as variables at the top of the `<style>` block (`--accent`, `--accent2`, etc.).

## Images
The three photos are embedded inside `index.html` as base64 (`src="data:image/jpeg;base64,…"`), so the file works offline. The originals are in `assets/`. To swap one, either replace the long base64 string, or point `src` at a file, for example `src="assets/madhav-photo.png"`, and keep the `assets` folder next to `index.html`.

## Needs internet for
Fonts only (Google Fonts). Offline, it falls back to system fonts and still works.
