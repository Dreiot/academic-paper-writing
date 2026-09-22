# Submission-grade Chinese-first manuscript

Use this phase to turn verified research materials into the content-authoritative Chinese master manuscript. The target is submission-grade scientific content and prose in Chinese, so later target-journal work can concentrate on language, length, and formal compliance rather than rebuilding the paper's argument.

## Establish the paper's spine

Construct the argument by separating four kinds of information before writing:

- **Original need:** the practical or modeling problem that existed before the proposed method, and why addressing it matters.
- **Chosen objective and conditions:** what this study elects to achieve and hold fixed. An author-selected budget, architecture, variable, or evaluation condition is not automatically a requirement for the entire field.
- **Supported technical obstacle:** the model relationship, known mechanism, or observed phenomenon that obstructs that objective, with its source or local evidence.
- **Downstream design problem:** an approximation, proxy, architecture, or solver choice may introduce another difficulty. Explain it as a consequence of this design and show how the method handles it; do not recast it as a gap that earlier work universally overlooked.

Connect the need and chosen conditions through the supported obstacle to the method response and testable evidence. “We intend to use this solver” is an objective or means, not a motivation. A specific objective may replace an unsupported broad literature gap, but it cannot replace the explanation of why the objective is worth studying. These distinctions are an internal reasoning aid, not four compulsory paragraphs, a permanent table, or an approval step.

For original research requiring motivation and novelty positioning, establish what prior work already provides; what remains unanswered, condition-dependent, or newly possible for the present task; why that matters for knowledge, model capability, practical use, or interpretation; and what this study adds and how the available evidence evaluates it. Distinguish a descriptive difference from a technically consequential difference under the stated conditions, and then from the research question or contribution that this consequence supports. Author-selected hardware, budget, variables, or step order initially define conditions or means: explain their significance before treating them as research value. A design-induced approximation error remains a consequence of this choice, not a field-wide defect.

