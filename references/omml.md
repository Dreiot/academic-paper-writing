# Editable Word mathematics with OMML

Use this reference for mathematical content in DOCX or Word-compatible output. For LaTeX manuscripts, retain LaTeX mathematics and follow the target template instead.

## Establish mathematical meaning first

- Typeset only equations supported by the method, code, derivation, or user-approved design.
- Preserve variable names, indices, dimensions, domains, constraints, optimization variables, and operator meaning.
- Define each important symbol at first use and keep it consistent across prose, equations, algorithms, tables, and figures.
- Include equations needed to state the problem, objective, mechanism, or reproducible update. Do not add decorative derivations to make the method appear more complete.
- If the mathematical claim or derivation is ambiguous or conflicts with evidence, use a Claim Decision before encoding it.

## Use native OMML structures

- Use inline `<m:oMath>` for mathematical expressions inside prose.
- Use `<m:oMathPara>` containing `<m:oMath>` for display mathematics.
- Represent fractions, subscripts, superscripts, combined subscript/superscript, radicals, n-ary operators, delimiters, functions, and matrices with their corresponding OMML structures such as `<m:f>`, `<m:sSub>`, `<m:sSup>`, `<m:sSubSup>`, `<m:rad>`, `<m:nary>`, `<m:d>`, `<m:func>`, and `<m:m>`.
- Do not leave LaTeX commands, UnicodeMath source, manual underscores, Unicode superscripts, text approximations, or equation screenshots in the final DOCX.
- Do not put an equation number inside the mathematical expression. Use the target template's equation-paragraph, tab-stop, field, or borderless layout mechanism.

## Apply mathematical typography consistently

Follow the target journal or supplied Word template. In the absence of a specified convention:

- scalar variables, parameters, and indices are italic;
- vectors and matrices are bold italic;
- named functions, operators, digits, punctuation, and transpose markers are upright;
- fixed identity or constant symbols use the field's established convention.

When a journal requires a particular mathematics font, set the document math font and mathematical runs consistently; changing only the surrounding body font is insufficient. Preserve an existing template's working math configuration unless the user asks to replace it.

The body-font fallback does not select the mathematics font. In particular, do not set the document math font to Times New Roman solely because Western prose and digits use Times New Roman. Preserve a compatible working math font or apply the target journal's required mathematics font across the document.

Treat a display equation as part of its sentence. Apply punctuation and explanatory prose according to the sentence logic and journal style. Number only equations that are referenced or required by the venue.

## Convert source mathematics carefully

- From LaTeX or UnicodeMath, parse the expression and generate OMML rather than pasting source tokens into Word.
- Compare grouping, operator precedence, limits, accents, norms, cases, matrix dimensions, and delimiters against the source after conversion.
- Keep multi-line equations as coherent aligned mathematics instead of independent text lines when the template supports it.
- Use ordinary text inside mathematics only for genuine labels or conditions, with the correct upright styling.

## Validate the DOCX

Use [docx-manuscript.md](docx-manuscript.md#render-with-the-tool-that-matches-the-deliverable) for renderer choice, verification scope, reuse of unaffected page checks, and unavailable-renderer handling. For affected mathematics:

1. inspect the DOCX package and confirm expected `<m:oMath>` and `<m:oMathPara>` elements exist;
2. confirm required source expressions are present and editable; for a complete conversion, cover every source display equation and required inline expression;
3. check that no formula was replaced by an image or left as raw LaTeX or Unicode pseudo-math;
4. verify symbol names, indices, equation references, and numbering against the manuscript text;
5. inspect the affected rendered pages and adjacent pagination for clipped fractions, misplaced limits, broken matrices, missing glyphs and detached equation numbers; use whole-document checks when the impact is global, without repeating still-valid checks after a local correction.
