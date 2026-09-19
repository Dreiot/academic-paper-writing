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

### O1. Concept entry and source-supported achievements

The following source excerpts are self-authored fictional test material, not published papers or real experiment results. F1 has two fictional authors, F2 one, and F3 a group author.

- F1, Lin Lan and Chen Ning (林岚、陈宁), section 2: “Residual-guided Growth (RG) adds a local prediction unit when its residual trigger fires. Backward Extraction (BE) then deletes units under the validation criterion and refits retained coefficients.” Section 4: “On toy regression datasets A and B, with the same split and three seeds, mean unit counts changed from 40 to 24 and 32 to 20 respectively. RMSE changed from 0.21 to 0.22 and 0.18 to 0.18. The comparison is BE against its pre-extraction RG model. No statistical significance analysis was performed.”
- F2, Xu Heng (许衡), section 3: “Binary Extraction (BX) assigns z_j in {0,1} to a fixed set of units. The evaluation E(z)=||y-Hz||^2+lambda sum_j z_j is quadratic for fixed H. It specifies subset inclusion and penalizes retained size. This note supplies a formulation and no predictive or runtime experiment.”
- F3, Structural Learning Group (结构学习工作组), section 2: “Continuous Gate Learning (CGL) jointly updates continuous unit gates and prediction coefficients under a gate penalty. A threshold maps gates to retained units, whose coefficients are refitted. The scope here is the update-and-extraction mechanism; no result table is supplied.”

Author request: Rewrite this Related Work fragment to make the conceptual entry understandable and coordinate author–method introductions in the form “X proposed/used ... to enable/obtain ...” while respecting the actual authors and source support. Preserve source labels. Discuss studies through the common research question rather than separate source cards. Closed corpus, local revision only.
Input: RG 先增加局部单元。BE 再删掉单元并重拟合 [F1]。BX 使用二进制变量、平方项和基数项 [F2]。CGL 更新门和系数，再用阈值提取 [F3]。这些方法不同，本文也进行结构选择。
Local context: A candidate pool determines available local prediction units; deployment cost depends on how many are retained. The present study fixes that pool and examines selection and subsequent coefficient learning; it has no performance result in this task.

Pass: Establishes why size control and the generation/extraction distinction matter, then compares mechanisms and achievements. F1's limited findings retain the comparator, tasks and mixed RMSE behavior; F2/F3 provide capabilities, not invented performance. Author forms remain correct, and studies serve shared comparisons.
Fail example: “林岚等使用 RG 增加单元，再用 BE 删减并重拟合 [F1]。另一方面，许衡使用 BX 表达二进制选择 [F2]。进一步，结构学习工作组使用 CGL 更新门和系数 [F3]。因此，本文研究固定候选池的结构选择。” Even with correct author forms and no invented performance, the reason to control size and the source-supported achievements advancing the comparison remain missing.

## D. Review language in results

Request: Produce a results paragraph; identify any material moved elsewhere in a separate short note.

Input: 必须提醒读者不能声称全面成功。准确率由 82% 到 84%，但召回率由 79% 到 73%。没有实施噪声实验，不能宣称稳健性。我们复算三次、检查版本并通过校验。该模型只在所有输入通道对齐时有定义。运行时间以秒计，对照为同一训练划分下的完整模型。

Evidence: These numbers and shared split are verified; the author requests no robustness claim. Alignment defines the method. Units and comparator belong to setup/table notes. No statistical test was performed.

Pass: Retains accuracy gain and recall loss together with calibrated interpretation; moves alignment to method, units/comparator to setup or table note; omits production records and irrelevant unperformed-work reminders. No significance claim.
Fail example: Deletes the recall loss to sound confident, or retains “不能声称” as the paragraph's organizing device.

### D1. Figure/table explanation belongs in the body

This is a synthetic text-editing fixture, not a real experiment or a figure-production task. Request: rewrite the supplied body and verbose captions/notes in Chinese, preserving numbering and supplied values. Help readers understand the figure and table and the supported implications; use concise captions with necessary decoding information. Also handle the simple Table 2 proportionately. No external interpretation, new analysis or asset regeneration is requested.

