---
source: willallstet/simple2026portfolio
commit: af63cc3a3b2137db130fafb4bc8ada75257de74a
files: [index.html, style.css, CNAME, scripts/make-display-images.py, scripts/reencode-gifs.sh]
updated: 2026-07-07
---

# simple2026portfolio — source overview

Will Allstetter's personal website: a **single-page, hand-written static site**
with no framework, no build step, and no runtime dependencies
(`package-lock.json:1` declares an empty package tree). It is served over GitHub
Pages at the custom domain in `CNAME:1` — **www.willallstetter.com**.

## Structure

The whole site is three tracked assets plus a photo library:

- `index.html` — the entire page: a `<h1>` masthead, an `.intro` bio block, and
  one long `<ul>` of ~40 works (art, writing, projects, exhibitions, teaching).
  Two inline `<script>` blocks handle a color-cycling title cube
  (`index.html:15`) and custom lazy-loading of images, `<video>`, and `<iframe>`
  embeds (`index.html:111`).
- `style.css` — a compact serif stylesheet (Times New Roman, star `☆` list
  bullets, responsive `70vw`/`20vw` breakpoints at `style.css:123`).
- `photos/` — the image/video library (gitignored `.DS_Store` aside), including
  pre-sized `photos/display/` derivatives and `photos/reencoded/` MP4/WebM
  versions of former GIFs.

## Tooling (`scripts/`)

Two local content-prep helpers, not part of the served site:

- `scripts/make-display-images.py` — reads image paths out of `index.html`,
  resizes them (default max-width 800px) into `photos/display/` using Pillow so
  Display-P3 / EXIF orientation survive (`scripts/make-display-images.py:1`).
- `scripts/reencode-gifs.sh` — re-encodes GIFs to much smaller MP4/WebM for
  `<video>` tags via ffmpeg (`scripts/reencode-gifs.sh:1`).

## Reading the site

The `<ul>` is the substance: each `<li>` is a work or reference — an art project,
a published essay, a video, or an affiliation. These are distilled into the
[entities](../entities/) (concrete projects, writings, affiliations) and
[concepts](../concepts/) (recurring research interests) pages. Start from the
person: [[will-allstetter]].

## Lazy-loading behavior (worth knowing)

Media uses `data-src` rather than `src`; the `index.html:111` script swaps them
in as elements enter the viewport (`IntersectionObserver`, 250px margin), loads
iframes one-at-a-time through a queue, and wakes lazy images/videos on
`scroll`/`resize`/`load`/`pageshow` (`index.html:187`–`index.html:255`). So a
raw fetch of the HTML shows embeds inert until scrolled into view.
