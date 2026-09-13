# Manuscript production separation and verification

Use this reference for a complete journal article, a substantial multi-section revision, a major literature-dependent claim change, or a compound task that combines scholarly writing with mathematical development, local evidence reconstruction, numerical checking, current platform verification, figures or tables, supplementary material, or DOCX/LaTeX production.

The hard requirement is a traceable separation between producing a candidate and deciding that it satisfies the scientific and authorial requirements. Subagents and an independent reviewer are useful implementations, not universal requirements. Choose the verification design that best fits the task, available tools, evidence access, cost, and risk.

## Keep one authoritative candidate

Identify one manuscript owner and one authoritative candidate. The owner integrates the prose, resolves evidence conflicts, and preserves a consistent argument and voice. When multiple agents or tools contribute, do not let them independently overwrite the same section or final file.

Freeze or clearly identify the candidate before a completion review. A plan, source draft, revision note, change summary, search log, paragraph count, keyword check, or successful render cannot serve as proof that the candidate contains the required scientific change.

## Choose a proportionate verification design

Use one or more of these mechanisms according to what materially improves reliability:

- **Independent reviewer or subagent:** preferred for a complete paper, broad novelty positioning, high-stakes scientific interpretation, or a demonstrated failure of self-review, when a separate reviewer can directly inspect the candidate and evidence.
- **Specialist delegation:** literature research, local evidence checking, mathematics, figures, or document engineering may be assigned to bounded specialists while one manuscript owner performs integration.
- **Separated verification pass:** when independent review is unavailable or unnecessary, finish the candidate, set aside the production narrative, rebuild the acceptance checklist from the author's original request and direct authorities, then inspect the final candidate source-first rather than validating the writer's intentions.
- **Deterministic or tool-assisted checks:** recompute derived values when authorized, compare manuscript numbers with accepted tables, validate citation identities and source locations, check formula or OOXML structure, and render the final artifact where layout matters.
- **External author or human review:** use when the user requests it or a scientific decision cannot be resolved from available evidence.

Do not call a review independent unless a reviewer that did not participate in drafting inspected the exact candidate and direct evidence. Lack of an independent reviewer does not by itself prevent completion unless the user explicitly requires one or unresolved risk makes the scientific result non-credible; report the verification mode accurately.

## Use explicit responsibility contracts when delegating

When delegation is useful, give each contributor:

1. the exact requested outcome and active author instructions;
2. the authoritative manuscript baseline and candidate, if one exists;
3. the evidence and literature it may use, including exact local paths or source links;
4. its owned responsibility and any files it may modify;
5. protected facts, claim boundaries, and prohibited assertions;
6. the required output and acceptance evidence.

Useful roles include literature and rhetoric research, scientific evidence verification, artifact production, and manuscript review. These are examples rather than a mandatory team shape. Run them in parallel only when their inputs and write ownership do not overlap.

Require factual outputs to use `verified`, `inference`, `conflict`, or `unsupported` and to name the exact source location. A bibliography, search snippet, revision note, or another contributor's assertion is not evidence by itself. The manuscript owner must inspect returned evidence and reconcile contradictions; do not resolve disagreement by majority vote.

## Verify high-impact facts completely

Check every numerical, statistical, novelty/priority, method-characterization, comparative, causal, clinical, policy, and current-platform claim against its direct authority. Verify that every citation supports the exact sentence to which it is attached. Derived values must either be recomputed from authorized data or matched to an accepted result whose derivation and scope are known.

No contributor or verification pass may fill a missing fact from plausibility, copy an unverified description from another paper, or convert an inference into an established result. A verification finding must identify the exact passage, unmet requirement or scientific issue, supporting evidence, practical consequence, and repair direction.

## Review the scholarly argument, not only its parts

Whether review is independent or performed as a separated evidence-based pass, inspect at least:

- whether the research problem, prior knowledge, unresolved gap, method response, evidence, and conclusion form a credible journal argument;
- whether literature coverage and synthesis meet [literature-and-rhetoric.md](literature-and-rhetoric.md);
- whether other work is represented fairly and every material claim has direct support;
- whether contributions are distinct, evidence-linked, and no broader than the manuscript establishes;
- whether explanations and interpretations belong in the correct sections and do not merely restate prompt bullets;
- whether active author or reviewer requests are visibly implemented in the candidate;
- whether the target journal's relevant scientific and rhetorical conventions are met;
- whether the delivered artifact preserves the reviewed content.

Classify findings as:

- **Blocker:** the section or manuscript cannot be considered scientifically credible or factually safe;
- **Major:** the requested scholarly outcome, literature grounding, core logic, or claim boundary is not yet satisfied;
- **Minor:** a localized improvement that does not overturn the section's scientific function or main conclusion.

Paragraph counts, keywords, citation totals, textual difference, schema checks, DOCX/Markdown agreement, and successful rendering may support artifact validation but cannot close a Blocker or Major semantic finding.

## Close the quality gate

Repair supported findings and recheck every material change against the candidate and direct evidence. If an independent reviewer is used, return material repairs to that reviewer when practical; otherwise perform a focused new verification pass that does not rely on the earlier completion explanation.

Do not claim the manuscript or affected major revision complete until:

- no Blocker or Major finding remains open;
- all active author/reviewer requirements have a verified final location;
- all high-impact facts and literature-dependent claims have passed their evidence checks;
- the final delivered artifact, rather than an intermediate source or revision note, was inspected;
- the delivery note accurately identifies whether the result received independent review, specialist checks, separated self-verification, or another review route.

If a Blocker or Major cannot be resolved within the authorized evidence or task scope, deliver the useful work as a provisional draft and state the unresolved item plainly. Do not downgrade it merely to permit a completion claim.
