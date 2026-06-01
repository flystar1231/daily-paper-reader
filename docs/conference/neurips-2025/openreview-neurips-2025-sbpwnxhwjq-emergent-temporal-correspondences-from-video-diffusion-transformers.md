---
title: Emergent Temporal Correspondences from Video Diffusion Transformers
title_zh: 来自视频扩散变换器的涌现时间对应
authors: "Jisu Nam, Soowon Son, Dahyun Chung, Jiyoung Kim, Siyoon Jin, Junhwa Hur, Seungryong Kim"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=SBPWnXhwjq"
tags: ["query:vgen-metrics"]
score: 7.0
evidence: 提出了用于分析视频扩散模型中时间对应的新颖评估指标
tldr: 视频扩散变换器（DiT）虽然能生成时序连贯的视频，但其内部如何建立时间对应尚不明确。本文提出DiffTrack，首个定量分析框架，利用伪真实追踪标注数据集和新的评估指标，系统分析DiT中不同组件（表示、层、时间步）对时间对应的贡献。结果表明查询-键相似性在建立对应中起关键作用。该工作为评估和提升生成视频的时序质量提供了新的度量工具。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1442, \"height\": 423, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 583, \"height\": 597, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 726, \"height\": 127, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 725, \"height\": 126, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1315, \"height\": 742, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 664, \"height\": 371, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 806, \"height\": 362, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 595, \"height\": 364, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1445, \"height\": 907, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1442, \"height\": 409, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 736, \"height\": 542, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1453, \"height\": 824, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1458, \"height\": 828, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1454, \"height\": 828, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1165, \"height\": 1061, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1420, \"height\": 435, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1439, \"height\": 335, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 573, \"height\": 531, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 735, \"height\": 332, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 341, \"height\": 230, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 344, \"height\": 232, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 340, \"height\": 253, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 339, \"height\": 237, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1449, \"height\": 260, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 512, \"height\": 230, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 933, \"height\": 262, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 707, \"height\": 131, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 709, \"height\": 131, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 708, \"height\": 135, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 707, \"height\": 131, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 706, \"height\": 131, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 708, \"height\": 137, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 710, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 710, \"height\": 130, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 711, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 711, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 711, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-038.webp\", \"caption\": \"\", \"page\": 0, \"index\": 38, \"width\": 711, \"height\": 132, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-039.webp\", \"caption\": \"\", \"page\": 0, \"index\": 39, \"width\": 710, \"height\": 131, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-040.webp\", \"caption\": \"\", \"page\": 0, \"index\": 40, \"width\": 711, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-041.webp\", \"caption\": \"\", \"page\": 0, \"index\": 41, \"width\": 711, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-042.webp\", \"caption\": \"\", \"page\": 0, \"index\": 42, \"width\": 713, \"height\": 131, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-043.webp\", \"caption\": \"\", \"page\": 0, \"index\": 43, \"width\": 1005, \"height\": 365, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-044.webp\", \"caption\": \"\", \"page\": 0, \"index\": 44, \"width\": 1442, \"height\": 486, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-045.webp\", \"caption\": \"\", \"page\": 0, \"index\": 45, \"width\": 1444, \"height\": 555, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-046.webp\", \"caption\": \"\", \"page\": 0, \"index\": 46, \"width\": 1449, \"height\": 697, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-047.webp\", \"caption\": \"\", \"page\": 0, \"index\": 47, \"width\": 1449, \"height\": 696, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-048.webp\", \"caption\": \"\", \"page\": 0, \"index\": 48, \"width\": 1447, \"height\": 1899, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-049.webp\", \"caption\": \"\", \"page\": 0, \"index\": 49, \"width\": 1430, \"height\": 171, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-050.webp\", \"caption\": \"\", \"page\": 0, \"index\": 50, \"width\": 1437, \"height\": 180, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-051.webp\", \"caption\": \"\", \"page\": 0, \"index\": 51, \"width\": 1433, \"height\": 174, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-052.webp\", \"caption\": \"\", \"page\": 0, \"index\": 52, \"width\": 1440, \"height\": 175, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-sbpwnxhwjq/fig-053.webp\", \"caption\": \"\", \"page\": 0, \"index\": 53, \"width\": 1437, \"height\": 174, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1444, \"height\": 548, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 916, \"height\": 197, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 735, \"height\": 187, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 727, \"height\": 155, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 868, \"height\": 212, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 584, \"height\": 213, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 725, \"height\": 172, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 512, \"height\": 230, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 797, \"height\": 151, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 795, \"height\": 191, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-sbpwnxhwjq/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1153, \"height\": 390, \"label\": \"Table\"}]"
motivation: 视频扩散模型内部时间对应机制不明确，缺乏定量分析指标。
method: 构建伪真实追踪数据集，提出新的评估指标，分析DiT注意力机制中各组件对时间对应的贡献。
result: 发现查询-键相似性是建立时间对应的关键，不同层和表示有不同影响。
conclusion: DiffTrack提供了理解和评估视频生成模型时序质量的工具，有助于改进模型设计。
---

