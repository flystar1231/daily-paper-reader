---
title: Hierarchical Fine-grained Preference Optimization for Physically Plausible Video Generation
title_zh: 面向物理合理视频生成的分层细粒度偏好优化
authors: "Harold Haodong Chen, Haojian Huang, Qifeng Chen, Harry Yang, Ser-Nam Lim"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=y0SRR9XGlZ"
tags: ["query:vgen-metrics"]
score: 4.0
evidence: 视频生成质量的细粒度偏好优化
tldr: 虽然PhysHPO主要关注物理合理性，但其分层偏好优化方法可间接用于视频生成质量评估，反映了对生成视频质量的关注。论文提出了一个分层跨模态直接偏好优化框架，通过实例、状态、运动和物理四个粒度对齐来增强物理合理性。实验表明该方法能生成更符合物理规律的视频，但并未直接提出评估指标。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1444, \"height\": 1017, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1429, \"height\": 714, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 532, \"height\": 592, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1446, \"height\": 1338, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1446, \"height\": 406, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1450, \"height\": 457, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1421, \"height\": 339, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1418, \"height\": 343, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1419, \"height\": 338, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1416, \"height\": 340, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1438, \"height\": 763, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1428, \"height\": 998, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1450, \"height\": 203, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 657, \"height\": 394, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1442, \"height\": 567, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1448, \"height\": 276, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1439, \"height\": 347, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1445, \"height\": 655, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1440, \"height\": 650, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1437, \"height\": 653, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1439, \"height\": 341, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1440, \"height\": 337, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1440, \"height\": 340, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1440, \"height\": 339, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1442, \"height\": 337, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1443, \"height\": 347, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1419, \"height\": 343, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1419, \"height\": 337, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1418, \"height\": 340, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1419, \"height\": 340, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 1419, \"height\": 339, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1420, \"height\": 342, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 1440, \"height\": 341, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1442, \"height\": 339, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 1442, \"height\": 342, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 1440, \"height\": 338, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 1439, \"height\": 337, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-y0srr9xglz/fig-038.webp\", \"caption\": \"\", \"page\": 0, \"index\": 38, \"width\": 1443, \"height\": 338, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-y0srr9xglz/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 533, \"height\": 151, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-y0srr9xglz/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1445, \"height\": 387, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-y0srr9xglz/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 581, \"height\": 219, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-y0srr9xglz/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1446, \"height\": 218, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-y0srr9xglz/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 531, \"height\": 228, \"label\": \"Table\"}]"
motivation: 现有视频生成方法缺乏物理合理性，需要更好的质量评估方法。
method: 提出分层跨模态直接偏好优化（PhysHPO），在四个粒度层级上对齐视频内容。
result: 生成的视频在物理合理性上显著优于基线。
conclusion: 偏好优化可作为提升视频质量的有效手段，但与评估指标直接相关度较低。
---

## Abstract
Recent advancements in video generation have enabled the creation of high-quality, visually compelling videos. However, generating videos that adhere to the laws of physics remains a critical challenge for applications requiring realism and accuracy. In this work, we propose **PhysHPO**, a novel framework for Hierarchical Cross-Modal Direct Preference Optimization, to tackle this challenge by enabling fine-grained preference alignment for physically plausible video generation. PhysHPO optimizes video alignment across four hierarchical granularities: a) ***Instance Level***, aligning the overall video content with the input prompt; b) ***State Level***, ensuring temporal consistency using boundary frames as anchors; c) ***Motion Level***, modeling motion trajectories for realistic dynamics; and d) ***Semantic Level***, maintaining logical consistency between narrative and visuals. Recognizing that real-world videos are the best reflections of physical phenomena, we further introduce an automated data selection pipeline to efficiently identify and utilize *"good data"* from existing large-scale text-video datasets, thereby eliminating the need for costly and time-intensive dataset construction. Extensive experiments on both physics-focused and general capability benchmarks demonstrate that PhysHPO significantly improves physical plausibility and overall video generation quality of advanced models. To the best of our knowledge, this is the first work to explore fine-grained preference alignment and data selection for video generation, paving the way for more realistic and human-preferred video generation paradigms.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）
- **核心问题**：当前文本到视频（T2V）生成模型虽能产生高质量视频，但生成的视频往往违反物理规律（如物体运动不自然、交互不合理），缺乏物理合理性。
- **挑战**：现有方法分为两类——① 测试时反射优化（如PhyT2V）增加推理开销且受限于模型自纠正能力上限；② 训练时微调（SFT）依赖固定监督信号，对特定能力优化效果欠佳，且需要大量人工构建数据集（如WISA、SynVideo）。
- **整体含义**：本文提出**PhysHPO**，首次将细粒度直接偏好优化（DPO）和数据选择引入视频生成领域，旨在无需昂贵数据集构建的前提下，通过分层对齐显著提升视频的物理合理性和整体质量。

