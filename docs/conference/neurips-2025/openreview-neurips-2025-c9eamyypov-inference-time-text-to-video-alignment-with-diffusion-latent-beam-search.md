---
title: Inference-Time Text-to-Video Alignment with Diffusion Latent Beam Search
title_zh: 基于扩散潜在束搜索的推理时文本到视频对齐
authors: "Yuta Oshima, Masahiro Suzuki, Yutaka Matsuo, Hiroki Furuta"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=c9EAmyYPOv"
tags: ["query:vgen-metrics"]
score: 8.0
evidence: 讨论了视频生成中应优化哪些指标以及如何优化
tldr: 本文指出文本到视频扩散模型生成视频常存在运动不自然等问题，强调需要明确视频生成中应使用何种评价指标及如何优化。为此提出扩散潜在束搜索算法，结合前向估计器在推理时选择更优的潜在变量以最大化给定奖励指标，从而提升视频感知质量。该方法直接回应对齐问题，为视频生成评估提供了可操作的优化框架。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1422, \"height\": 509, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1446, \"height\": 746, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1436, \"height\": 231, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 713, \"height\": 196, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1443, \"height\": 225, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1402, \"height\": 290, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1445, \"height\": 263, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1440, \"height\": 267, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 711, \"height\": 240, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1445, \"height\": 420, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1440, \"height\": 378, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1450, \"height\": 377, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1434, \"height\": 756, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1433, \"height\": 759, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1430, \"height\": 383, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 856, \"height\": 436, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1454, \"height\": 622, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1454, \"height\": 752, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1453, \"height\": 343, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1447, \"height\": 519, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1446, \"height\": 522, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1453, \"height\": 515, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1429, \"height\": 472, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1429, \"height\": 474, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1429, \"height\": 474, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 749, \"height\": 485, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 864, \"height\": 562, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1450, \"height\": 288, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1449, \"height\": 287, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1452, \"height\": 290, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 718, \"height\": 270, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1449, \"height\": 288, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 716, \"height\": 269, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1437, \"height\": 957, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 1430, \"height\": 393, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 1160, \"height\": 424, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-c9eamyypov/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 1148, \"height\": 517, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 704, \"height\": 223, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1396, \"height\": 187, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1425, \"height\": 321, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1023, \"height\": 341, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 991, \"height\": 184, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 966, \"height\": 141, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 971, \"height\": 438, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-c9eamyypov/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 946, \"height\": 437, \"label\": \"Table\"}]"
motivation: 生成的视频存在不自然运动、变形等问题，需要有效的指标和优化方法来对齐用户期望。
method: 提出扩散潜在束搜索，利用前向估计器评估潜在变量的长期奖励，选择最优潜在编码。
result: 在多个指标上显著提升了生成视频的感知质量，验证了方法有效性。
conclusion: 该工作为视频生成模型的对齐和评估提供了实用的推理时优化策略。
---

## Abstract
The remarkable progress in text-to-video diffusion models enables the generation of photorealistic videos, although the content of these generated videos often includes unnatural movement or deformation, reverse playback, and motionless scenes. Recently, an alignment problem has attracted huge attention, where we steer the output of diffusion models based on some measure of the content's goodness. Because there is a large room for improvement of perceptual quality along the frame direction, we should address which metrics we should optimize and how we can optimize them in the video generation. In this paper, we propose diffusion latent beam search with lookahead estimator, which can select a better diffusion latent to maximize a given alignment reward at inference time. We then point out that improving perceptual video quality with respect to alignment to prompts requires reward calibration by weighting existing metrics. This is because when humans or vision language models evaluate outputs, many previous metrics to quantify the naturalness of video do not always correlate with the evaluation. We demonstrate that our method improves the perceptual quality evaluated on the calibrated reward, VLMs, and human assessment, without model parameter update, and outputs the best generation compared to greedy search and best-of-N sampling under much more efficient computational cost. The experiments highlight that our method is beneficial to many capable generative models, and provide a practical guideline: we should prioritize the inference-time compute allocation into enabling the lookahead estimator and increasing the search budget, rather than expanding the denoising steps.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

