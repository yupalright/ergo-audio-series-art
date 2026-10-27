# Ergo Audio series art tool

Creates 3000 × 3000 px JPEG series art for Apple Podcasts and Spotify, using six category backgrounds.

## How to use
1. Open `index.html` in a browser (double-clicking it works).
2. Pick a category.
3. Enter the series title (3–10 words). Caps are set automatically.
4. Click **Download JPEG**, or **Send to Apple Podcasts and Spotify** once that's connected.

## Categories
- 01: Ancient and classical
- 02: Modern and Enlightenment
- 03: Continental and 20th century
- 04: Mind, self and consciousness
- 05: Science, math and logic
- 06: Ethics and how to live

## Layout rules
- Titles set in ABC Monument Grotesk Heavy, black on white bars, on one or two lines.
- Three-word titles stay on one line, shrinking to fit.
- A single word is never left alone on line two. The title holds on one line instead, or a word moves down.
- Bars anchor at the bottom left and grow upward, staying clear of the figure.

## Files
- `index.html`: the tool. Backgrounds and font are embedded, so it works offline.
- `assets/`: the six background masters (3000 × 3000 JPEG). If a background changes, update it here and rebuild the embedded copy in `index.html`.

## For developers
- **Send button:** replace `sendToPlatforms(blob, filename)` in `index.html` with an upload to the podcast host. The host's RSS feed delivers the artwork to Apple Podcasts and Spotify.
- **Font:** the embedded font is a trial file. Replace it with Ergo's licensed ABC Monument Grotesk Heavy before production use.
- **Layout settings:** sliders at the bottom of the page adjust type sizes and spacing. Hide the panel once the values are final.

The # and ## lines become headings, and GitHub displays the formatted version on the repository’s main page.
