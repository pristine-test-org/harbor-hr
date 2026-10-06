---
name: Harbor
description: Calm, editorial landing page for on-demand HR counsel for service businesses
colors:
  paper: "#F4F7F6"
  card: "#FAFCFB"
  ink: "#182320"
  ink-soft: "#4A5C57"
  line: "#D2DFDB"
  accent: "#1F7A6B"
  accent-hover: "#196658"
  accent-ink: "#F2FAF8"
typography:
  display:
    fontFamily: "Newsreader, Georgia, serif"
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Plus Jakarta Sans, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
  eyebrow:
    fontFamily: "{typography.body.fontFamily}"
    fontSize: "0.875rem"
    fontWeight: 600
    letterSpacing: "0.06em"
    textTransform: uppercase
rounded:
  sm: "6px"
  md: "10px"
  lg: "16px"
spacing:
  container: "64rem"
  gutter: "1.25rem"
  section-y: "6rem"
  section-y-mobile: "4rem"
components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.accent-ink}"
    rounded: "{rounded.sm}"
    padding: "0.85rem 1.4rem"
  topic-card:
    backgroundColor: "{colors.card}"
    borderColor: "{colors.line}"
    rounded: "{rounded.lg}"
    padding: "1.75rem"
---

## Overview

Harbor sells a conversation with a senior HR advisor for service businesses, so the page should feel like a calm, well-written letter rather than a SaaS dashboard. Soft sea-glass paper background, dark ink, one teal accent, and a serif display face carry the tone: steady, human, direct. The whole site is a single self-contained `index.html` with no JavaScript.

## Colors

- **Paper** is the page background. **Card** is a slightly lighter cool white for topic cards.
- **Ink** is for headings and body. **Ink-soft** is for supporting copy.
- **Accent** (teal) is used only for the primary button, the eyebrow and the step numbers. Use it sparingly so it stays a signal.
- **Line** is for section dividers and card borders.

## Typography

- **Newsreader** (serif, weight 600) for the logo, headings and step numbers.
- **Plus Jakarta Sans** for body, buttons and links.
- Hero headline scales with `clamp(2.5rem, 6vw, 4.25rem)` and is capped at `16ch` wide.
- Section headings use `clamp(1.75rem, 3.5vw, 2.5rem)`.
- Body copy is 1.0625rem at line-height 1.6. The hero lede is 1.25rem.

## Layout

- Single centered column, `max-width: 64rem`, with a `1.25rem` side gutter.
- Order: header → hero → "What operators bring" (2×2 cards) → "How it works" (3 numbered steps) → closing CTA → footer.
- Sections are separated by a 1px `line` border and `6rem` vertical padding (`4rem` under 720px).
- Under 720px the card grid and the steps collapse to one column.

## Elevation & Depth

- Flat. There are no shadows. Depth comes from the card color against the paper and hairline borders.

## Shapes

- Buttons use `6px` radius. Cards use `16px`.
- There are no pills, icons or illustrations. Typography does the work.

## Components

- **Primary button:** teal fill, cool-white text, darkens on hover. Use one per view.
- **Quiet link:** underlined text link used next to the primary button for the secondary action.
- **Topic card:** serif title plus one line of ink-soft copy.
- **Step:** a two-digit counter in the serif accent (`01`, `02`, `03`), then a title and one sentence.

## Do's and Don'ts

**Do**
- Write copy in plain, specific language about real HR situations in service businesses.
- Keep one primary action per section and point it at booking.
- Keep the page to one HTML file with inline CSS.

**Don't**
- Add fake testimonials, customer logos, ratings or compliance badges.
- Introduce a second accent hue, gradients or drop shadows.
- Add JavaScript, a build step or extra pages.
