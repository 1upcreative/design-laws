# 05 · Color and contrast

## Accent ink comes from the math

The text color placed on an accent fill is never a literal. Compute it:

1. Measure the accent's contrast against white and against near-black.
2. Use near-black only when it clears 7:1 and beats white. Mid blues and teals measure a hair better with black yet read worse, so white wins the tie.
3. If white wins but does not clear 4.5:1, darken the fill until it does. Keep the brand hue; change the fill, not the rule.
4. Expose the result as two tokens, `--accent-ink` and `--accent-fill`, and let every button and pill read them.

Put a test on it. A build that lets an accent pair drop under 4.5:1 should fail.

## Every pair passes AA

Body text at 4.5:1 or better, large text at 3:1. Check dark mode on its own. Do not invert light-mode values; use desaturated, lighter tonal variants.

## One accent carries meaning

One brand accent for actions and "live". One second accent (amber) for "needs confirmation" or "prototype". Red only for danger. That is the palette. More colors, less meaning.

## Color is never the only signal

Pills carry a dot and a word. Deltas carry an arrow and a word. Status is readable in grayscale.

## Drop shadows are duct tape

When a brand mark reads weak on a background (light on light, gold on tan), do not recolor the brand. Lift it with a drop shadow at the template level so the whole family stays consistent. `filter: drop-shadow(0 3px 7px rgba(0,0,0,.5))` rescues most logos in one line.

## Dark surfaces

Avoid pure `#000`. Use a deep ink with a hint of the brand hue. Surfaces step up in two or three tones. Borders are visible in both themes.
