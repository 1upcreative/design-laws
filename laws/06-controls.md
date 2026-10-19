# 06 · Controls

## The caret is inset

Every dropdown, select and combobox draws its own chevron, inset 14px from the right edge, with `appearance: none` and enough right padding (40px) that text never runs under it. One shared rule per codebase on the base select selector. The browser's edge-hugging native caret is a defect.

## The status pill is the control

A record's status pill is tappable. Tap it, see every status with the current one checked, pick, done. Publish, unpublish, backgrade, any status, any moment. Statuses that need input open their modal from the same menu. Server-side rules still govern; the pill routes to the same endpoints.

## Grips, not arrows

Reordering uses a grip handle: drag with the mouse, drag with touch through a pointer fallback, and move with arrow keys when the grip has focus. No up and down arrow buttons. Keyboard users lose nothing when the visible arrows go.

## Buttons

Outlined by default. One primary (filled accent) per screen. Back actions carry a left arrow. Destructive actions sit apart and wear the danger color. Buttons that submit show a loading state and disable until the response lands.

## Mark AI actions

Any control that hands work to an AI, a switch, a button, a banner offer, wears one shared mark (a four-point sparkle) applied by one class. Mentions of past AI work do not get the mark; only the places where the person chooses AI. In onboarding, AI switches default on; the person can turn them off.

## Locked-on choices

When a thing comes with every plan, show it as a switch that is on and disabled, with a lock mark and a pill that says so. Never let someone un-choose what they are paying for.

## Doors, not sidebars

Live previews belong behind two tiles (Desktop, Mobile) that open a modal, not in a sidebar that stretches the page. Close, Escape and the backdrop all shut it.

## Basics that never slip

Touch targets 44px or larger with 8px between them. Visible focus rings. Every icon-only button has an accessible label. Every input has a visible label, not a placeholder standing in for one.
