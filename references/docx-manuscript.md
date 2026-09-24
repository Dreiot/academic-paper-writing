# Academic manuscript DOCX production

Read this reference when creating a new academic manuscript in DOCX or making substantial content or layout changes to an existing one. These rules specialize the general document-authoring workflow for journal manuscripts; they do not apply to a text-only response or a minor wording edit that does not touch the file.

## Resolve formatting authority

Use the following order:

1. the user's explicit instructions;
2. the current official journal requirements and an official or user-supplied journal template;
3. the source manuscript's established working styles;
4. the neutral academic fallback below.

If current official instructions and a supplied template materially conflict on a submission requirement, identify the exact conflict before finalizing the affected formatting. Do not replace a working journal template with a generic document design, colored report styling, or a default office theme.

## Inspect the document before editing

For an existing DOCX, inspect the page size, margins, sections, columns, headers and footers, paragraph and character styles, table styles, captions, bibliography style, math settings, fields, bookmarks, comments, and tracked changes that the requested edit may affect.

Do not assume that a localized or externally generated template contains English built-in style names such as `Table Grid`, `Caption`, or `Bibliography`. Resolve styles by their actual role and available identifiers. If a named style is absent, reuse a verified equivalent or apply the required formatting explicitly; a missing English style name is not by itself a reason to block saving.

Before editing citations or bibliography content, check whether the document contains live reference-manager fields. If Zotero fields are present or Zotero use is requested, follow [zotero.md](zotero.md).

## Use restrained academic fallbacks

When no user or journal formatting authority exists:

- Use A4 portrait for a new Chinese-first manuscript. Preserve an existing manuscript's page size unless the user asks to change it.
- Keep ordinary body text and headings black and use the smallest practical style set, distinguishing hierarchy through size, weight, spacing and numbering. This prose-layout default does not force scientific figures or data encodings into monochrome; use journal-appropriate color under [scientific-figures.md](scientific-figures.md). Follow an explicit grayscale requirement when one applies.
- For Chinese titles, section headings, body text, table text, algorithm text, and ordinary captions, set East Asian runs to SimSun and Western letters, digits, and Western punctuation to Times New Roman. Use weight, size, and spacing—not a different font family—to distinguish heading levels. Apply fonts at the relevant style and run levels so mixed-script text remains deterministic.
- Set explicit `ascii`, `hAnsi`, and `cs` fonts to Times New Roman and `eastAsia` to SimSun on the title and heading paragraph styles and their linked character styles. Remove or override `asciiTheme`, `hAnsiTheme`, `eastAsiaTheme`, and `cstheme` values that can reintroduce Calibri, MS Gothic, or another theme font. Use an appropriate Simplified Chinese East Asian language setting for Chinese headings rather than relying on theme-language fallback, and normalize direct run formatting that conflicts with the intended style.
- For a new English manuscript without a venue template, use Times New Roman for Western body text. Choose readable sizes and spacing from the manuscript's purpose rather than forcing a universal journal size.
- Follow the journal or established manuscript treatment for tables. Otherwise use a restrained academic three-line treatment without vertical rules for a submission-grade Chinese master manuscript; use a full grid only when the data structure, accessibility needs, or target venue calls for it. Do not apply `Table Grid` merely because it is a familiar built-in name.
- Size columns deliberately, repeat multi-page header rows, and vertically center cells. For Chinese manuscript tables, unless a formatting requirement specifies otherwise, use regular-weight table titles/captions and horizontally center cell contents, including header and data cells. Set all cell paragraphs to single line spacing and zero after-spacing in both points and lines; clear or override inherited line-based (`afterLines`) and automatic after-spacing so body or table styles cannot reintroduce it. The caption rule does not remove meaningful emphasis within cells. For other manuscripts, left-align narrative labels and center or decimal-align compact numeric values as appropriate.

Format algorithms and pseudocode as an academic three-line table by default: a top rule, one deliberate separator after the algorithm title or header block, and a bottom rule, with no vertical borders or boxed body rows. Keep the algorithm title, input, output, and numbered steps structurally together. Use plain step numbers rather than bullet glyphs, and do not simulate the algorithm with a loose sequence of ordinary paragraphs and horizontal lines.

