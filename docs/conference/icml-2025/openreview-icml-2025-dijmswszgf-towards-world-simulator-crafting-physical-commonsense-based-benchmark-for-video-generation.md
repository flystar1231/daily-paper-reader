---
title: "Towards World Simulator: Crafting Physical Commonsense-Based Benchmark for Video Generation"
title_zh: 走向世界模拟器：构建基于物理常识的视频生成基准
authors: "Fanqing Meng, Jiaqi Liao, Xinyu Tan, Quanfeng Lu, Wenqi Shao, Kaipeng Zhang, Yu Cheng, Dianqi Li, Ping Luo"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=dIjMswSzgF"
tags: ["query:vgen-metrics"]
score: 6.0
evidence: 视频生成物理常识评估基准
tldr: 现有文本到视频模型在常识物理理解方面缺乏系统评估。为此提出PhyGenBench基准，包含160个精心设计的提示，覆盖27条物理规律，评估生成视频的物理正确性，为视频生成模型的质量评估提供新工具。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1565, \"height\": 898, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1394, \"height\": 1095, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1420, \"height\": 758, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1235, \"height\": 548, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1753, \"height\": 694, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1704, \"height\": 1941, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1740, \"height\": 451, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1738, \"height\": 1020, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1723, \"height\": 510, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1727, \"height\": 1524, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dijmswszgf/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1329, \"height\": 2247, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 862, \"height\": 186, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1286, \"height\": 518, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1772, \"height\": 439, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1771, \"height\": 210, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 595, \"height\": 663, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1248, \"height\": 323, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1428, \"height\": 901, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1771, \"height\": 414, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1423, \"height\": 524, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1772, \"height\": 593, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1772, \"height\": 355, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 980, \"height\": 149, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1148, \"height\": 455, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dijmswszgf/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1342, \"height\": 286, \"label\": \"Table\"}]"
motivation: 视频生成模型对物理常识的准确表现尚未被充分评估。
method: 设计涵盖27条物理定律的160个提示的PhyGenBench基准。
result: 基准能揭示模型在物理常识遵循上的不足。
conclusion: 为视频生成模型物理正确性评估提供标准化基准。
---

## Abstract
Text-to-video (T2V) models like Sora have made significant strides in visualizing complex prompts, which is increasingly viewed as a promising path towards constructing the universal world simulator. Cognitive psychologists believe that the foundation for achieving this goal is the ability to understand intuitive physics. However, the capacity of these models to accurately represent intuitive physics remains largely unexplored. To bridge this gap, we introduce PhyGenBench, a comprehensive \textbf{Phy}sics \textbf{Gen}eration \textbf{Ben}chmark designed to evaluate physical commonsense correctness in T2V generation. PhyGenBench comprises 160 carefully crafted prompts across 27 distinct physical laws, spanning four fundamental domains, which could comprehensively assesses models' understanding of physical commonsense. Alongside PhyGenBench, we propose a novel evaluation framework called PhyGenEval. This framework employs a hierarchical evaluation structure utilizing appropriate advanced vision-language models and large language models to assess physical commonsense. Through PhyGenBench and PhyGenEval, we can conduct large-scale automated assessments of T2V models' understanding of physical commonsense, which align closely with human feedback. Our evaluation results and in-depth analysis demonstrate that current models struggle to generate videos that comply with physical commonsense. Moreover, simply scaling up models or employing prompt engineering techniques is insufficient to fully address the challenges presented by PhyGenBench (e.g., dynamic scenarios). We hope this study will inspire the community to prioritize the learning of physical commonsense in these models beyond entertainment applications. We will release the data and codes at https://github.com/OpenGVLab/PhyGenBench

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 核心问题与整体含义（研究动机和背景）

- **研究动机**：当前文本到视频（T2V）生成模型（如Sora）在可视化复杂提示方面取得了显著进展，被视为通往通用世界模拟器的有前景路径。然而，这些模型是否真正理解直观物理常识（intuitive physics）——即物体在现实世界中如何行为的基本物理规律——尚未得到系统评估。认知心理学认为，理解直观物理是构建世界模拟器的基础。
- **核心问题**：现有T2V模型在生成视频时经常违反基本物理常识（例如，石头本应沉入水中却浮在水面，鸡蛋撞击石头应破裂却弹起），表明它们与真实世界模拟器之间存在巨大差距。缺乏一个专门评估物理常识正确性的基准和评价方法。
- **整体意义**：填补该空白，通过提出PhyGenBench基准和PhyGenEval评估框架，全面衡量T2V模型对物理常识的理解能力，推动模型向物理一致的世界模拟器发展，而非仅用于娱乐。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：
  - 构建一个覆盖多个物理领域的基准（PhyGenBench），包含精心设计的提示，每个提示对应一个明确的物理现象和物理定律。
  - 提出一个层次化的自动评估框架（PhyGenEval），逐步从单帧关键现象检测、多帧物理顺序验证到整体自然度评估，利用高级视觉语言模型（VLM）和大语言模型（LLM）实现与人类判断高度一致的自动化评估。

