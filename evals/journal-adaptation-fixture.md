# J1: Mature main text and supplement adaptation — writer input

Self-authored, project-neutral simulation. All study records, source labels T1/T2 and the venue below are fictional test materials, not real literature, research findings or current journal requirements. The excerpts are the complete permitted corpus for this bounded exercise.

## Author request

请将下列已成熟的中文主文与补充材料改写为自然学术英文，作为模拟期刊的 Methods Article。交付 main.md 和 supplement.md，保持必要的公式、表格及已有图形的引用；无需 DOCX/PDF 或绘图。可按英文叙述习惯调整段落、缩减重复，不设字数或段落数。使用闭合材料，不联网、不重新检索、不运行实验。下列版本是唯一内容起点，命名决定与尚有效的修改要求仍适用。普通笔误按来源直接修正，研究定位不变。单独提供简短交付说明，不把工作记录写进正文。

模拟期刊格式摘录（测试给定的当前、已核定要求）：主文图、表、公式、算法各自从 1 编号；补充图表使用 S 前缀；表名、图名常规字重，表格列名加粗；正文保留图表分析。没有本用例之外的页数限制或声明要求。引用保留测试来源身份 T1/T2，不补造 DOI、作者或正式书目信息。现有图形已使用英文标签并通过本测试设定的尺寸检查，仅保留其资产身份与译后题注即可。

## Effective author decisions

- D1：英文方法名已确定为 Reliability-weighted Window Fusion (RWF)，比较方法使用 Fixed-Weight Fusion (FWF) 和 Adaptive Window Fusion (AWF)，不要重新命名。
- D2：贡献是研究共同固定窗口下的权重调整及其误差—代价表现，不主张首创自适应融合或普遍优越。
- D3：上一轮要求在结果正文解释图3上下两部分为何需要一起读，并保留跳变工况的反向结果。版本说明曾写“完成”，但当前正文只引用图3；该要求尚未撤销。
- D4：对正文“FWR”按已确认命名修正；差异用描述性语言。本轮可以落实 D3，但不改研究目标。

## Verified source extracts and study record

T1, synthetic source, Mechanism §2: “FWF computes the arithmetic mean of two estimates in the same prescribed observation window. It does not estimate reliability weights. Its evaluation concerns stationary sequences.” This source establishes the equal-weight operation, not inability to process a changing sequence.

T2, synthetic source, Mechanism §3: “AWF updates inverse-residual weights and selects the observation-window length jointly. Reported comparisons therefore combine weight and window changes.” This establishes an existing adaptive route, not a failure of adaptive fusion.

R1, local synthetic study: RWF and the local FWF reproduction use the same two input estimates and the same three-sample window. Residuals use only observations available before the current output; weights are normalized inverse smoothed residual magnitudes. Epsilon is 0.01 in the recorded observation units. No future sample or evaluation label enters the weights. Existing Eq4 defines fusion; Algorithm2 below gives the actual steps. AWF is discussed from T2, not evaluated locally.

R2, local synthetic results: the same three fixed test sequences are used for both methods. Each table entry is mean absolute error over one full sequence; latency is mean wall-clock milliseconds per output on the same machine. Steady: RWF 0.80, FWF 1.00; gradual drift: RWF 1.20, FWF 1.50; abrupt change: RWF 2.20, FWF 2.00. RWF latency 1.50 ms and FWF 1.00 ms in all three. No repeated-run uncertainty or significance test exists. Fig3's upper panel plots these paired errors (lower is better), lower panel plots these latencies; colors encode method, horizontal positions encode condition. Both panels use the same condition order. The existing English-labeled asset identity is `error-cost-panels`; it must not be replaced with invented observations.

R3, local diagnostic: in the abrupt-change sequence, RWF assigns over 0.70 weight to the formerly better input for the first two outputs after the change. That interval has larger error than FWF. This temporal association is compatible with slow weight adjustment, but there is no component-isolation experiment establishing causation. Supplement Table S1 records 2 outputs and the >0.70 threshold, not a new accuracy benchmark.

Already studied writing exemplar E1 (self-authored synthetic editorial extract): a paired accuracy/cost display is explained through one comparison question before a separate mechanism diagnosis; scope conditions stay beside the inference they affect. Its style role is not scientific evidence. It is applicable to this fictional article type; no additional exemplar search is requested.

## Latest main text

### 引言与相关工作

