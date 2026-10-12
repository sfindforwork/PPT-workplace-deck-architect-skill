# Source-to-slide decomposition

The most important job is to preserve the author's reasoning while reducing the reading burden. Do not start with visual components. Start with a traceable content map.

## 1. Read the hierarchy as structure

When a source uses headings such as `1 → 1.1 → 1.1.1 → 1.2`, treat them as semantic structure:

- top-level headings define chapters or major arguments;
- second-level headings define the main content units of a chapter;
- third-level headings define evidence, methods, cases, or sub-arguments.

Use the source headings directly unless they are too long for a page title. If shortening is necessary, preserve the original meaning and keep the original wording in a supporting label or speaker notes.

The hierarchy is a source map, not a presentation chrome system. Do not expose a chain such as `1.2.1 → 1.2.2 → 1.2.3` as the main visual route: it makes the deck feel like a paper outline and forces the audience to decode numbering. Instead, show the chapter index once, use a human-readable page title and a concise page-role label, and let the relationship between pages be carried by order, section navigation, repeated layout, and meaningful components. Keep the original node path in the source-to-page map, presenter notes, `data-source` metadata, or a small secondary reference when auditability matters.

Do not replace a clear source heading with an invented title such as “从认知到增长” or “把需求做成一条路”. Those may sound polished but can hide the actual structure and make the deck feel like an advertisement.

## 2. Make a source-to-slide map

Before building, create a compact map with these fields:

| Field | Question |
|---|---|
| Source node | Which exact heading and paragraph does this come from? |
| Page role | Is this a chapter cover, overview, method, case, summary, or plan? |
| Main point | What should the viewer understand after one glance? |
| Evidence | Which facts, cases, images, or numbers must remain? |
| Relationship | Are the contents sequential, parallel, causal, comparative, or hierarchical? |
| Visual form | Which component makes that relationship easiest to read? |
| Page budget | Which explicit page count or outline constraint applies? |

Keep enough detail in the map to trace every important slide statement back to the source. Do not use the map to create new claims.

## 3. Abstract at the right level

Use the following transformation:

```text
long paragraph
  → one source-faithful claim
  → two to four evidence points
  → a visible relationship between those points
  → a concise slide layout
```

Do not collapse a detailed argument into a single vague sentence. Do not preserve every sentence as a bullet either. Important cases and constraints should usually remain as evidence below the main claim.

For a method or learning section, distinguish:

- what was done;
- what rule or method was learned;
- what the method is useful for;
- what ability or outcome it supports.

For a summary section, distinguish improvement, limitation, case, cause, direction, and execution. Do not put all of them into one undifferentiated paragraph.

## 4. Respect explicit page allocation

If the outline says a content unit occupies one page, solve density with hierarchy and layout before proposing another page. Typical compression tools are:

- a two-column relationship;
- a short lead plus a structured evidence list;
- a timeline or process line;
- an evidence thumbnail that opens at full resolution;
- a compact matrix with repeated labels.

Only propose a split when the page would otherwise make the main relationship unreadable. Explain what would move to the new page and ask before changing the page budget.

## 5. Verify the narrative from the viewer's perspective

For every page, answer:

1. Where am I in the overall presentation?
2. What is this page's one main job?
3. What relationship connects the visible parts?
4. Which details support the main point rather than compete with it?
5. What should I understand before moving to the next page?

As a visual QA check, hide the decimal source numbers and look at the page by itself. If the viewer cannot tell the page's role without the numbers, strengthen the chapter index, title wording, or component relationship instead of restoring more numbering.

If these answers are not obvious from the page, revise the hierarchy before decorating it.
