# 03 · Grid and layout

## No dead right gap

Capped text inside a full-width container leaves an orphaned strip on the right. That is a defect. Text spans its container. No measure caps (`max-width: 65ch`) inside full-width blocks, and no multi-column splits with gutters through running copy. If a container is full width, its content runs edge to edge, padding aside.

## No stop-short elements

An element whose siblings span the row while it stops short (a badge, a pill, a bar floating with dead space beside it) is a defect at every viewport. Sweep every breakpoint tier, not just desktop.

## Rows fill their grid

In a 12-column grid, every row's spans add to 12. A card at 8 columns with nothing beside it is a dead gap. Give it 12 or give it a neighbor.

## Cards hug content

A sidebar or aside card must not stretch to the height of its neighbor. Set `align-self: start` and `align-content: start`. If the aside should follow the reader, make it sticky below the fixed bars, and make it static under 720px.

## No excess gaps

Do not scaffold a two-line answer. Do not pad a simple block into a report. Big empty regions that exist only because a grid row stretched are "Mr Bean gaps": awkward silence on the page.

## 320 works

Every web-delivered build must be genuinely usable at 320px wide, iPhone SE and cheap Android class. Check 320 x 568 before every ship, alongside both orientations. Page-level horizontal scroll is never acceptable unless deliberate and specified.

Rich pages (3D, HUD, scroll cinema) need a designed degradation ladder: content intact, delight simplified on purpose, never sheared off by accident.

## Grid children never widen the page

A table with a minimum width inside a grid column will push the column wider than the phone unless the child has `min-width: 0` and the table lives in a scrolling wrapper. Set `min-width: 0` on grid and flex children by default.

## Breakpoints

Use a small, consistent set: 375, 640 or 720, 900 or 1024, 1440. Mobile first. Never disable zoom.
