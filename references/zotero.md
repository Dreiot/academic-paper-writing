# Zotero-aware citation workflow

Read this reference when the user explicitly asks to use Zotero, a DOCX contains live Zotero fields that the task may affect, or a needed citation should be retrieved from the user's local Zotero library. Use the installed Zotero capability for permitted read-only library operations when it is available. Zotero-library writes are paused until the integration can safely create, select, and assign paper-specific collections and the user explicitly re-enables writes.

## Trigger Zotero proportionately

- Use Zotero for a targeted local-library search, item verification, read-only BibTeX export, or citation-key retrieval for supported LaTeX and Markdown drafts when the task requires it.
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

## Keep the Zotero library read-only for now

- Target read-only searches narrowly by title, author, DOI, year, or claim topic and verify the selected item's identity before citing it.
- Metadata presence is not evidence that a paper supports a scientific claim. An explicit manuscript request that requires literature grounding authorizes reading the selected in-scope Zotero attachment or indexed text after its identity is verified; it does not authorize a broad scan of unrelated library content. For other tasks, retrieve attachment paths or indexed full text only when the user asks for that content.
- Do not call `import-bibtex`, `import-ris`, connector save, attachment save, collection creation, collection assignment, retagging, relocation, merge, deletion, metadata rewrite, or another Zotero-library write. A request to collect papers does not override this pause; explain that imports are deferred and offer a local `.bib`/RIS file or a verified source list instead.
- Do not change Zotero application settings merely to work around the pause. Readiness probes, narrow searches, collection listings, selected-target inspection, item/attachment inspection, and exports that do not modify the library remain allowed.
- Citation insertion or revision in the manuscript may use already existing verified Zotero items when the available route preserves the document's citation mechanism; the Zotero library itself must remain unchanged.

## Defer collection organization and imports

Do not create or populate a paper-specific collection during this paused period, even if the user previously gave general permission to organize references. If the user asks to save newly gathered literature, prepare a deduplicated local `.bib`/RIS file or source list containing only the selected cited, core-comparison, and journal-rhetoric papers, then leave Zotero import pending. Excluded screening results are not included by default.

Re-enable library writes only after the user makes a new explicit decision and the active integration has been verified to create or select the intended collection, assign both new and existing items to it, detect duplicates, and confirm the final destination and attachment state. At that time, revise this reference before performing imports; do not silently treat improved tooling as authorization.

## Keep citation style and Word formatting stable

- Use the target journal's current citation and bibliography requirements and the corresponding verified CSL style. Do not manually force citation-range behavior that the active CSL processor does not produce.
- Treat CSL output and the Word `Bibliography` paragraph style as separate layers. Apply font, spacing, indentation, and tab-stop corrections at the style level when possible; direct formatting of individual entries may be lost on the next Zotero refresh.
- After an authorized citation refresh or style change, verify representative in-text citations, ranges, disambiguation, bibliography ordering, hanging indents, fonts, and multi-digit label alignment in the final Word render.
- Confirm that every added citation supports the attached statement and that the bibliography contains no uncited or unresolved item introduced by the current task.
- When literature grounding is in scope, reconcile the existing source record with Zotero item identity, exported citation key or live Word field, DOI/title deduplication, in-text order, and the final bibliography. Preserve unresolved mismatches instead of silently substituting a similarly titled item; a separate matrix is not required.
