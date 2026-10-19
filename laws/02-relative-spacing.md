# 02 · Relative spacing

**Everything is relational in distance to everything else. No guesses, no random spacing. Every gap is either equal to a neighbor or a clean relative of one.**

## The rule

- **Siblings are equal.** Cards in a row, rows in a list, peers in a stack: one gap, the same gap.
- **Levels halve or double.** Inside a group, use half the gap that separates groups. Between chapters, double what separates sections inside a chapter. 100, 50, 100. Or 24, 12, 24.
- **One scale.** Every value comes from the project's spacing scale, such as 8, 16, 24, 32, 48, 72, 112. A value that is not on the scale is a defect, even if it looks fine today.
- **Measure to the visual edge.** A badge that pokes above a card, a card lifted for emphasis, a drop shadow: the eye reads the gap from the first visible pixel, not from the box. Adjust the arithmetic so the visual gap matches.
- **Optical, then arithmetic.** When line height or ascenders make two equal gaps look unequal, nudge until they look equal and write the reason in a comment next to the value.

## How to apply

1. Walk each section top to bottom. For every gap, say its ratio to the gap next to it: 1:1, 1:2 or 2:1.
2. Any gap you cannot name is the markup you will get back. Fix it before showing the work.
3. Put spacing in tokens (`--space-1` through `--space-7`, or a Tailwind scale). Never type a magic number into a component.
4. Document the vertical rhythm once per project: section padding, heading to body, inside a card.

## Example

A proposal label sits between a row of stat tiles and three pricing cards. The middle card lifts 6px and wears a badge that pokes 13px above its top edge. Arithmetic says 32px above and 32px below the label. The eye says the bottom gap is 13px tighter. Fix: bottom margin 32 + 20, so the gap to the badge's top reads 32. Then measure: 32 above, 34 below. Equal.

## Related

- 03 Grid and layout: no excess gaps and no orphaned space. Those say "not too much." This one says "the right amount, in relation."
