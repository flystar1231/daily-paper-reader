---
title: Improving Video Generation with Human Feedback
title_zh: 利用人类反馈改进视频生成
authors: "Jie Liu, Gongye Liu, Jiajun Liang, Ziyang Yuan, Xiaokun Liu, Mingwu Zheng, Xiele Wu, Qiulin Wang, Menghan Xia, Xintao Wang, Xiaohong Liu, Fei Yang, Pengfei Wan, Di ZHANG, Kun Gai, Yujiu Yang, Wanli Ouyang"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=nHkg4yc7SP"
tags: ["query:vgen-metrics"]
score: 9.0
evidence: 提出了VideoReward，一种多维度视频奖励模型，用于评估视频生成质量
tldr: 该论文针对视频生成中运动不流畅和文本-视频不对齐的问题，构建了大规模人类偏好数据集，并提出多维度视频奖励模型VideoReward。该模型从多个维度评估视频质量，涵盖运动、语义对齐等。基于该奖励模型，作者进一步引入三种强化学习对齐算法，显著提升了生成视频的平滑度和一致性。工作为视频生成模型的自动化评估与优化提供了重要参考。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1425, \"height\": 839, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 708, \"height\": 395, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 698, \"height\": 379, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1451, \"height\": 525, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 760, \"height\": 415, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 642, \"height\": 400, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1416, \"height\": 997, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1426, \"height\": 515, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1393, \"height\": 844, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1401, \"height\": 469, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1235, \"height\": 1145, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1390, \"height\": 1921, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nhkg4yc7sp/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1394, \"height\": 1897, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1450, \"height\": 535, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1442, \"height\": 319, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1445, \"height\": 257, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1188, \"height\": 280, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 745, \"height\": 205, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1441, \"height\": 245, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1073, \"height\": 353, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1442, \"height\": 1054, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1441, \"height\": 214, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1099, \"height\": 561, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nhkg4yc7sp/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 943, \"height\": 853, \"label\": \"Table\"}]"
motivation: 视频生成模型存在运动不流畅和提示不对齐问题，需要有效的自动评估指标。
method: 构建人类偏好数据集，训练多维度视频奖励模型VideoReward，并通过强化学习将其用于模型优化。
result: VideoReward在多个维度上准确评估视频质量，并有效指导模型生成更优视频。
conclusion: 人类反馈和奖励模型可以显著提升视频生成的质量和可控性。
---

## Abstract
Video generation has achieved significant advances through rectified flow techniques, but issues like unsmooth motion and misalignment between videos and prompts persist. In this work, we develop a systematic pipeline that harnesses human feedback to mitigate these problems and refine the video generation model. Specifically, we begin by constructing a large-scale human preference dataset focused on modern video generation models, incorporating pairwise annotations across multi-dimensions. We then introduce VideoReward, a multi-dimensional video reward model, and examine how annotations and various design choices impact its rewarding efficacy. From a unified reinforcement learning perspective aimed at maximizing reward with KL regularization, we introduce three alignment algorithms for flow-based models. These include two training-time strategies: direct preference optimization for flow (Flow-DPO) and reward weighted regression for flow (Flow-RWR), and an inference-time technique, Flow-NRG, which applies reward guidance directly to noisy videos. Experimental results indicate that VideoReward significantly outperforms existing reward models, and Flow-DPO demonstrates superior performance compared to both Flow-RWR and supervised fine-tuning methods. Additionally, Flow-NRG lets users assign custom weights to multiple objectives during inference, meeting personalized video quality needs.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）
- **问题**：当前基于 rectified flow 技术的视频生成模型在运动流畅性、图文一致性等方面仍有不足，与人类主观偏好存在偏差。
- **整体含义**：本文旨在通过系统性地引入**人类反馈**来改进视频生成模型，构建了大规模、多维度的偏好数据集，训练出更可靠的视频奖励模型（VideoReward），并在此基础上提出针对流匹配模型的强化学习对齐算法（Flow-DPO、Flow-RWR 和 Flow-NRG），从而显著提升生成视频的质量与用户满意度。

## 2. 方法论
### 核心思想
- **数据层面**：收集 16k 高质量 prompt，用 12 个代表性 T2V 模型（含现代模型）生成 108k 视频，形成 182k 个 prompt-视频对（triplet），每个 triplet 由专业标注员在**视觉质量（VQ）、运动质量（MQ）、文本对齐（TA）** 三个维度分别给出偏好标注（A 胜 / 平局 / B 胜），同时给出 1-5 分的点级评分。
- **奖励模型（VideoReward）**：以 Qwen2-VL-2B 为 backbone，采用 **Bradley-Terry with Ties（BTT）** 损失函数进行训练，并设计**分离 token 定位策略**——将 [VQ]、[MQ] token 置于视频编码后、提示词之前（仅关注视觉内容），[TA] token 置于完整提示后（同时关注视频和文本），从而避免上下文泄漏，获得更纯净的奖励信号。
- **对齐算法**：从统一的 KL 正则化奖励最大化目标出发，为 rectified flow 模型推导并实现了三种策略：
  - **Flow-DPO**（训练时）：基于 Diffusion-DPO 迁移，但发现 βt = β(1-t)² 会导致高噪声层过拟合，采用**常数 β** 后显著提升性能（如公式：直接优化 velocity 预测误差的偏好对比损失）。
  - **Flow-RWR**（训练时）：对获胜样本的 velocity 回归损失赋予奖励权重 exp(r(x₀, y))。
  - **Flow-NRG**（推理时）：通过奖励梯度引导噪声潜空间的 velocity 场偏移（类似 classifier guidance），训练轻量级时域依赖的奖励模型直接在潜空间计算梯度，避免完整 VAE 解码的昂贵计算，并允许用户自定义各维度权重。

