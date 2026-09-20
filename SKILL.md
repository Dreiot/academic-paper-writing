---
name: academic-paper-writing
description: "Draft, translate, journal-adapt, or substantially revise academic manuscripts and manuscript figures, including author revisions and reviewer responses. Do not use for standalone literature searches, general translation, routine copyediting, research discussion reports, or ordinary document formatting."
---

# Academic Paper Writing

Produce reader-facing academic manuscripts with a clear argument, natural human prose, evidence-calibrated claims, and only the boundaries that materially affect interpretation. Keep internal research governance and production bookkeeping out of the manuscript.

## Work within the authorized evidence

- Ground scientific statements in the user's materials, the current manuscript, verified project evidence, and authoritative literature actually consulted for the task.
- Do not invent citations, results, experimental settings, mathematical derivations, reviewer intent, completed changes, or missing method details.
- Preserve material negative and mixed evidence where it changes the conclusion. Distinguish established results, interpretation, hypotheses, and future work.
- Work only on the requested manuscript or sections. Do not run experiments, change the method, submit externally, update project authority, commit, or push unless the user separately authorizes that work.

For a governed research project, read the current `AGENTS.md`, `docs/PROJECT_CORE.md`, `docs/CURRENT_STAGE.md`, and only the evidence needed to avoid stale or contradictory manuscript claims. These files are drafting authority, not reader-facing content. This Skill alone does not invoke `$codex-research-workflow`, create a Goal, run an audit, open a Gate, request formal review, prepare an evidence packet, or promote a claim. When the user explicitly invokes both Skills or the assigned Goal is already governed, follow both without duplicating their shared rules.

## Route to the writing phase

Infer the phase from the request and available artifacts. Ask only when choosing the phase would materially change the deliverable.

- **Submission-grade Chinese manuscript:** read [references/drafting.md](references/drafting.md). Use Chinese by default and complete the scientific content, literature grounding, argument, prose, any needed figures and tables, references, and necessary mathematics to a level that should require journal adaptation rather than later substantive reconstruction.
- **Target-journal adaptation:** read [references/optimization.md](references/optimization.md). Translate or rewrite into natural academic English and adapt a content-complete manuscript to the user-selected journal and article type. Reopen the Chinese-manuscript or author-revision phase when a material scientific or rhetorical gap remains.
- **Reviewer revision:** read [references/revision.md](references/revision.md). Analyze actual editor and reviewer comments, revise the manuscript naturally, and prepare response text when requested.

For a substantial author-directed revision of an existing draft outside a post-submission reviewer cycle, also read [references/author-revision.md](references/author-revision.md). It supplies the revision record and concrete paragraph/section continuity method; use that continuity method for substantial drafting as well. Treat the author's exact request and latest author-controlled manuscript as the revision record; do not route ordinary author feedback through the reviewer-response workflow.

For any manuscript claim whose scholarly meaning depends on external literature, read [references/literature-and-rhetoric.md](references/literature-and-rhetoric.md). This follows the claim, not its section. Reuse valid source support and search where coverage or a changed claim needs it; honor an explicit closed corpus or no-browsing instruction. Standalone literature search remains outside this Skill.

If institutional or publisher authentication is needed for full text, read [references/literature-access.md](references/literature-access.md). After the user manually verifies a profile's official login route once, default to automatic access through the approved local browser, including browser-managed reauthentication. Interrupt only for an actual user-only step or new authorization decision under that reference, then resume the pending search. Never read, export, display, copy, log, or place the credential or token value in Skill files, manuscript files, Git, prompts, screenshots, or model-visible tool arguments.

For a complete journal article, substantial multi-section revision, major literature-dependent claim change, or compound manuscript-and-technical task, read [references/manuscript-quality-control.md](references/manuscript-quality-control.md). Its hard requirement is a traceable separation between producing the candidate and verifying it against the author's request and direct evidence—not a particular agent arrangement. Use specialist delegation or an independent reviewer when the user requests it or it materially improves reliability; otherwise use separated source-first verification and relevant deterministic checks. Never describe a self-check as independent review.

For any substantial drafting or rewriting, also read [references/anti-overdefense.md](references/anti-overdefense.md). For a new or substantially edited Word/DOCX manuscript, read [references/docx-manuscript.md](references/docx-manuscript.md). When that deliverable contains mathematics, also read [references/omml.md](references/omml.md).

When presenting quantitative results in manuscript prose, tables, or figures, read [references/numeric-reporting.md](references/numeric-reporting.md) and apply one consistent reader-facing scale and precision without changing the underlying data.

