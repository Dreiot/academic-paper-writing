# Reader-facing quantitative results

Read this reference when an academic manuscript presents quantitative results in prose, tables, or figures. These rules control reader-facing scale and precision only; they do not authorize recalculation, change stored values, or replace the source data and statistical protocol.

## Use a consistent metric scale

- Present AUC, ACC, balanced accuracy, sensitivity, specificity, precision, recall, F1, and other performance measures that the manuscript treats as rates as percentages by default. First confirm whether the source stores the value on a `0–1` or `0–100` scale; convert exactly once.
- When a complete table column uses percentages, place `(%)` in the column header and normally omit a repeated percent sign from every cell. In prose, include the percent sign with the value.
- Keep confidence intervals, standard deviations, error bars, and changes on the same scale as their associated metric.
- Express an absolute difference between percentages in percentage points, such as `0.93 percentage points` or `0.93 个百分点`. Use relative percent change only when that quantity is intentionally computed and identified.
- Do not convert counts, ranks, rule number `K`, dimensions, time, memory, loss, objective values, hyperparameters, p-values, or other non-rate quantities into percentages. Preserve a field's established convention when a percentage representation would be misleading.

## Default to two displayed decimal places

- Display ordinary reader-facing numerical results with two decimal places by default, including percentage metrics, means, standard deviations, confidence-interval endpoints, average model sizes, runtimes, and derived differences.
- Keep integer counts as integers. Use a consistent number of decimal places within the same table column, metric family, or directly compared sentence.
- Apply rounding only at presentation time. Do not round the underlying data, intermediate calculations, statistical inputs, ranking logic, or stored evidence.
- Use additional digits only when two-decimal rounding would change interpretation, collapse a material small difference to zero, obscure a prespecified threshold, or violate a target journal or field convention. State the higher precision consistently for the affected comparison rather than adding digits arbitrarily to isolated cells.
- Report p-values using the target journal convention; in the absence of one, use three decimal places and `p < 0.001` for smaller values. Preserve exact threshold inequalities and use scientific notation when it materially improves clarity.

## Validate the presentation

- Do not mix `0.9365` and `93.65%` for the same metric within one manuscript unless a formula explicitly requires the fractional form.
- Ensure prose, tables, figures, abstracts, captions, and conclusions show the same rounded value and scale for the same result.
- Verify that percent headers, signs, units, confidence intervals, and percentage-point language survive Word or PDF rendering.
- If displayed percentages no longer total exactly 100% because of independent rounding, change precision or add a short rounding note only when the discrepancy could confuse interpretation.
- Preserve negative and mixed results; formatting and rounding must not make an unfavorable or null difference appear favorable.