- **关键技术细节**：
  - **PhyGenBench构建**：
    - 物理分类：涵盖四大领域——力学（7条定律）、光学（6条）、热学（6条）、材料性质（8条），共27条物理定律。
    - 数据构造流程：概念化 → 手动编写初始提示 → 使用GPT-4o增强提示细节（不泄露预期现象） → 通过物体替换增加多样性 → 生成用于各评估阶段的物理相关问题 → 人工质量控制（检查提示的清晰性、简单性、多样性及物理定律的对应关系）。
    - 最终得到160个提示，每个提示对应单一物理现象，避免多重物理定律混淆。
  - **PhyGenEval评估框架**：
    - **语义对齐（SA）评估**：先用GPT-4o从原始提示中提取物体和动作，再分别判断视频中是否出现这些物体和动作，降低VLM直接评估的复杂度。
    - **物理常识对齐（PCA）评估**：三阶段层次化策略：
      1. **关键物理现象检测**：使用检索提示定位关键帧，通过VLM（基于VQAScore）判断关键帧中是否出现预期物理现象（如鸡蛋破裂）。
      2. **物理顺序验证**：验证关键事件发生的顺序是否正确（如鸡蛋先接触石头再破裂）。使用检索提示定位关键帧，并利用多帧问题（q1, q2, q3）分别验证前序、后续和全局顺序。
      3. **整体自然度评估**：利用视频级VLM（如InternVideo2、GPT-4o）基于LLM生成的四个等级描述（完全幻想、明显不真实、略微不真实、几乎真实）对视频整体动态自然度评分。
    - 最终得分：将三个阶段得分离散化为0-3分，取平均并向下取整。集成GPT-4o和开源模型结果以提高鲁棒性。

## 3. 实验设计

- **数据集/场景**：
  - **PhyGenBench**：包含160个提示，覆盖27条物理定律，分为力学（40个）、光学（50个）、热学（30个）、材料性质（40个）四个领域。
  - 每个提示经人工验证，确保语义简单且物理现象清晰可辨。

- **Benchmark**：
  - 使用PhyGenBench作为测试基准，评估生成视频的物理常识正确性（PCA）和语义对齐（SA）。

- **对比方法**：
  - **视频生成模型**：8个开源模型（CogVideoX 2B/5B, Open-Sora V1.2, LaVie, Vchitect 2.0, Hunyuan, Pyramid Flow等）和6个闭源模型（Kling, Pika, Sora, Vidu, Hailuo, Gen-3）。
  - **评估指标对比**：与现有指标比较相关性，包括DEVIL（基于Gemini 1.5 Pro）、VideoPhy（微调VLM）、VideoScore（基于Mantis微调）、Grid-LLaVA（T2V-CompBench使用）等。

- **人类评估**：
  - 从8个T2V模型中随机选择64个提示，生成视频，由三位标注员分别对语义和物理正确性进行0-3分评分，取平均并取整，计算与自动评估的Kendall’s τ和Spearman’s ρ相关系数。

## 4. 资源与算力

- 论文未明确说明训练模型所需的算力（因为评估使用已训练好的模型），但提供了**PhyGenEval评估过程的资源消耗**（附录F，表13）：
  - GPT-4o（阶段2）：8 batch，费用约1.4美元，耗时5分钟。
  - GPT-4o（阶段3）：8 batch，费用约3.1美元，耗时5分钟。
  - LLaVA-Next-Interleave-7B：1 batch，1×A100-80GB GPU，2分钟，显存20,408 MiB。
  - VQAScore：3 batch，1×A100-80GB GPU，10分钟，显存72,726 MiB。
  - InternVideo2：1 batch，1×A100-80GB GPU，1分钟，显存7,766 MiB。
- **总结**：评估过程快速且成本低，但未提及模型训练资源。

## 5. 实验数量与充分性

