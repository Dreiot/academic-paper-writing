# Literature grounding and journal-rhetoric study

Read this reference whenever manuscript work introduces, removes, reframes, interprets, compares, or verifies content whose correctness or scholarly force depends on external literature. This trigger follows the claim, not the section name. It includes background, problem importance, prior work, novelty and positioning, theoretical rationale, method comparisons, design choices, dataset or metric descriptions, experiment interpretation, application context, discussion, limitations, future work, reviewer responses, and evidence-bearing figure or table narration.

Pure formatting, citation-style conversion, faithful translation, and local copyediting do not require a new search when they preserve every scientific meaning, claim boundary, and citation attachment. If such work changes or adds a literature-dependent proposition, apply this reference to that proposition before finalizing it.

Direct reporting of verified local results, exact definitions of the paper's own method, and local code or artifact facts do not trigger literature search by themselves. Apply this reference when the manuscript compares them with external work, interprets them through external knowledge, generalizes beyond the observed evidence, or uses them to support novelty or disciplinary positioning.

If the user explicitly defines a closed evidence corpus or prohibits external browsing, work within that boundary. Verify relevant sources in the permitted corpus, identify the result as corpus-bounded outside the manuscript when needed, and do not claim current, exhaustive, or global novelty coverage. Use a Claim Decision only when the requested scholarly claim cannot be made credibly within that boundary.

## Choose the necessary search depth

Use the smallest search that can support the requested scholarly outcome, but never substitute a token search for a literature-dependent judgment.

- **Comprehensive search:** required for a complete journal manuscript, a new or substantially reconstructed scientific section, a cross-family synthesis, novelty or state-of-the-art positioning, target-journal intellectual adaptation, or a major author/reviewer revision that changes the paper's scholarly argument.
- **Focused search:** appropriate for a narrow paragraph, definition, mechanism, comparison, interpretation, or missing citation. Search every named or directly implicated source and enough independent primary papers to support the scope of the sentence. A synthesis or generalization requires at least three directly relevant full-text primary papers for that claim cluster unless the literature is demonstrably smaller.
- **Citation verification:** appropriate when checking whether an existing citation supports an unchanged claim. Open the cited primary source and verify the exact proposition and source location. Broaden to a focused or comprehensive search when the claim is broader than the source, the source disagrees, or the cited work is not primary.

Search before drafting the affected passage. A fresh search requires live use of available scholarly search, publisher, DOI, or connected-library tools; model memory and the manuscript's existing bibliography cannot establish current coverage. User-supplied references and a local Zotero library are valuable starting points, but they do not by themselves establish comprehensive coverage. If live discovery is unavailable, focused verification may proceed from supplied full texts, while a comprehensive-search gate remains unpassed and must be reported as such.

## Build a coverage map

Before a comprehensive search, identify the literature families that the manuscript actually depends on, such as:

- the research object and problem setting;
- the central method family and its terminology variants;
- direct comparators and the nearest novelty-adjacent approaches;
- theoretical, algorithmic, or empirical mechanisms used to justify the design;
- application-domain evidence invoked in the manuscript;
- the target journal and the closest high-quality venues.

Form multiple query families from these concepts rather than repeating one broad query. Use at least two independent scholarly discovery routes, plus target-journal searching and backward/forward or related-work citation chasing when those routes are available. Prefer official publisher pages, DOI records, discipline-specific scholarly indexes, and author manuscripts only when the publisher full text is unavailable.

Prioritize peer-reviewed primary research that is directly relevant and exposes enough method or evidence to support the intended claim. Recent papers from the target journal or closest reputable venues and foundational papers both have roles; citation count alone does not define quality. Do not use search snippets, listicles, generic web summaries, or a later paper's description of an earlier method as the final authority for a scientific claim.

## Set an adaptive comprehensive-search target

Use numeric ranges to plan effort, not as universal minima or completion proof. For a broad, complete journal manuscript, a reasonable starting target is usually to screen about 20–30 potentially relevant peer-reviewed papers, read about 8–12 core papers in full, and study about 3–5 recent target-journal or closest-venue papers as journal-rhetoric exemplars. Increase the search when the manuscript spans several research families, makes a strong novelty claim, or new sources continue to change the map. Reduce it for a demonstrably narrow field or a tightly bounded task. Do not stop merely because a count was reached or continue reading irrelevant papers to satisfy a quota.

The hard completion conditions are coverage and convergence:

- every major literature family actually used in the manuscript has enough directly relevant primary evidence to support the synthesis; three full-text papers per family is a useful default, while a smaller set is acceptable only when the search demonstrates that the literature itself is smaller and the claim is narrowed accordingly;
- every named comparator and the work closest to a novelty or priority claim is inspected at its primary source;
- enough recent target-journal or closest-venue exemplars are studied to identify recurring rhetorical practices rather than copying one paper;
- an additional complete pass across the planned query families and citation-chasing routes reveals no new major method category, closer competing work, or claim-changing contradiction;
- the search log explains the achieved coverage, remaining gaps, and why further search is unlikely to change the affected manuscript argument.

If a demonstrably narrow literature, inaccessible full text, or unavailable scholarly source prevents adequate coverage, record the exact shortfall, narrow the affected claim, and continue unaffected work. Do not silently waive the condition, infer unavailable content, or mark the affected section or novelty statement final.

