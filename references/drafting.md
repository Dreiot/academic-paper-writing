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

Within normal abstract length, compress the actual need, specific question, design response and principal supported result. “The field is important” followed by “we propose a method” does not establish motivation. Let the question indicate why the response matters, without requiring a literature review, a particular connective or a fixed sentence count. Use exact numbers only when verified and introduce no contribution absent from the paper.

### Introduction

Establish why the research question matters and its specific position relative to what is already known, then introduce the method and verifiable contributions. Apply the research-value and contribution tests above. A declaration of the study objective or an inventory of method components does not replace this reasoning; a narrower design question still needs a reason to be investigated.

Judge the Introduction by whether this reasoning is established, not by paragraph count, length, citation count, or coverage of an instruction checklist. When revising an existing Introduction in response to author feedback, follow [author-revision.md](author-revision.md) and verify the requested argumentative change in the final manuscript.

### Related work

Supply the research development, nearest-work comparisons and source-supported boundary analysis that substantiate the Introduction's position, following [literature-and-rhetoric.md](literature-and-rhetoric.md#derive-positioning-from-the-nearest-work). Use meaningful comparison axes rather than one procedure description per source. The ending may lead into the method, but a bridge cannot replace comparison reasoning missing from the body. The Abstract, Introduction and Related Work serve the same research question at different levels; do not copy the same motivation paragraph across them or impose a fixed paragraph template. Honor explicit author structure requirements.

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

Remove redundancy without removing reasoning needed to establish research significance. When an author identifies weak motivation or literature analysis, add supported comparisons and explanations where necessary; fewer words or paragraphs are not the default improvement. Under an explicit length limit, compress repeated background and secondary implementation details first.

## Check the submission-grade Chinese manuscript

- The research need, chosen objective, supported obstacle, method, experiments, and conclusion form one argument; a claimed literature gap has direct support.
- Every substantive claim has supporting evidence or is explicitly framed as a hypothesis or objective.
- Every literature-dependent statement has passed the required focused or comprehensive literature gate, including claim-level source support and any required journal-rhetoric study.
- Motivation and positioning requirements pass the substantive level of the [reader-recovery test](manuscript-quality-control.md#test-what-the-reader-can-recover); coherent method description alone does not close them.
- Related Work supports that position through source-grounded comparisons rather than repeating the Introduction or Method.
- Symbols and component names remain consistent across text, formulas, tables, and figures.
- Equations needed to understand the method are present and explained; decorative derivations are absent.
- Negative and mixed evidence is not hidden, and limitations are not repeated mechanically.
- No unresolved scientific, bibliographic, or narrative placeholder remains in the reader-facing manuscript; any pending author-only administrative metadata is reported outside it.
- A later target-journal adaptation should not need to reconstruct the core problem, literature gap, method rationale, result interpretation, or conclusion. If it does, reopen this phase before adapting the journal format.
- No unrequested technical-note, evidence-index, or supplementary-index section has been appended to the Chinese master manuscript.
- The anti-overdefense checks pass.