Record: Figure 2 has a shared x-axis K (retained units). Panel (a) plots mean AUC (%) at K=8,16,32 as 91.00,93.00,93.20, with SD error bars 0.40,0.30,0.50 over five repeated runs. Panel (b) plots corresponding mean runtime in seconds 1.00,2.00,5.00, with no error bars. All use the same specified data splits; no significance test, causal mechanism or task-utility preference is supplied. Table 1 compares those K=32 and K=16 models: AUC (%) 93.20/93.00, recall (%) 88.00/81.00, runtime (s) 5.00/2.00. Table 2 only identifies fixed split sizes: training 600, validation 200, test 200.

Old body: 结果如图2和表1所示，效果较好。表2列出样本数。
Old Figure 2 caption: 图2. 规模研究。横轴是保留单元数。图(a)是 AUC，误差条是五次重复的标准差，图(b)是秒计的时间。规模增加时 AUC 上升，16之后变化较小，时间仍增长，所以读者应该看两个子图的关系，而不是只看最高点。32到16速度更快，但这还需要与表1的召回率一起考虑。正文应该详细解释为什么这个取舍重要。
Old Table 1 note: 表1. 两个模型的对比。这里应该详细解释规模、AUC、召回率和时间之间的取舍。16个单元的模型不能只因为 AUC 相近就被称作全面更好，读者需要理解召回率差异及部署选择。
Old Table 2 caption: 表2. 数据划分。

Pass: Body introduces Figure 2 and its relevant panels, explains their joint evidence and key tradeoff, connects Table 1's recall decline to the conclusion, and explicitly addresses Table 2 briefly. Figure caption retains panel identity, units or clear encoding, and SD/repetition meaning where needed; analytical prose moves into the argument without being pasted unchanged. Does not claim statistical equivalence, significance, causal explanation or universal best K. Does not enumerate all cells or force a full analysis paragraph for Table 2.
Fail example: Shortens captions but leaves “如图2所示，效果较好” as the entire body; removes SD meaning to minimize caption length; or reads a higher AUC point as proof of universal superiority.

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

For a depth-allocation revision of B1, use the following B1-depth input instead of duplicating the simple transition test. Its sources are fictional technical excerpts.

- G1, Representation note, section 2: “Inclusion/exclusion can be represented by binary z. Fixed unary costs plus pairwise interaction costs have a quadratic polynomial form. This represents that stated objective; extra terms in another training objective require their own treatment.”
- G2, Learning note, section 3: “For retained local units, f_z(x;theta)=sum_j z_j h_j(x) g_j(x;theta_j) / sum_j z_j h_j(x), defined for positive retained response. Coefficients theta are fitted for each subset. For fixed full-pool response matrix H, ||y-Hz||^2+lambda sum_j z_j is a quadratic subset proxy; it contains no fitted local coefficients and is not an identity for the complete normalized training loss.”

Author roles: A (domain review) introduces direction and representational fit; B (optimization review) adds prior modeling foundations and feasible paths; Method formally defines the current proxy and subset prediction. Do not change these roles or the method. Return revised A/B/Method and, separately, the destination of removed implementation details. Keep the evaluation pair at the end naturally continuous; edit it only if necessary.

Draft A: 我们选择二次求解器，所以需要解决把训练目标塞进接口的困难。为此本文提出二进制掩码、固定响应代理、子集归一化、重拟合和验证选择，调用接口 20 次，将参数 seed=7 写入配置并检查恢复点。本文研究这一完整流程。
Draft B: 局部模型是重要的预测方法，模型结构值得研究。另一方面，G1 使用二进制形式。G2 拟合系数。为此本文再次提出掩码、代理、归一化、重拟合和选择。由于形式天然适配，完整训练目标可直接精确求解并取得加速。
Draft Method: 近年来，局部模型受到了广泛关注。本文研究掩码、代理、归一化、重拟合和选择。为比较结构规模与预测质量，所有候选使用相同的数据划分。下一节在这一划分下报告保留单元数及预测误差。

