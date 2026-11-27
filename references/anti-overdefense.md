# Evidence-grounded, continuous academic prose

This is the shared prose standard for substantive writing, analysis, translation, revision, and polishing across the manuscript. Apply it within the requested genre and scope as an **internal two-step sequence**—not an extra approval gate or separate deliverable:

1. **Draft the reasoning chain directly (Pass 1):** Establish shared setup and scope once where they belong, then state supported judgments and develop their evidence, comparisons, and explanations in natural academic prose without attaching preventive disclaimers to each sentence or paragraph ending.
2. **Verify scope and prune overdefense (Pass 2):** Check factual and inferential accuracy against direct records, integrate material counterevidence into the reasoning it qualifies, and apply the deletion and meta-language checks below so every remaining qualification does real logical work.

## Establish supported judgments

Express the best-supported judgment directly and develop the evidence and reasoning that make it useful. Problem development, literature synthesis, methods, and interpretation can need different orders. Choose the order that advances the question rather than a fixed claim-first opening or a `claim -> evidence -> caveat` loop in every paragraph.

Carry scientific scope through accurate research objects, measured endpoints, explicit comparators, and calibrated inferential verbs (for example, distinguishing *lowers task-equal mean error in the evaluated pool* from *establishes global optimality*), rather than asserting broadly and retracting in the next clause. Once methods or experimental setup establish a shared condition, continue within that scope without restating it after every result.

When establishing or substantially reorganizing the manuscript's argument, organize it around the research question and the central contributions supported by the evidence. Select and order results, figures, and tables by what they establish, qualify, or rule out. State supported advantages, observed tradeoffs, and material adverse or mixed outcomes together as part of one analytical comparison rather than framing paragraphs around what the paper "cannot claim."

## Run five diagnostic checks

Run these checks in Pass 2 on the drafted text (proportionately to the affected scope) after the reasoning chain is in place, so defensive self-auditing does not fragment sentence generation during Pass 1.

### 1. Phantom-objection check

Use neutral academic language at the strength the evidence supports. Keep a concession or contrast only when it resolves a real evidential distinction, a confounded or adverse observation in the record, or an actual reviewer concern. Delete promotional inflation, preemptive replies to imagined reviewer attacks, routine reminders of unperformed experiments unrelated to the active claim, and self-assurance remarks about the writing or verification process (such as stating that sections now agree or that checks were run three times).

### 2. Deletion check

Read each qualification, hedge, or scope reminder together with the established methods, setup, and immediate context:

- If removing the phrase leaves the proposition accurate and its inferential strength unchanged, **delete it** (for example, drop repeated paragraph-end tags like *within this experimental configuration* or *this does not prove universal superiority* when the main verb is already descriptive and scoped).
- If a condition is needed for the sentence itself to be true, fold it concisely into the main clause (for example, *Across the 48 memory-feasible candidates, Method A achieved...*) instead of appending a separate disclaimer sentence.

### 3. Logic check

Let the section's scientific job determine the progression. Give readers the context needed to follow the question, develop the comparison or mechanism, and carry it to the supported interpretation. State a qualified judgment at its accurate strength from the start instead of overstating and then retreating.

Remove empty meta-discourse and throat-clearing openers that announce rather than advance reasoning—such as `It should be noted/emphasized that`, `From an evidential perspective`, `In this section we will`, `需要指出的是`, `需要强调的是`, `值得注意的是`, `从证据角度看`, and `本节将`. Treat contrast or boundary markers (`however`, `this does not imply`, `并非……而是……`, `这并不意味着`) as diagnostic signals: retain them only when separating two genuinely plausible interpretations or introducing real counterevidence, and rewrite them when they merely hedge an already accurate statement. Use uncertainty verbs when the evidence requires them; do not add automatic hedges to a verified descriptive observation.

### 4. Information-gain check

Give each sentence a clear grammatical spine and primary job while linking sentences within a paragraph through **given-to-new progression**: let a concept, constraint, or observation introduced near the end of one sentence anchor the opening of the next (through natural reference, a concise condition phrase, or a genuine contrast) instead of cold-starting consecutive sentences with the same repeated subject (`Method A... Method A...` or `Both implementations... Both implementations...`). Merge adjacent short sentences that share the same subject or experimental control layer so setup conditions read as connected prose rather than an itemized checklist; split an overloaded sentence when it stacks findings, literature contrast, mechanism speculation, and scope defense together. Let sentence length vary naturally.