## Recover access to necessary full text

When institutional or publisher authentication, a reusable signed-in session, or an additional account may be needed, also read [literature-access.md](literature-access.md).

When a source is necessary but its full text is unavailable, try lawful access routes in this order as applicable:

1. the official publisher page, DOI record, open-access copy, accepted author manuscript, preprint, or institutional repository;
2. the user's supplied files, project literature folder, local Zotero library, or an already authorized scholarly connector;
3. an institutional subscription or publisher account that the user can authenticate in their own browser or connected session;
4. a legally obtained PDF that the user uploads or identifies by local path.

It is acceptable to ask which institutional or publisher access the user has and, on first enrollment or after a session expires, to ask the user to sign in through the normal site or connector flow. Never ask the user to paste a password, session cookie, access token, MFA code, or other secret into the conversation, and never store such credentials in the manuscript workspace. After first human verification, prefer automatic reuse of the approved local session under [literature-access.md](literature-access.md). If access still fails, identify the exact paper and affected claim, use the abstract only for bibliographic discovery or a claim it plainly establishes, and keep any deeper interpretation unverified.

## Verify sources at claim level

For each included paper, verify the title, authors, venue, year, volume/issue/pages or article number, and DOI when available. Then record the precise proposition supported and its location in the full text.

Abstracts and metadata can establish bibliographic identity and help discover papers. They are not sufficient authority for method mechanics, comparative limitations, novelty, causal interpretation, or a detailed claim when the full text is required to judge it. Mark preprints and non-peer-reviewed sources explicitly and do not present them as peer-reviewed evidence.

Give complete claim-level attention to:

- novelty, priority, and state-of-the-art statements;
- descriptions of another method's objective, mechanism, assumptions, limitations, or results;
- comparative, causal, clinical, safety, policy, or broad application claims;
- current platform, dataset, benchmark, or journal facts;
- any literature statement that determines why the paper's method is needed.

If sources conflict, preserve the conflict, determine whether the scope or conditions explain it, and use the Claim Decision process when the manuscript's conclusion would materially change.

## Learn how strong papers construct the argument

For comprehensive journal work, inspect the relevant full sections of the journal-rhetoric exemplars, not only their abstracts or individual sentences. Build a private cross-paper pattern map covering:

- how the opening establishes the research object, stakes, and concrete problem;
- how earlier work is grouped by question, assumption, mechanism, or limitation;
- how the unresolved gap is derived from what prior work already establishes;
- how the need for a design choice leads into the proposed method;
- how contributions are separated and connected to later evidence;
- how methods, experiments, discussion, limitations, and conclusion are kept in their proper roles;
- how the venue handles paragraph scale, transitions, citation placement, and claim strength;
- how many studies are synthesized within one paragraph, where paragraph breaks mark a genuine argumentative turn, and how the final sentence of one paragraph prepares the next.

Use patterns that recur across several strong papers to design the manuscript's own reasoning. Do not copy sentences, distinctive phrasing, or the complete organization of one paper. Learning journal rhetoric is evidence for editorial decisions, not permission to imitate an author's expression.

Prefer rhetoric exemplars with the same article type and a related methodological domain. Keep their editorial role separate from scientific evidence: a paper chosen to study writing style supports a manuscript claim only when its content independently supports that claim.

For Related Work, use the fewest paragraphs that preserve real changes in research question, comparison axis, or synthesis role. Discuss several studies together when they contribute to the same comparison; do not assign a paragraph to each paper or method merely because the search log lists them separately. A blank line must reflect an argumentative turn, not the boundary between two source notes.

## Keep private working evidence

Maintain task-local temporary records proportionate to the search:

- a search log containing date, discovery route, query, candidate, inclusion/exclusion reason, and full-text status;
- a source-claim matrix connecting each manuscript proposition to a stable source identity, intended citation key or live field, exact support location, and manuscript location, with status `verified`, `inference`, `conflict`, or `unsupported`;
- for comprehensive work, a cross-paper rhetorical-pattern map recording shared conventions, useful alternatives, and paper-specific choices that must not be copied.

These records are quality-control material. Keep them outside the reader-facing manuscript and, by default, outside tracked manuscript deliverables; do not commit or deliver them unless the user requests it. Do not add a literature evidence index, verification log, or technical appendix to the paper unless requested.

## Pass the literature gate

Do not call the affected manuscript content final until:

- the required search depth and coverage are complete;
- every material literature-dependent statement is linked to appropriate primary evidence;
- bibliographic identities and citation attachments are correct;
- DOI/title duplicates, citation keys or live fields, in-text citations, and final bibliography entries resolve to one consistent source identity without orphaned additions;
- novelty and broad comparative wording matches what the search can actually establish;
- the rhetorical study has changed the organization or reasoning where the previous draft was inadequate;
- unresolved conflicts and inaccessible decisive sources are disclosed outside the manuscript.

Keyword presence, citation count, paragraph count, a populated evidence log, or successful document rendering cannot satisfy this gate. In the delivery note, state the search scope, full-text coverage, and any unresolved literature limitation concisely; provide the private records only when requested.