文本到视频扩散模型（如Latte、CogVideoX、Wan 2.1）已能生成逼真的视频，但生成内容常出现不自然的运动、变形、反向播放或无动作场景。现有对齐方法（如贪心搜索、最佳N采样）因奖励估计不准确（尤其在早期去噪步）而陷入次优。因此，需要解决两个问题：
- **优化哪些指标**：单一指标（如主体一致性或运动平滑度）与人类/VLM偏好相关性低，需校准多指标奖励。
- **如何优化**：在推理时高效搜索更好的扩散潜变量路径，避免近似误差累积。

## 2. 方法论：核心思想、关键技术细节

### 2.1 对齐问题的最优控制视角
将奖励最大化问题转化为随机最优控制，最优漂移项为：
\[
u^*(\nu_t, t) = g(t)^2 \nabla_\nu \log \mathbb{E}_{p_{\text{pre}}}\left[\exp\left(\frac{r'(\nu_T)}{\lambda}\right) \mid \nu_t = \nu\right]
\]
为降低计算复杂度，采用三步近似：Jensen不等式 → Tweedie公式（后验均值近似） → 将奖励梯度转化为argmax操作。

### 2.2 扩散潜在波束搜索（DLBS）
- 初始化B个潜变量束。
- 在每个去噪步（从t到t-1）：
  - 对每个束，采样K个候选潜变量（加噪声）。
  - 用Tweedie公式估计当前步的后验均值 \(\hat{z}_{0|t-1}\)。
  - 评估奖励，选择Top-B高奖励束进入下一步。
- 重复至t=0，从最终束中选择奖励最高的输出。

**作用**：通过宽束保持更多候选，减少单步argmax误差的传播。

### 2.3 前瞻估计器（Lookahead Estimator, LA）
- 从当前潜变量 \(z_{t-1}\) 出发，用T′-步确定性DDIM（T′ << T）推断到t=0，得到更干净的估计 \(\tilde{z}_{0|\tilde{t}(0)}\)。
- 用该估计计算奖励，降低后验均值的噪声。
- 理论上T′增大可单调降低奖励估计误差上界；实践中T′=6已足够。

### 2.4 奖励校准（Reward Calibration）
- 六项基础指标：主体一致性、运动平滑度、动态程度、美学质量、成像质量、文本-视频一致性。
- 加权线性组合：\(r^*(x_0, c) = \sum_i w_i r_i(x_0,c) / \sum_i w_i\)，权重通过暴力搜索（0~1，步长0.25）最大化与VLM（Gemini/GPT-4o）的皮尔逊相关性。
- 不同动态等级的提示需不同权重：高动态场景动态程度权重更大，静态场景主体一致性权重更大。

## 3. 实验设计

### 3.1 数据集与场景
- **DEVIL**：按动态度分为high、medium、static、very-high，各选22~30条提示。
- **MSRVTT-test**：30条随机提示。
- **Movie Gen Video Bench**：1003条复杂提示用于鲁棒性测试。

### 3.2 对比方法
- **Best-of-N (BoN)**：独立生成N个样本，选奖励最高者。
- **Greedy Search (GS)**：每步从K个候选中选最佳（束数B=1）。
- **DLBS**：给定预算KB，探索不同(K,B)组合。
- **DLBS-LA**：DLBS结合前瞻估计器（T′=6）。

### 3.3 评估指标
- **校准奖励**：Gemini或GPT-4o校准后的加权组合。
- **VLM评分**：Gemini-1.5-pro、GPT-4o给出1-10分。
- **VideoScore**：基于人类偏好的五维度评分（视觉质量、时间一致性、动态度、文本对齐、事实一致性）。
- **人类评估**：三名人打分员进行两两对比。
- **多样性**：ViCLIP embedding的均值成对距离。

### 3.4 模型与配置
- **Latte**（1.1B）：DDIM，T=50，η=1.0。
- **CogVideoX-5B/2B**：DDIM，帧长17。
- **Wan 2.1-14B/1.3B**：SDE-DPMSolver++，分辨率832×480，帧长33。
- 各实验超参见Appendix B。

## 4. 资源与算力

- **Latte**：单张NVIDIA A100 (40GB)，FP16，batch size=1。
- **CogVideoX**：单张NVIDIA A100 (40GB)，BF16。
- **Wan 2.1**：四张NVIDIA H100 (80GB)，FP16。
- 所有方法为推理时搜索，无需训练。计算量以NFE（前向函数评估次数）衡量，例如DLBS-LA (KB=8, T′=6)约2500 NFE，BoN (KB=64)约3200 NFE。

## 5. 实验数量与充分性

论文进行了大量实验，包括：
- 四个提示集（DEVIL-high/medium/static、MSRVTT-test）上对比BoN、GS、DLBS、DLBS-LA，预算从1到64。
- 两个VLM（Gemini、GPT-4o）的奖励校准与评估。
- 在三个SoTA模型（Latte、CogVideoX、Wan 2.1）上验证可扩展性。
- 消融研究：LA步数（T′）、搜索步范围、η值、扩散步数T、束与候选的比例。
- 与微调方法（VideoDPO）的兼容性。
- 人类评估：三轮两两对比。
- 多样性分析。
- 在1003条MovieGen提示上的大规模测试。

**评价**：实验设计较充分，覆盖了多种场景、模型和指标，对比方法合理，消融全面。但VLM作为代理存在固有偏差，且仅使用英语提示，缺乏多语言泛化测试。

## 6. 主要结论与发现

1. **DLBS优于BoN和GS**：在相同搜索预算下，DLBS获得更高的校准奖励，且随预算增加持续改进。
2. **LA估计器显著提升效率**：仅需少量额外DDIM步（T′=6），DLBS-LA即可达到甚至超过DLBS（KB=32）的性能。
3. **奖励校准至关重要**：单一指标与VLM相关性低（如主体一致性R=0.05），校准后相关系数提升至0.46~0.51。
4. **推理时对齐与微调互补**：DLBS+DPO进一步改善性能，优于单独DPO。
5. **分配指南**：优先将推理计算投入LA估计器和搜索预算，而非增加扩散步数。
6. **保持多样性**：DLBS在提升奖励的同时维持了比BoN更高的样本多样性。

## 7. 优点

- **无需模型参数更新**：纯推理时方法，可直接应用于预训练模型。
- **计算高效**：相比BoN，同样执行时间下获得更高奖励（图1右、图6左）。
- **鲁棒性强**：波束搜索减少近似误差累积，LA估计器降低奖励估计噪声。
- **通用性**：在多种SoTA模型（Latte、CogVideoX、Wan 2.1）上均有效。
- **实用性指导**：提供了具体的计算分配策略。
- **奖励校准方法实用**：通过暴力搜索快速获得与VLM高相关的代理奖励，避免频繁查询VLM。

## 8. 不足与局限

- **依赖VLM作为代理**：VLM可能不完全等同于人类偏好（如对文本渲染、数量理解有偏差），实验中的“oracle”假设存在局限。
- **奖励校准过拟合风险**：权重针对特定VLM（Gemini/GPT-4o）和特定提示集优化，跨域泛化能力有限（虽有一定转移性，但性能下降）。
- **推理计算开销**：虽然比BoN高效，但DLBS-LA仍需约2500 NFE，实时应用仍困难。
- **未考虑物理一致性**：评估指标不包括物理规律（如刚性、流体模拟），可能仍会生成不符合物理的视频。
- **仅限英语提示**：未测试多语言场景，VLM评估可能对非英语提示不公。
- **人类评估规模小**：仅三名打分员，未报告信效度指标。

（完）