Write for disciplinary peers using established technical terms. Explain a familiar concept or routine step only when this study's specific use changes interpretation or reproducibility. Delete empty signposting sentences that merely announce a display or the next sentence (such as standalone `Figure 2 shows the MAE of each device` when the figure number can sit directly inside the comparative sentence), and delete clauses that repeat the preceding point in different words. Retain exact technical terms that name a defined quantity or operation; vary surrounding syntax rather than inventing synonyms for core objects. Keep repository paths, run IDs, hashes, and production logs outside the manuscript.

### 5. Paragraph-focus check

Open each paragraph with the **scientific question, analytical angle, or comparison step** it advances—picking up the thread left by the previous paragraph—and fold unchanged control conditions (`under the same split and evaluation budget`) into a brief modifier rather than spending the opening sentence on a standalone compliance statement. Develop the paragraph through the steps of that one question or comparison, keeping linked sources, observations, and their immediate interpretation together while the reasoning continues. A new method name, metric, figure/table mention, or citation does not by itself start a new paragraph or require a miniature closing summary. Consolidate repeated setup and order the evidence; deleting blank lines alone does not create continuity.

When examples shift across tasks or settings within a paragraph, make the shared comparison axis explicit. Start a new paragraph when the question, level of explanation, or inferential direction changes enough to give the reader a useful boundary. Vary paragraph scale with the argument, without fixed counts, uniform lengths, or a mandatory caveat or conclusion at every paragraph ending. Use the [continuity method](author-revision.md#build-continuity-before-polishing-connectives) for cross-section transitions.

## Concentrate necessary boundaries

- Place design assumptions, data splits, sampling or analysis units, metric definitions, and shared comparison conditions once in Methods or Experimental Setup. Introduce a local scope statement only when a specific analysis changes population, denominator, or protocol. Across a multi-section draft, resist **long-context defensive ratcheting**: do not re-append global conditions (`within this finite candidate pool`, `as a descriptive comparison`) in later Results or Discussion paragraphs once earlier sections have established them and the local verbs remain calibrated. Independently readable abstracts and summaries carry the concise conditions required for their own statements.
- Present material negative or mixed results directly beside the finding they qualify, as concrete observations or tradeoffs rather than repeated apologies. Distinguish specific adverse observations from general design limitations already stated elsewhere.
- Consolidate shared limitations of design, sample, measurement, external reach, and unperformed validation once where the genre places them (normally Discussion), explaining their consequence once. Conclusions state the resulting knowledge and significance at their supported scope rather than ending with a routine disclaimer list.
- Keep method-defining and interpretation-critical conditions in the main text; move reproduction-only parameters (buffer sizes, polling intervals, seeds, CLI flags) to a named appendix, supplement, or accessible code/config destination, and verify that destination in the final deliverable. Follow [section responsibilities](drafting.md#give-each-section-a-scientific-job) and [display guidance](drafting.md#explain-figures-and-tables-in-the-main-text). Selection timing, data roles, hardware, or software remain scientific content when they define the measured endpoint; production bookkeeping does not.
- In reviewer revision, answer the reviewer directly in the response letter while integrating any reader-relevant clarification seamlessly into the manuscript's own argument.

## Run a final authoring-quality pass

When a draft stalls, oscillates between claim and withdrawal, reads like a list of negations, stacks defensive clauses, or accumulates scar tissue across multiple revision rounds, rebuild the smallest complete reasoning unit cleanly before polishing surface words: state the concrete question, express constraints positively as method definitions or evaluation protocols, arrange the supporting observations and contrasts with given-to-new sentence openings, and rewrite neighboring joins so multi-round additions read as one coherent thought rather than layered patches. Mechanical sentence splitting or connective insertion cannot repair inverted or defensive logic.

Preserve scientific meaning, citation attachment, necessary conditions, and material contrary findings—not the location or wording of every disclaimer or prior-round patch. Reuse the manuscript's writing brief and exemplar learning; style refinement alone does not restart literature search.

## Final prose audit

Review the affected passages and their neighboring transitions in the final artifact as a continuous reader-facing text, setting aside chat-history debates and superseded intermediate drafts:

- **Language-only edits:** Change the smallest span needed for natural clarity and compare directly against the source sentence so quantities, comparators, conditions, inferential verbs, and citations remain intact.
- **Substantive drafting and revision:** Verify key claims and numerical statements against [direct evidence](manuscript-quality-control.md#verify-high-impact-facts-completely) and any confirmed user Claim Decision. Read paragraphs and section seams in sequence to confirm that section and paragraph openings lead with the active question or object (rather than repeated subject checklists, standalone compliance lines, or back-to-back section previews/recaps), then apply the **Deletion check** and **Logic check** one final time to strip residual meta-discourse, duplicated caveats, and process assurances. Check [abstract result selection](drafting.md#abstract) when applicable, and apply [quality verification](manuscript-quality-control.md) at the task's scale.
