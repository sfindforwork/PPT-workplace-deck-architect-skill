# Visual and functional QA checklist

Run this checklist after generation and after any meaningful layout change. A rendered page is not finished until the deck is readable, coherent, and interactive.

## Source fidelity

- [ ] Every major page title maps to a user-provided or source-document heading.
- [ ] The page order follows the approved outline.
- [ ] Explicit page counts are respected.
- [ ] Important facts, cases, constraints, and current-state qualifiers remain present.
- [ ] No unsupported conclusion, slogan, metric, or capability claim was introduced.

## Page architecture

- [ ] Cover, contents, chapter covers, content pages, summary/planning, and closing page have clear roles.
- [ ] The active chapter and current page are obvious.
- [ ] Each page has one dominant relationship that can be described in one sentence.
- [ ] The title, body, evidence, and footer are in a clear reading order.
- [ ] Similar pages use matching title positions and title sizes.

## Visual system

- [ ] Background color is consistent unless a deliberate section change was approved.
- [ ] Main gutters, page markers, footer, navigation, and page counter align across pages.
- [ ] Accent colors have stable semantics; no unexplained one-off color appears.
- [ ] Lines and borders separate real groups rather than decorate empty space.
- [ ] Components are not repeated beyond what the information requires.
- [ ] The page does not resemble an advertising landing page.

## Density and viewport

- [ ] No text, image, border, or footer is clipped at the target viewport.
- [ ] No content is hidden behind controls, navigation, or the footer.
- [ ] Large empty areas have a structural reason.
- [ ] Image and text columns are balanced; neither is squeezed only to preserve a decorative image.
- [ ] Mobile or narrow layouts scroll intentionally and do not create horizontal overflow.

## Images and interactions

- [ ] Every referenced image exists in the local asset directory.
- [ ] Visible thumbnails preserve an appropriate aspect ratio.
- [ ] Images that need detail open at high resolution.
- [ ] Related images open in the correct order and under the correct label.
- [ ] Gallery, lightbox, slideshow, and close interactions work with mouse, keyboard, and ESC where applicable.
- [ ] Image alt text or accessible labels describe the actual image or content node.

## Implementation sanity

- [ ] The expected number of slides/sections is present.
- [ ] Navigation targets still resolve after reordering.
- [ ] Page counters match the actual order.
- [ ] HTML/JavaScript parses without errors.
- [ ] No stale class, placeholder, duplicate component, or old content remains after a redesign.
