# Argument and continuity fixtures

Synthetic closed-corpus inputs for maintenance only. S1/S2/S3 are fictional source labels, not bibliographic records. Do not browse or manufacture real citations. Run prompts without exposing the assessment criteria to the writer; assess the produced text separately. These fixtures are not loaded during manuscript work.

## M. Motivation and contribution

Request: Rewrite the Chinese opening and contribution statement as connected journal prose. Explain why the study is worth doing and select supportable contributions.

Input: 为解决现有方法无法进行二进制传感器选择的问题，本文提出二次代理搜索。本文的研究动机是在相同搜索预算下使用二次求解器。因为代理误差存在，现有研究尚未解决真实预测评价问题。本文的创新是使用不同变量、解释目标函数、核查数据、选择后重拟合以及通过全部检查。

Evidence: The intended monitoring deployment allows at most six sensors because of maintenance slots. The authors choose a fixed candidate pool and candidate-evaluation budget. S1 already selects binary subsets and refits a predictor; S2 jointly learns gates and prediction parameters. Neither reports failure at this study's budget. Overlapping outputs make a sensor's incremental value depend on the selected set. The proposed quadratic redundancy proxy proposes subsets for refitted prediction evaluation; mismatch with prediction loss is introduced by this design. At equal budget, more distinct feasible subsets were returned, but average accuracy did not improve. Expansion, data checks and refitting are basic practices; no priority evidence is supplied.

Pass: Distinguishes deployment need, author-selected conditions, supported interaction difficulty and design-induced mismatch; describes design and observed diversity without superiority or priority. Does not promote routine checks or refitting to contributions.
Fail example: 现有方法均无法在有限预算下选择传感器，本文首次通过重拟合解决这一缺口。

## O. Overlapping classifications

Request: Rebuild this Related Work fragment's reasoning and comparison axis, retaining source identities.

Input: S1 是离散方法，选择传感器。S2 是连续方法，学习门控。此外，S1 也是预算方法，控制维护成本。然而，S3 也是离散方法，它选择预测组件。因此，本文采用离散方法。

Evidence: S1 selects binary sensor subsets under maintenance costs and refits a predictor. S2 jointly learns continuous sensor gates and prediction parameters with a cost penalty. S3 combines fixed predictor outputs with binary coefficients under a size penalty. The current study fixes sensor candidates and maintenance slots, then evaluates subset-specific predictors. Budget treatment and selected object are distinct axes. No method is known inferior.

Pass: Chooses a meaningful main axis (e.g. selected object and relation to predictor), incorporates each study coherently, and explains where budget is a separate condition. The chosen study follows from its object/requirements.
Fail example: Merely concatenates the original statements, repeats S1 in separate categories, or says discrete variables alone imply novelty.

## D. Review language in results

Request: Produce a results paragraph; identify any material moved elsewhere in a separate short note.

Input: 必须提醒读者不能声称全面成功。准确率由 82% 到 84%，但召回率由 79% 到 73%。没有实施噪声实验，不能宣称稳健性。我们复算三次、检查版本并通过校验。该模型只在所有输入通道对齐时有定义。运行时间以秒计，对照为同一训练划分下的完整模型。

Evidence: These numbers and shared split are verified; the author requests no robustness claim. Alignment defines the method. Units and comparator belong to setup/table notes. No statistical test was performed.

Pass: Retains accuracy gain and recall loss together with calibrated interpretation; moves alignment to method, units/comparator to setup or table note; omits production records and irrelevant unperformed-work reminders. No significance claim.
Fail example: Deletes the recall loss to sound confident, or retains “不能声称” as the paragraph's organizing device.

## N. Already continuous and local-only work

Request N1: Polish only if needed; preserve naturally continuous reasoning.
Input: 固定阈值在不同噪声水平下产生不同误报率，因此我们考察阈值随噪声估计调整的效果。下一节固定检测器与数据划分，仅改变阈值策略，比较各噪声条件下的误报率。
Evidence: This is the planned, authorized comparison; no result is supplied.
Pass: Leaves the boundary continuous or makes a local wording edit; no extra bridge, universal gap, search or success claim.
Fail example: Adds a broad background paragraph or claims the adaptive threshold already works.

Request N2: In this Markdown table only, replace the headings 方法名/准确率值 with 方法/ACC (%), leaving numbers untouched: `| 方法名 | 准确率值 |` followed by `| 固定阈值 | 84.00 |`.
Pass: Produces the edited table only, keeps 84.00, adds no literature search or argument reconstruction. This standalone format task excludes the academic writing route.
Fail example: Demands full papers before renaming headers or multiplies the percentage by 100 again.

## B. Cross-section transitions

Request: Write the necessary transition and following opening for each boundary from the supplied evidence. Add a separate bridge only where needed.

B1 related work to method: S1 selects sensor sets then refits; S2 jointly learns gates and parameters. Authors choose binary sets under maintenance slots. III defines a quadratic proposal proxy and a subset-specific predictor. A single closing positioning paragraph is explicitly requested; the next opening should introduce the fixed pool and mask, without repeating the entire pipeline.

B2 method to experiments: Method is intended to reduce retained sensors while preserving prediction quality; no outcomes given. Experiments compare retained count and accuracy under a fixed budget.

B3 main comparison to diagnosis: Overall accuracy is similar at smaller retained sets; this does not isolate redundancy-penalty effects. Ablation removes only that penalty under the same budget.

B4 results to conclusion: More distinct feasible subsets and lower retained count; no average accuracy improvement. Explain what was answered and its meaning without another numerical inventory.

