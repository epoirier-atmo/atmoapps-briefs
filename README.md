# AtmoApps Briefs

Short, interactive briefs from AtmoApps. Each one is a single, self-contained
web page that makes one focused point: a case study, a design principle, a way
to think through a software decision. They are calm, honest, and quick to read,
and they are used as outreach and marketing assets.

## Briefs

| Brief | Path | Status |
| --- | --- | --- |
| Why Field Apps Live or Die | `field-apps/` | Live |

Each brief lives in its own folder with an `index.html`, so it gets a clean
URL and the next brief is added as a sibling folder with no rework.

## How these are built

- One self-contained `index.html` per brief. No backend, no build step, no
  database. Design tokens and animation libraries are inlined into the file so
  it is fully portable and can be hosted anywhere.
- Scroll-driven storytelling, built on GSAP with ScrollTrigger and Lenis.
  Animation is tied to scroll position, so it runs both directions and is
  reversible.
- Progressive enhancement. With JavaScript off, or with reduced motion
  requested, the page degrades to a calm, readable static article.
- Built on the AtmoPulse design system: dark-first, AtmoApps brand color and
  type, restrained motion.

## Editing copy

All of a brief's wording lives in one clearly-marked `CONTENT` object near the
top of the page script. To change wording, edit the text between the quote
marks and leave the surrounding punctuation alone. Nothing else in the file
needs to be touched to change copy.

## Hosting

Published with GitHub Pages from the `main` branch. Each brief is reachable at
`/<brief-folder>/`. The pages are self-contained, so they behave identically
when served from atmoapps.com.

## A note on direction

This started as a single brief and is being kept as a collection. As more are
added, the shared pieces (the scrollytelling shell, the design tokens) will be
extracted into a `shared/` folder so each new brief is mostly copy and its own
illustration rather than a rebuild. That extraction is intentionally deferred
until a few briefs exist, since the briefs themselves show what is genuinely
shared.

---

Copyright AtmoApps. All rights reserved.