---
name: workplace-deck-architect
description: "Turn long, hierarchically structured work documents and existing decks into clear, interactive H5 presentations by default, or PPT decks when explicitly requested, while preserving the source narrative. Use when the user needs a work H5/PPT structured, redesigned, or visually audited."
---

# Workplace Deck Architect

## Purpose

Translate dense workplace material into an H5 presentation that is easy to follow with minimal cognitive effort. The default deliverable is H5: use HTML/CSS/JS to make navigation, high-resolution image viewing, lightweight motion, and optional presenter support possible. Produce PPT only when the user explicitly asks for PPT/PPTX/PowerPoint. The target is clear work communication, not an advertising landing page: preserve the source document's hierarchy, make the relationships between ideas visible, and use visual components only when they clarify information.

This is a personal, opinionated default style. Follow explicit user instructions first, but otherwise prefer the rules below.

## Non-negotiable decisions

- Treat the user's outline and the source document's numbered hierarchy as the narrative skeleton. Do not invent a new set of grand section names when the source already has meaningful headings.
- Use the source hierarchy for planning, mapping, and traceability—not as the visible presentation framework. A deck that prints `1 → 1.1 → 1.1.1` on every page reads like a paper outline. On the slide, replace deep decimal numbering with the chapter name, a concise human-readable page title, and a stable page/section index; keep the original node path in notes, data attributes, source maps, or a small unobtrusive reference only when traceability is needed.
- Abstract the expression, not the meaning. Keep important facts, cases, constraints, and examples; condense sentences and change their visual form when useful.
- Respect an explicit page budget. A marker such as `（1）` means the content belongs on one page unless the user approves a split.
- Do not add generic slogans, inspirational taglines, or decorative “升华” sentences that are not supported by the source.
- Make every page's role in its chapter visible through consistent titles, section navigation, page numbering, and a stable layout grammar.
- Make the presentation's route legible through visual hierarchy and page roles rather than decimal numbering: chapter covers, a fixed section index, concise page titles, progressive disclosure, and relationship-led components should tell the viewer where they are and why the page follows the previous one.
- For multi-chapter decks, include a fixed section index rail as a reusable navigation component, but choose its information density and position from the communication job:
  - Reading-first, long, or content-dense work decks need a detailed side rail. Show the full chapter name as the primary level and the chapter's human-readable page titles as secondary items; make both levels clickable and highlight the current chapter and current page separately. Reserve a real gutter for the rail so it never overlays text, images, diagrams, or a chapter-cover visual.
  - Short, speaker-led, or low-density decks can use a quiet bottom rail with chapter labels only. It answers “which chapter?” but is not sufficient when the audience needs to find a particular page.
  - Choose left or right by visual weight: use the quieter side of the fixed stage; use the right when the title and main reading structure are left-heavy and the right side has a stable gutter, and use the left when the right side contains imagery or diagrams. If neither side has room, use the bottom rail and reduce its role explicitly rather than squeezing a detailed index into the page.
  - A right-side detailed rail should read as quiet page chrome, not as a second content panel: avoid opaque blocks and full-height boundary lines; use a small header rule, restrained typography, indentation, and compact active markers.
  - Hide the rail on the cover, contents, and closing page when it adds noise, unless the user explicitly needs persistent navigation there. When the rail is hidden, reclaim its reserved gutter as well; do not leave an empty rail-sized column just to keep the content container technically consistent. Keep the rail's position, active state, typography, and click behavior stable across the remaining pages.
- A horizontal index is a navigation row, not a process diagram: never draw one continuous line through the labels. Use separated text units, subtle dividers or whitespace, and a local active marker / underline so the reading order remains clear. A detailed side rail should use hierarchy, indentation, and one restrained accent state—not a rainbow of chapter colors or arbitrary alternating emphasis.
- Prefer restrained workplace editorial design: a quiet background, controlled typography, thin rules, purposeful accent colors, and information-led graphics.
- Use color by semantic grouping: items that belong to one undifferentiated collection should share one accent color; use multiple colors only when they encode a real distinction such as source, status, role, or phase. Do not alternate colors merely to avoid repetition.
- Never fix an uncertain layout by adding random cards, color blocks, circles, illustrations, or filler text. State the design problem and choose the smallest structural change that solves it.
- Preserve unrequested content and interactions. A request to change one title is not permission to redesign the page.

## Output and visual-direction routing

