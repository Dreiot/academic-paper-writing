# Submission-grade Chinese-first manuscript

Use this phase to turn verified research materials into the content-authoritative Chinese master manuscript. The target is submission-grade scientific content and prose in Chinese, so later target-journal work can concentrate on language, length, and formal compliance rather than rebuilding the paper's argument.

## Establish the paper's spine

Identify the research question, the limitation in existing work, the central idea, the method that realizes it, the evidence available, and the conclusion that evidence supports. Maintain a private claim-to-evidence map when it helps consistency; do not insert that production artifact into the paper.

Apply [literature-and-rhetoric.md](literature-and-rhetoric.md) to every part of the draft whose scientific meaning, positioning, design rationale, comparison, interpretation, or application context depends on external scholarship. A complete journal-paper draft requires the comprehensive literature route before those passages can be treated as final; this obligation is not limited to the Introduction or Related Work.

If the target journal is unknown, use a journal-neutral structure informed by high-quality venues in the field. A private production placeholder may be used temporarily for a missing local fact, but the reader-facing manuscript cannot be called submission-grade while a scientific, bibliographic, or narrative placeholder remains. Author-supplied administrative metadata such as final affiliations or funding identifiers may remain an external completion item when it does not change the paper's scientific argument. If evidence and a claim conflict or the scientific meaning is unclear, use the Claim Decision process from `SKILL.md`.

The final layout may adapt to the field and paper type. For an empirical methods paper, a useful default is:

1. title, abstract, and keywords;
2. introduction;
3. related work;
4. problem formulation and notation;
5. proposed method;
6. experimental setup;
7. results and analysis;
8. conclusion.

Do not create a section merely because this list contains it. Merge, split, or omit sections when the paper's argument or target venue calls for a different structure.

A Chinese master manuscript is a complete academic paper, not a rough outline or a designed report. It must contain the arguments, evidence, explanations, figures, tables, equations, captions, and references needed for scholarly evaluation. Use the minimum styling needed to make them clear. Unless the user or target venue requests them, do not append a `技术注与补充材料索引`, evidence inventory, verification log, production note, repository map, or other internal traceability section. Keep such working material outside the reader-facing manuscript.

## Give each section a scientific job

### Abstract

State the problem, precise gap, central method idea, most important supported result, and resulting conclusion. Use exact numbers only when verified. Do not fill the abstract with background, generic importance, defensive limitations, or contributions absent from the paper.

### Introduction

Move from the concrete research problem to the unresolved limitation, then explain the paper's response and contributions. Treat contribution statements as distinct scientific contributions, not a list of modules, implementation details, or engineering safeguards. Do not create a straw-man version of prior work merely to make the gap appear larger.

Judge the Introduction by whether this reasoning is established, not by paragraph count, length, citation count, or coverage of an instruction checklist. When revising an existing Introduction in response to author feedback, follow [author-revision.md](author-revision.md) and verify the requested argumentative change in the final manuscript.

### Related work

Organize literature by research question, assumption, mechanism, or limitation. Synthesize relationships among studies instead of producing one sentence per paper. End each subsection with the exact connection to the present work only when that connection advances the argument.

Use one meaningful comparison axis within each subsection and make prior mechanisms lead to the unresolved question addressed by the paper. A fixed subsection count, a renamed heading, or the same paragraph roles under new wording does not by itself constitute a substantive Related Work revision.

### Problem formulation and method

Define the task, inputs, outputs, central notation, objective, component roles, and information flow needed to understand the method. Include initialization, optimization, update rules, stopping conditions, or complexity only when required for scientific interpretation, reproducibility, or the claimed contribution. Do not invent an implementation detail to make the exposition look complete.

Explain why each major component exists and how it addresses the stated limitation. Keep mechanism, parameter fitting, model selection, and final evaluation conceptually distinct when the distinction matters.

### Experiments and results

Make the experimental questions visible through the organization, but do not force every question into a heading. Report only datasets, baselines, splits, metrics, settings, ablations, sensitivity studies, and statistical analyses that actually exist or that the user has asked to plan. Separate observed results from interpretation.

When the section contains numerical performance results, follow [numeric-reporting.md](numeric-reporting.md) for percentage scale, displayed precision, percentage-point differences, and exceptions that require more digits.

Place an important negative, mixed, or scope-limiting result beside the conclusion it changes. Do not request more baselines, robustness checks, or experiments merely to make the draft look comprehensive.

### Conclusion

Answer the research question at the level established by the paper. Summarize the method and evidence without repeating the abstract sentence by sentence. Do not introduce a new claim, experiment, application area, or speculative defense.

## Write natural Chinese academic prose

- Prefer established Chinese academic terminology; give a necessary English abbreviation at first occurrence and then use one stable form.
- Preserve official method, dataset, benchmark, variable, and metric identities.
- Build paragraphs from connected sentences rather than labels, fragments, or status language.
- Treat paragraph breaks as changes in argumentative stage, question, comparison, or evidence role. Do not create one paragraph per paper, equation, result, or prompt bullet when the material belongs to the same line of reasoning.
- Choose connectives from the actual relation: continuation, progression, parallelism, contrast, cause, or consequence.
- Keep internal Git, Gate, review, authority, artifact, and workflow terminology outside the manuscript.

Draft evidence-bearing sections before relying on the abstract or contribution list. The authoring order may differ from the final reading order.

## Check the submission-grade Chinese manuscript

- The research question, gap, method, experiments, and conclusion form one argument.
- Every substantive claim has supporting evidence or is explicitly framed as a hypothesis or objective.
- Every literature-dependent statement has passed the required focused or comprehensive literature gate, including claim-level source support and any required journal-rhetoric study.
- The Introduction establishes problem, gap, design need, response, and contribution as connected reasoning rather than a compressed compliance list.
- Related Work synthesizes prior mechanisms on explicit comparison axes and leaves a precise unresolved question rather than repeating the Introduction or Method.
- Symbols and component names remain consistent across text, formulas, tables, and figures.
- Equations needed to understand the method are present and explained; decorative derivations are absent.
- Negative and mixed evidence is not hidden, and limitations are not repeated mechanically.
- No unresolved scientific, bibliographic, or narrative placeholder remains in the reader-facing manuscript; any pending author-only administrative metadata is reported outside it.
- A later target-journal adaptation should not need to reconstruct the core problem, literature gap, method rationale, result interpretation, or conclusion. If it does, reopen this phase before adapting the journal format.
- No unrequested technical-note, evidence-index, or supplementary-index section has been appended to the Chinese master manuscript.
- The anti-overdefense checks pass.