## 2. 论文提出的方法论
- **核心思想**：采用分层跨模态直接偏好优化（Hierarchical Cross-Modal DPO），在四个粒度层级上对齐视频生成，同时引入自动数据选择流水线从现有数据集中高效挑选“好数据”。
- **关键技术细节**：
  - **数据选择**：从大规模高质量数据集（OpenVidHD-0.4M）出发，分三步：
    1. **真实性过滤**：使用VLM（Qwen2.5-VL + DeepSeek-VL2）筛选真实世界视频（准确率>99%）。
    2. **物理保真度评分**：采用“深度演化提示”增强视频描述，基于LLM对动态、热力学、光学三大类共17种物理现象进行细粒度打分，整合为总分 \( s = s_d \times s_t \times s_o \)。
    3. **多样性选择**：基于caption嵌入的余弦距离，迭代挑选多样性样本（阈值τ=0.9），最终得到约21K子集。
  - **偏好优化——PhysHPO**：
    - **实例级对齐**（Instance Level）：使用真实世界视频作为偏好样本（`y_w`），并构造两种非偏好样本：`y_err`（基模型生成且视觉相似的错误视频）和`y_gap`（通过随机掩码prompt产生语义差距的视频）。损失函数为DPO损失，其中非偏好得分混合两个来源。
    - **状态级对齐**（State Level）：将偏好视频的首尾N帧替换，构成状态非偏好样本（`y_state`），强制模型关注边界帧的物理状态。
    - **运动级对齐**（Motion Level）：提取偏好和非偏好视频的结构信息（如光流），构建`y_motion_w`和`y_motion_l`，在运动表征空间进行DPO对齐。
    - **语义级对齐**（Semantic Level）：使用VLM根据非偏好视频修改prompt生成`c_l`，保持偏好视频caption`c_w`，让模型在给定不同文本条件下对同一视频产生不同得分，从而实现文本-视频语义一致性。
  - **总体损失**：\( L_{\text{PhysHPO}} = L_{\text{Instance}} + \lambda L_{\text{State}} + \rho L_{\text{Motion}} + \mu L_{\text{Semantic}} \)，其中超参数经实验调优（λ=0.4, ρ=0.3, μ=0.2, β_err=0.7, β_gap=0.3, N=2）。
- **算法流程**：
  1. 数据选择：过滤→评分→多样性迭代选择，得到高质量子集。
  2. 训练：加载预训练视频生成模型（如CogVideoX-2B/5B），以子集数据作为偏好样本，构造各类非偏好样本，按总体损失联合优化。

## 3. 实验设计
- **数据集/场景**：
  - **数据选择来源**：OpenVidHD-0.4M（用于后训练的高质量视频-文本数据集）。
  - **物理聚焦基准**：VideoPhy（ICLR 2025，评估固体-固体、固体-流体、流体-流体交互）和PhyGenBench（ICML 2025，评估力学、光学、热学、材料等物理常识）。
  - **通用质量基准**：VBench（评估整体质量和语义一致性）。
  - **额外测试**：使用IPV-T XT（Impossible Videos）评估模型对违反物理常识的创造性prompt的鲁棒性。
- **对比方法**：
  - 基线：CogVideoX-2B/5B（基模型）、PhyT2V（测试时反射优化）、Vanilla DPO（标准DPO）、SFT（监督微调）。
  - 还对比了数据选择的不同策略（随机选择、直接评分、WISA-32K人工数据集、原始全量数据等）。
  - 在HunyuanVideo上进一步验证。
- **评估指标**：
  - VideoPhy：物理一致性（PC）和语义一致性（SA）同时满足的比例。
  - PhyGenBench：物理常识对齐（PCA）得分。
  - VBench：整体质量和语义得分。
  - 用户研究：5个维度（全局偏好、语义遵循、物理常识、视觉质量、运动质量）的MOS评分。
  - 鲁棒性测试：视觉质量（VQ）和不可能prompt遵循（IPF）得分。