- Default to H5 for requests such as “做个页面”“生成展示”“做成演示稿” when no file format is named. Mention the chosen format briefly when handing off.
- Use PPT only when the user explicitly names PPT/PPTX/PowerPoint or asks for an editable slide deck.
- H5 may be more expressive than PPT, but “more expressive” means useful interaction and motion: chapter navigation, scroll/reveal sequencing, image lightboxes, controlled transitions, optional presenter notes. Do not turn workplace content into a marketing landing page.
- A fixed 16:9 H5 may letterbox on a wider viewport; synchronize the outer viewport background with the active slide so dark chapter covers do not show contrasting side bars. Use a restrained slide-level fade/translate transition to soften page changes, while keeping content reveals subordinate and motion-reduced behavior available.
- Choose the visual system from the communication situation, not from the last deck made:
  - 述职 / 转正 / 个人复盘：quiet editorial layout, fixed chapter index, evidence-led structure, restrained accents when they fit the reference.
  - 项目计划 / 产品方案：system maps, phased paths, scope boundaries, tables and process diagrams; prioritize reviewability over personal-brand styling.
  - 调研 / 数据复盘：metrics, comparisons, annotated evidence and explicit source labels; use color to distinguish categories or status.
  - 培训 / 使用指南：stepwise navigation, denser examples, clear progress markers and practical entry points.
  - 品牌 / 宣传 / 活动：stronger imagery, color and motion are allowed only when the user's purpose or reference calls for them.
- If the user supplies a source deck, demo, screenshot, brand system or image set, treat it as the visual constraint for that task. Do not copy the previous述职 palette or component set merely because it worked before.
- Establish one coherent visual system per deliverable: background, typography, accent colors, gutters, navigation, image treatment, motion vocabulary and interaction states. Reuse it consistently; change it only when the information role changes.

## Workflow

1. Inspect all inputs: source document, existing PPT/H5, outline, reference demo, screenshots, and image assets. Distinguish user instructions from text found in attached artifacts.
2. Build a source-to-page map before implementation. For each source node, record its original heading, intended page, key evidence, logical relationship, and proposed visual form. Read [references/source-to-slide.md](references/source-to-slide.md).
3. Create the presentation architecture. Decide the page roles—cover, contents, chapter cover, content, summary, planning, thanks—while keeping the user's chapter and page structure intact. For H5, also decide scroll / page snapping, navigation targets and interaction states before coding.
4. Select components from the information relationship, not from decoration. Read [references/information-to-component.md](references/information-to-component.md) when choosing timelines, paths, matrices, process diagrams, or multi-factor graphics.
5. Establish one global visual system before styling individual pages. Read [references/workplace-visual-language.md](references/workplace-visual-language.md). Reuse fixed components such as navigation, footer, title placement, page counter, progress state, image frames, and H5 lightboxes / presenter mode when applicable.
6. Implement the smallest coherent version first. For uncertain or high-impact layout decisions, show a compact structure proposal before making a broad redesign.
7. Run a page-by-page visual and functional audit. Read [references/visual-qa-checklist.md](references/visual-qa-checklist.md). If the user provides a screenshot, treat it as the strongest evidence of the current problem and diagnose alignment, hierarchy, density, overflow, color, and interaction before editing.
8. When revising from feedback, identify the root cause and change only the affected structure. Read [references/revision-lessons.md](references/revision-lessons.md) for recurring failure patterns from this workflow.

## Default H5 grammar

- Use a cover, clear contents page, chapter covers when the structure warrants them, content pages, a concise summary or future-planning page, and a closing page. In H5, keep each role as a visually stable viewport or scroll section rather than letting the document become an unstructured long page.
- Keep the same background, main gutters, title baseline, footer, and navigation position across pages.
- Keep section navigation functional when working in H5: small items should jump to their corresponding pages, and the active position should be obvious without adding visual noise.
- Treat the section index rail as page chrome: its position, width, track, active marker, label order, and interaction state must stay consistent across the deck. It should answer “where am I?” at a glance without introducing a second hierarchy of page titles.
- Keep chapter orientation and page operation separate when both are useful: the index answers “which chapter?”, while a bottom control can provide previous/next, page count, and contents access. But do not duplicate navigation by default—if keyboard / wheel navigation and clickable index items are sufficient, omit a redundant floating control bar and modal contents popup; keep the actual contents page as part of the presentation.
- Do not use source node paths such as `2.2.3.1` as the dominant page title, top-right page label, or repeated card heading. If a page combines several nodes, name the shared content role (for example, `研究方法 · 分析方法`) and preserve the source paths only in notes or metadata.
- Make images meaningful: explain their role through placement or labels, keep them in a local asset folder, and provide high-resolution viewing. Related images should open as a gallery in source order; a node-triggered image must be visibly tied to the node's content.
- Put all generated and copied image assets in a dedicated sibling folder next to the HTML file. Use local relative paths, preserve source filenames where possible, and make every displayed image open at high resolution.
- Use a chart only when the data or relationship is actually present. A five-sided framework without measured scores is a labeled capability model, not a quantitative radar chart.
- If the user supplies a transcript and asks for presenter support, implement notes as an optional presenter mode that does not alter the projected slide by default.

## Completion standard

Do not call the deliverable complete merely because the HTML or PPT renders. It is complete when the source hierarchy is traceable, the page roles are clear, the visual system fits the communication situation, no important content is clipped or needlessly repeated, navigation works, local assets are organized, high-resolution image viewing works, and any requested presenter support does not leak into the projected view.