多源估计可以减少对单一输入的依赖，但组合规则也决定输入质量变化时怎样分配影响。在观测窗口由采集条件预先固定的任务中，延长或缩短窗口并非当前研究可用的调整手段。因此，有意义的问题是：保持可见样本不变时，依据已观测误差调整融合权重能得到什么收益，又会付出什么代价？这里的固定窗口是本文条件，不是所有融合任务的限制。

FWF 在共同窗口内取两个估计的算术平均，不学习可靠性权重；其原研究考察平稳序列 [T1]。AWF 已把逆残差加权与窗口选择结合起来 [T2]，表明自适应融合并非尚未研究的方向。然而，其联合更新不能单独回答固定窗口下改变权重会怎样影响误差与处理代价。本文沿用固定窗口，在 RWF 中仅改变融合权重，并与相同输入上的 FWF 比较。这一对照用于分析当前条件下的表现，不把未测试的 AWF 宣称为劣势方法。

### 方法

RWF 对两路估计使用共同的三样本窗口。设第 j 路当前估计为 z_j，依据当前输出前可获得观测计算平滑残差幅值 e_j。令 a_j=1/(e_j+epsilon)，并将其归一化为 w_j=a_j/(a_1+a_2)。这一关系使较小的近期残差对应较大的融合权重，同时保持 w_1+w_2=1。融合输出由式（4）定义：y_hat=w_1 z_1+w_2 z_2。该式和估计来源不因英文适配而改变。

算法2（资产身份 residual-fusion-steps）：读取同窗口的两路估计；用输出前的可用观测更新平滑残差；计算并归一化逆残差权重；输出式（4）的融合值。FWF 保留相同输入与窗口，只把权重固定为 1/2。平滑参数、缺测处理及时间测量边界见补充材料 S1，不能由方法名称推断其实现。

### 结果与分析

表2汇总了三个工况的误差与延迟。FWR 在平稳与缓慢漂移工况的平均绝对误差分别为0.80和1.20，低于FWF的1.00和1.50；跳变工况则为2.20，高于FWF的2.00。图3给出了结果。因而，相同窗口下的可靠性加权在前两个工况有较低平均误差，但没有在全部条件下改善。延迟从1.00 ms增至1.50 ms，是权重更新对应的实际处理代价。

跳变后的局部诊断见补充材料表S1。前两次输出仍对原先较好的输入赋予超过0.70的权重，同期误差较大。这与权重调整滞后相容，但仅凭这种对应关系无法把误差上升确定归因于该机制。该诊断与整体对照分别回答局部变化和最终表现，不能互相替代。

表2（资产身份 main-error-cost）：三个工况的平均绝对误差与每次输出延迟。

| 工况 | RWF MAE | FWF MAE | RWF 延迟/ms | FWF 延迟/ms |
| --- | --- | --- | --- | --- |
| 平稳 | 0.80 | 1.00 | 1.50 | 1.00 |
| 缓慢漂移 | 1.20 | 1.50 | 1.50 | 1.00 |
| 跳变 | 2.20 | 2.00 | 1.50 | 1.00 |

图3（资产身份 error-cost-panels）：上图为平均绝对误差，下图为每次输出延迟；横轴工况一致，颜色区分方法。

### 结论

在共同固定窗口下，RWF 的可靠性加权表现出依赖工况的误差—代价取舍：两类序列误差较低，跳变序列误差较高，且处理延迟增加。研究把权重调整放在不改变窗口的对照中分析，结果不支持对任意变化条件的普遍改善。

## Latest supplement

### S1 实现与评价边界

平滑残差使用指数更新 e_j(t)=0.8 e_j(t-1)+0.2 |r_j(t-1)|，只使用当前输出前可用的残差；初始 e_j 为首个可用残差幅值。epsilon=0.01，单位与残差相同。任一路缺测时，该输出位置在两种方法的评价中同时排除，不插值；三个序列分别排除0、2、3个位置。主文算法2与式（4）中的窗口均为3样本。计时包含残差更新、权重计算与融合，不含文件加载。这些参数和排除规则只在本节给出。

### S2 跳变附近的诊断

表S1对应主文图3的跳变条件和表2的整体误差，不是独立数据集或新实验。跳变后连续2次输出中，RWF对原先较好的输入的权重均超过0.70，同期误差大于FWF；没有逐次独立重复或受控的组件干预。

| 诊断对象 | 输出次数 | 权重条件 | 同期比较 |
| --- | --- | --- | --- |
| 跳变后最初输出 | 2 | 原优势输入 >0.70 | RWF误差高于FWF |

补充表S1（资产身份 transient-weights）：跳变附近的权重与误差对应关系。