Local record: The pool is fixed. Binary inclusion and retained count describe the study's structural choice. The prescribed proxy is E(z)=||y-Hz||^2+lambda sum_j z_j with fixed H and lambda>=0; a backend returns finite masks. Each nonempty valid subset renormalizes retained responses, refits coefficients and is validation-evaluated. The complete predictor is G2's f_z; positive retained response is required. Twenty calls, seed=7 and recovery-state checking are implementation facts, not comparative evidence. There are no verified speed or prediction gains, no exact full-objective conversion, and no guarantee of a globally optimal returned mask.

Pass: A introduces selection properties and their useful representational match before route-induced issues; B adds G1/G2 relations and correctly locates feasibility at the proxy/formulation layer; Method begins formal objects instead of broad background. Preserves necessary learning relationships without repeating the complete method in every section. Moves interface details appropriately and leaves the already continuous evaluation pair without an extra bridge. Not every source needs a criticism or a performance result.
Fail example: “因此本文采用二次求解器；然而，G1提出二进制形式；为此，本文在两个综述小节再次介绍全部训练步骤。” Reject the remaining reverse motivation and repeated information even if it avoids explicit unsupported speedup.

For owner-integration maintenance, extend B1-depth rather than rerunning O1/B1-depth as separate prior tests. Use its fictional G1/G2 extracts and the following additional context and fresh draft. Author request: revise the domain-review ending, adjacent optimization review and Method opening in one authorization; choose blocks by dependency, retain their actual draft text, check relevant neighbors, then have the same owner edit one continuous candidate and verify it source-first. Do not copy an earlier test output. No new experiments, method changes or per-block approval are requested.

Whole-paper question: within a fixed pool of local prediction units, how can discrete retention and subset-specific prediction learning be organized to study the size/quality tradeoff? Confirmed terms are “candidate pool,” “retained unit,” “quadratic structural proxy,” and “validation prediction error”; use z for the mask, m for pool size, K for retained size. A prepares the direction, B develops source-based modeling relations, and Method defines this study's objects. Author-approved style sample: “候选池界定可以选择的结构，保留规模刻画最终使用的单元数。” This guides expression only.

Additional local record: the method uses B1-depth's E(z) and f_z; H is fixed on structural-training data, and coefficients are fitted per valid subset. The author chooses a held-out validation split to rank these fitted candidates by prediction error, breaking ties by smaller K. That ranking/tie rule is a study record, not a statement in G1/G2. No speed, test-accuracy or globally optimal-mask result is provided. Shared evaluation context remains: “各候选沿用同一数据划分。后文在此基础上比较保留单元数与预测误差。”

Fresh draft A: 为了运行二次后端，我们研究局部规则。本文采用 B 掩码、固定响应、重新归一化、参数训练和验证选择。我们的完整训练流程包括所有这些步骤。由于二次形式适合接口，本研究具有计算收益。
Fresh draft B: 模型压缩一直很重要。G1 讨论二进制，G2 拟合模型，因此本文使用规则掩码、固定响应、重新归一化、参数训练和验证选择。拟合后以验证误差和规模排序的机制来自 G2。我们研究这一流程。
Fresh draft Method: 本文再次提出以上流程。b 是规则子集，H 是响应，结构损失等于完整模型损失。保留规模记为 R。各子集拟合系数并以验证误差、较小规模选出最终模型 [G2]。各候选沿用同一数据划分。后文在此基础上比较保留单元数与预测误差。

Observe actual block and integration artifacts rather than a plan alone. Pass requires owner edits across the boundary, consistent argument/terms/symbols, new information in each part, source citations that stop at their supported clauses, and study-specific validation rules attributed to the local record. Local checks and an integrated check have different scopes; neither reopens untouched evidence or requires another user approval. No fixed block count, agent count or comparative model experiment is needed. A preserved local draft may contain a later-repaired issue; judge the final integrated text and the documented repair without relabeling its history.

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
