# J2, D5 and J3 — scoped revision inputs

Self-authored maintenance inputs extending the existing J (adaptation) and D (prose/conditions) cases. The filename markers describe the separable request and source files to supply; do not give a writer the other request variants or the verification paragraph in behavior-cases.md. All evidence and venue references are fictional. These samples are not runtime manuscript templates.

## File: a-small.md

# a-small request

Use the complete latest main text and source record in a-source.md. This is a text-only length-limited English revision. Only a small overrun remains. Make proportionate edits to meet the limit and stop unnecessary compression; keep the mature article as the starting point.

The baseline has 737 words under the counting rule below. The main text must contain no more than 697 words, including headings, table cells and captions. Count tokens matching [A-Za-z0-9]+(?:['’.-][A-Za-z0-9]+)*, so Markdown punctuation does not itself count. Supplement and delivery note are excluded. This is not a page limit; no rendered document is provided or requested.

Deliver main.md, supplement.md and a short delivery.md. Preserve the source-supported scientific meaning, accepted names and evidence scope; choose natural prose rather than targeting a paragraph count. No new search, experimental data or figure production is requested. Work on the baseline directly, not another compressed output.

## File: a-large.md

# a-large request

Use the complete latest main text and source record in a-source.md. This is a text-only length-limited English revision. A substantial reduction is required. You may reorganize and relocate supporting detail while retaining a usable main argument and keeping the supplement coherent.

The baseline has 737 words under the counting rule below. The main text must contain no more than 471 words, including headings, table cells and captions. Count tokens matching [A-Za-z0-9]+(?:['’.-][A-Za-z0-9]+)*, so Markdown punctuation does not itself count. Supplement and delivery note are excluded. This is not a page limit; no rendered document is provided or requested.

Deliver main.md, supplement.md and a short delivery.md. Preserve the source-supported scientific meaning, accepted names and evidence scope; choose natural prose rather than targeting a paragraph count. No new search, experimental data or figure production is requested. Work on the baseline directly, not another compressed output.

## File: a-source.md

# A source package — self-authored simulation

This is fictional, project-neutral evidence, not a real paper or journal. The latest English main text below is the content baseline. Preserve the accepted name Poolwise Selection (PS). Its existing figures have readable English labels; no drawing or file rendering is requested. Deliver revised main.md, supplement.md and a brief delivery.md. Work only from this corpus, with no search or experiments.

## Direct records

S1: Uniform Retention keeps the first eight elements of a fixed candidate list and refits coefficients on training data. Its published toy study demonstrates fixed-size prediction, not optimal selection.
S2: Joint Gating learns gates and coefficients together under a size penalty. The authors report a lower average error across their two tasks; this is not an experiment on PS or a comparison with S1.
Local: PS enumerates a finite pool of eight-element subsets, refits each subset on training data, and chooses by validation error. The tested pool is not exhaustive. One final held-out test is used per task with five repeated training seeds. Task A/B/C mean MAE: PS 1.00/1.40/2.20, Uniform 1.20/1.60/2.00. The task-equal mean is 1.5333 versus 1.6000. MAE standard deviations across seeds: PS .10/.20/.30, Uniform .10/.20/.20. No significance test or component-isolation experiment exists.
Figure 1 identity `paired-error-cost`: panel (a) MAE, panel (b) platform-reported solver time in ms; same task order A/B/C and method colors. Solver-time means PS 4/5/6, Uniform 3/3/3. Timing excludes pool construction, transfer and final refitting. There are no end-to-end measurements. SD bars in (a) describe the five training seeds, not confidence intervals. Table 1 describes settings, not new results.
Existing supplement S1: common split sizes 600/200/200; seed identifiers 11–15; fixed retained size eight; validation tie broken by lower retained-list index; no test data enter selection. Reference identities S1/S2 and all records here are fictional labels.

## Main text to revise

### Introduction

Selecting a compact predictor from a fixed library involves two related decisions: which elements to retain and how to fit their coefficients. A size constraint makes the deployed predictor small, but does not by itself determine which retained elements will work well together. This motivates studying subset-specific fitting within a fixed retained size rather than comparing models that change both their size and their fitting procedure. The present work addresses this question within a finite candidate pool.

Poolwise Selection (PS) constructs candidate subsets, fits each subset on training data, and selects a fitted candidate using validation error. The method therefore links subset identity to its fitted predictor while keeping the retained size fixed. We construct subsets, fit their coefficients, and then select on validation data. The following sections introduce the comparison, describe the method, and report the results in that order.

### Related work and method

Uniform Retention fixes the retained size by taking the first elements in a candidate list and refitting their coefficients on training data [S1]. Joint Gating instead learns gates and coefficients together under a size penalty; its authors observed lower average error across two toy tasks [S2]. These approaches differ in the relationship between structure and fitting, not merely in their names. PS examines fitted alternatives at the same size as Uniform Retention; it does not test Joint Gating or inherit that method's reported gains.

For a candidate subset s, let f_s denote the predictor fitted using only the training split. PS evaluates each fitted predictor on the validation split and returns a member attaining the smallest validation error within the evaluated pool. The pool is finite and not exhaustive. This definition identifies both the candidate set and the data used to choose among its members. All retained subsets have eight elements, so the local comparison changes subset choice while retaining size and coefficient refitting. Because training a candidate and selecting it use different splits, test results do not determine which candidate is returned.

### Evaluation settings

Both methods use the same training, validation and test partitions and five training seeds. Mean absolute error (MAE) describes held-out prediction error, and its reported standard deviation describes variability across those seeds. Tasks contribute equally to the overall mean, rather than being weighted by their numbers of samples. The platform also reports solver time. This timing endpoint excludes pool construction, data transfer and final refitting, so it measures a narrower operation than the full procedure. Reproduction details are given in Supplement S1.

Table 1. Comparison configuration.

| Method | Configuration |
| --- | --- |
| PS | This method uses the same training, validation and test partitions as the other method, retains eight elements, refits coefficients on training data and chooses a fitted candidate by validation error within the evaluated subset pool. |
| Uniform Retention | This method uses the same training, validation and test partitions as the other method, retains eight elements, refits coefficients on training data and takes the first eight elements in the fixed candidate list. |

### Results

Figure 1 addresses the error and measured processing cost of comparing fitted subsets at a fixed size. Panel (a) shows MAE for tasks A, B and C, with standard deviations over five training seeds. PS has lower mean error on A and B, but higher error on C: the paired means are 1.00 versus 1.20, 1.40 versus 1.60, and 2.20 versus 2.00. Its task-equal mean is 1.53 compared with 1.60 for Uniform Retention. The aggregate reduction therefore does not describe every task, and the adverse result on C remains relevant to the interpretation.

Panel (b) uses the same task order and method colors to show solver time: PS takes 4, 5 and 6 ms, compared with 3 ms in every task for Uniform Retention. Reading the panels together relates task-dependent predictive differences to additional solver time. It does not establish end-to-end acceleration. This comparison concerns selection among fitted candidates; it does not isolate an independent component effect. The next section concludes the paper by returning to the question introduced earlier.

Figure 1. Error and solver-time comparison: (a) mean MAE with standard-deviation bars across five training seeds; (b) platform solver time in milliseconds. Task order and method colors are shared across panels.

### Conclusion

At a common retained size with training-only refitting, PS lowers task-equal mean error in the evaluated pool while increasing error on one task and increasing platform solver time. This identifies a conditional selection tradeoff, not a universal improvement or a globally best predictor.

## File: b.md

# B / D5 — external suggestions, self-authored simulation

Request: 按下列建议精修摘要和方法—结果片段，取有据且有益的部分，不照单全收。给出可直接使用的中文 main.md 与简短 delivery.md。没有期刊已确认的字数限制；闭合材料，不检索、不做实验，不改变研究对象。现有作者决定仍是：本文比较有限候选池内的选择，不宣称全局最优或组件独立有效。

Current abstract: 本文在开发期确定的候选生成范围内比较两种选择策略。对同一评估池，策略甲的任务等权平均误差低于乙，但任务B的误差较高。平台记录的求解时间描述返回候选所用的求解阶段，本文未测量端到端加速。

Current body: 研究先形成候选，再在同一候选池内进行选择。候选形成之后，研究在相同池中选择方案。开发期共生成60个候选，查看开发集的内存使用后去掉12个超内存预算候选，形成48个评估候选。两个选择策略使用这同一个池；最终任务测试结果未用于筛选候选。阶段内的误差—规模非支配仅指这48个候选中的关系。甲返回的一个候选未出现在乙本次返回的集合中。

Current results: 三项任务A/B/C的误差，甲分别为1.00/1.50/2.00，乙为1.20/1.40/2.30。任务等权均值分别为1.50和1.6333。平台记录甲的求解时间20 ms、乙25 ms；没有数据准备、传输或重拟合耗时。两个策略不仅选择规则不同，返回的子集也不同，因此这不是固定子集下的组件开关实验。确定性并列排序以候选序号较小者优先，决定返回成员身份。采用 `mean(axis=tasks)` 汇总任务，而非汇总全部样本。制作脚本的导出重试和文件编号在内部记录中。

Source P: 以上候选计数、开发期筛选时点、集合身份和数值均已经核实。筛选规则是在查看开发集内存使用后确定；未查看最终测试结果。未枚举所有可行模型，也没有证明另一策略的能力边界。求解时间与端到端时间不同。没有统计显著性或独立组件干预的结果。
Source S1 (fictional primary excerpt): “We assign binary subset indicators and refit prediction coefficients after subset selection.”
Source S2 (fictional primary excerpt): “We jointly optimize continuous gates and coefficients before thresholding the gates.”
Official fictional venue excerpt: 图注需标明分面和误差条含义；没有禁止报告开发期选择过程的条款。两篇示例论文都用了简短图注，但它们不是本任务的官方规范。

Supplied suggestions (not accepted author decisions):
1. 合作者：前两句在同一层级重复，合并；mean代码语法换成读者可理解的统计定义。
2. 导师：开发期看过内存再筛选容易引起质疑，删掉过程，统一写为预先确定且完全独立的候选池。
3. 另一模型：平均下降可以写成全部任务改善，更简洁。
4. 另一模型：把“候选池内非支配”改成“全局Pareto最优”，去掉繁琐限定。
5. 合作者：乙本次没返回甲的候选，说明乙无法产生该候选。
6. 导师：20对25毫秒足以写计算效率领先和端到端加速；候选选择的差异也证明组件有效、预测器最优。
7. 编辑建议：将 S1/S2 合成“已有方法都不重新拟合系数，因此本文弥补这一缺陷”。
8. 另一模型：英文论文通常只说一次限制，摘要中的开发期、同一池和未测端到端可删；两篇范例图注短，故期刊强制删除全部分面解释。

## File: c.md

# C / J3 — stage integration, self-authored simulation

Request: 基于下列最新中文内容和有效决定，将过时英文片段更新为自然英文 main.md，同步 supplement.md 和 figure-map.md，并用 delivery.md 简述实际变化。figure-map 仅是已有图的对象/标签修改说明，不绘图、不渲染。没有字数限制。不改真实论文，不检索、不实验。适用现有期刊适配路线，尊重内容与操作身份。

Latest Chinese main text:
引言：候选结构不同会改变需要拟合的预测器，因此本文把结构形成、训练拟合与验证选择区分，分析固定候选池中的预测取舍。这一问题要求知道返回的是哪个已拟合模型，而不只是给筛选器换一个名称。
框架概述：训练数据形成结构池，各结构在训练数据上拟合，验证集从已拟合模型中选择一个，测试集仅评价最终返回模型。
方法：原写法有两个阶段：阶段一称“生成”，包含结构形成与系数拟合；阶段二称“选择”，按验证误差选择已拟合候选。对每个结构s，在训练集上求出系数theta_s，形成f_s。返回 argmin_s E_val(f_s)，域为实际已拟合的有限候选池。这是池内选择，不是全部可行预测器的最优性证明。并列时按候选序号排序。阶段一形成结构、拟合系数；阶段二选择已拟合候选。（最后一句重复了前述完整流程。）
贡献：区分固定池中的拟合与选择关系，并通过已完成的候选对照报告取舍，不宣称额外算法模块。
结果：表2中方法在任务A误差1.00、对照1.20，在任务B为1.40、对照1.30；图4上面板显示这些误差，下面板显示返回模型规模，分别为方法8/8、对照8/8。相同规模不意味着两个模型相同，拟合结构仍可能不同，故该对照不是组件独立作用证据。

Stale English:
Introduction: We introduce a new jointly learned validation architecture with globally optimal predictors. The pipeline generates structures, fits their coefficients, and selects candidates; all sections follow this complete pipeline.
Overview: Generation takes training data and produces fitted candidates, and Selection uses validation error. We again generate structures, fit coefficients, and select candidates.
Method: Two stages jointly learn candidate structures and coefficients using validation data. Equation (3) gives the global optimum. Contributions: a new third optimization module independently improves every task.
Results: Table 2 and Figure 4 demonstrate uniformly improved error at the same model size. All explanations have been aligned.

Existing supplement S1: 原阶段一包括训练数据上的结构生成与拟合，原阶段二只在验证数据上选成员。候选池含12个结构，固定规模8，输入有2个通道；这些数值不因阶段改名变化。测试集没有用于拟合、选择或决定阶段重组。式(3)和主文同一 argmin 关系，引用图4与表2。
Existing figure asset `train-fit-select`: 当前有 Generation 与 Selection 两个分组框。Generation 中有“training -> structures”和“structures + training -> fitted candidates”两条操作关系；Selection 中为“fitted candidates + validation -> returned model”。另有“returned model + test -> evaluation”箭头。现有英文标签和画面清晰，原始图数据关系正确。结果图资产 `error-size` 对应图4，分面a误差、b规模；表2资产为 `heldout-comparison`。

Effective author decisions: 改为三个叙述阶段，正式名称 Candidate generation、Candidate fitting、Validation selection；只是拆分原第一个叙述阶段，不增加运算，不把验证数据用于训练。论文保留研究问题、独立贡献角色和结果条件；删除同层级重复流程即可。当前交付按图1（框架）、图2（误差/规模）、表1、式(1)编号；对象身份优先于数字。维持现有资产，仅标明框架分组/标签需要的变化。
Direct source record: 中文操作、补充材料参数和结果已核实；旧英文是待修正对象。数值和数据职责以中文记录为准，不支持新增模块、全局最优或全面优越。图/表/式原编号只是编辑身份，不等于阶段数、通道数或规模。