- **实验组数**：
  - 主表（表2）对比了14个T2V模型在4个物理领域和总体的PCA分数。
  - 消融实验（附录D.4）：对PhyGenEval各阶段（S、M、V）进行单独及组合的影响分析（表11）；对比不同VLM（开源小模型、开源大模型、闭源模型）的评估效果（表12）；分析检索操作的鲁棒性（表10）。
  - 语义对齐相关性实验（表8）：对比PhyGenEval与VideoPhy、VideoScore、Grid-LLaVA等方法的SA相关性。
  - 提示重写实验（表3）：对Kling和CogVideoX 5B进行重写提示前后的PCA对比。
  - VEnhancer增强实验（表4）：验证Vchitect 2.0在VEnhancer增强前后的PCA分数变化。
  - 低质量视频鲁棒性测试（附录E）：对100个低质量视频计算PCA得分。

- **充分性评价**：
  - **客观**：消融实验覆盖评估框架的每个组件，对比多种模型和多种基线，且使用人工标注作为黄金标准，计算相关性。
  - **公平**：所有实验使用统一基准和评估协议，API设置温度0以确保可重复性。
  - **充分**：覆盖了物理常识的多个方面，但未涉及跨模态交互、长时间动态物理等更复杂场景。实验数量合理，但部分分析（如缩放定律影响）仅基于两个模型规模的对比，可进一步扩展。

## 6. 主要结论与发现

1. **当前模型表现差**：即使是最好模型（Gen-3）的PCA分数仅为0.51（0-1），表明T2V模型在遵循物理常识方面严重不足，距离世界模拟器尚远。
2. **光学领域表现最好**：所有模型在光学领域（反射、折射等）相对较好，归因于预训练数据中光学知识丰富且明确。
3. **闭源模型优于开源**：Sora和Hailuo达到0.55，显著优于大多数开源模型（0.36-0.47）。
4. **缩放定律局限**：仅增加模型规模（如CogVideoX 2B→5B）在静态场景有所提升，但对动态物理现象（如弹性、浮力）改善有限。
5. **提示重写效果有限**：添加预期物理过程描述的提示仅带来小幅提升（Kling从0.49到0.56），无法解决根本问题。
6. **视频增强无效**：VEnhancer改善视觉质量但不改善物理正确性，说明PhyGenBench评估的是物理常识而非视觉质量。
7. **人类相关性高**：PhyGenEval的PCA评估与人类判断的Spearman’s ρ达0.81，显著优于现有指标（DEVIL 0.18, VideoScore 0.19, VideoPhy 0.04）。

## 7. 优点

- **基准设计合理**：PhyGenBench覆盖多个物理领域和27条明确定律，提示简洁且与物理现象对应明确，有利于评估和自动检测。
- **评估方法创新**：PhyGenEval采用层次化策略（单帧→多帧→全视频），专门针对物理正确性设计，而非通用视频质量，从而解决VLM难以理解物理常识的问题。
- **自动化与人类一致**：无需参考视频，完全自动化，与人类反馈高度相关（ρ=0.81），可大规模应用于不同模型。
- **鲁棒性验证充分**：通过消融实验证明了各阶段、不同VLM选择的必要性，并对检索失败、低质量视频等情况进行了鲁棒性分析。
- **开源发布**：将数据和代码开源，促进社区研究。

## 8. 不足与局限

- **场景简单**：基准仅包含基本物理现象（如鸡蛋碰撞、石头沉没），未覆盖更复杂的多物体交互、长时间动态、流体-固体耦合、非刚性物体形变等，可能低估模型对未来更复杂场景的表现。
- **评估依赖大模型**：PhyGenEval使用GPT-4o等大模型，虽然提供了开源方案，但纯开源方案的相关性（0.66-0.72）仍低于闭源方案（0.81），存在一定偏差风险和成本门槛。
- **实验覆盖局限**：仅对8/6个模型进行系统评估，未测试更多最近模型（如Pika 2.0、Gen-3后续版本等）；缩放定律分析仅基于CogVideoX两个尺寸，不够全面。
- **缺乏多物理定律组合**：每个提示只对应一个物理现象，现实世界视频常涉及多重定律交互，基准未能反映这种复杂性。
- **人类注释偏差**：人工评分基于少数标注员（3位），可能存在主观差异，但相关性已较高。
- **应用限制**：目前仅适用于评估，未提出如何训练模型以改善物理常识的方法（除提及WISA微调实验外）。

（完）