## 4. 资源与算力
- **明确说明**：所有PhysHPO训练在**8块NVIDIA H100 GPU**上进行。
- **训练细节**：全局batch size=8，AdamW优化器，学习率2e-5。未明确给出总训练时长或GPU小时数。
- **数据选择方面**：caption方式比逐帧视频筛选节省约18% GPU显存、27.6% GPU小时和约$674成本（以8块H100计）。

## 5. 实验数量与充分性
- **主实验**：在CogVideoX-2B和5B上分别对比三个基线在VideoPhy、PhyGenBench、VBench上的结果（表2），共8行×3列=24个指标比较。
- **消融实验**：表3逐步移除各层级损失，验证分层有效性；图3对比不同数据选择策略（5种）；图5与SFT在不同数据量下的对比（5种量级）。
- **超参数分析**：图13（4个子图）探讨λ, ρ, μ, β_err/β_gap的影响；图14分析非偏好样本选择策略（实例数量、帧交换数量、运动表示类型）。
- **额外验证**：在HunyuanVideo上复现（表4、图7），展示人类动作视频（图17、18）、更多定性比较（图15、16）。
- **用户研究**：15名志愿者，5维度MOS评分。
- **总体充分性**：实验覆盖了不同模型大小、不同基准、不同优化方法（DPO vs SFT）、不同数据策略、多组消融及超参数调优，且在同一设定下与基线公平比较（均使用相同基模型和训练细节）。结论较为扎实。

## 6. 论文的主要结论与发现
- **物理合理性显著提升**：PhysHPO在VideoPhy和PhyGenBench上超越所有基线（包括PhyT2V和Vanilla DPO），且不损害VBench通用质量（甚至略有提升）。
- **分层对齐有效**：逐步去除层级损失导致性能稳步下降，表明实例、状态、运动、语义四个层级协同作用。
- **数据选择优于从头构建**：使用21K精选数据比WISA-32K人工数据集和433K原始数据更好，且多样性选择带来额外收益。
- **PhysHPO比SFT更优**：在相同数据量下，PhysHPO在物理和通用指标上均优于SFT，且数据效率更高（小量数据就超过SFT大量数据）。
- **鲁棒性增强**：即使面对不可能prompt，PhysHPO生成视频更能遵循语义意图并保持内部一致性，说明模型学到了更广义的物理规律而非单纯过拟合。
- **用户偏好**：用户研究显示PhysHPO在所有维度上都比基线更受欢迎。

## 7. 优点
- **方法创新**：首次将细粒度DPO用于视频生成，设计了分层对齐框架（实例、状态、运动、语义），全面覆盖视频理解的不同层面。
- **数据策略创新**：提出自动数据选择流水线，利用现有真实世界数据，无需昂贵人工标注，并首次将数据选择问题引入视频生成领域。
- **高效实用**：caption级评分比视频级评分更省资源，且通过多样性选择进一步压缩数据量（21K vs 433K），同时提升性能。
- **实验全面**：覆盖多个模型、多类基准、多种对比方法、充分消融和超参数分析，结论可信度高。
- **代码公开**：基于CogVideoX的代码以匿名方式提供，促进可复现性。
- **鲁棒性分析**：验证了模型对违反物理常识的prompt的适应能力，表明学习到的是更普遍的物理机制。

## 8. 不足与局限
- **计算成本高**：尽管数据选择节省了资源，但训练大规模视频生成模型仍需8块H100 GPU，对资源有限的研究者/企业仍具门槛（附录E明确提及）。
- **数据选择较简单**：当前设计追求实用性，仅基于caption和LLM评分+多样性，未进一步考虑更精细的物理细节或任务特定优化（附录E指出未来可改进）。
- **实验未覆盖所有模型**：仅测试了CogVideoX和HunyuanVideo两个系列，其他主流模型（如Wan、Open-Sora等）未验证。
- **未报告误差棒**：由于训练时间长、成本高，论文未进行多次重复实验报告统计显著性（论文声明）。
- **物理分类有限**：虽涵盖17种物理现象，但可能遗漏其他重要物理效应（如声学、电磁学等），对极端场景（如微观尺度）可能不适用。
- **伦理风险**：生成高质量视频可能被滥用于制造虚假内容，论文在附录F中建议加水印和设置使用准则，但未落地具体防护措施。
- **用户研究规模**：仅15名志愿者，样本量较小，结果可能存在个体差异。

（完）