Do not apply `keep_with_next`, `keep_together`, or `page_break_before` indiscriminately to every paragraph inside a table or algorithm. Use caption-to-table keeping, repeating header rows, row-level no-split behavior, or targeted pagination only where needed. Remove accidental list formatting and bullet glyphs from table cells. Word's table move handle and formatting-mark indicators are editing-interface elements, not printable document content; verify the exported page rather than trying to encode or erase a UI handle. If widespread black-square paragraph markers are caused by unnecessary pagination flags, remove those flags while preserving intentional page behavior.

Body-font defaults do not determine the Word mathematics font. Preserve a working template math configuration or apply the journal-required math font consistently; do not change the document math font to Times New Roman solely because Western prose uses Times New Roman.

## Preserve academic document structure

- Keep figure, table, equation, section, and bibliography identities stable unless renumbering is part of the request.
- Preserve `SEQ`, `REF`, `PAGEREF`, citation, bibliography, and other live fields, together with their bookmarks and relationships.
- Do not flatten fields, accept tracked changes, remove comments, or convert a dynamic bibliography to static text unless the user explicitly requests that result.
- Avoid whole-paragraph replacement when a paragraph contains live fields, comments, bookmarks, or tracked changes. Use a field-preserving Word or targeted OOXML edit path.
- Treat a clean manuscript, marked manuscript, supplement, and response letter as distinct deliverables. Do not overwrite the source or confuse the marked copy with the primary clean copy.

When inserting a figure, determine its intended single-column, double-column, or page-text width before setting the size. Preserve the source aspect ratio, keep the image within the available text area, and avoid defaulting every figure to full-page width. At the actual insertion size, labels, line weights, symbols, and panel letters must remain readable without excessive zoom. If a figure becomes unreadable when it fits the page, simplify, recompose, or split it instead of shrinking it further. Keep the figure and caption visually associated and re-render the page to check white space, sharpness, wrapping, and page breaks.

## Render with the tool that matches the deliverable

When Microsoft Word is available and the requested deliverable is a Word manuscript, use Word to open or export the final DOCX and inspect the resulting pages; Word is the primary fidelity check for its native format. Close Word documents and automation handles after export so temporary and final files are not left locked.

Use the packaged LibreOffice renderer when it is available and useful as a fallback or cross-platform compatibility check. Do not require the user to install desktop LibreOffice solely to complete a Word manuscript when Word provides a verified render path. If both renderers are available, compare them only when cross-renderer portability materially affects delivery.

After a local layout-sensitive correction, render and inspect the affected pages and adjacent pages. Reinspect the whole document when the change affects global styles, sections, fields, pagination, repeated elements, or other document-wide behavior. For final delivery, ensure verification covers all pages of the latest file at readable zoom; reuse unaffected page checks after local corrections only while their content and layout remain unchanged. If no visual renderer is available, complete content and structural OOXML checks and deliver with an explicit statement that visual QA was not completed; do not claim a visual pass. Visual verification blocks completion only when the user explicitly requires it. Retry failed rendering only after a concrete diagnosis or changed condition.

## Validate the final manuscript

Confirm, in proportion to the task, that:

- the final DOCX opens successfully in Word and uses the intended page geometry and styles;
- mixed Chinese and Western fonts are explicit and consistent where the fallback applies;
- title and heading styles do not resolve through theme fonts to Calibri, MS Gothic, or another unintended family;
- tables and algorithms fit the page, use the intended three-line structure, contain no accidental bullets or pervasive pagination markers, and do not depend on a missing style name;
- Chinese manuscript tables follow the caption-weight, cell-spacing, and alignment defaults above unless an applicable formatting requirement overrides them; inspect effective formatting, not only the assigned style name;
- figures, tables, equations, captions, numbering, bookmarks, and cross-references agree;
- figures are inserted at an appropriate document size with preserved aspect ratio, readable labels, sufficient effective resolution, and stable caption placement;
- live citation and bibliography fields remain live when they were present initially;
- every required equation is editable OMML and no raw LaTeX or pseudo-math remains;
- numerical values and emphasis match the authorized evidence;
- any page or line locations cited in a response letter are verified only after final pagination;
- the delivered clean, marked, supplementary, and response files have unambiguous roles.
