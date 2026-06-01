---
title: "RLVR-World: Training World Models with Reinforcement Learning"
title_zh: RLVR-World：用强化学习训练世界模型
authors: "Jialong Wu, Shaofeng Yin, Ningya Feng, Mingsheng Long"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=jpiSagi8aV"
tags: ["query:vgen-metrics"]
score: 4.0
evidence: 使用可验证奖励直接优化世界模型的预测准确率和感知质量等指标
tldr: 现有世界模型训练目标（如最大似然估计）往往与任务目标（如预测准确率、感知质量）不一致。本文提出RLVR-World框架，利用带可验证奖励的强化学习（RLVR）直接优化这些指标。在语言和视频世界模型上均取得显著性能提升，证明了该方法在优化评估指标上的有效性。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1418, \"height\": 542, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1417, \"height\": 712, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 462, \"height\": 373, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 488, \"height\": 362, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1414, \"height\": 381, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 812, \"height\": 412, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1445, \"height\": 1110, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 521, \"height\": 413, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1432, \"height\": 352, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1448, \"height\": 1137, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jpisagi8av/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1446, \"height\": 1118, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 939, \"height\": 462, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 939, \"height\": 302, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1437, \"height\": 456, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1439, \"height\": 645, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1169, \"height\": 739, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1320, \"height\": 243, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1278, \"height\": 1115, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1272, \"height\": 1155, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1231, \"height\": 338, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1175, \"height\": 281, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1326, \"height\": 515, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1462, \"height\": 223, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jpisagi8av/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1340, \"height\": 520, \"label\": \"Table\"}]"
motivation: 标准世界模型训练目标（MLE）与任务specific指标（如预测准确率、感知质量）不一致。
method: 提出RLVR-World框架，将世界建模建模为自回归token预测，并将解码预测的指标作为可验证奖励进行强化学习优化。
result: 在语言和视频世界模型上，RLVR-World均显著提升了预测准确率和感知质量。
conclusion: 通过直接优化任务指标，RLVR-World为世界模型训练提供了更对齐的范式。
---

## Abstract
World models predict state transitions in response to actions and are increasingly developed across diverse modalities. However, standard training objectives such as maximum likelihood estimation (MLE) often misalign with task-specific goals of world models, i.e., transition prediction metrics like accuracy or perceptual quality. In this paper, we present RLVR-World, a unified framework that leverages reinforcement learning with verifiable rewards (RLVR) to directly optimize world models for such metrics. Despite formulating world modeling as autoregressive prediction of tokenized sequences, RLVR-World evaluates metrics of decoded predictions as verifiable rewards. We demonstrate substantial performance gains on both language- and video-based world models across domains, including text games, web navigation, and robot manipulation. Our work indicates that, beyond recent advances in reasoning language models, RLVR offers a promising post-training paradigm for enhancing the utility of generative models more broadly. Code, datasets, models, and video samples are available at the project website: https://thuml.github.io/RLVR-World.

---

## 论文详细总结（自动生成）

# 论文《RLVR-World: Training World Models with Reinforcement Learning》中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **核心问题**：现有世界模型（World Models）的训练目标通常是最大似然估计（MLE），如语言模型的 next-token prediction 或视频模型的均方误差。但这些目标与世界模型实际任务指标（如预测准确率、感知质量）不一致，导致模型在任务度量上表现不佳，甚至出现重复生成、模糊预测等问题。
- **背景**：世界模型在游戏、机器人、自动驾驶等领域日益重要。传统训练方法（如 teacher forcing）无法直接优化任务相关指标，且无法处理多步累积误差。近年来，带可验证奖励的强化学习（RLVR）在语言模型的数学推理和代码生成上取得突破，作者将其引入世界模型训练，提出 RLVR-World 框架。

