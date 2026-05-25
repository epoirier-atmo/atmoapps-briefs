# AtmoPulse Design System

The shared visual and voice language for AtmoApps briefs. This folder is the
canonical source. A brief keeps the tokens inlined in its own file so it stays
self-contained; this folder is what those inlined values are kept in sync with.

## Files

- `tokens.css` — the design tokens: color, type, motion. The single source of
  truth for these values.
- `brand/` — shared brand assets (watermark glyph, wordmark). Add the real
  AtmoApps brand SVGs here as they become available.

## Voice

Briefs are written to sound like AtmoApps: direct, plainspoken, specific.

- **No em dashes.** None. Use a comma, a period, or a colon instead.
- **Avoid AI tells.** No "it's not X, it's Y." No "journey," "passion,"
  "elegant fusion," "testament to," "delve," "underscores," "I want to be
  upfront." Write plainly.
- **Lead with the problem.** The strongest openings name a real, messy
  situation, not an abstraction.
- **Specific beats adjective.** A concrete proof point lands harder than a
  descriptor. Name the thing.
- **Honest over promotional.** A brief is allowed to reach a conclusion that
  is not a sales pitch. That honesty is what makes the format work.
- Title Case for headings, sentence case for supporting copy. No emoji, no
  exclamation marks.

## Color roles

- **Teal** (`--ap-teal`, `--ap-teal-bright`, `--ap-teal-deep`) is the one
  interactive accent: links, controls, active and focus states, and the
  "alive / healthy" signal in illustrations.
- **Gold** (`--ap-gold`) is for rare callouts only, such as a single
  emphasized phrase. If gold appears more than once or twice in a brief, it is
  being overused.
- **Red is not an AtmoApps brand color.** It is not used.
- **Dark-first.** Briefs ship on the dark navy field (`--ap-bg`). There is no
  light theme.

## Type

Archivo throughout, loaded from Google Fonts. Light (300) for body copy, Black
(900) for all-caps eyebrows and labels. Headings sit at a normal-to-light
weight, large, with tight letter-spacing.

## Motion

- One easing curve (`--ap-ease`): a hard-decelerating ease that reads as a
  crisp settle. **No bounce, no spring, no overshoot.**
- Motion should carry meaning. Animate to show something happening, not for
  decoration. When in doubt, less.
- Briefs are built scroll-driven: animation is tied to scroll position, so it
  runs both directions and is reversible.
- Honor `prefers-reduced-motion`. With reduced motion requested, or with
  JavaScript off, a brief degrades to a calm, readable static article.

## Surfaces and depth

Translucency and hairline dividers (`--ap-divider`, `--ap-divider-2`) over
heavy borders and drop shadows. Faint, restrained. Keep read-critical text at
or above `--ap-fg-3`; anything fainter is decorative only.

---

Copyright AtmoApps. All rights reserved.
