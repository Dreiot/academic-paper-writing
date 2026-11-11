# Submission-grade Chinese-first manuscript

Use this phase to turn verified research materials into the content-authoritative Chinese master manuscript. The target is submission-grade scientific content and prose in Chinese, so later target-journal work can concentrate on language, length, and formal compliance rather than rebuilding the paper's argument.

## Establish the paper's spine

Start with the field and study/article type in the [manuscript basis](manuscript-basis.md#identify-the-writing-context). Establish the concrete research question, what prior work makes known or unresolved, how this study addresses it, and what the evidence answers. A clinical association, an experimental finding, a theoretical result, and a new algorithm can require different argument and evidence structures; do not turn all of them into a proposed-method paper.

For work proposing a method or technical design, separate four kinds of information before writing:

- **Original need:** the practical or modeling problem that existed before the proposed method, and why addressing it matters.
- **Chosen objective and conditions:** what this study elects to achieve and hold fixed. An author-selected budget, architecture, variable, or evaluation condition is not automatically a requirement for the entire field.
- **Supported technical obstacle:** the model relationship, known mechanism, or observed phenomenon that obstructs that objective, with its source or local evidence.
- **Downstream design problem:** an approximation, proxy, architecture, or solver choice may introduce another difficulty. Explain it as a consequence of this design and show how the method handles it; do not recast it as a gap that earlier work universally overlooked.

Connect the need and chosen conditions through the supported obstacle to the method response and testable evidence. “We intend to use this solver” is an objective or means, not a motivation. A specific objective may replace an unsupported broad literature gap, but it cannot replace the explanation of why the objective is worth studying. These distinctions are an internal reasoning aid, not four compulsory paragraphs, a permanent table, or an approval step.

For original research requiring motivation and novelty positioning, establish what prior work already provides; what remains unanswered, condition-dependent, or newly possible for the present task; why that matters for knowledge, model capability, practical use, or interpretation; and what this study adds and how the available evidence evaluates it. Distinguish a descriptive difference from a technically consequential difference under the stated conditions, and then from the research question or contribution that this consequence supports. Author-selected hardware, budget, variables, or step order initially define conditions or means: explain their significance before treating them as research value. A design-induced approximation error remains a consequence of this choice, not a field-wide defect.

Value can come from an explanation, modeling relationship, applicability condition, implementation capability, efficiency tradeoff, or empirical finding. In the [nearest-work comparison](literature-and-rhetoric.md#derive-positioning-from-the-nearest-work), explain what applying the closest approach under comparable conditions already yields. If the methods coincide under a supported condition, state that overlap and explain the question or capability that remains. Ground the resulting contribution in the study's evidence. Do not change the method, add experiments, or raise a claim to make the prose appear complete.

Screen potential contributions by their role: a new design or research object; definitions and derivations needed to explain it; empirical findings that test it; or basic practices that make the study correct. State a contribution only when its scientific content and evidence warrant it. Explaining a formula, checking data, ordinary refitting, and passing verification are not automatically contributions. A combination must explain what capability, learning relationship, or verifiable outcome the combination changes; novelty still requires literature support. Use a private claim-to-evidence map only when useful.

When introducing a technical route, first identify which properties of the research problem match it and what meaningful model relationship, evaluation or implementation this match enables. Then explain difficulties introduced by adopting that route and how they are handled. Assuming a solver or architecture first and making the cost of adapting to it the entire motivation reverses this reasoning. Implement the order in the prose without imposing another paragraph template or replacing the nearest-work value analysis above.

Keep four claims distinct: problem structure fits a representation; the complete original objective is exactly transformed; an explicit approximation or proxy is adopted; and an algorithm delivers verified prediction or computational gains. None follows automatically from the preceding one. “Naturally suited” may describe a stated correspondence between variables and objective form under specified conditions; it must not imply arbitrary exact conversion, no additional modeling, or guaranteed benefit.

Apply [literature-and-rhetoric.md](literature-and-rhetoric.md) to every part of the draft whose scientific meaning, positioning, design rationale, comparison, interpretation, or application context depends on external scholarship. A complete journal-paper draft requires the comprehensive literature route before those passages can be treated as final; this obligation is not limited to the Introduction or Related Work.

If the target journal is unknown, use a journal-neutral structure informed by high-quality venues in the field. A private production placeholder may be used temporarily for a missing local fact, but the reader-facing manuscript cannot be called submission-grade while a scientific, bibliographic, or narrative placeholder remains. Author-supplied administrative metadata such as final affiliations or funding identifiers may remain an external completion item when it does not change the paper's scientific argument. If evidence and a claim conflict or the scientific meaning is unclear, use the Claim Decision process from `SKILL.md`.

Choose the final structure from the field, article type, and relevant venue requirements. Empirical biomedical or social research may use Introduction, Methods, Results, and Discussion; a methods paper may need a separate literature comparison, formulation, and experimental analysis; a theoretical paper may center definitions, propositions, and proofs. These are examples, not fixed templates. Put earlier work, limitations, and the concluding judgment where the genre and argument need them; do not create separate sections merely because another article type uses them.

A Chinese master manuscript is a complete academic paper, not a rough outline or a designed report. It must contain the arguments, evidence, explanations, numbered figures and tables, equations, and references needed for scholarly evaluation. Use the minimum styling needed to make them clear. Unless the user or target venue requests them, do not append a `技术注与补充材料索引`, evidence inventory, verification log, production note, repository map, or other internal traceability section. Keep such working material outside the reader-facing manuscript.

A whole-manuscript rewrite should not default to abstract-level summaries of its scientific sections. Preserve or develop the comparative reasoning, mechanism explanation and evidence interpretation needed for the requested article, even when consolidating paragraphs or formulas. A draft/version filename or a preference for concise prose is not a page limit. Let substantive coverage determine length unless the author or journal supplies a real constraint; do not treat fewer paragraphs, equations or pages as evidence that the rewrite is better.

## Give each section a scientific job

### Abstract

Within normal abstract length, connect the background and specific question to the method, principal findings and supported conclusion. Select the results that answer that question instead of enumerating datasets or analyses. Use verified numbers where they carry the answer, without introducing a contribution absent from the paper.

Select the findings that directly answer the research question and support the conclusion before compressing their wording. Include secondary or supporting results only if they materially change the interpretation or scope of the main findings, or if the venue or applicable reporting framework requires them. Retain negative or mixed evidence when it changes the conclusion.

### Introduction

Develop the research need through relevant prior achievements and the remaining question, then introduce the proposed response and verifiable contributions. Keep application detail only when it establishes that need or condition. A brief finding may close the Introduction where appropriate; the abstract's compressed background–method–results–conclusion sequence does not replace the Introduction's development of the problem. Apply the research-value and contribution tests above.

Read the opening in order: can the reader identify the research object and concrete problem before encountering technical details whose purpose depends on them? Retain an application example when it helps this entry; move or omit examples that merely delay the problem. Introduce a representation or route through the relationship it helps express, then explain its technical difficulty and the reason for the method choice. This is a dependency check, not a prescribed opening or paragraph count.

Inspect adjacent paragraphs using [continuity](author-revision.md#build-continuity-before-polishing-connectives) and [paragraph focus](anti-overdefense.md#5-paragraph-focus-check). If they repeatedly overview the same method, merge or redistribute their content so the next passage advances the problem, rationale or evidence. The method overview explains how the response works; the contribution summary identifies distinct supported additions and findings. Edit both together rather than appending a second pipeline description. Honor an author's explicit contribution form without imposing a fixed count otherwise.

Judge the actual argument, not length, citations, connectives or reduced paragraph count. For author revisions, follow [author-revision.md](author-revision.md) and verify the requested change in the final manuscript.

### Related work

Supply the research development, nearest-work comparisons and source-supported boundary analysis that substantiate the Introduction's position, following [literature-and-rhetoric.md](literature-and-rhetoric.md#derive-positioning-from-the-nearest-work). Use meaningful comparison axes rather than one procedure description per source. The ending may lead into the method, but a bridge cannot replace comparison reasoning missing from the body. The Abstract, Introduction and Related Work serve the same research question at different levels; do not copy the same motivation paragraph across them or impose a fixed paragraph template. Honor explicit author structure requirements.

### Problem formulation and method

Define the task, inputs, outputs, central notation, objective, component roles, and information flow needed to understand the method. Include initialization, optimization, update rules, stopping conditions, or complexity only when required for scientific interpretation, reproducibility, or the claimed contribution. Do not invent an implementation detail to make the exposition look complete.

Explain the general role, input–output relation and rationale of each component, including interchangeable inputs. In a methods paper, separate the proposed mechanism from its evaluation setup. Place application-specific preprocessing, tested parameter values, comparator implementations and evaluation protocols with that setup. A measure needed to define the proposed mechanism belongs with it; other metrics belong with the evaluation. Keep later result values and table-specific cases out of the general method explanation.

Before detailed component equations, give a connected account of the method's inputs, dependencies and outputs. In a complete methods paper, include an overview diagram when the contribution depends on how distinct inputs or stages interact, or on how fitted quantities pass into selection or evaluation under different data roles. Explain those relationships in the body before the details. Use [scientific-figures.md](scientific-figures.md) and reuse a suitable verified asset. A straightforward method can be clear in prose. If a needed visual cannot be completed, identify the remaining gap.

### Experiments and results

For observational and experimental studies, organize around substantive questions and findings rather than a list of assays, statistical tests, or software outputs. Use existing primary observations and quantitative summaries together when each contributes necessary evidence. In fields using experimental images, this can include morphology, molecular measurements, and functional observations where they actually exist and answer the question; it is not a requirement to add these modalities to every paper. Keep sample/analysis units and material uncertainty clear, with essential results in the body and fuller detail in suitable tables or supplements. Simplifying presentation does not authorize changing the analysis or suppressing adverse findings. Follow [scientific-figures.md](scientific-figures.md#present-original-observations) for evidence images.

Define shared evaluation conditions before dependent results. Name a comparison-specific variant when the same endpoint uses a different reference, eligible set or aggregation, and give the distinction where it is used. Use headings for distinct questions or useful navigation. Report only settings and analyses that exist or that the user has asked to plan. Distinguish observations from interpretation.

Develop each central experimental question across the comparisons needed to answer it. Explain how the observed pattern, magnitude, tradeoff and exceptions bear on the method's purpose, then what the next diagnostic can resolve. Organize related observations into that reasoning rather than ending every dataset or metric with a generic caution. Inspect available group-level contrasts when averages hide different directions. Separate observations and supported explanations; claims about effect differences or mechanisms require the corresponding evidence under the [existing evidence check](manuscript-quality-control.md#verify-high-impact-facts-completely).

Describe empirical objects at the level needed to interpret the comparison: dataset source/version, view or group construction and dimensions when these affect the method, material sampling/preprocessing, identifiable comparator algorithms and consequential reproduction changes. A count table, opaque internal alias or list of parameter values alone may not identify the study. Use existing records to fill such gaps. Place interpretation-critical details in the main text and give reproduction-only settings a reader-accessible destination from the first complete draft, following the [shared placement rule](anti-overdefense.md#concentrate-necessary-boundaries).

When the section contains numerical performance results, follow [numeric-reporting.md](numeric-reporting.md) for percentage scale, displayed precision, percentage-point differences, and exceptions that require more digits.

Use the [shared prose standard](anti-overdefense.md) for result interpretation, paragraph progression, and the distinct placement of actual counterevidence and common limitations. Do not request more baselines, robustness checks, or experiments merely to make the draft look comprehensive.

### Discussion

Develop the best-supported answer and explain what it adds to the field. Relate the study's concrete findings to relevant prior evidence, explain meaningful agreement or disagreement and plausible reasons supported by sources, and state the resulting scientific or practical value. Description of measured changes alone does not supply an authorial judgment. Keep the research focus distinct from the strength of its answer under the [manuscript basis](manuscript-basis.md#identify-the-writing-context); neither naming a studied mechanism nor finding associated markers establishes causal confirmation.

When a paper combines different evidence streams, make each stream's question, inferential role, and limits legible before drawing their supported connection. Complementary observations do not automatically validate one another or establish a single causal chain. Whether they need separate subsections depends on the argument and venue, not a universal clinical/basic or qualitative/quantitative split.

Use the [shared prose standard](anti-overdefense.md) and [continuity method](author-revision.md#build-continuity-before-polishing-connectives) to develop these relationships. Future work, when useful, should resolve a specific question left by the evidence. Use these functions within a combined Results and Discussion when that is the appropriate genre.

### Conclusion

Answer the research question at the level established by the paper and state the resulting knowledge or significance. Synthesize the findings rather than listing endpoints, numbers, or procedural steps again. A defining method contribution or decisive quantity may belong when the article type or author request needs it; neither method recap nor a blanket ban on methods or numbers is universal. Preserve conditions needed to make the conclusion true. Future research may follow from limitations already discussed; distinguish it from completed work and promise no gain. Do not introduce unrelated applications, unreported findings, or speculative defenses. Future work and a separate Conclusion section are optional unless required by the venue or author.

## Explain figures and tables in the main text

Across writing phases, use a numbered short figure or table title by default. Explain the display in the relevant body passage, including any comparison-specific definition, interval meaning or reading condition needed to interpret it. Keep essential units, symbols, panel labels and concise visual keys in the figure or column headers. Add separate explanatory captions or table notes only when the author or venue explicitly requires them. When such notes are required, they support the main-text explanation.

Explicitly introduce every figure and table by its number where the argument uses it, naming relevant panels when useful. Expressions such as “as shown in Figure/Table X” are examples, not mandatory wording. A number-only mention does not explain the display's role. Tell the reader which question it addresses and, when the encoding is not obvious, how to read the important axes, groups, colors, panels or comparisons. Preserve short visual keys and essential local definitions; do not make readers hunt through prose merely to decode a symbol.

Use the main text to develop the observations that matter, their evidence-grounded interpretation and the conclusion they support. For complex figures, explain how panels or visual relationships jointly answer the question. For tables, select the comparisons, tradeoffs and exceptions that advance the argument instead of narrating every cell. Conceptual figures need explanation of their relationships and design roles, not invented empirical findings. These are argumentative functions, not a fixed sequence or one paragraph per display; discuss several related displays together when that makes the reasoning clearer. A simple display may need only a brief, substantive explanation.

Keep the observation, its interpretation and its evidential limits distinguishable. Explain plausible mechanisms only to the degree supported by the sources and results, preserving material negative or mixed findings. Visual differences alone do not establish statistical significance, causation or component efficacy. Do not move a long caption wholesale into the body and call it analysis, repeat the same explanation in both places, or substitute “better performance” for the actual comparison and its meaning. Existing literature rules apply when the interpretation adds an external scholarly claim; direct reporting of supplied results does not itself restart retrieval.

When compressing prose-heavy tables, consolidate shared conditions and use concise configuration phrases while retaining the information that identifies each comparator; explain their scientific role outside the table. Reuse correct assets. A change in stage meaning or actual insertion size calls for checking and adjusting the affected figure, not restarting visual beautification after every prose edit; use the existing [figure](scientific-figures.md) and [document](docx-manuscript.md) size/readability checks together with the text budget.

## Write natural Chinese academic prose

- Prefer established Chinese academic terminology; give a necessary English abbreviation at first occurrence and then use one stable form.
- Preserve official method, dataset, benchmark, variable, and metric identities.
- Apply the [shared prose standard](anti-overdefense.md) to Chinese sentence structure, paragraph progression, and inferential wording.
- Keep internal Git, Gate, review, authority, artifact, and workflow terminology outside the manuscript.

Draft evidence-bearing sections before relying on the abstract or contribution list. The authoring order may differ from the final reading order.

Remove redundancy without removing reasoning needed to establish research significance. When an author identifies weak motivation or literature analysis, add supported comparisons and explanations where necessary; fewer words or paragraphs are not the default improvement. Under an explicit length limit, compress repeated background and secondary implementation details first.

For an actual length-limited revision, use [the shared compression rule](optimization.md#compress-to-the-actual-length-gap), including its proportional edit scope and stopping condition; do not maintain a separate Chinese compression procedure.

## Check the submission-grade Chinese manuscript

Apply [manuscript-quality-control.md](manuscript-quality-control.md) to the complete candidate, using the section responsibilities above, [literature-and-rhetoric.md](literature-and-rhetoric.md) for scholarly support, and [anti-overdefense.md](anti-overdefense.md) for prose. Do not repeat their checks under a separate phase checklist.

This phase is complete only when the Chinese manuscript contains the scientific argument, necessary method explanations and evidence interpretation that later journal adaptation can build on. No unresolved scientific, bibliographic or narrative placeholder may be called submission-grade. Pending author-only administrative metadata can be reported outside the manuscript when it does not affect the argument. If English adaptation would need to reconstruct the scientific spine, reopen the affected content before adapting the format.