## Abstract
Recent advancements in video diffusion models based on Diffusion Transformers (DiTs) have achieved remarkable success in generating temporally coherent videos. Yet, a fundamental question persists: how do these models internally establish and represent temporal correspondences across frames?  We introduce DiffTrack, the first quantitative analysis framework designed to answer this question. DiffTrack constructs a dataset of prompt-generated video with pseudo ground-truth tracking annotations and proposes novel evaluation metrics to systematically analyze how each component within the full 3D attention mechanism of DiTs (e.g., representations, layers, and timesteps) contributes to establishing temporal correspondences. Our analysis reveals that query-key similarities in specific (but not all) layers play a critical role in temporal matching, and that this matching becomes increasingly prominent throughout denoising. We demonstrate practical applications of DiffTrack in zero-shot point tracking, where it achieves state-of-the-art performance compared to existing vision foundation and self-supervised video models. Further, we extend our findings to motion-enhanced video generation with a novel guidance method that improves temporal consistency of generated videos without additional training. We believe our work offers crucial insights into the inner workings of video DiTs and establishes a foundation for further research and applications leveraging their temporal understanding.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：尽管基于 Diffusion Transformers（DiTs）的视频扩散模型在生成时间连贯视频方面取得了显著成功，但一个根本问题尚未被解答：这些模型在内部是如何建立和表示帧间时间对应的？现有工作（如 DIFT）主要分析 U-Net 图像扩散模型的两帧对应，缺乏对视频 DiTs 中完整 3D 注意力机制的系统研究。
- **整体含义**：理解视频 DiTs 中时间对应的涌现机制，不仅能揭示模型内部工作原理，还能直接服务于下游任务（如零样本点跟踪）并改进视频生成质量（如运动一致性）。本文旨在提供首个定量分析框架 DiffTrack，填补这一空白。

## 2. 论文提出的方法论

- **核心思想**：DiffTrack 通过模拟视频生成过程，构建提示生成视频数据集并获取伪真实轨迹，再利用 3D 注意力中的中间表示（查询-键相似度 vs. 中间特征）在不同层和去噪时间步上估计帧间对应，并设计三个互补的评估指标（匹配精度、置信度、注意力分数）来量化时间匹配的准确性与影响力。
- **关键技术细节**：
  - **3D 注意力分解**：视频 DiTs 中的 full 3D attention 可分解为自帧、跨帧、文本-帧和自文本注意力。其中跨帧注意力 $A_{t,l}^{i,j}$（$i\neq j$）负责不同帧像素间的交互，是研究时间对应的核心。
  - **对应估计**：在给定时间步 $t$ 和层 $l$，对第一帧与第 $j$ 帧的查询-键相似度做 Softmax 得到匹配代价 $C_{t,l}^{1,j}$，再通过 Argmax 得到匹配点 $p_{t,l}^j$，最后上采样得到轨迹 $\hat{T}_{t,l}$。
  - **评估指标**：
    - **匹配精度**：基于 PCK（百分比正确关键点）衡量估计轨迹与伪真实轨迹的偏差。
    - **置信度**：跨帧注意力图的最大值，反映匹配的确定性。
    - **注意力分数**：跨帧注意力值的总和，反映跨帧交互对生成过程的影响力。
  - **分析策略**：对三个指标计算调和平均，以联合评估准确性、置信度和影响力，从而识别最优层和时间步。
