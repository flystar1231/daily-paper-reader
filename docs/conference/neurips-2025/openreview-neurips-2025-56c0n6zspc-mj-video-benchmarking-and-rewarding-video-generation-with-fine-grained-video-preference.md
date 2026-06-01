---
title: "MJ-Video: Benchmarking and Rewarding Video Generation with Fine-Grained Video Preference"
title_zh: MJ-Video：通过细粒度视频偏好对视频生成进行基准测试和奖励
authors: "Haibo Tong, Zhaoyang Wang, Zhaorun Chen, Haonian Ji, Shi Qiu, Siwei Han, Kexin Geng, Zhongkai Xue, Yiyang Zhou, Peng Xia, Mingyu Ding, Rafael Rafailov, Chelsea Finn, Huaxiu Yao"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=56C0n6zSpC"
tags: ["query:vgen-metrics"]
score: 9.0
evidence: 提出了一个用于全面评估视频生成的基准和奖励模型
tldr: 现有的视频生成模型在指令对齐、内容幻觉、安全性和偏差方面存在挑战。为此，本文提出了MJ-BENCH-VIDEO，一个大规模视频偏好基准，从对齐、安全、精细度、一致性与一致性以及偏见与公平五个方面共28个细粒度标准来评估视频生成。基于该基准，进一步提出MJ-VIDEO，一个基于混合专家（MoE）的奖励模型。实验表明该奖励模型能够有效评估和指导生成模型，从而提升视频生成的整体质量。该工作为视频生成评估提供了全面的指标框架。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1344, \"height\": 846, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 705, \"height\": 358, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1388, \"height\": 433, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 730, \"height\": 313, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1381, \"height\": 682, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1445, \"height\": 798, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1440, \"height\": 470, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1452, \"height\": 733, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-56c0n6zspc/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1429, \"height\": 1995, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1450, \"height\": 472, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 719, \"height\": 488, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 708, \"height\": 254, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1449, \"height\": 226, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1269, \"height\": 586, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1268, \"height\": 604, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1268, \"height\": 513, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1269, \"height\": 729, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1268, \"height\": 548, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1151, \"height\": 637, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 988, \"height\": 279, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1434, \"height\": 639, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1435, \"height\": 638, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1439, \"height\": 443, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1436, \"height\": 530, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1437, \"height\": 641, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1091, \"height\": 367, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-56c0n6zspc/table-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1144, \"height\": 363, \"label\": \"Table\"}]"
motivation: 现有视频生成评估缺乏全面细粒度标准，难以覆盖对齐、安全等多方面质量。
method: 构建MJ-BENCH-VIDEO基准，包含28个细粒度评价标准，并设计基于MoE的奖励模型MJ-VIDEO。
result: MJ-VIDEO奖励模型在多个评估维度上有效区分高质量与低质量生成视频。
conclusion: 该工作为视频生成提供了系统的评估指标和奖励模型，有助于推动模型改进。
---

## Abstract
Recent advancements in video generation have significantly improved the ability to synthesize videos from text instructions. However, existing models still struggle with key challenges such as instruction misalignment, content hallucination, safety concerns, and generation bias. To address these limitations, we introduce MJ-BENCH-VIDEO, a large-scale video preference benchmark designed to evaluate video generation across five critical aspects: Alignment, Safety, Fineness, Coherence & Consistency, and Bias & Fairness. This benchmark further incorporates 28 fine-grained criteria to provide a comprehensive evaluation of video preference. Building upon this dataset, we propose MJ-VIDEO, a Mixture-of-Experts (MoE)-based video reward model designed to deliver fine-grained reward. MJ-VIDEO can dynamically select relevant experts to accurately judge the preference based on the input text-video pair. This architecture enables more precise and adaptable preference judgments. Through extensive benchmarking on MJ-BENCH-VIDEO, we analyze the limitations of existing video reward models and demonstrate the superior performance of MJ-VIDEO in video preference assessment, achieving 17.58% and 15.87% improvements in overall and fine-grained preference judgments, respectively. Additionally, MJ-VIDEO is able to improve the alignment performance in video generation via preference fine-tuning.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

近年来视频生成技术取得显著进展，但从文本指令生成视频仍面临指令对齐不准、内容幻觉、安全隐患和生成偏见等关键挑战。现有视频奖励模型多局限于整体对齐评估，缺乏细粒度、多维度评估体系，无法适应不同应用场景下多样化的对齐目标（如体育视频更注重连贯性，卡通视频更注重安全性）。因此，本文旨在构建一个大规模、细粒度视频偏好基准和相应的奖励模型，以系统评估和改善视频生成质量。

## 2. 方法论：核心思想、关键技术细节、公式或算法流程

### 核心思想
- 提出 **MJ-BENCH-VIDEO**：涵盖五个关键评估方面（对齐、安全、精细度、连贯一致性、偏见公平性），共28条细粒度标准，提供结构化、多维度的视频偏好标注。
- 提出 **MJ-VIDEO**：基于视频大语言模型（InternVL2-2B）和混合专家（MoE）架构的奖励模型，能够动态选择相关专家对输入文本-视频对进行精准偏好判断。

