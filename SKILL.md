---
name: academic-paper-writing
description: "Draft, translate, journal-adapt, and revise evidence-grounded academic manuscripts and manuscript figures across Chinese-first drafting, author-directed substantive revision, English optimization, reviewer revision, ImageGen conceptual diagrams, local-data-only result figures, and editable Word OMML mathematics. Use for substantial scholarly-paper writing or revision; do not use for literature search alone, general translation, routine copyediting, research discussion reports, or ordinary document formatting."
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

- **Initial draft:** read [references/drafting.md](references/drafting.md). Use Chinese by default and establish the paper's structure, argument, method explanation, evidence path, and necessary mathematics.
- **Optimization:** read [references/optimization.md](references/optimization.md). Translate or rewrite into natural academic English and adapt the manuscript to the user-selected journal and article type.
- **Reviewer revision:** read [references/revision.md](references/revision.md). Analyze actual editor and reviewer comments, revise the manuscript naturally, and prepare response text when requested.

For a substantial author-directed revision of an existing draft outside a post-submission reviewer cycle, also read [references/author-revision.md](references/author-revision.md). Treat the author's exact request and latest author-controlled manuscript as the revision record; do not route ordinary author feedback through the reviewer-response workflow.

For any substantial drafting or rewriting, also read [references/anti-overdefense.md](references/anti-overdefense.md). For a new or substantially edited Word/DOCX manuscript, read [references/docx-manuscript.md](references/docx-manuscript.md). When that deliverable contains mathematics, also read [references/omml.md](references/omml.md).

When presenting quantitative results in manuscript prose, tables, or figures, read [references/numeric-reporting.md](references/numeric-reporting.md) and apply one consistent reader-facing scale and precision without changing the underlying data.

If the user asks to use Zotero, the source DOCX contains live Zotero citation fields, or a citation task genuinely needs the user's local Zotero library, also read [references/zotero.md](references/zotero.md) and use the installed Zotero capability when available. Zotero is a conditional integration, not a prerequisite for ordinary drafting, translation, or revision.

When creating or substantially revising manuscript figures, read [references/scientific-figures.md](references/scientific-figures.md). Use ImageGen for non-evidentiary workflow, principle, mechanism, and method-overview illustrations; generate every result or evidence-bearing figure from authentic local data without a generative image model.

## Escalate evidence-claim conflicts to the user

Do not hide a material evidence conflict or an unclear scientific claim behind vague wording. If the proposed claim's meaning, scope, novelty status, causal interpretation, or evidential support is materially contradictory or unclear, present a compact **Claim Decision** containing:

1. the claim under consideration;
2. the supporting evidence;
3. the contradiction or ambiguity;
4. its practical effect on the manuscript;
5. two or three evidence-consistent wording or evidence options;
6. a recommendation;
7. the one decision needed from the user.

Wait for the user's choice before finalizing the affected claim. Continue unaffected sections when useful. Routine terminology, sentence structure, formatting, and other reversible presentation choices are not Claim Decisions.

Offer only scientifically permissible options. If a stronger factual claim is unsupported, it may be removed, narrowed, or identified as a hypothesis or future objective; user preference cannot turn absent or contradictory evidence into an established result.

## Write like an academic author, not a defensive assistant

- Lead with the best-supported judgment, design choice, or result; then provide mechanism, evidence, and a boundary only when needed.
- Let each paragraph perform one main argumentative function. Use transitions for real continuation, contrast, cause, or progression, not to display balance.
- State a material limitation where it changes interpretation, normally once. Do not distribute the same caveat across the abstract, introduction, results, discussion, and conclusion.
- Do not anticipate objections merely to appear cautious, comprehensive, or reviewer-proof. In reviewer revision, the actual comment is the objection; answer it and the scientific concern necessary to resolve it, not imagined follow-up questions.
- Prefer concrete information over attitude management. Do not weaken a clear conclusion merely to sound moderate, but do not inflate a claim during drafting or English polishing.

## Handle journals, citations, and artifacts proportionately

- For journal-specific optimization, obtain the target journal and article type. Verify current requirements from the official journal or publisher source and follow any user-provided template as the formatting authority.
- Do not fabricate references or use secondary descriptions when a cited scientific claim requires the primary paper. Preserve citation identities, live reference-manager fields, and unresolved citation placeholders explicitly.
- Preserve source files by default and create a new version unless overwrite is unambiguous or explicitly authorized.
- Classify each manuscript figure as conceptual/illustrative or result/evidence-bearing before choosing its production route. Do not use a generative image model for measured results, quantitative study-flow counts, exact plots, or any panel whose visual marks encode research evidence.
- For a DOCX deliverable, use the installed document-authoring capability together with the academic-manuscript decisions in [references/docx-manuscript.md](references/docx-manuscript.md). Produce editable OMML, not equation images or Unicode pseudo-formulas. If visual rendering is unavailable, perform structural checks and disclose that limitation.
- For LaTeX output, retain native LaTeX mathematics; OMML applies only to Word-compatible output.

## Deliver only what the user needs

Return the requested manuscript, section, revision, or response material and a concise description of material changes. A plan, revision note, structural count, or synchronized intermediate is not proof that a requested revision reached the final manuscript; verify the actual delivered artifact before claiming completion. Do not add source inventories, repository identities, governance states, generic risk lists, or internal Claim Decision notes to the reader-facing paper. Keep unresolved author decisions outside the manuscript unless the user requests visible placeholders.