- **公式与算法流程**：（文字说明）
  1. 给定视频 DiT 模型和文本提示 → 生成视频。
  2. 在第一帧中预定义起始点，用 CoTracker 获取伪真实轨迹。
  3. 在特定层 $l$ 和时间步 $t$ 提取查询-键或中间特征。
  4. 计算 $C_{t,l}^{1,j}$ 并执行 Argmax 得到匹配点。
  5. 计算匹配精度、置信度、注意力分数及其调和平均。
  6. 分析不同表示、层、时间步的贡献。

## 3. 实验设计

- **数据集**：
  - **分析用数据集**：针对待分析模型（如 CogVideoX-2B）构建两类提示生成视频数据集：
    - 物体数据集（object dataset）：50 个视频，聚焦动态物体，使用 SAM 分割前景并采样网格点。
    - 场景数据集（scene dataset）：50 个视频，聚焦静态场景的相机运动，均匀采样 $10\times10$ 网格。
    使用 CoTracker 获取伪真实轨迹。
  - **零样本跟踪 Benchmark**：
    - TAP-Vid-DAVIS（30 个视频）和 TAP-Vid-Kinetics（1189 个视频），评估 δ0-δ4 阈值下的点精度 δx_avg。
- **对比方法**：
  - 视觉基础模型：DINO, DINOv2, DINOv2-Reg, DIFT (SD1.5, SD2.1), Diffusion Hyperfeatures, CleanDIFT, TLR。
  - 自监督视频模型：SMTC, CRW, Spa-then-Temp, VFS, SVD, ZeroCo。
- **运动增强生成评估**：
  - 自动指标：VBench 中的 Subject Consistency, Background Consistency, Dynamic Degree, Imaging Quality。
  - 人类评估：Two-Alternative Forced Choice（2AFC）协议，收集 750 个响应（25 名参与者）。
  - 对比基线：CogVideoX-2B, CogVideoX-5B，以及 STG（Spatiotemporal Skip Guidance）。

## 4. 资源与算力

- **文中未详细说明训练资源**，仅提到零样本点跟踪实验在 **A6000 GPU** 上完成（附录 C.2）。也未提及训练时长、GPU 数量等信息。推测所有推理和分析均在单卡 A6000 上完成，无需额外训练，因此算力需求较低。

## 5. 实验数量与充分性

- **实验组数**：
  - 表示选择分析（图 4(a)）。
  - 层分析（图 4(b)）。
  - 去噪时间步分析（图 4(c), 图 5）。
  - 额外分析：真实视频（DAVIS，图 A.5）、PCA 可视化（图 A.7, A.9）、注意力可视化（图 A.17-A.19）、查询-查询/键-键/查询-键对比（图 A.8）。
  - 零样本点跟踪定量比较（表 1, 表 A.7）和定性比较（图 8, 图 A.20）。
  - 消融实验：时间压缩、第一帧插入、交错帧（表 A.2）；特征选择（表 A.3）；多特征融合（表 A.4）；帧数影响（图 A.11）；CAG 层选择（表 A.5）；内存/时间消耗（表 A.6）。
  - 运动增强生成对比（表 2, 表 3, 图 10, 图 A.21）。
  - 跨模型分析：CogVideoX-5B, HunyuanVideo, CogVideoX-5B-I2V（附录 B, 图 A.1-A.3, 表 A.1）。