### 关键技术细节
- **架构**：两层MoE堆叠——第一层**Aspect MoE**负责将输入路由到五个方面，第二层**Criteria MoE**为每个细粒度标准打分。最终通过方面加权得到总体偏好分数。
- **公式**：
  - 方面路由权重：\( AR = \text{softmax}(g(h)) \)（\( h \)为视频-文本隐藏状态）
  - 细粒度标准得分：\( C[U_i] = \text{softmax}(g'(h)[U_i]) \odot f(h)[U_i] \)
  - 总体偏好得分：\( OS = \sum_{i=1}^5 \left( \sum_{t \in U_i} C[t] \right) AR[i] \)
- **三阶段训练**：
  1. **阶段I（标准评分训练）**：用MSE损失训练Criteria MoE预测细粒度标注分数。
  2. **阶段II（方面路由训练）**：用排序损失（Bradley-Terry）训练Aspect MoE，同时继续优化阶段I损失。
  3. **阶段III（联合训练）**：引入总体偏好排序损失，联合优化两个MoE层，并用超参数\(\lambda\)平衡各损失。

## 3. 实验设计

### 数据集与场景
- **MJ-BENCH-VIDEO**：构建了5,421个视频偏好对（10,842个视频，5,421个提示），来自三个来源：现有视频偏好数据集（Safesora）、图像-视频转换（MJ-BENCH, HPDv2 → Stable Video Diffusion）、文本-视频直接生成（OpenVid, VidProM, VidGen → 多种开源模型）。按4:1划分为训练集（4,336对）和测试集（1,085对）。
- **额外整体偏好评估**：Safesora-test和GenAI-Bench。

### 基准与对比方法
- **多模态评委模型**：开源（InternVL2-2B/4B/8B/26B, Qwen2-VL-2B/7B, MiniCPM-8B, CogVLM2）和闭源（GPT-4o, Gemini-1.5-flash）的LVLMs，以及VideoScore。
- **评估指标**：视频质量评价使用准确率（Acc）和F1分数；视频偏好评价使用严格准确率（strict）和平局感知准确率（tie-aware）。

## 4. 资源与算力

论文中未明确说明训练MJ-VIDEO所使用的具体GPU型号、数量及训练时长。仅在附录F.1中提及训练参数（批次大小64，学习率3e-5，优化器AdamW，3个epoch共201步等），但未提供硬件配置细节。因此，算力信息不充分，无法复现成本。

## 5. 实验数量与充分性

- **整体实验量**：
  - 在MJ-BENCH-VIDEO测试集上进行细粒度质量评估与偏好评价（表1、表10）。
  - 在Safesora-test和GenAI-Bench上进行整体偏好评估（表2）。
  - 在VBench和人类评估上对文本-视频生成模型进行偏好调优测试（表3）。
  - 消融实验：去除Criteria MoE层（图4a）和去除Aspect MoE层（图4b）；多阶段训练对比（表17）；专家模块去除分析（表18）。
  - 案例研究（图5、图8、图9）。
- **充分性与公平性**：实验覆盖了多种基线模型（不同规模、开源/闭源），使用多个公开数据集，评估指标全面（Acc、F1、strict、tie-aware）。消融实验验证了各个组件的贡献。但受限于开源模型的性能，生成视频的质量普遍低于闭源模型（如Sora），可能影响基准的绝对质量。整体上实验设计较为充分、客观，但未提供统计显著性检验（如误差棒）。

## 6. 主要结论与发现

1. 现有LVLMs在细粒度视频评估上存在显著不足：在严格准确率上大多低于30%，尤其是Fineness和Bias & Fairness方面。
2. **MJ-VIDEO**在几乎所有方面超越所有基线模型：相比类似规模的InternVL2-2B，准确率提升20.12%，F1提升16.97%，偏好比较提升51.67%；甚至超过26B模型（准确率+15.52%，F1+9.05%）。
3. 在整体偏好评估上，MJ-VIDEO在三个数据集上均取得最佳结果：比最好基线在MJ-BENCH-VIDEO上提升17.58%，在Safesora-test上提升15.95%，在GenAI-Bench上提升1.65%。
4. 作为奖励模型进行偏好调优，MJ-VIDEO优于VideoScore，能有效提升VideoCrafter2生成的视频质量和文本对齐（人类评估：质量69.9% vs 64.5%，对齐79.2% vs 74.8%）。
5. 消融实验证明MoE两层的必要性：去除任一MoE层均导致性能下降。

## 7. 优点

- **细粒度、多维度基准**：首次将视频评估拆分为五个方面28条标准，并提供高质量人工标注，为后续研究提供系统化评估工具。
- **创新MoE架构**：通过动态路由机制实现自适应评估，无需人工指定视频类型，提升了奖励模型的灵活性和准确性。
- **三阶段渐进式训练**：从细粒度标准到方面偏好再到总体偏好，有效利用不同层级的监督信号。
- **实验设计全面**：覆盖质量、偏好两个维度，使用多个基线、多个数据集，并进行消融和组件分析，结论可靠。
- **实际应用验证**：将奖励模型用于文本-视频模型的偏好调优，验证了其在提升生成质量上的实用价值。

## 8. 不足与局限

- **数据质量受限**：MJ-BENCH-VIDEO中的视频主要来自开源生成模型，整体质量和动态性远不如闭源模型（如Sora），可能限制基准的判别力和泛化性。
- **仅关注短视频**：未涉及长视频生成评估，实用性有限。
- **算力信息不透明**：未提供训练硬件细节，影响复现性和成本评估。
- **缺乏统计显著性验证**：未报告误差棒或置信区间，部分结果差异可能不具有统计意义。
- **Bias & Fairness方面数据量较小**：导致某些指标（如tie-aware）可能被给同分的模型拉高，严格准确率更具参考性，但数据维度的不平衡可能影响结论稳健性。
- **闭源模型评估不全面**：仅测试了GPT-4o和Gemini，未覆盖其他近期闭源模型（如Claude、o1），虽然附录C.1补充了o1等对比，但总体仍不够系统。

（完）
