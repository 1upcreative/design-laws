---
name: design-laws
description: Design rules for web layout, spacing, typography, color, controls and copy, rooted in Bauhaus and the Swiss grid. Use when building or reviewing any page, component, comp or wireframe, when choosing spacing or colors, and before shipping anything people will see.
---

# Design Laws (condensed)

Read `laws/` for the why and the examples. This file is the checklist your assistant should hold while it works.

## 1. Everything is relational
- Every gap is **equal** to a neighbor or a **clean relative** of one (half, double). No random numbers.
- Siblings get the same gap. Inside a group, half the gap that separates groups.
- All spacing comes from one scale (for example 8, 16, 24, 32, 48, 72, 112). A value off the scale is a defect.
- Measure to the **visual** edge: a badge that pokes above a card, a lifted card, a shadow. The eye reads the visible pixel.
- Before showing work, name the ratio of every gap to its neighbor: 1:1, 1:2, 2:1. If you cannot name it, fix it.

## 2. Grid and layout
- **1440 is the desktop review width.** Every layout must fit there. Public pages share one container: 1240px + `clamp(16px, 4vw, 48px)` gutters. Admin apps may run wider.
- Text spans its container. No measure caps inside full-width blocks, no column gutters splitting running copy.
- No element stops short while its siblings span the row. No dead right gap, at any viewport.
- No equal-height stretching of a sidebar or aside card just because its neighbor is tall. Cards hug content.
- Must work at **320px** wide: usable, not merely unbroken. Page-level horizontal scroll is a defect, always.
- Rich pages get a designed degradation ladder down to 320: content intact, delight simplified on purpose.

## 3. Typography
- Two faces at most: one display, one utility or mono for labels. One type scale.
- Hierarchy by size and weight, not by color alone. Bold headings, regular body, medium labels.
- Body at least 16px on phones. Line height 1.5 to 1.75 for body. Tabular figures for numbers in columns.
- Title Case for buttons, labels and nav. Sentence case for body and helper text.

## 4. Color and contrast
- Ink on an accent fill comes from the contrast math, never a literal. Compute the on-accent ink (white or near-black) per accent, and darken the fill until it clears 4.5:1 if white wins.
- Every text pair passes WCAG AA. Dark mode gets its own check; do not invert light-mode values.
- Pick the palette from the color wheel: complementary (brand + the color across the wheel), monochrome (one hue in steps), or three evenly spaced colors. Neutrals are even black-to-white steps (90%, 80%, 70%…). A color that fits none of these does not get in.
- One accent carries meaning. A second accent from the scheme (the complement, in a complementary palette) marks "needs confirmation" or "prototype". That is the whole palette.
- A weak logo on a background gets a drop shadow at the template level. Never recolor a brand.
- Color is never the only signal. Pills carry a dot and a word, deltas carry an arrow and a word.

## 5. Controls
- A dropdown draws its own chevron, inset 14px from the right edge, with `appearance: none`. Never the browser's edge-hugging caret.
- The status pill **is** the control: tap it, pick any status in one hop. No hunting through menus.
- Reordering uses a grip handle: drag, touch fallback, arrow keys on the focused grip. No up and down arrow buttons.
- Buttons are outlined by default; one primary per screen. Back actions carry a left arrow.
- Any control that hands work to an AI wears one shared mark (a sparkle), applied by one class. Never an inline one-off.
- Touch targets at least 44px. Visible focus rings. Every icon-only button has a label.

## 6. Density and copy
- No cricket text: nothing under 12.5px, no gray on gray.
- No redundancy: say a thing once on a screen. If the section is titled "Colors", the labels are "Main", not "Main color".
- Chunk content: one idea per section, one number row at most, one call to action at most.
- Instructions and how-tos read at a fifth-grade level. Jargon stays in the engineering room.
- Run outbound copy through a slop filter: no filler, no hedging, no "delve".

## 7. Verification (before you say done)
- Measure, do not eyeball: read bounding boxes, computed styles and scroll widths from the page.
- Check 320 x 568 and both orientations on every responsive change.
- Honor `prefers-reduced-motion`. Animations use transform and opacity only, 150 to 400ms.
- Fonts self-hosted, images sized with width and height, below-the-fold media lazy.
- Lighthouse 90 or better on all four categories, mobile and desktop, before launch. Automated accessibility catches about a third; do the manual pass.
- Sweep shipped files for tool fingerprints and internal names. The code should read as the client's own.

## 8. The loop
- Design as live HTML on a bench. The reviewer red-pens screenshots. Apply each markup, measure, commit. One markup, one commit.
- Questions get answered, not built. A musing is not a build order until it is confirmed.
- Never break what already works as a side effect. Flag first, then change.
