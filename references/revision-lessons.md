# Revision lessons and failure patterns

When a user says a page is “奇怪”“拥挤”“空”“不搭” or “不像话”, diagnose the structural cause before changing the visual surface. The following patterns were repeatedly exposed during the reference project.

## Unrequested invention

**Symptom:** The page contains polished but vague slogans or a new set of grand section headings.

**Cause:** The content was summarized for style instead of mapped to the source hierarchy.

**Correction:** Restore the user's headings and facts. Express the relationship through layout, numbering, or a short evidence label. Do not add a slogan unless the user supplied or requested one.

## Decoration filling a gap

**Symptom:** A new color block, illustration, line, circle, or image appears in an empty area but has no clear relation to the page.

**Cause:** Empty space was treated as a defect before the page's hierarchy was solved.

**Correction:** First check the title baseline, content density, grid tracks, and footer position. Use an image or component only when it explains, proves, or navigates something.

## Removing a component without reflowing the page

**Symptom:** Removing a top navigation row leaves an unexplained blank band; removing a card leaves the remaining content too low or too high.

**Correction:** Recalculate the page composition after every structural deletion. Move the title and main relationship into the freed area, then check the footer and viewport edge.

## Misleading visual relationship

**Symptom:** A path looks like parallel categories, a decorative curve looks accidental, or a circle diagram appears repeatedly without showing order.

**Correction:** Name the relationship first. For serial content use numbered nodes on one line; for parallel content use columns; for a hierarchy use nesting; for multi-factor qualities use a labeled framework. Avoid a component whose geometry contradicts the content.

## Overflow disguised as density

**Symptom:** A block reaches below the viewport or the last line is hidden behind the footer.

**Correction:** Remove duplicated prose, move the value statement below the rules when space permits, narrow image columns only when it improves text wrapping, and reduce padding before reducing type. Validate at the actual viewport size.

## Repeated-component drift

**Symptom:** Similar page titles, footers, navigation labels, or ability components sit at different positions or use inconsistent text.

**Correction:** Make the component global. Keep one source of truth for its wording and states. Use active/inactive styling consistently and remove duplicate labels.

## Image without meaning

**Symptom:** A screenshot is placed in a corner, or a thumbnail is visible but there is no reason to click it.

**Correction:** Attach the image to the method, case, or node it documents. Use a gallery when multiple images belong to one point. Preserve high-resolution access and test both the trigger and the close behavior.

## Changing too much at once

**Symptom:** A request to change one title or one image causes unrelated spacing, colors, or sections to move.

**Correction:** Scope the patch to the requested element. If a broader layout change is genuinely necessary, explain the dependency and propose it separately.

## User screenshot as evidence

When a screenshot is supplied, use it to locate the actual defect. Compare it against the intended page role and global system. Do not assume the screenshot is merely an aesthetic preference; it may reveal clipping, wrong ordering, stale navigation, or a mismatch between the source structure and the rendered page.
