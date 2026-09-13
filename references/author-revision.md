# Author-directed substantive revision

Use this reference when an author asks for a substantial revision to an existing manuscript outside a formal editor or reviewer response cycle. This route can operate within Chinese drafting or English optimization. It is not a response-letter workflow.

## Establish the real revision record

Read the latest author-controlled manuscript and the author's exact requests, annotations, corrections, and accepted decisions. Use an older draft, revision note, controller summary, or generated Markdown only as comparison material unless the author identifies it as the current textual authority.

Keep **textual authority** separate from **revision obligations**. The latest author-controlled version is the only textual starting point, but an unresolved author request from the active version chain remains binding until the author withdraws it, replaces it, or the final artifact demonstrably satisfies it. Starting a new version from its immediate predecessor must not silently close an earlier request merely because that predecessor is now the baseline or its modification note described the work as complete.

Inspect only the immediate predecessor and the still-active requests needed for the current revision. Do not revive superseded drafts or every historical suggestion. When the author says an earlier change was not truly implemented, reopen that exact request and compare the current output with the version and instruction in which the request arose; do not answer it with another free paraphrase of the latest text.

Separate three kinds of instruction:

- **Required outcome:** the scientific or rhetorical change the author expects, such as a convincing motivation, a sharper gap, or a mechanism-based related-work synthesis.
- **Hard invariant:** content or structure that the author explicitly requires to remain, such as a target journal, evidence boundary, section count, or protected result.
- **Suggested means:** a proposed paragraph count, outline, example wording, or organizational device that may help but is not itself the outcome unless the author explicitly confirms it as fixed.

Do not let a suggested means replace the required outcome. Even when a paragraph count or subsection structure is a hard invariant, satisfying that shape does not prove that the requested scientific argument was implemented.

If the request for deep reconstruction and a fixed structure can both be satisfied, do so. Ask for a decision only when two explicit requirements are genuinely incompatible and the choice would materially change the manuscript.

## Make a private revision contract

Before editing, create a compact private map for each requested change:

1. the author's request or diagnosed weakness;
2. the current passage and why it does not yet meet the request;
3. the intended change in scientific meaning, argumentative function, comparison, or reader understanding;
4. the evidence or literature that supports the change;
5. the wording, structure, data, and claim boundaries that must remain fixed;
6. an observable acceptance test in the final manuscript.

Carry forward each item as `open`, `partially satisfied`, `ready for verification`, `satisfied`, `superseded`, or `withdrawn`. A generated revision note cannot mark its own item `satisfied`; that status follows only from inspection of the final manuscript against the acceptance test. When [manuscript-quality-control.md](manuscript-quality-control.md) applies, drafting advances a material item to `ready for verification`; a separate source-first verification pass or an actual independent reviewer assigns final `satisfied` after inspecting the exact candidate and direct evidence.

Keep this map temporary unless the user asks to see it. Do not turn it into a reader-facing checklist or append it to the manuscript.

When a requested change depends on external scholarship, follow [literature-and-rhetoric.md](literature-and-rhetoric.md) before rewriting the affected content. This applies wherever the revision changes background, novelty, theory, design rationale, comparisons, interpretation, application context, discussion, limitations, future work, or a reviewer-facing factual response. Adding citations to the old paragraph structure is not implementation if the requested outcome requires a different scholarly argument.

## Distinguish substantive revision from textual churn

A revision is substantive when it changes at least one relevant relationship in the paper, for example:

- makes the research problem or unresolved gap more precise;
- explains why a design choice is needed rather than merely naming it;
- changes a paper-by-paper catalogue into a comparison organized by a meaningful scientific axis;
- adds or repairs the bridge from prior work to the proposed method;
- makes contributions distinct and ties them to the method and available evidence;
- removes or relocates material that obscures the argument;
- corrects a scientific interpretation, scope, or claim boundary.