Value can come from an explanation, modeling relationship, applicability condition, implementation capability, efficiency tradeoff, or empirical finding. Give that value a precise meaning and supporting basis; another way to perform the same task alone is insufficient. Use the nearest-work comparison in [literature-and-rhetoric.md](literature-and-rhetoric.md#derive-positioning-from-the-nearest-work). If the nearest work already answers the proposed question, acknowledge that coverage and identify only the additional contribution the evidence supports and what remains missing. Renaming or recoding it cannot create novelty. Do not change the method, add experiments, or raise a claim to make the prose appear complete.

Screen potential contributions by their role: a new design or research object; definitions and derivations needed to explain it; empirical findings that test it; or basic practices that make the study correct. State a contribution only when its scientific content and evidence warrant it. Explaining a formula, checking data, ordinary refitting, and passing verification are not automatically contributions. A combination must explain what capability, learning relationship, or verifiable outcome the combination changes; novelty still requires literature support. Use a private claim-to-evidence map only when useful.

When introducing a technical route, first identify which properties of the research problem match it and what meaningful model relationship, evaluation or implementation this match enables. Then explain difficulties introduced by adopting that route and how they are handled. Assuming a solver or architecture first and making the cost of adapting to it the entire motivation reverses this reasoning. Implement the order in the prose without imposing another paragraph template or replacing the nearest-work value analysis above.

Keep four claims distinct: problem structure fits a representation; the complete original objective is exactly transformed; an explicit approximation or proxy is adopted; and an algorithm delivers verified prediction or computational gains. None follows automatically from the preceding one. “Naturally suited” may describe a stated correspondence between variables and objective form under specified conditions; it must not imply arbitrary exact conversion, no additional modeling, or guaranteed benefit.

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

A whole-manuscript rewrite should not default to abstract-level summaries of its scientific sections. Preserve or develop the comparative reasoning, mechanism explanation and evidence interpretation needed for the requested article, even when consolidating paragraphs or formulas. A draft/version filename or a preference for concise prose is not a page limit. Let substantive coverage determine length unless the author or journal supplies a real constraint; do not treat fewer paragraphs, equations or pages as evidence that the rewrite is better.

## Give each section a scientific job

### Abstract

Within normal abstract length, compress the actual need, specific question, design response and principal supported result. “The field is important” followed by “we propose a method” does not establish motivation. Let the question indicate why the response matters, without requiring a literature review, a particular connective or a fixed sentence count. Use exact numbers only when verified and introduce no contribution absent from the paper.

### Introduction

Establish why the research question matters and its specific position relative to what is already known, then introduce the method and verifiable contributions. Apply the research-value and contribution tests above. A declaration of the study objective or an inventory of method components does not replace this reasoning; a narrower design question still needs a reason to be investigated.

Read the opening in order: can the reader identify the research object and concrete problem before encountering technical details whose purpose depends on them? Retain an application example when it helps this entry; move or omit examples that merely delay the problem. Introduce a representation or route through the relationship it helps express, then explain its technical difficulty and the reason for the method choice. This is a dependency check, not a prescribed opening or paragraph count.

Inspect adjacent paragraphs using [continuity](author-revision.md#build-continuity-before-polishing-connectives) and [paragraph focus](anti-overdefense.md#5-paragraph-focus-check). If they repeatedly overview the same method, merge or redistribute their content so the next passage advances the problem, rationale or evidence. The method overview explains how the response works; the contribution summary identifies distinct supported additions and findings. Edit both together rather than appending a second pipeline description. Honor an author's explicit contribution form without imposing a fixed count otherwise.

Judge the actual argument, not length, citations, connectives or reduced paragraph count. For author revisions, follow [author-revision.md](author-revision.md) and verify the requested change in the final manuscript.

### Related work

Supply the research development, nearest-work comparisons and source-supported boundary analysis that substantiate the Introduction's position, following [literature-and-rhetoric.md](literature-and-rhetoric.md#derive-positioning-from-the-nearest-work). Use meaningful comparison axes rather than one procedure description per source. The ending may lead into the method, but a bridge cannot replace comparison reasoning missing from the body. The Abstract, Introduction and Related Work serve the same research question at different levels; do not copy the same motivation paragraph across them or impose a fixed paragraph template. Honor explicit author structure requirements.

### Problem formulation and method

Define the task, inputs, outputs, central notation, objective, component roles, and information flow needed to understand the method. Include initialization, optimization, update rules, stopping conditions, or complexity only when required for scientific interpretation, reproducibility, or the claimed contribution. Do not invent an implementation detail to make the exposition look complete.

Explain why each major component exists and how it addresses the stated limitation. Keep mechanism, parameter fitting, model selection, and final evaluation conceptually distinct when the distinction matters.

Before detailed component equations, make the whole method recoverable: inputs and outputs, shared versus component-specific quantities, iterative feedback and final prediction or selection. For a multi-stage or coupled framework, assess whether an overview diagram materially helps readers recover these relationships; if needed, include it as part of the authorized manuscript work using [scientific-figures.md](scientific-figures.md), reusing a verified existing asset where suitable. A symbol table or algorithm listing does not automatically replace this visual explanation. If a needed visual cannot be completed, identify that omission explicitly rather than silently declaring the method presentation complete. A straightforward method does not require a diagram merely to fill a slot.

### Experiments and results

Make the experimental questions visible through the organization, but do not force every question into a heading. Report only datasets, baselines, splits, metrics, settings, ablations, sensitivity studies, and statistical analyses that actually exist or that the user has asked to plan. Separate observed results from interpretation.

For each central experimental question, state the concrete pattern, magnitude, conditions and supported inference. When averages hide different directions, inspect available group-level contrasts; when a mechanism claim depends on internal changes, use the relevant diagnostic evidence. Distinguish missing explanation from a substantive evidence gap under the [existing evidence check](manuscript-quality-control.md#verify-high-impact-facts-completely): the latter may need an analysis or research recommendation rather than another disclaimer. “Curves vary,” “results are heterogeneous,” or precautions alone do not analyze a display. Do not invent mechanisms from dataset names or demand experiments to repair prose alone.

Describe empirical objects at the level needed to interpret the comparison: dataset source/version, view or group construction and dimensions when these affect the method, material sampling/preprocessing, identifiable comparator algorithms and consequential reproduction changes. A count table, opaque internal alias or list of parameter values alone may not identify the study. Use existing records to fill such gaps, with necessary detail in the manuscript or explicitly available reproduction material; do not fabricate missing specifications.

When the section contains numerical performance results, follow [numeric-reporting.md](numeric-reporting.md) for percentage scale, displayed precision, percentage-point differences, and exceptions that require more digits.

Place an important negative, mixed, or scope-limiting result beside the conclusion it changes. Do not request more baselines, robustness checks, or experiments merely to make the draft look comprehensive.

Within a results subsection, apply the [paragraph-focus rule](anti-overdefense.md#5-paragraph-focus-check): consolidate evidence and interpretation that jointly answer the same question, including across metrics or displays, while keeping genuinely distinct analyses legible. Reporting an observation, explaining it and drawing its supported implication need not become three separate paragraphs.

### Conclusion

Answer the research question at the level established by the paper, summarizing the method and evidence without repeating the abstract. Future research may follow from limitations already discussed; distinguish a proposed direction or test from a completed result, and promise no performance gain. Do not introduce unrelated applications, unreported findings or speculative defenses. Future work is optional, not a required closing template.

## Explain figures and tables in the main text

Apply this division of work to manuscript prose in any language or writing phase. Keep figure/table titles and captions concise, and minimize explanatory table footnotes. Retain information needed to identify and correctly decode the display, such as panel identities, units, abbreviations, sample scope, error-bar definitions or symbol meanings that are not already clear in the display. Follow explicit journal requirements, including any requirement for self-contained legends. Put extended background, procedural explanation, comparisons, interpretation and conclusions in the relevant main-text passage rather than accumulating them below the figure or table.

Explicitly introduce every figure and table by its number where the argument uses it, naming relevant panels when useful. Expressions such as “as shown in Figure/Table X” are examples, not mandatory wording. A number-only mention does not explain the display's role. Tell the reader which question it addresses and, when the encoding is not obvious, how to read the important axes, groups, colors, panels or comparisons. Preserve short visual keys and essential local definitions; do not make readers hunt through prose merely to decode a symbol.

Use the main text to develop the observations that matter, their evidence-grounded interpretation and the conclusion they support. For complex figures, explain how panels or visual relationships jointly answer the question. For tables, select the comparisons, tradeoffs and exceptions that advance the argument instead of narrating every cell. Conceptual figures need explanation of their relationships and design roles, not invented empirical findings. These are argumentative functions, not a fixed sequence or one paragraph per display; discuss several related displays together when that makes the reasoning clearer. A simple display may need only a brief, substantive explanation.

Keep the observation, its interpretation and its evidential limits distinguishable. Explain plausible mechanisms only to the degree supported by the sources and results, preserving material negative or mixed findings. Visual differences alone do not establish statistical significance, causation or component efficacy. Do not move a long caption wholesale into the body and call it analysis, repeat the same explanation in both places, or substitute “better performance” for the actual comparison and its meaning. Existing literature rules apply when the interpretation adds an external scholarly claim; direct reporting of supplied results does not itself restart retrieval.

## Write natural Chinese academic prose

- Prefer established Chinese academic terminology; give a necessary English abbreviation at first occurrence and then use one stable form.
- Preserve official method, dataset, benchmark, variable, and metric identities.
- Build paragraphs from connected sentences rather than labels, fragments, or status language.
- Use the shared [paragraph-focus rule](anti-overdefense.md#5-paragraph-focus-check); a change from observation to interpretation alone does not require a break within one argumentative unit.
- Choose connectives from the actual relation: continuation, progression, parallelism, contrast, cause, or consequence.
- Keep internal Git, Gate, review, authority, artifact, and workflow terminology outside the manuscript.

Draft evidence-bearing sections before relying on the abstract or contribution list. The authoring order may differ from the final reading order.

Remove redundancy without removing reasoning needed to establish research significance. When an author identifies weak motivation or literature analysis, add supported comparisons and explanations where necessary; fewer words or paragraphs are not the default improvement. Under an explicit length limit, compress repeated background and secondary implementation details first.

## Check the submission-grade Chinese manuscript

Apply [manuscript-quality-control.md](manuscript-quality-control.md) to the complete candidate, using the section responsibilities above, [literature-and-rhetoric.md](literature-and-rhetoric.md) for scholarly support, and [anti-overdefense.md](anti-overdefense.md) for prose. Do not repeat their checks under a separate phase checklist.

This phase is complete only when the Chinese manuscript contains the scientific argument, necessary method explanations and evidence interpretation that later journal adaptation can build on. No unresolved scientific, bibliographic or narrative placeholder may be called submission-grade. Pending author-only administrative metadata can be reported outside the manuscript when it does not affect the argument. If English adaptation would need to reconstruct the scientific spine, reopen the affected content before adapting the format.