## 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：将不同模态的世界模型统一为自回归生成框架，利用任务特定的可验证指标作为 RL 奖励，通过 RLVR 直接优化这些指标。
- **关键技术细节**：
  - **统一序列建模**：将状态和动作编码为 token 序列（语言使用 BPE，视频使用离散视觉 tokenizer，低维连续量使用均匀分箱量化），按模板构建“问题”序列 q(s,a) 和“回答”序列 o(s')，构成自回归预测任务。
  - **可验证奖励**：对生成的多组样本进行解码，使用任务指标（如准确率、F1 分数、MSE、LPIPS、SSIM 等）计算奖励。对于越大越好的指标（如 SSIM）取正值，对于越小越好的指标（如 MSE）取负值。
  - **RL 算法**：采用 GRPO（Group Relative Policy Optimization），无需值函数，通过组内归一化计算优势函数，并使用 KL 惩罚项防止偏离参考模型。
  - **两阶段训练**：先在目标数据集上通过 MLE 预训练（语言模型使用 SFT，视频模型从头预训练），再用 RLVR 进行后训练（post-training）。

## 3. 实验设计：数据集、场景、基准、对比方法

- **语言世界模型**：
  - **文本游戏状态预测**：使用 ByteSized32-State-Prediction 数据集（76,369 条转换，2,954 条测试）。训练 DeepSeek-R1-Distill-Qwen-1.5B/7B，先 SFT，再 RLVR 优化（二元奖励或任务特定奖励）。对比基础模型、SFT 模型、GPT-4 结果。
  - **网页状态预测**：使用 WebArena 数据集（约 7K 样本子集）。同样基于 DeepSeek-R1-Distill-Qwen-1.5B，先 SFT（使用 WMA 的 CoT 数据），再 RLVR 优化 F1 分数。对比基础模型和 SFT 模型。
  - **下游应用：模型预测控制（MPC）**：在 WebArena 上构建 web agent，用 RLVR 训练的世界模型预测动作结果，再通过价值模型评分选最优动作。对比 SFT 世界模型。

- **视频世界模型**：
  - **机器人操作轨迹预测**：主要使用 RT-1 数据集（87,212 条轨迹）。预训练 iVideoGPT 变体（自回归视频世界模型），单步预测和多步预测设置。对比基础模型（MLE 预训练）、基础模型+重复拒绝、RLVR-World 变体（带重复惩罚奖励）。还对比了 DINO-WM、AVDC 等最先进模型。
  - **额外数据集**：PushT、Rope、Granular（来自 DINO-WM）。对比多种 baseline（R3M、ResNet、DINO CLS、DINO-WM、AVDC）。
  - **下游应用：Real2Sim 策略评估**：在 SIMPLER 模拟器上评估 RT-1 和 RT-1-X 策略的打开/关闭抽屉任务，对比 handcrafted SIMPLER 模拟器和基础世界模型。

- **消融与模型分析**：测试时间缩放（不同采样数）、组大小对 RL 训练的影响、不同奖励函数（MAE/MSE/PSNR/SSIM/LPIPS）的优化效果、重复率降低、训练曲线对比（MLE 预训练 vs RLVR 后训练）。

## 4. 资源与算力

- **文本游戏**：SFT 使用 4×80G A100 GPU，训练 6.5 小时；RLVR 使用 8×80G A100 GPU，训练 22.5 小时。框架：verl。
- **网页状态预测**：SFT 使用 8×40G A100 GPU，17 小时；RLVR 使用 8×80G H100 GPU，25 小时。框架：verl。
- **机器人操作轨迹预测**：所有实验在 40G A100 GPU 集群进行。单步预测：tokenizer 预训练约 360 GPU 小时，Transformer 预训练 530 GPU 小时，RLVR（200 步）需 4×40G A100 GPU 共 3.5 小时。多步预测：tokenizer 预训练 480 GPU 小时，Transformer 预训练 500 GPU 小时，RLVR（200 步）需 4×40G A100 GPU 共 10 小时。框架：accelerate 和 verl。
- **其他数据集**：PushT、Rope、Granular 算力未单独统计，但使用类似配置。

## 5. 实验数量与充分性

- 实验覆盖语言世界模型（两个数据集+MPC 应用）、视频世界模型（四个数据集+策略评估应用），共计 **5 个**主要数据集，加上多个消融和分析实验（10+ 组）。
- 实验充分性：控制变量（对比 MLE 预训练、SFT、RLVR）、对比多种 SOTA 方法、引入多组消融（测试时缩放、组大小、不同奖励函数、重复率）、下游应用验证。方法公平性良好，对比基准均采用公开或重现的模型。
- 部分实验（如 Rope 数据集）上 RLVR 提升较小，作者分析了原因（过拟合），并进行了跨任务联合训练验证。实验总体客观。

## 6. 论文的主要结论与发现

- RLVR 可显著提升语言世界模型的预测准确率（文本游戏 +30.7%，网页 F1 +15.1%），并增强 MPC 性能。
- RLVR 可显著提升视频世界模型的预测质量（单步 LPIPS +6.0%，多步 LPIPS +9.2%，重复率从 48.6% 降至 9.9%），且仅需少量训练步数（数百步对比 MLE 预训练的数十万步）。
- RLVR 能有效缓解重复生成问题（视频模型），且通过加入重复惩罚奖励可完全消除。
- 指标导向优化成立：用不同指标训练后，模型在对应指标上表现最优。
- 测试时缩放显示 RLVR 提升单样本性能，但大量采样时基础模型可追平。
- 下游应用（MPC 和策略评估）中，RLVR 世界模型带来更优性能。

## 7. 优点

- **新颖范式**：首次将 RLVR 系统性地应用于世界模型训练，覆盖语言和视频模态，提出统一框架。
- **实用性强**：训练高效（仅需数百步），即能显著改善任务指标，同时减少伪影（重复）。
- **实验详实**：涵盖多领域、多数据集、多评价指标，包含消融、分析、下游应用，验证充分。
- **开源友好**：公开代码、数据、模型和视频样例，可复现性强。
- **跨模态统一**：将世界模型统一为自回归序列建模，使 RLVR 可直接适用。

## 8. 不足与局限

- **性能瓶颈**：RLVR 训练收敛较快（数百步），无法持续提升，需进一步分析模型、数据和算法瓶颈。
- **OOD 泛化未深入**：仅初步讨论了跨任务泛化（Rope/Granular），缺乏对分布外动作的鲁棒性研究。
- **视频世界模型非通用预训练**：目前是在同一数据集上先 MLE 再 RLVR，缺少通用预训练→SFT→RLVR 的完整链条；若社区开发出通用视频世界模型，潜力更大。
- **奖励设计依赖人工**：虽然可验证，但经典视觉指标（如 LPIPS）仍不能完全捕捉用户意图；需更复杂的物理规则等奖励设计。
- **算法局限**：GRPO 需要较大组大小（group size）以提升探索，测试时 RLVR 模型在大量采样时优势被基础模型反超，未来需要更优的 RL 算法。
- **部分实验未覆盖**：如 MPC 只在 PushT 上测试，未在 Rope/Granular 上执行；策略评估仅用人类标注，未开发自动评估方法。
- **算力消耗不低**：虽然 RLVR 步数少，但 tokenizer 和 MLE 预训练仍需大量 GPU 小时。

（完）
