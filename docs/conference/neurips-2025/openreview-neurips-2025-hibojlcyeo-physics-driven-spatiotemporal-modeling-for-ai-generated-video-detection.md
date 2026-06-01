---
title: Physics-Driven Spatiotemporal Modeling for AI-Generated Video Detection
title_zh: 物理驱动时空建模用于AI生成视频检测
authors: "Shuhai Zhang, ZiHao Lian, Jiahao Yang, Daiyuan Li, Guoxuan Pang, Feng Liu, Bo Han, Shutao Li, Mingkui Tan"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=HiBoJLCyEo"
tags: ["query:vgen-metrics"]
score: 4.0
evidence: AI生成视频检测的时空度量
tldr: 论文针对AI生成视频检测问题，提出了基于概率流守恒的归一化时空梯度统计量（NSG），用于量化视频中违反物理规律的异常。虽然检测任务与生成评估不同，但NSG作为一种视频质量度量，可迁移至生成视频的质量评估。该工作为视频质量评估指标提供了新思路。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1427, \"height\": 446, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1452, \"height\": 492, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 612, \"height\": 380, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 662, \"height\": 473, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 852, \"height\": 550, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 835, \"height\": 517, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1248, \"height\": 1065, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1245, \"height\": 932, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1359, \"height\": 1013, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1357, \"height\": 1007, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1358, \"height\": 1013, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1358, \"height\": 1014, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1360, \"height\": 1014, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1358, \"height\": 1008, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1358, \"height\": 1015, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1357, \"height\": 1011, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1360, \"height\": 1015, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1358, \"height\": 1013, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-hibojlcyeo/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1360, \"height\": 1299, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1448, \"height\": 759, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1449, \"height\": 758, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1450, \"height\": 759, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 654, \"height\": 215, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1090, \"height\": 499, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1451, \"height\": 465, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 761, \"height\": 378, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1335, \"height\": 349, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1449, \"height\": 890, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-hibojlcyeo/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1448, \"height\": 209, \"label\": \"Table\"}]"
motivation: AI生成视频日益逼真，需要可靠检测方法，其中涉及对视频质量的评估。
method: 提出归一化时空梯度（NSG）统计量，基于物理守恒原理检测异常。
result: 在多个AI视频检测基准上达到优异性能。
conclusion: NSG可作为视频自然度评估的有效指标，与生成质量评估间接相关。
---