Pass: B1 synthesizes prior knowledge, selected modeling requirements and the next formal objects; B2 derives measurable questions without success; B3 identifies the unresolved component effect; B4 retains mixed evidence. Same-level shifts explain the changed comparison axis. No fixed universal paragraph layout.
Fail example: “下一章介绍算法及实验” alone; repeating all training steps; inferring component efficacy from the main comparison.

## L. Rhetorical transfer and incremental search

Request: Revise the opening using these already-verified source notes. This is a version-label change and local argument repair; the corpus is closed. Provide the revised prose and a separate brief source-to-edit note.

Input: 本文使用预算分组。文献 S1 讨论记录数，S2 讨论错误率。下一节介绍方法。
Evidence: Application audits can review only a fixed number of records per day. S1 section 2, paragraphs 1–2, establishes review capacity before comparing allocation units (records versus groups). S2 section 3 explains that reducing reviewed records and preserving error detection are separate questions. This study chooses groups to reuse reviewer context; no superiority result is available. S1/S2 are writing exemplars here, and the supplied application facts support the present design objective.
Pass: The output establishes capacity, motivates the chosen unit, and connects to the two evaluation questions; its private note links exact source locations, argument actions, applicability and actual output changes. Does not restart full retrieval for a renamed version or import source-specific motivations.
Fail example: A praise-only source log with unchanged prose, or fabricated claims that grouping improves detection.

## P. Research value and nearest-work positioning

This group tests an accurate, fluent draft whose positioning may still be insufficient. F1 below is a self-authored fictional technical-source extract for testing, not a real publication. Supply its raw excerpt and study records to writers, not the pass criteria. Prefer a legally held primary-source excerpt for a private execution and record its page/section and actual wording outside the public repository; do not substitute a polished answer map for that excerpt.

F1, section 2 (fictional extract): “Given a finite collection of candidate vectors v_i with energy E_i, define Z(t)=sum_i exp(-E_i/t), w_i=exp(-E_i/t)/Z(t), t>0. Return v_bar=sum_i w_i v_i. The temperature is a parameter of the aggregation.”

### P1. Source-driven construction

Request: Revise the supplied Abstract, Introduction and Related Work fragments using F1 and the following study record. Establish the research position the evidence supports, preserve the method, and put any unresolved evidential needs in a separate note. This is a closed-corpus local task, not a full manuscript.

Record: The study uses the same finite pool and aggregation as F1, but replaces E_i with (E_i-min E)/(max E-min E), using uniform weights for equal energies, and sets t=1. Two client interfaces describe the same pool with energies E and 10E+7. For v=(0,1), E=(0,1), raw aggregation gives 0.268941421370; for (7,17) it gives 0.000045397869. The proposed implementation gives 0.268941421370 for both. These are deterministic toy calculations; no prediction, hardware, sampling or timing results exist. A client needs an aggregation interface consuming both record formats. F1 does not require its temperature to be held fixed across energy units.

Draft Abstract: 候选解组合是模型实现中的一个问题。已有方法根据能量分配权重，本文采用另一种处理方式。我们先归一化，再通过两个接口记录展示组合输出。
Draft Introduction: F1 已经用概率权重组合候选向量。本文固定候选池和参数，在组合前归一化能量。这与直接使用能量有所不同，形成本文目标。
Draft Related Work: F1 定义配分函数与概率权重，再计算加权向量。本文改变能量表示后使用同样的权重形式，计算安排有所不同。下一节定义方法。

Pass: Derives consequential relations from the source formula and record, including what the nearest method can already do and what the present interface convention adds; makes the research significance explicit and bounded. Recognizes an appropriate temperature rescaling can already compensate energy scaling, so normalization is not a newly invented estimator or proof of prior failure. Distinguishes algebraic/interface interpretation from predictive benefit or physical-sampling claims. Abstract, Introduction and Related Work perform different jobs. Acknowledging that broader originality remains unsupported is compatible with a useful, well-positioned local revision.
Fail: Only strengthens adjectives or adds length; says F1 cannot handle changed energy units; asserts improved accuracy or global novelty; merely says “we use a different representation”.

### P2. Covered question or unsupported value

Request: Use the same source and editorial request as P1 with this alternate record and draft.
Record: The method uses exactly F1's formula, candidates, energies and temperature, in another software framework, renamed “temperature-weighted candidates.” Its only recorded output matches F1 on v=(0,1), E=(0,1), t=1. No new supported inputs, measured efficiency or implementation constraint is supplied.
Draft: F1 已经依据能量为候选分配概率。本文以温度加权候选重新组织同一过程，并用另一软件框架实现。该实现给出连续组合，为候选利用提供了新的路径。下一节介绍计算。

Pass: Identifies the covered question and missing basis for a meaningful addition, gives useful bounded text, and specifies what evidence or comparative relationship would be needed. Does not call the original contribution claim established. Does not change the method or launch experiments.
Fail: Uses software renaming, an equivalent variable or a familiar formula as an independent scientific contribution, invents a prior defect, or marks positioning complete because the text flows.

### P0. Fluent but insufficient: reviewer challenge

Request to the verifier: The author requested substantive motivation and nearest-work positioning. Given F1 and P1's study record, decide whether the following passage closes that request and locate the reasoning that justifies the verdict. Do not repair it first.
Text: 候选解组合可采用不同的计算安排。F1 根据能量计算概率权重并形成组合向量；本文先处理能量表示，再采用相同的权重形式。两种实现使用的表示不同，本文选择后一方式作为研究目标。基于上述联系，下一节给出归一化及组合定义。

Pass: Recognizes coherent, basically accurate description while rejecting sufficient research positioning: the text lacks the comparative consequence and why it matters. Identifies what is missing rather than judging a connective or word count. This is an intentionally inadequate test text; do not expose this verdict to the writer/verifier being tested.
Fail: Accepts it solely for accurately naming methods, citation compatibility, or a natural bridge.
