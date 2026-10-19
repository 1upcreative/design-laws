# 04 · Typography

- **Two faces at most.** One display face for headings, one utility face (or a mono) for labels and data. A third face is a smell.
- **One scale.** A fixed type ramp, such as 12.5, 14, 16, 18, 24, 32, 48. Use `clamp()` for the hero, but the stops are still the ramp.
- **Weight for hierarchy.** Bold (600 to 700) headings, regular (400 to 500) body, medium (500 to 650) labels. Do not use color alone to make something a heading.
- **Readable body.** 16px minimum on phones. Line height 1.5 to 1.75 for body, 1.05 to 1.2 for display.
- **Measure follows the container.** Inside full-width blocks, text spans the block. Inside a column, 60 to 75 characters is the comfortable line.
- **Tabular figures** for prices, counts and timers, so columns do not jitter.
- **Title Case** for buttons, labels, nav items and column heads. Sentence case for body, helper text and notes.
- **Letter-spacing** only on small uppercase labels (0.12 to 0.2em). Never tighten body text.
- **Self-host fonts** with `font-display: swap`. Preload only the display weight the hero needs.