- **充分性与公平性**：
  - 实验覆盖了表示、层、时间步三个维度，并对多个开源模型进行了验证，增强了结论的泛化性。
  - 零样本跟踪对比基准包括多种类型模型，并统一输入规模和特征分辨率，较为公平。
  - 消融实验系统性地检验了各组件贡献。
  - **不足**：仅分析了 3-4 个 DiT 模型（CogVideoX-2B/5B, HunyuanVideo, CogVideoX-I2V），未涵盖所有开源 DiT 架构（如 Mochi1, LTX-Video 等）。伪真实轨迹依赖 CoTracker，可能引入偏差。

## 6. 论文的主要结论与发现

1. **查询-键匹配优于中间特征匹配**：在 3D 注意力中，查询-键相似度能捕获几何线索，而值包含外观信息，会稀释对应精度。
2. **少数特定层主导时间对应**：例如 CogVideoX-2B 中第 13、17、21 层（调和平均排名靠前），其他层贡献较小。
3. **时间匹配随去噪过程逐渐增强**：早期噪声大，依赖文本和自帧注意建立语义和布局；后期跨帧注意增强，但最终步略有下降（外观细化）。
4. **三个指标需联用**：仅用置信度或注意力分数可能被位置偏置或文本注意持续激活误导。
5. **零样本点跟踪达到 SOTA**：在 TAP-Vid-DAVIS 和 Kinetics 上，DiffTrack 使用最优层和时间步（如 l=17, t=1）超越所有对比方法。
6. **Cross-Attention Guidance (CAG) 提升运动一致性**：通过零化主导层的跨帧注意图并引导模型远离退化样本，无需额外训练即可改善生成视频的运动自然度和一致性，优于 STG。

## 7. 优点

- **新颖性与首创性**：首个定量分析视频 DiTs 中时间对应机制的框架。
- **系统性**：从表示、层、时间步三个维度进行全面的量化分析，并提出调和平均来联合评估，避免单一指标误导。
- **实用性**：揭示的结论可直接迁移到下游任务（零样本点跟踪 SOTA）和生成改进（CAG 无需训练）。
- **通用性**：框架适用于多种 DiT 架构（CogVideoX-2B/5B, HunyuanVideo, CogVideoX-I2V），易于复现和扩展。
- **方法轻量**：零样本跟踪和 CAG 均无需额外训练或微调，仅利用预训练模型的内部表示。
- **实验严谨**：包含丰富的消融研究和跨模型验证，结论可靠。

## 8. 不足与局限

- **模型覆盖有限**：仅分析 3-4 个开源 DiT 模型，未涵盖 Mochi1、LTX-Video 等新模型，也缺乏对非 DiT 结构（如 U-Net 视频扩散模型）的对比。
- **伪真实轨迹偏差**：使用 CoTracker 作为伪真实标签，其自身误差可能影响分析准确性；对于未见过的复杂运动或遮挡，CoTracker 可能不可靠。
- **零样本跟踪的局限性**：未针对点跟踪任务进行微调，性能上限受限于预训练视频 DiT 的能力；长视频处理需分块插入首帧，增加计算开销，且分块间匹配可能不连续。
- **运动增强生成**：CAG 仅通过零化跨帧注意图进行引导，不直接支持用户指定的运动轨迹操控（如轨迹条件生成）。
- **计算开销**：CAG 需要两次前向传播（原始和退化），推理时间增加约 77%；虽然优于需训练的方法，但仍比基线慢。
- **公平性与安全讨论不足**：附录 J 简要提及伦理风险，但未深入探讨如何防止恶意利用生成增强的视频。
- **实验重复性**：未提供代码和数据（计划开源），当前仅靠文字描述可能难以精确复现。

（完）