## Abstract
AI-generated videos have achieved near-perfect visual realism (e.g., Sora), urgently necessitating reliable detection mechanisms. However, detecting such videos faces significant challenges in modeling high-dimensional spatiotemporal dynamics and identifying subtle anomalies that violate physical laws. In this paper, we propose a physics-driven AI-generated video detection paradigm based on probability flow conservation principles. Specifically, we propose a statistic called Normalized Spatiotemporal Gradient (NSG), which quantifies the ratio of spatial probability gradients to temporal density changes, explicitly capturing deviations from natural video dynamics. Leveraging pre-trained diffusion models, we develop an NSG estimator through spatial gradients approximation and motion-aware temporal modeling without complex motion decomposition while preserving physical constraints. Building on this, we propose an NSG-based video detection method (NSG-VD) that computes the Maximum Mean Discrepancy (MMD) between NSG features of the test and real videos as a detection metric. Last, we derive an upper bound of NSG feature distances between real and generated videos, proving that generated videos exhibit amplified discrepancies due to distributional shifts. Extensive experiments confirm that NSG-VD outperforms state-of-the-art baselines by 16.00\% in Recall and 10.75\% in F1-Score,  validating the superior performance of NSG-VD. The source code is available at \url{https://github.com/ZSHsh98/NSG-VD}.

---

## 论文详细总结（自动生成）

# AI生成视频检测中的物理驱动时空建模（NSG-VD）——论文详细总结

## 1. 核心问题与整体含义
- **研究动机**：以Sora为代表的AI生成视频已达到近乎完美的视觉真实感，但常违反物理规律（如运动不连贯、纹理不连续）。现有的检测方法多依赖局部伪影（如光流、外观一致性）或大规模监督学习，难以捕捉这些细微的时空异常，尤其在面对新型生成模型时性能显著下降。
- **核心问题**：如何建模自然视频固有的时空动态，以暴露AI生成视频中违反物理规律的异常？
- **整体含义**：论文提出一种基于物理守恒原理（概率流守恒）的新检测范式，通过统计量归一化时空梯度（Normalized Spatiotemporal Gradient, NSG）来量化视频对物理规律的偏离，从而在不依赖特定伪影的前提下实现通用、鲁棒的检测。

## 2. 方法论
- **核心思想**：
  - 将视频的动态演化类比为流体力学中的概率流，连续性方程要求概率质量守恒：∂p/∂t + ∇·(pv) = 0。
  - 通过假设流场近似不可压缩（∇·v可忽略），得到简化关系：v·∇log p ≈ −∂log p/∂t。
  - 由此定义NSG：g(x,t) = ∇log p(x,t) / (−∂log p(x,t) + λ)，其中λ防止除零。NSG作为速度场的对偶场，同时捕捉空间概率梯度与时间密度变化。

- **关键技术细节**：
  - **空间梯度估计**：利用预训练扩散模型（Guided Diffusion）的得分函数sθ近似∇log p(x,t)，通过单次前向传播得到。
  - **时间导数近似**：基于亮度恒常假设（p(x+Δx, t+Δt)≈p(x,t)），导出∂log p(x,t)/∂t ≈ −∇log p(x,t)·(Δx/Δt)，避免显式光流计算。
  - **NSG特征提取**：对视频每帧计算g(x,t)，聚合得到G(x)={g(x,t)}ₜ。
  - **检测度量**：采用最大均值差异（MMD）衡量测试视频NSG特征与真实视频参考集NSG特征之间的分布差异，超过阈值τ则判定为AI生成。
  - **内核优化**：使用可学习的深度高斯核，通过多总体感知优化（MMD-MP框架）最大化检测能力。
  - **理论保证**：在高斯分布假设下，推导出真实与生成视频NSG特征距离的上界，证明分布偏移越大，距离越大，从而保证MMD检测的有效性。

- **公式流程**（文字说明）：
  1. 输入视频帧xt → 通过扩散模型得分网络sθ → 得到空间梯度≈sθ(xt)。
  2. 从相邻帧计算Δx/Δt，结合sθ(xt)近似时间导数。
  3. 构建NSG特征g(x,t) = sθ(xt) / (−∂log p/∂t + λ)。
  4. 对参考集和测试集计算各帧NSG，组成特征序列。
  5. 计算MMD²(参考集, 测试视频) = kernel均值差异。
  6. 若MMD>τ，判为假；否则判为真。

## 3. 实验设计
- **数据集**：使用GenVideo benchmark。真实视频来自Kinetics-400和MSR-VTT；生成视频来自多种模型：SEINE、Pika、HotShot、Show1、Gen2、Crafter、Lavie、Sora、MoonValley、MorphStudio、WildScrape等，涵盖开/闭源生成模型。
- **使用场景**：
  - 标准评估：训练用10k真实+10k生成（分别以Pika或SEINE作为生成源），测试10种生成模型。
  - 数据不平衡场景：训练仅用1k生成视频（SEINE）+10k真实视频。
  - 消融实验：评估空间梯度和时间导数的独立贡献。
  - 阈值灵敏性、参考集大小、参考集领域覆盖等分析。
- **基准方法**：对比DeMamba、NPR、TALL、STIL等最新AI视频检测方法。
- **评价指标**：Recall、Accuracy、F1-score、AUROC。

## 4. 资源与算力
- 论文在附录C.3明确指出：所有实验使用**1× NVIDIA RTX 3090 GPU**，Python 3.10.17，PyTorch 2.7.0。
- 训练细节：Adam优化器，batch size 24，学习率0.0001，权重衰减0.1。可训练参数仅0.25M（深度内核部分）。
- **未明确说明训练总时长**，但提供了推理时间：NSG-VD（256×256输入）每视频0.3605秒；并展示了通过降低分辨率可大幅加速（如64×64时0.0298秒/视频）。
- 总体而言，算力要求适中，但预处理依赖扩散模型前向传播。

## 5. 实验数量与充分性
- **实验组数**：约7大类实验：
  1. 标准评估（两种训练设置：Pika / SEINE）→ 20个模型×数据集组合（每个表含10种生成模型）。
  2. 数据不平衡实验（1k vs 10k）→ 10种生成模型。
  3. 消融实验（空间梯度 vs 时间导数 vs 组合）→ 平均指标。
  4. 阈值影响实验（τ ∈ [0.4,1.3]）→ 可视化曲线。
  5. 参考集大小影响（10~500）→ 可视化。
  6. 参考集领域覆盖实验（MSR-VTT与Kinetics-400比例）→ 额外表格。
  7. 效率与参数规模对比。
- **充分性评价**：
  - **充分性较高**：覆盖了主要生成模型类型（含闭源Sora、Pika，开源多种），包含标准和不平衡场景，做了必要的消融和超参数分析。
  - **公平性较好**：对比基线使用同一代码库复现，评价指标全面。但在同一基准（GenVideo）上评估，缺乏跨域泛化验证（如不同分辨率、不同场景的视频）。
  - **偏差风险**：仅使用一个主数据集（GenVideo），可能引入数据集偏差；理论分析基于高斯假设，实际数据分布可能偏离，但实验表明鲁棒。

## 6. 主要结论与发现
- NSG-VD在所有评价指标上超越现有方法，在标准评估中Recall提升16.00%，F1提升10.75%；在数据不平衡场景下Recall提升29.12%。
- 在挑战性模型（Sora、HotShot、WildScrape）上表现突出，例如Sora Recall达78.57%（Demamba仅48.21%）。
- 消融实验表明空间梯度与时间导数联合使用效果远优于单独使用，证实物理驱动建模的必要性。
- 理论分析证明真实与生成视频的NSG特征距离随分布偏移增大而增大，为检测提供可靠性保证。
- NSG-VD对阈值、参考集大小不敏感，具备实用稳定性。

## 7. 优点
- **物理原理驱动**：不依赖特定生成伪影，对新型未知生成模型具有泛化潜力。
- **可解释性强**：NSG直接对应概率流守恒关系，从物理角度解释自然与合成视频的差异。
- **轻量高效**：可训练参数仅0.25M，远低于全参数微调的基线（如DeMamba需119.89M）。
- **理论支撑**：给出NSG特征距离上界，从理论上证明检测可行性。
- **鲁棒性**：在数据不平衡、参考集有限等实际场景下仍保持高性能。

## 8. 不足与局限
- **对扩散模型质量的依赖**：NSG估计依赖于预训练扩散模型的得分网络，若该模型与目标域不匹配，估计精度可能下降。
- **计算开销**：虽然参数少，但推理时仍需运行扩散模型，导致比基于CNN的方法慢（0.36s/视频 vs 0.03s/视频），难以用于实时场景。
- **物理假设局限**：假设∇·v可忽略（不可压缩近似），对于剧烈或突变的运动可能不成立，论文未深入探讨极限情况。
- **实验范围有限**：仅在一个基准（GenVideo）上验证，未在其他真实/合成混合数据集或不同分辨率的视频上测试泛化能力。
- **缺乏公平性/偏见讨论**：未分析检测方法对不同人群、场景的公平性影响。
- **理论假设简化**：高斯分布假设有助于推导，但实际数据分布更复杂，理论界与实际表现之间的差距未量化。

（完）
