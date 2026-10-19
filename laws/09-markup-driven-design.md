# 09 · Markup-driven design: the loop

Hand-drawn wireframes are optional when the live version can be the wireframe.

## The loop

1. Build the screens as real HTML on a local bench and, if you have one, a staging URL. Section files plus a small build script that assembles one page and runs gates (contrast, forbidden words, cache stamps).
2. The reviewer looks at the bench, screenshots, and red-pens: circles, arrows, two words.
3. The assistant reads the markup, applies it, measures (desktop and 320, no overflow, the laws above), commits, and replies with what changed in three lines.
4. Repeat. One markup, one commit.

## Rules of the loop

- Questions get answered, not built. "Should we use X?" is not "migrate to X."
- A musing about how something should work is not a build order until it is confirmed.
- Never break what already works as a side effect of a markup. If a change touches a working flow, flag it first.
- Every product decision made during markup gets logged the same session, with the date, in plain words.
- Nothing deploys to a client-facing address until the reviewer has seen it on the bench and said go.

## Why it works

The live version already obeys the laws as it goes. Static comps have to be re-drawn into code later and the laws get re-learned; the bench carries them forward. The result is reusable markup, not a picture of markup.
