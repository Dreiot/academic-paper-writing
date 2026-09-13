# Zotero-aware citation workflow

Read this reference when the user explicitly asks to use Zotero, a DOCX contains live Zotero fields that the task may affect, or a needed citation should be retrieved from the user's local Zotero library. Use the installed Zotero capability for library operations when it is available.

## Trigger Zotero proportionately

- Use Zotero for a targeted local-library search, item verification, BibTeX export or synchronization, or citation insertion into supported LaTeX and Markdown drafts when the task requires it.
- Do not inventory or scan the whole library when the manuscript already has sufficient verified sources. Literature search alone remains outside this Skill's scope.
- Check Zotero readiness only after one of these triggers occurs. If Zotero is merely optional and unavailable, continue with the supplied sources or an explicit unresolved citation placeholder instead of changing application settings.
- If the user explicitly asked Codex to operate Zotero, follow the Zotero capability's readiness and enablement procedure. Report an exact blocker if the application, local API, connector, or requested item is unavailable.

## Distinguish formats and citation mechanisms

The Zotero helper can search the local library, export or synchronize BibTeX, and insert citation keys into LaTeX or Markdown. It does not turn plain DOCX text into a live Zotero Word citation.

For Word manuscripts:

- Detect live Zotero fields such as field instructions containing `ADDIN ZOTERO_ITEM` or `ADDIN ZOTERO_BIBL` before editing affected paragraphs.
- Preserve complete field structures and their surrounding bookmarks or content controls. Do not rebuild a field-bearing paragraph from extracted plain text with `python-docx`.
- Add, edit, refresh, or change the style of live Word citations through the Zotero Word add-in or another validated field-preserving Word route. If that route is unavailable, leave a clear citation placeholder and do not imitate a live Zotero field with static text.
- Do not claim that citations or the bibliography were refreshed unless the Zotero Word integration actually completed the refresh.

For LaTeX or Markdown, use Zotero-exported BibTeX keys and keep the associated `.bib` file synchronized. Distinguish Zotero item keys from exported BibTeX citation keys when reporting or resolving ambiguity.

## Protect the Zotero library

- Target read-only searches narrowly by title, author, DOI, year, or claim topic and verify the selected item's identity before citing it.
- Metadata presence is not evidence that a paper supports a scientific claim. Use only source content actually available and authorized for the task; retrieve attachment paths or indexed full text only when the user asks for that content.
- Treat imports and connector saves as Zotero-library writes. Confirm the exact record or source and destination unless the user's request already explicitly authorizes that import.
- Check for likely duplicates before importing. Do not silently merge, delete, retag, relocate, or rewrite existing library items.

## Keep citation style and Word formatting stable

- Use the target journal's current citation and bibliography requirements and the corresponding verified CSL style. Do not manually force citation-range behavior that the active CSL processor does not produce.
- Treat CSL output and the Word `Bibliography` paragraph style as separate layers. Apply font, spacing, indentation, and tab-stop corrections at the style level when possible; direct formatting of individual entries may be lost on the next Zotero refresh.
- After an authorized citation refresh or style change, verify representative in-text citations, ranges, disambiguation, bibliography ordering, hanging indents, fonts, and multi-digit label alignment in the final Word render.
- Confirm that every added citation supports the attached statement and that the bibliography contains no uncited or unresolved item introduced by the current task.
