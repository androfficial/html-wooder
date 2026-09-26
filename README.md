# Wooder

Landing page for a woodworking studio that scrolls one full-screen section at a time, with entrance animations and videos in a lightbox. Built in July 2021 as a learning project.

**Live demo:** [androfficial.github.io/wooder](https://androfficial.github.io/wooder/)

## Features

- On screens wider than 768 px, fullPage.js moves through the six sections one screen at a time. The side navigation links to every section and marks the current one, and a counter next to it shows its number (01 to 06).
- On screens wider than 1024 px, the header, title, button, scroll hint, footer and side navigation enter with Animate.css effects. After that the button keeps pulsing (it pauses on hover) and the scroll hint keeps sliding up and down.
- The play buttons and "Watch video" open YouTube videos in an fslightbox lightbox.
- The language dropdown opens on click and closes on a click anywhere else.
- On touch devices narrower than 768 px, the menu button opens a full-screen menu and locks page scroll.

## Tech stack

- **Framework:** none, plain HTML and JavaScript
- **UI:** fullPage.js 3 with the Scrolloverflow extension, fslightbox
- **Styling:** SCSS compiled to CSS (the SCSS sources are not in the repository)
- **Animation:** Animate.css 4, CSS keyframes
- **Tooling:** built with Gulp 4, which produced the plain and minified bundles in `css/` and `js/`
- **Hosting:** GitHub Pages

## Getting started

The repository holds the compiled site, with no dependencies and no build step. The icons come from an external SVG sprite that browsers do not load from `file://`, so serve the folder over HTTP, for example with `npx serve .` on Node.js 18 or later.

```bash
git clone https://github.com/androfficial/wooder.git
cd wooder
npx serve .
```

Then open the local address that `serve` prints.

## Notes

- The footer credits the design to Viacheslav Olianishyn.
- The menu, "Learn more" and language links point to `#`.