## 3. 实验设计
### 数据集与 Benchmark
- **奖励模型评估**：
  - **VideoGen-RewardBench**：基于第三方 Prompt-Video 数据集 VideoGen-Eval，构建 26.5k 标注对，覆盖现代 T2V 模型。
  - **GenAI-Bench**：1.9k 标注对，来自前 Sora 时代模型（短、低分辨率），用于评估泛化能力。
- **视频生成对齐评估**：
  - **VBench**（包含 Total Quality 和 Semantic 子项）
  - **VideoGen-Eval**
  - **TA-Hard**：自定义的复杂语义对齐困难集。
  - 人类评估：每个样本由两名标注员评审，第三人裁决分歧。

### 对比方法
- **奖励模型基线**：VideoScore、LiFT、VisionReward
- **对齐方法基线**：Supervised Fine-Tuning (SFT)、Flow-RWR、Flow-DPO（βt 与常数 β 两种）、Flow-NRG

### 主要对比结果
- **表2**：VideoReward 在 VideoGen-RewardBench 上显著优于所有基线（整体含平局准确率 61.26%），在 GenAI-Bench 上表现相当，展示跨时代泛化能力。
- **表3 & 表4**：Flow-DPO（常数 β）在多维对齐和单维文本对齐上均领先，而 timestep-dependent β 变体在 TA 上出现 reward hacking。
- **表5**：Flow-NRG 通过调整 VQ:MQ:TA 权重实现可定制化生成。

### 消融实验
- **奖励模型设计**（表6）：回归 vs BT vs BTT + 分离 token；BTT 和分离 token 各贡献增益。
- **β 选择**（图6）：常数 β 在所有 β 值下均优于 timestep-dependent β，避免训练不均衡。

## 4. 资源与算力（文中明确说明）
- **奖励模型训练**：8 台 NVIDIA A800 (80G) GPU，全参数训练 vision encoder，LoRA 训练语言模型，batch size 32，训练 2 个 epoch。
- **视频对齐实验（Flow-DPO / Flow-RWR / SFT）**：16 台 NVIDIA A800 (80G) GPU，LoRA 微调，batch size 64，学习率 5e-6，1 个 epoch。
- **推理时引导（Flow-NRG）**：使用潜空间奖励模型，无需额外大规模资源。

## 5. 实验数量与充分性
- **实验数量**：涵盖 2 个奖励模型评估 benchmark、3 个视频生成评估场景 + 人类评估，消融实验包括奖励模型类型（3 种）、β 方案（多个值）、分离 token 等。
- **充分性与公平性**：采用一致的随机种子、公平的基准对比（包括 ties-included 和 ties-excluded 准确率）。人类评估由三审制保证可靠性。消融实验覆盖了关键设计决策，逻辑清晰。但未报告误差棒（如多次运行的标准差），受限资源。
- **总体评价**：实验设计较全面，支撑了主要结论，但缺少统计显著性检验。

## 6. 主要结论与发现
1. **奖励模型**：VideoReward 优于现有视频奖励模型，BTT 损失和分离 token 设计是关键改进。
2. **训练时对齐**：Flow-DPO 使用常数 β 显著优于 SFT 和 Flow-RWR，能同时提升 VQ、MQ 和 TA；而 timestep-dependent β 导致 reward hacking（TA 下降但 VQ/MQ 虚高）。
3. **推理时对齐**：Flow-NRG 允许用户自由调整多维度权重，无需重新训练，实用性强。
4. **数据重要性**：基于现代高质量 T2V 模型构建的偏好数据集是实现有效对齐的基础。

## 7. 优点
- **大规模、多维度、高质量偏好数据集**：覆盖 12 种模型和 3 个维度，弥补了旧数据集（低分辨率、短时长）的缺陷。
- **系统性奖励模型设计研究**：首次深入对比了回归、BT、BTT 以及 token 定位策略，为后续工作提供指导。
- **流匹配对齐方法的统一框架**：从 RL 视角统一导出三种算法，并发现常数 β 的关键作用，纠正了直接迁移 Diffusion-DPO 的错误。
- **推理时可定制对齐**：Flow-NRG 实现轻量级、用户可调的推理时质量控制。
- **开源基准**：VideoGen-RewardBench 为现代奖励模型提供标准化评估。

## 8. 不足与局限
- **训练稳定性**：Flow-DPO 过度训练仍会导致模型质量整体下降，需依赖 LoRA 缓解，未提出根本性解决方案。
- **奖励模型鲁棒性**：VideoReward 仍可能遭受 reward hacking（人类评估分数下降但 RM 得分高），需要更鲁棒的训练或不确定性建模。
- **实验覆盖**：
  - 仅在文本到视频任务上验证，未扩展到图像到视频等条件生成。
  - 未与其他 RL 算法（如 PPO）对比。
  - 未提供多次运行的统计误差棒，局限性明确但未量化。
- **应用限制**：依赖大量人工标注，数据集和模型不公开（仅提供部分代码），复现受限；计算资源需求较高。

（完）
