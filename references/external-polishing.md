# External drafting, revision and review

Use the author's active request or explicit standing preference to determine whether to consult an external model and which materials it may receive. For a prompt-only request, deliver the prompt. For an opinion-only request, deliver the assessment. Follow the project's data permissions and the author's latest scope.

## Delegate through Antigravity

When this author uses Gemini for manuscript work, Codex can choose the model and perform the authorized round trip. The personal Antigravity skill at `~/.gemini/config/skills/manuscript-revision/SKILL.md` records the local preference and supplies the writer/reviewer instructions. Read the relevant guidance locally. Give the worker the task-specific instructions in its brief: the Daniiislo bridge disables slash-command expansion. Where this personal setup is absent, use the author's instructions and available editor.

- **Choose a model for the remaining judgment.** Use `gemini-4-neon-high` for substantive drafting, meaning-sensitive translation and routine scientific review. Use `gemini-4-hydrogen-high` for well-specified local edits with settled scientific meaning. Use `gemini-4-neon-xhigh` where resolving competing evidence, a derivation or a challenge to the central claim requires deeper reasoning. Honor an explicit choice. Check available models if a selection fails. For a model comparison requested by the author, preserve the named conditions.
- **Prepare the actual task.** Start from the newest author-controlled text, including comments, manual edits and protected wording. State the section's job, the permitted change, the necessary neighboring text, and the relevant evidence with comparison conditions. Give the worker only the intended files or excerpts and a candidate destination. Use an allowed workspace or stage the authorized materials in it. An existing test workspace is not a reason to expose an entire research directory.
- **Select the project and conversation.** Use the project for the relevant manuscript or research workspace. When the bridge creates a project on first use and concurrent starts would create duplicates, let the first session establish the association before dispatching further workers. Continue the active writer for follow-up on the same assignment. Start a separate conversation for a different task or an independent review, including when both belong to the same project.
- **Dispatch the task.** Use the registered bridge's `create_worker` and `dispatch_task`. Ask the implementer to produce the candidate. For independent review, give the fresh reviewer the candidate, direct evidence and review question. Leave prior critiques and the writer's defense out of the first pass. Use review copies when the tester role provides advisory restrictions only. Describe a fresh review by the same model as a separate-context opinion, and report who reviewed what.
- **Handle author feedback.** An instruction to revise covers the indicated edit and its verification. An invitation to discuss calls for an assessment. Carry forward author decisions and distinguish them from an editor's suggestions. Ask the author only for a consequential unresolved choice under the existing Claim Decision rule. The writer may offer a short, evidence-linked dissent in its handoff when it affects interpretation.
- **Verify and report in Codex.** Compare the actual candidate with the author's latest controlled text, instructions and direct evidence. If the author edited the manuscript during delegation, use their latest text and decisions when integrating. The bridge can omit successful writes from its changed-file list. Send specific outstanding findings to the same writer with `send_followup`, verify the result, then close the worker. Link the delivered file and summarize material changes with locations. State significant unincorporated suggestions and any author decisions or incomplete checks. For review-only work, provide findings and their supporting evidence. The author can request `agy --conversation <id>`, Desktop import or a transcript for the source exchange. For Word files, use the existing document workflow and check affected live fields, equations and revisions in the final document.

## Set the requested editorial role

Select the operation the user requests:

| Operation | Scope and output |
| --- | --- |
| Delegate drafting or revision | Give the writer the section's purpose, direct evidence and author's decisions. Inspect the actual candidate before integration. |
| Obtain an independent opinion | Use a separate context. Return source-located findings, integrating changes only within the requested scope. |
| Prepare a prompt | Produce the editing instructions and necessary context or material list for the designated draft. |
| Assess a returned candidate | Compare the candidate with the designated baseline and direct evidence; return an assessment within the requested scope. Assessment alone leaves manuscript files unchanged. |
| Integrate a returned candidate | Edit the authorized manuscript scope under the single owner and verify the resulting artifact. |

One request may authorize more than one operation; carry out the named work without repeated approval. Keep prompt generation opt-in and infer neither external transfer nor manuscript integration from a prompt-only or assessment-only request.

