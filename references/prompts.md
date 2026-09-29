# Reusable Prompts

Use these as starting points. Replace bracketed fields and keep the supplied source text attached to any visual reconstruction request.

## 1. Visual Reference

```text
Create one professional 16:9 slide visual reference for the content below.
Audience: [audience]
Purpose: [what the audience should understand or decide]
Core message: [one sentence]
Show a clear hierarchy, generous whitespace, and a visual structure suited to this page (for example, a study timeline, comparison, or process diagram). Keep the main text areas and complex illustration visually separable. Use only the facts and values in the source; do not invent labels, numbers, outcomes, or citations. Keep text concise and legible. If exact Chinese text cannot be rendered reliably, use a neutral placeholder rather than approximate characters; the final PowerPoint text will be rebuilt from the source.

Source text:
[paste the approved page content and source/version]
```

## 2. Rebuild as Editable PowerPoint

```text
Use the supplied slide image only as a layout and visual-style reference. Rebuild it as a 16:9 editable PowerPoint slide and save a .pptx.

Use the source text below as the only authority for wording, values, and conclusions. Create separate native PowerPoint text boxes for the title, body, labels, numbers, captions, and footnotes. Use native shapes for simple frames, lines, and arrows. Use editable chart objects for data charts when feasible. Keep complex illustrations as separate image objects, never as a flattened full-slide background. Preserve the main hierarchy and composition while making text readable and avoiding overlaps.

After building, report which elements are native/editable and which remain images. Render the slide and check for clipping, text overflow, and content mismatches.

Source text:
[paste the approved source text]
```

## 3. Deck QA and Repair

```text
Review this PowerPoint against the approved outline and source/fact ledger. Do not introduce new content.

1. Compare names, values, dates, units, denominators, statistical notation, qualifiers, conclusions, and citations slide by slide.
2. Render every slide and identify clipping, overlap, unreadable text, contrast problems, layout drift, and inconsistent components.
3. Check that key text, values, charts, and simple diagrams are separate editable PowerPoint objects, and identify anything flattened into an image.
4. Fix only errors that are clearly supported by the source. List unresolved ambiguities rather than guessing.

Return the repaired PPTX, a concise issue log, and the editability limits.
```