When writing or revising manuscript discussion of figures or tables, follow [the main-text explanation rules](references/drafting.md#explain-figures-and-tables-in-the-main-text), including for existing displays. This prose task does not itself require regenerating figures or invoking document production.

If the user asks to use Zotero, the source DOCX contains live Zotero citation fields, or a citation task genuinely needs the user's local Zotero library, also read [references/zotero.md](references/zotero.md) and use the installed Zotero capability when available. Zotero is a conditional integration, not a prerequisite for ordinary drafting, translation, or revision. Zotero-library imports and other library writes are currently paused; use only the read-only operations permitted by that reference until the user explicitly re-enables writes after the integration is improved.

When creating or substantially revising manuscript figures, read [references/scientific-figures.md](references/scientific-figures.md). Use ImageGen for non-evidentiary workflow, principle, mechanism, and method-overview illustrations; generate every result or evidence-bearing figure from authentic local data without a generative image model.

## Escalate evidence-claim conflicts to the user

Resolve routine factual corrections and presentation choices from direct sources and existing author decisions. When a material uncertainty in scientific meaning, scope, novelty, causality or support cannot be resolved that way and requires a new author choice, present a compact **Claim Decision**: the disputed claim and evidence, its consequence, credible options, and your recommendation plus the decision needed. Do not manufacture multiple options or use a mandatory form when one clear question suffices.

Wait only for that consequential decision while continuing unaffected work. An already authorized, evidence-supported correction or narrowing does not require the same approval again; do not silently weaken an author-controlled central claim when that changes the research position. Reversible reorganization, terminology and formatting within the task can proceed. Unsupported claims may be removed, narrowed or identified as hypotheses where authorized; user preference cannot make missing evidence an established result.

## Write like an academic author, not a defensive assistant

- Lead with the best-supported judgment, design choice, or result; then provide mechanism, evidence, and a boundary only when needed.
- Within each subsection, prefer complete argumentative units that combine related evidence and explanation around one question or judgment. Follow the [paragraph-focus rule](references/anti-overdefense.md#5-paragraph-focus-check) to consolidate overlapping passages and preserve meaningful changes of question or reasoning stage; a new source, metric, display or sentence role alone does not require a new paragraph.
- State a material limitation where it changes interpretation, normally once. Do not distribute the same caveat across the abstract, introduction, results, discussion, and conclusion.
- Do not anticipate objections merely to appear cautious, comprehensive, or reviewer-proof. In reviewer revision, the actual comment is the objection; answer it and the scientific concern necessary to resolve it, not imagined follow-up questions.
- Prefer concrete information over attitude management. Do not weaken a clear conclusion merely to sound moderate, but do not inflate a claim during drafting or English polishing.

## Handle journals, citations, and artifacts proportionately

- For journal-specific optimization, obtain the target journal and article type. Verify current requirements from the official journal or publisher source and follow any user-provided template as the formatting authority.
- For manuscript types governed by dedicated reporting frameworks—such as systematic or scoping reviews, meta-analyses, clinical or observational studies, diagnostic or prognostic studies, qualitative research, or animal studies—verify the applicable current reporting guidance before substantial drafting or revision. Treat systematic evidence synthesis as a distinct methodology rather than an ordinary narrative search, and never invent missing protocol, screening, registration, or risk-of-bias work.
- Do not fabricate references or use secondary descriptions when a cited scientific claim requires the primary paper. Search snippets and bibliographic metadata cannot establish detailed method, comparison, or novelty claims. Preserve citation identities, live reference-manager fields, and unresolved citation placeholders explicitly.
- Preserve source files by default and create a new version unless overwrite is unambiguous or explicitly authorized.
- Classify each manuscript figure as conceptual/illustrative or result/evidence-bearing before choosing its production route. Do not use a generative image model for measured results, quantitative study-flow counts, exact plots, or any panel whose visual marks encode research evidence.
- For a DOCX deliverable, use the installed document-authoring capability together with the academic-manuscript decisions in [references/docx-manuscript.md](references/docx-manuscript.md). Produce editable OMML, not equation images or Unicode pseudo-formulas. If visual rendering is unavailable, complete content and structural checks and deliver with that limitation; do not claim a visual pass. Visual verification blocks completion only when the user explicitly requires it.
- For LaTeX output, retain native LaTeX mathematics; OMML applies only to Word-compatible output.

## Deliver only what the user needs

Return the requested manuscript, section, revision, or response material and a concise description of material changes. A plan, revision note, structural count, or synchronized intermediate is not proof that a requested revision reached the final manuscript; verify the actual delivered artifact before claiming completion. When the task requires literature or manuscript-quality gates, report their status and the verification mode honestly; do not call a provisional or inadequately verified candidate complete. Do not add source inventories, repository identities, governance states, generic risk lists, literature-search logs, or internal Claim Decision notes to the reader-facing paper. Keep unresolved author decisions outside the manuscript unless the user requests visible placeholders.