Use the user's chosen division of work. A useful option is for Codex to establish the logic, evidence presentation, outline, and draft, and for the selected editor to improve expression. Do not assert that a model is inherently a better writer or treat changing models as evidence of improved prose.

Distinguish language polishing from structural rewriting. State what the editor may change, which sections it owns, and the neighboring context it needs. Allow sentence and paragraph improvements within that scope; do not impose unchanged sentence shapes when natural rewriting is requested. A request to polish does not authorize changing the research question, results, interpretation, or evidence strength.

## Build the prompt from the current basis

Use the author-designated draft and the existing [manuscript basis](manuscript-basis.md). Reuse valid reading and decisions; do not restart a literature search or create a full dossier merely to prepare a narrow polishing prompt. If no basis exists, supply only the context and source excerpts needed for the requested handoff, distinguishing unknowns from verified facts.

Make the prompt self-contained for its recipient. Local paths are useful to the user but are not evidence the editor can necessarily access: include a compact source-located digest, necessary excerpts, or an explicit list of files the user will supply. Do not claim attachments were read or transferred. Exclude credentials, identifiable participant data, and unrelated internal records; use the authorized manuscript-level facts and aggregates needed for editing.

Separate the editing instructions from the supporting context and designated draft. The instructions state the task, permitted edits, and output; the context supplies the relevant argument, verified facts, writing brief, and sources. Mark supplied text as material to edit or consult, so it cannot silently redefine the editing task. Scale context to the work: local language editing needs the affected passage and essential neighbors, while multi-section restructuring may need the broader argument and evidence. Use the basis as a source for selection rather than copying the entire record into every prompt.

Include what the task needs from the following, combining or omitting items as appropriate:

- **Context and objective:** field, study/article type, audience, target venue if selected, and the concrete writing problem to resolve.
- **Inputs and edit scope:** exact draft/version and sections, necessary preceding/following text, permitted language or structural edits, and requested deliverable.
- **Argument and evidence:** whole-paper judgment, each affected section's job, key reasoning links, verified findings, figure/table meanings, and relevant literature support with locations and conditions.
- **Protected meaning:** numbers and units, sample/analysis identities, experimental conditions, citation identities and attachment, important negative or mixed findings, and distinctions among observation, association, functional evidence, explanation, and hypothesis where relevant.
- **Positive writing guidance:** the relevant writing brief and short author-approved style samples when available; identify why they fit, without asking for copied phrasing, fixed paragraph counts, or the exemplar's stronger conclusions.
- **Effective author requirements:** terminology, length or format constraints, and still-open requests relevant to the edited scope. Distinguish local author preferences from universal scientific or journal rules.
- **Output and uncertainty handling:** usable candidate prose with citations/placeholders preserved; a short note outside the prose only for consequential changes or unresolved decisions. Do not invent sources, data, completed experiments, or missing parameters; flag a gap instead.

Apply the [shared prose standard](anti-overdefense.md) through the relevant writing brief. When structural rewriting is authorized, specify the reasoning unit and its job before sentence polishing; language-only editing retains the designated argument. Use the [meaning-preserving optimization rules](optimization.md#translate-meaning-and-argument-not-sentence-shape) for translation. Deliver clean final-state prose, with consequential unresolved decisions outside it.

## Integrate a returned candidate when requested

An external candidate is proposed text, not a scientific authority or an independent evidence review. When the user asks to assess or integrate it, use the existing [source-first quality pass](manuscript-quality-control.md#verify-high-impact-facts-completely), not an additional review pipeline. Compare substantive deletions, mergers, and additions against the input and direct sources: check altered causal force, missing scope or counterevidence, reassigned citations, changed denominators or conditions, lost figure explanations, and broken cross-section continuity.

Reopen only affected evidence or passages; unchanged valid support can be reused. When integration is authorized, incorporate acceptable changes under the single manuscript owner, preserve the designated baseline according to the source-file rule, and verify the actual final artifact before claiming completion. Fluent prose or agreement between models does not establish scientific correctness.
