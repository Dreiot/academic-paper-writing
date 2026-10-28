# Optional external polishing handoff

Use this reference when the user requests a prompt or handoff for Gemini or another external editor, or asks to assess or integrate a returned polished candidate. Prompt generation remains optional: do not generate one as a routine attachment to manuscript work or infer the request from a wish to reduce formulaic prose. Producing the handoff does not itself authorize uploading material, contacting an external service, or replacing the manuscript with a returned candidate.

## Set the requested editorial role

Select the operation the user requests:

| Operation | Scope and output |
| --- | --- |
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
