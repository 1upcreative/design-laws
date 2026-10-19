# 08 · Verification: measure, do not eyeball

- **Read the page, not the screenshot.** Bounding boxes, computed styles, scroll widths, font load status. A screenshot proves a moment; a measurement proves a rule.
- **320 x 568 every time.** Document scroll width equals the viewport width, or it fails. Check both orientations.
- **Equal gaps are measured.** Report the pixel values above and below a line, not "looks even".
- **Fonts self-hosted and loaded.** Check `document.fonts` for the weights you use.
- **Images sized.** Width and height or `aspect-ratio` on every image. Lazy load below the fold. Hero gets `fetchpriority="high"`.
- **Reduced motion honored.** Transform and opacity only. 150 to 400ms. Nothing blocks input.
- **Lighthouse 90 or better** on Performance, Accessibility, Best Practices and SEO, mobile and desktop, before launch, and again before every launch.
- **Manual accessibility pass.** Keyboard only, screen reader, focus order, contrast, labels. Automated tools catch about a third.
- **Fingerprint sweep.** Grep shipped files for tool names, assistant names and internal partner names. The code reads as the client's own.
- **Cache stamps.** Build steps stamp css and js links with a content hash so a rebuild is never served stale.
- **Never trust a cached asset.** If a change does not show, check the transfer size before you debug the code.
