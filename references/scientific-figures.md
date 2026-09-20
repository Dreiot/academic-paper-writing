# Scientific manuscript figures

Read this reference when a manuscript needs a new figure or a substantial revision to an existing figure. Figure production must preserve the manuscript's evidence boundary while giving conceptual illustrations a consistent, journal-appropriate visual system.

## Treat visual quality as part of scientific communication

Figures and tables are prominent entry points into a paper's reasoning and evidence. Treat workflows, principle and mechanism diagrams, and result visualizations as substantive communication, with visual appeal an explicit quality requirement alongside scientific accuracy and technical clarity. Aim for professional, journal-appropriate finish through intentional composition, hierarchy, typography, color, linework, alignment, whitespace and a coherent reading path. Correct labels and connected boxes alone do not demonstrate effective visual explanation.

Choose the visual representation from the research question, verified relationships and intended reader understanding. Make the central idea, relevant technical operations and dependencies readily understandable, with enough detail to explain how the method works or what the evidence shows. Let the research determine the balance between overview and detail. Preserve creative freedom: do not prescribe paper-specific objects, a fixed layout, a panel count or a mandatory visual vocabulary. Match complexity to the information; a simple design can be complete when it communicates the necessary relationships well.

Evaluate the figure both on its own and at its actual manuscript size. Aesthetic refinement should improve comprehension and emphasis while preserving the meaning and visibility of the scientific content. Use the shared style brief and target-journal requirements to keep the visual set coherent without forcing different scientific roles into identical compositions. Keep substantial explanation in the body under [drafting.md](drafting.md#explain-figures-and-tables-in-the-main-text), with concise captions and the local information needed to decode the display.

## Classify the figure before production

For a complete methods manuscript or broad rewrite, first identify the visual roles actually needed: explaining the overall coupled method and presenting empirical evidence are different roles. Check existing assets for scientific validity and reuse suitable ones. If an overview is needed to understand feedback, shared variables or the relation between learning and final output, plan it before producing only result plots; absence of a separate user request for a flowchart does not by itself exclude it from complete manuscript work. Do not mandate a framework figure when the method is already clear without one.

Use two primary classes:

1. **Conceptual or illustrative figure:** a workflow, principle diagram, mechanism illustration, method overview, conceptual architecture, or graphical explanation that communicates the verified design without encoding measured results.
2. **Result or evidence-bearing figure:** any plot, chart, heatmap, confusion matrix, embedding, ablation figure, sensitivity figure, resource comparison, dataset composition, study-flow count, sample image used as evidence, statistical display, or other visual whose marks encode observations, measurements, labels, sample identities, or quantitative conclusions.

Classify by what the visual communicates, not by its layout name. A CONSORT-style flowchart or dataset pipeline containing actual participant or sample counts is evidence-bearing even though it is a flowchart. If a composite contains result panels, produce every result panel deterministically from authentic data and keep generated illustration outside those panels. Do not use generated backgrounds, icons, textures, or decorative data-like marks inside a result figure.

## Follow the target journal

When a target journal is known, verify its current requirements for figure dimensions, single- or double-column width, resolution, file format, color mode, font size, line weight, accessibility, and AI-generated or AI-assisted imagery. A supplied official template remains the formatting authority.

If the journal prohibits generated scientific illustrations or requires disclosure, follow that policy and surface any material conflict before preparing a submission figure. Do not label a raster ImageGen output as editable vector art, and do not convert formats or upscale an image in a way that falsely implies additional source detail.

When no journal is selected, use a journal-neutral scientific design: clean background, restrained color, legible labels at final print size, colorblind-distinguishable encodings, and no decorative elements that compete with the scientific message.

## Establish one visual system per manuscript

Before the first new conceptual figure, keep a compact style brief within the existing task note where practical, covering:

- palette and background;
- shape language, line weight, arrow treatment, and icon abstraction;
- spatial treatment and perspective appropriate to the content;
- typography, label language, capitalization, and notation treatment;
- information density, whitespace, panel labels, and caption relationship;
- intended journal width, aspect ratio, and output resolution.

Derive this brief from the target journal, supplied template, and existing accepted manuscript figures. Reuse the same brief in every ImageGen prompt. After selecting the first satisfactory conceptual figure, use it as a style reference for later figures when the image tool supports references. Keep deliberate differences for scientific roles, but do not let palette, rendering style, arrow logic, icon family, or visual depth drift between figures.

Unless the user, target journal, or supplied figure template specifies otherwise, use SimSun for Chinese figure text and Times New Roman for English text, digits, and Western punctuation. Apply these fonts to deterministic overlays, chart labels, legends, axes, and panel letters. Ask ImageGen for the same typography where text must appear in a generated draft, but do not trust the generated raster to establish exact font identity or spelling; replace precision-critical text with a verified deterministic overlay.

## Generate conceptual figures with the latest built-in ImageGen model

Use the built-in `image_gen` tool directly for workflows, principle diagrams, mechanism illustrations, and method-overview figures. For this academic-paper workflow, this user-selected route overrides the generic preference to construct a simple diagram directly in SVG or other code-native shapes. Use the built-in tool's current default and latest generally available model; do not pin a model version in this Skill. Name a model version only when the runtime confirms it. Do not switch to an API or CLI fallback, or deliberately select an older model, unless the user explicitly requests that route.

For each conceptual figure:

1. ground every component, relationship, direction, and stage in the verified manuscript, method specification, or user-approved design;
2. use the `scientific-educational` or `infographic-diagram` prompt route as appropriate and include the shared style brief, target aspect ratio, panel role, and avoid list;
3. do not invent modules, causal arrows, equations, variables, datasets, performance values, or biological or physical structures;
4. minimize text embedded by the image model. Add precision-critical labels, equations, symbols, numbers, and panel letters afterward with a deterministic editable overlay when necessary;
5. inspect the generated image for arrow direction, topology, duplicated or missing components, label accuracy, visual ambiguity, and unintended quantitative implications;
6. make targeted corrections for scientific meaning, technical explanation, visual hierarchy, professional finish and final-size readability while retaining the shared style brief; stop when these material checks pass, or report the unresolved limitation instead of continuing open-ended cosmetic variations;
7. save the selected project-bound image with a stable descriptive name and retain enough prompt and source context to reproduce its visual intent.

A conceptual illustration explains the method; it is not experimental evidence. Use a concise caption to identify it as a schematic where needed, and explain its relationships and scientific role in the main text under [drafting.md](drafting.md#explain-figures-and-tables-in-the-main-text). Neither caption nor prose may turn generated appearance, spatial arrangement or relative size into an observed quantitative result.

## Generate result figures only from authentic local data

Create result and evidence-bearing figures with deterministic plotting, analysis, or domain-specific visualization code operating on the authorized local data and result artifacts. Do not call ImageGen or another generative image model for any result figure or evidence-bearing panel.

- Preserve the exact observed values, sample identities, group labels, units, missingness, negative results, mixed results, and uncertainty represented by the source.
- Do not invent plausible points, smooth away inconvenient variation, remove outliers, interpolate missing values, change denominators, or add significance markers without an authorized analytical basis.
- Use fixed seeds and record the transformation when a reproducible visualization algorithm is stochastic, such as an embedding or layout.
- Retain a regenerable link from the figure to its local source files, selected rows, preprocessing, metric definitions, plotting code, and relevant parameters. Keep production provenance outside the reader-facing caption unless the journal requires it.
- Validate plotted coordinates or aggregates, axis limits and direction, units, legends, colors, error bars, sample sizes, labels, and statistical annotations against the source data.
- Follow [numeric-reporting.md](numeric-reporting.md) for percentage scale, two-decimal display defaults, percentage-point differences, and justified precision exceptions in axes, legends, annotations, and captions.
- If required result data are absent or not authorized, leave an explicit placeholder or omit the figure. Never use a generative model to fill the gap.

Give result visualizations the same attention to composition, legibility and professional finish as conceptual illustrations. Choose a presentation that makes the important comparisons and relationships clear, while preserving observed magnitudes, uncertainty and material adverse or mixed evidence. Styling may not alter, hide or exaggerate the result or imply unsupported relationships. Prefer vector or high-resolution deterministic output when supported by the plotting route and target journal.

Design each figure for its final manuscript placement rather than generating or plotting first and shrinking later. Use the target journal's single- or double-column width when known; otherwise fit within the document's available text width while preserving aspect ratio. Check effective raster resolution and label size after insertion. If the intended placement makes labels or scientific structure unreadable, recompose or split the figure instead of accepting an oversized page, distorted aspect ratio, or miniature text.

## Assemble and validate the figure set

Check the complete manuscript figure set, not only each image in isolation:

- visual hierarchy and reading order make the main idea or comparison apparent, and technical detail supports understanding rather than merely listing component names;
- composition, typography, color and linework have a coherent professional finish; assess concrete visual weaknesses at final size, not conformity to one preferred layout;

- conceptual figures share the approved visual system and remain faithful to the method;
- result figures use a compatible typographic and color system without imitating generated illustration textures;
- the same component, dataset, method, group, or variable uses consistent naming and color across figures unless a clear legend explains a necessary change;
- every label, equation, number, and arrow is readable at intended single- or double-column size;
- captions distinguish schematic explanation from observed results and retain essential decoding information and required data scope; substantial explanation and interpretation follow the shared main-text rules;
- numbering and panel references agree, and the body actually introduces and explains each figure's role, findings or design relationships rather than only citing its number;
- raster images meet actual resolution requirements, vector outputs remain genuinely vector, and no watermark, model artifact, malformed text, or clipped element remains;
- the final DOCX or PDF render preserves figure sharpness, placement, captions, and page flow.
