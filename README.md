# Design Laws

Plain-English design rules for web builds, written so a human **or an AI coding assistant** can follow them. They come from the Bauhaus school and the Swiss grid, tightened by shipping real sites and products with an AI pair.

If you build with Claude Code, Cursor, Copilot or any assistant, drop these in and your assistant stops guessing at spacing, contrast and controls.

## What is in here

| File | What it covers |
|---|---|
| `SKILL.md` | A drop-in skill for Claude Code. The laws, condensed, with a pre-ship checklist. |
| `laws/01-foundations.md` | Bauhaus and Swiss grid, in plain words. Why the rest exists. |
| `laws/02-relative-spacing.md` | Every gap is equal to a neighbor or a clean multiple of one. Never random. |
| `laws/03-grid-and-layout.md` | 1440 desktop standard, full-width text, no dead right gap, no stop-short elements, 320px works. |
| `laws/04-typography.md` | Two faces, one scale, weight for hierarchy, readable measure. |
| `laws/05-color-and-contrast.md` | Palettes come from the color wheel. Ink on an accent comes from the math. Drop shadows as duct tape. |
| `laws/06-controls.md` | Carets inset from the edge, the status pill is the control, grips not arrows, mark AI actions. |
| `laws/07-density-and-copy.md` | No cricket text, no redundancy, chunked content, fifth-grade how-tos. |
| `laws/08-verification.md` | Measure, don't eyeball. Both orientations, 320, reduced motion, Lighthouse. |
| `laws/09-markup-driven-design.md` | Design as live HTML, red-pen screenshots, rebuild each markup. The loop. |

## Install as a Claude Code skill

```bash
git clone https://github.com/1upcreative/design-laws ~/.claude/skills/design-laws
```

Then in any session: `/design-laws` loads the condensed rules, or just build a page and the skill description will pull it in when layout, spacing, color or controls are on the table.

For Cursor or others, paste `SKILL.md` into your rules file. The laws are tool-agnostic.

## The one-sentence version

**Everything on the page is relational: every distance, size and weight is equal to a neighbor or a clean multiple of one, every color pair passes the math, every control looks like what it does, and nothing ships until it is measured at 320px.**

## Why this is free

Whatever we know that we can share, we do. These rules were paid for with real shipped work; passing them on costs nothing and helps the next builder and their assistant skip the same hills. Love your neighbor, share your notes.

> "Love the LORD your God with all your heart and with all your soul and with all your strength."
> — Deuteronomy 6:5

## Contributing

Open an issue with the rule, the why, and one example of it breaking. Rules without a why do not get in.

## License

MIT. Use them, teach them, fork them.
