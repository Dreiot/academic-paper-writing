---
name: academic-paper-writing
description: "Draft, translate, adapt, or refine academic manuscripts and manuscript figures, including substantive author revisions, academic prose polishing, reviewer responses, and requested external-editor handoffs or candidate assessment. Do not use for standalone literature searches, general translation, routine proofreading alone, research discussion reports, or ordinary document formatting."
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

Choose the route and scope from the author's requested change in what the reader can understand, including when the request is called polishing or optimization. Resolve the task, source authority, constraints, and deliverable as needed from the request, manuscript, attachments, and active author decisions. Use the existing writing brief or task context internally and proceed directly when enough is known. Preserve the author's scope and strength of inference. Return a rewritten prompt only when explicitly requested, retaining the author's exact technical terms and the distinctions between them. A prompt-only request ends with that deliverable.

After checking the available materials and context, ask a concise question only when an unresolved input or choice would materially change the manuscript or deliverable. Limit the question to information the author must supply or decide now. Verify downstream requirements at their sources once the missing input is known. Continue unaffected preparation, wait before drafting dependent text or offering a substitute deliverable, and resume the original task after clarification. Handle consequential evidence and claim conflicts through [Claim Decision](#escalate-evidence-claim-conflicts-to-the-user).

Before substantive drafting or reorganization, read the applicable [section responsibilities](references/drafting.md#give-each-section-a-scientific-job), including for a short passage in any language.

For a complete manuscript or substantial multi-section revision, read [references/manuscript-basis.md](references/manuscript-basis.md). Establish or reuse the field, study and article type, audience, and evidence roles before choosing the structure or writing exemplars, and maintain one local manuscript basis for reusable evidence, learning, and active author requirements. For bounded passage work, reuse the relevant sources and effective author decisions in the current task context or an existing note. A bounded edit, pure formatting or discussion does not require a new basis file.

When the user explicitly borrows this Skill for a research proposal, reuse its evidence and prose principles while following the proposal's template and supplied exemplars. Adapt rhythm and emphasis to the research question, proposed mechanism and validation plan; distinguish established work from intended findings. Do not impose paper sections or turn internal feasibility checks into the proposal's narrative. This is a genre adjustment, not a separate workflow.

- **Submission-grade Chinese manuscript:** read [references/drafting.md](references/drafting.md). Use Chinese by default and complete the scientific content, literature grounding, argument, prose, any needed figures and tables, references, and necessary mathematics to a level that should require journal adaptation rather than later substantive reconstruction.
- **Target-journal adaptation:** read [references/optimization.md](references/optimization.md). Translate or rewrite into natural academic English and adapt a content-complete manuscript to the user-selected journal and article type. Reopen the Chinese-manuscript or author-revision phase when a material scientific or rhetorical gap remains.
- **Author-directed refinement:** use [references/author-revision.md](references/author-revision.md) when the requested change affects a passage's argument, explanation, evidence use, or role, at any length. This includes authorized revision based on advisory comments from collaborators or external models. Use the exact request and latest author-controlled text as the revision record. Verify advisory comments against direct evidence and active author decisions before applying them. For language-only refinement, compare the original and revised passage using the [shared prose audit](references/anti-overdefense.md#final-prose-audit).
- **Reviewer revision:** read [references/revision.md](references/revision.md). Analyze actual editor and reviewer comments, revise the manuscript naturally, and prepare response text when requested.

Use the [continuity method](references/author-revision.md#build-continuity-before-polishing-connectives) for substantial drafting as well.

For any manuscript claim whose scholarly meaning depends on external literature, read [references/literature-and-rhetoric.md](references/literature-and-rhetoric.md). This follows the claim, not its section. Reuse valid source support and search where coverage or a changed claim needs it; honor an explicit closed corpus or no-browsing instruction. Standalone literature search remains outside this Skill.

If institutional or publisher authentication is needed for full text, read [references/literature-access.md](references/literature-access.md). After the user manually verifies a profile's official login route once, default to automatic access through the approved local browser, including browser-managed reauthentication. Interrupt only for an actual user-only step or new authorization decision under that reference, then resume the pending search. Never read, export, display, copy, log, or place the credential or token value in Skill files, manuscript files, Git, prompts, screenshots, or model-visible tool arguments.

For a complete journal article (including journal adaptation), substantial multi-section revision, major literature-dependent claim change, compound manuscript-and-technical task, or local rewrite that changes evidence selection, comparisons, reasoning or conclusion strength, use [manuscript quality control](references/manuscript-quality-control.md). Prepare with its working brief, then verify the actual candidate against the direct records and locate the essential findings in the final text. Resolve supported findings before delivery. Limit this pass to the requested scope and its dependencies. Ordinary copyediting and formatting use affected-text checks. Keep production and verification traceably separate. Use specialist delegation or an independent reviewer when requested or when it materially improves reliability; otherwise use separated source-first verification and relevant deterministic checks. Never describe a self-check as independent review.

For substantive writing, analysis, translation, revision, or polishing within this Skill, read the [shared prose standard](references/anti-overdefense.md). For a new or substantially edited Word/DOCX manuscript, read [references/docx-manuscript.md](references/docx-manuscript.md). When that deliverable contains mathematics, also read [references/omml.md](references/omml.md).

When presenting quantitative results in manuscript prose, tables, or figures, read [references/numeric-reporting.md](references/numeric-reporting.md) and apply one consistent reader-facing scale and precision without changing the underlying data.

When writing or revising manuscript discussion of figures or tables, follow [the main-text explanation rules](references/drafting.md#explain-figures-and-tables-in-the-main-text), including for existing displays. This prose task does not itself require regenerating figures or invoking document production.

If the user asks to use Zotero, the source DOCX contains live Zotero citation fields, or a citation task genuinely needs the user's local Zotero library, also read [references/zotero.md](references/zotero.md) and use the installed Zotero capability when available. Zotero is a conditional integration, not a prerequisite for ordinary drafting, translation, or revision. Zotero-library imports and other library writes are currently paused; use only the read-only operations permitted by that reference until the user explicitly re-enables writes after the integration is improved.

When creating or substantially revising manuscript figures, read [references/scientific-figures.md](references/scientific-figures.md). Use ImageGen for non-evidentiary workflow, principle, mechanism, and method-overview illustrations; generate every result or evidence-bearing figure from authentic local data without a generative image model.

For a user-requested polishing prompt or external-editor handoff, or requested assessment/integration of a returned polished candidate, read [references/external-polishing.md](references/external-polishing.md). Generate a scoped prompt for Gemini or the user's chosen editor only when requested; otherwise assess or integrate within the designated scope. Ordinary drafting, revision, or a general wish for natural prose does not trigger prompt generation or external submission.

## Escalate evidence-claim conflicts to the user

Resolve routine factual corrections and presentation choices from direct sources and existing author decisions. When a material uncertainty in scientific meaning, scope, novelty, causality or support cannot be resolved that way and requires a new author choice, present a compact **Claim Decision**: the disputed claim and evidence, its consequence, credible options, and your recommendation plus the decision needed. Do not manufacture multiple options or use a mandatory form when one clear question suffices.

Wait only for that consequential decision while continuing unaffected work. An already authorized, evidence-supported correction or narrowing does not require the same approval again; do not silently weaken an author-controlled central claim when that changes the research position. Reversible reorganization, terminology and formatting within the task can proceed. Unsupported claims may be removed, narrowed or identified as hypotheses where authorized; user preference cannot make missing evidence an established result.

## Write like an academic author, not a defensive assistant

Apply the [shared prose standard](references/anti-overdefense.md) across sections and languages: establish evidence-supported judgments through clear, continuous reasoning. Its sentence, paragraph, qualification-placement, and authoring checks are shared by all writing phases rather than repeated as phase-specific rules.

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