Synonym substitution, shortening, sentence reordering, retaining the same paragraph functions under new wording, changing headings, adding citations without using them in the argument, or preserving a requested paragraph count is not sufficient by itself. Do not report a section as "substantively rewritten" solely because its text differs or its length changed.

Translate detailed prompt bullets into connected academic reasoning. Do not write one sentence per instruction item or make a paragraph read like a compliance checklist.

## Test every affected section by function

Judge the revision first by the author's required outcome and the scientific job of the affected passage. Verify that new literature changes the reasoning where warranted, that method or result material remains in its proper section, and that every new factual relationship is supported. Paragraph counts, headings, keywords, citation counts, and text difference remain presentation or artifact checks rather than semantic acceptance.

For an Introduction revision, verify that:

- the opening establishes the actual research object, stakes, and unresolved problem before introducing the proposed method;
- the prior-mechanism discussion leads to the precise gap rather than functioning as a compressed literature list;
- every transition advances problem, limitation, design need, method response, or evidence;
- the proposed components are introduced through their scientific necessity and relationship, not as an implementation inventory;
- contribution items are non-overlapping, identify the new element, and correspond to later method and evidence sections;
- paragraph count and word count remain presentation constraints rather than substitutes for these functions.

For a Related Work revision, verify that:

- each subsection has one explicit comparison axis, such as what is selected, how structure is represented, what objective is optimized, or what must be learned after selection;
- representative studies are compared on that axis using claims verified from the actual sources;
- the synthesis identifies what existing approaches establish, where their mechanisms differ, and which unresolved question motivates the present design;
- the section does not repeat the Introduction's compressed survey or pre-write the Method section;
- literature study requested by the author changes the organization or reasoning where warranted, rather than appearing only in a separate evidence log.

For other affected sections, apply their scientific jobs from [drafting.md](drafting.md) and verify the requested change in the final candidate:

- an Abstract revision changes the problem-gap-method-evidence-conclusion summary without introducing a claim absent from the paper;
- a Method revision repairs definitions, rationale, information flow, or reproducibility rather than only renaming symbols or adding decorative derivation;
- an Experiments or Results revision preserves the actual protocol and evaluation boundary, reports verified observations, and keeps interpretation distinct from measurement;
- a Discussion or Limitations revision uses literature and results to change interpretation or scope without repeating generic caveats;
- a Conclusion revision answers the research question at the supported level and introduces no new evidence, application, or superiority claim.

Across both sections, confirm the same research gap connects coherently to the method design, experimental questions, results, and final claim. If those sections use different gaps, reconcile them before completion.

## Verify implementation in the final artifact

After editing:

1. compare the final manuscript with the author-controlled baseline by paragraph function, scientific claim, and logical connection—not only by character or word difference;
2. for a carried request, also compare against the version and instruction where that request originated, without restoring superseded text;
3. resolve every item in the private revision contract against an exact final location and assign its closure status from the manuscript itself;
4. inspect the actual DOCX, LaTeX, or other requested deliverable, not only a Markdown source, plan, or revision note;
5. treat DOCX/Markdown agreement, section counts, citation counts, successful rendering, and style checks as necessary artifact checks, not semantic acceptance;
6. generate any revision note from the verified final manuscript rather than using the note as evidence that a change occurred;
7. identify any request that is only partially satisfied and state the remaining gap without relabeling it as complete.

When the task meets the manuscript-quality criteria, freeze the candidate and apply [manuscript-quality-control.md](manuscript-quality-control.md) after the drafting pass. Resolve every `Blocker` and `Major` finding and derive final revision-contract status from the rechecked candidate. Use an independent reviewer when requested or materially beneficial; otherwise use a separated source-first verification pass and report that mode accurately.

Claim completion only when the final artifact passes the author's requested outcome, the relevant scientific evidence boundary, the applicable literature gate, and the manuscript-quality gate. Report the material changes, verification mode, and unresolved author decisions concisely; do not expose the private revision contract unless requested.
