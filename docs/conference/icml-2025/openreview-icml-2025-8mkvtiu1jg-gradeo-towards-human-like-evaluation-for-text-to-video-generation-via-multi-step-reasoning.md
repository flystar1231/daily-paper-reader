---
title: "GRADEO: Towards Human-Like Evaluation for Text-to-Video Generation via Multi-Step Reasoning"
title_zh: GRADEO：通过多步推理实现类人评估文本到视频生成
authors: "Zhun Mou, Bin Xia, Zhengchao Huang, Wenming Yang, Jiaya Jia"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=8mkVTiU1jG"
tags: ["query:vgen-metrics"]
score: 9.0
evidence: 提出了GRADEO，一种类人评估模型用于文本到视频生成
tldr: 论文指出当前自动评估指标缺乏高级语义理解和推理能力导致不可解释。为此构建了GRADEO-Instruct数据集（包含3.3k视频和16k人类标注的多步推理评估），并训练了专门用于视频生成评估的模型GRADEO。该模型通过多步推理进行类人评分，实验表明其与人类判断高度一致，为视频生成质量评估提供了可解释且有效的新方案。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 852, \"height\": 514, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1765, \"height\": 1016, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 830, \"height\": 415, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 275, \"height\": 157, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 60, \"height\": 61, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 270, \"height\": 158, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 560, \"height\": 362, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1427, \"height\": 550, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1425, \"height\": 748, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1089, \"height\": 138, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1081, \"height\": 133, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1081, \"height\": 223, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1725, \"height\": 853, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1753, \"height\": 994, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1784, \"height\": 234, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1778, \"height\": 644, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1671, \"height\": 1729, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1365, \"height\": 717, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1381, \"height\": 528, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1364, \"height\": 750, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1372, \"height\": 720, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-8mkvtiu1jg/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1377, \"height\": 721, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 860, \"height\": 341, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1778, \"height\": 513, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 859, \"height\": 355, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 864, \"height\": 348, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1106, \"height\": 318, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1780, \"height\": 566, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1426, \"height\": 761, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1776, \"height\": 1535, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 903, \"height\": 541, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1080, \"height\": 672, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-8mkvtiu1jg/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1314, \"height\": 283, \"label\": \"Table\"}]"
motivation: 现有视频生成自动评估指标缺乏高层语义理解和推理能力，不可解释。
method: 构建GRADEO-Instruct数据集，训练GRADEO模型，通过多步推理对生成视频进行类人评分。
result: 在多个基准上，GRADEO与人类评估一致性显著优于现有指标。
conclusion: GRADEO为视频生成评估提供了可解释、有效的自动化方法。
---

## Abstract
Recent great advances in video generation models have demonstrated their potential to produce high-quality videos, bringing challenges to effective evaluation. Unlike human evaluation, existing automated evaluation metrics lack high-level semantic understanding and reasoning capabilities for video, thus making them infeasible and unexplainable. To fill this gap, we curate **GRADEO-Instruct**, a multi-dimensional T2V evaluation instruction tuning dataset, including 3.3k videos from over 10 existing video generation models and multi-step reasoning assessments converted by 16k human annotations. We then introduce **GRADEO**, one of the first specifically designed video evaluation models, which **grades** AI-generated **videos** for explainable scores and assessments through multi-step reasoning. Experiments show that our method aligns better with human evaluations than existing methods. Furthermore, our benchmarking reveals that current video generation models struggle to produce content that aligns with human reasoning and complex real-world scenarios. The models, datasets, and codes will be released soon.

---

## 论文详细总结（自动生成）

# GRADEO：通过多步推理实现类人评估文本到视频生成 —— 详细中文总结

## 1. 核心问题与整体含义（研究动机与背景）

- **研究动机**：文本到视频（T2V）生成模型（如Sora、VideoCrafter等）已能生成高质量视频，但现有自动评估指标（如FVD、CLIPSim、图像质量度量）存在三大缺陷：
  1. 缺乏高层语义理解能力，仅关注低层视觉质量（清晰度、伪影等），无法评估理性、安全性、创意等高层次维度。
  2. 仅输出分数，没有解释性（不可解释）。
  3. 预训练模型基于真实世界数据，难以准确评估生成视频的分布，与人类评估一致性差。
- **整体含义**：亟需一种可解释、类人的自动化评估方法，能像人类一样通过多步推理（观察、描述、分析、评分）全面评估AI生成视频，尤其在高层次语义维度上。

## 2. 方法论：核心思想与关键细节

### 核心思想
- 提出 **GRADEO**（Generates Reasoning-based Assessments for Video Evaluation），通过指令微调多模态大语言模型（MLLM），使其学习人类评估过程——先进行多步推理（概述→描述→分析→评估），再给出可解释的分数。
- 区别于现有直接输出分数的方法，GRADEO模拟“慢思考”过程，提升准确性和可解释性。

### 关键技术细节
1. **评估维度**：定义7个维度，从低层感知到高层理解：
   - 质量（Quality）、美学（Aesthetic）、一致性（Consistency）、对齐（Alignment）、理性（Rationality）、安全（Safety）、创意（Creativity）。每个维度有细粒度关键方面（见表1）。
2. **数据集构建：GRADEO-Instruct**
   - 从WebVid、VidProM、VBench、EvalCrafter、SafeSora等收集prompt和生成视频（涉及10+开源/闭源模型，如OpenSora、VideoCrafter、Kling等），过滤动态性不足及含水印视频。
   - 5名人类标注者对每个样本按维度（1-5分）打分并撰写理由（要求50%以上一致且分差≤2，共16k标注）。
   - 使用GPT-4o将人类理由和分数转化为结构化的思维链（Chain-of-Thought, CoT）响应，包含四个标签：`<Overview>`、`<Description>`（或`<Prompt>`/`<Reasoning>`，针对对齐/理性维度）、`<Analysis>`、`<Assessment>`。最终得到3.3k视频的指令微调数据。
3. **模型训练与评估**
   - 基模型：**Qwen2-VL-7B**（具备视频理解能力）。
   - 微调方法：**LoRA**（低秩适配），以保留原有能力。
   - 损失函数：对答案（推理过程+最终分数）进行最大似然估计，如公式(1)所示。
   - 评估流程：输入视频（三帧关键帧）+维度指令+评估标准，输出四步推理及分数。

## 3. 实验设计：数据集、Benchmark与对比方法

### 数据集与场景
- **测试集**：从GRADEO-Instruct中抽取340个样本（每维度约49个），计算Spearman秩相关系数（SROCC）、Pearson线性相关系数（PLCC）、平均绝对误差（Δ̅）。
- **成对偏好数据集（Pairwise）**：
  - T2VQA-DB（10k视频，1000 prompts）
  - GenAI-Bench-Video（1.6k prompt，4个T2V模型）
  - TVGE（2.5k视频，5个模型，分quality和alignment）
  - 每个数据集随机采样200 prompt，每个prompt选两个视频（高分与低分），共1600个pair，评估模型选出高分视频的准确率。
- **Benchmark for T2V模型（GRADEO-BENCH）**：自行构造700个prompt（每维度100个），用于评测8个开源T2V模型（Hotshot-XL, Lavie, Latte, ModelScope, ZeroScope, VideoCrafter-1/2, Open-Sora）。

### 对比方法
- **自动指标**：PIQE、BRISQUE、CLIP-Score、ImageReward、HPS v2.1（仅用于成对数据集）。
- **图像MLLMs**：LLaVA-1.5/1.6-7B、GLM-4v、GPT-4-Turbo、GPT-4o。
- **视频MLLMs**：InternVL2.5-8B、LLaVA-NeXT-Video-7B、Qwen2-VL-7B、Gemini-1.5-Flash/Pro、VideoScore v1.1。
- **消融基线**：去除CoT各组件、仅输出分数、CNN基础模型（从零训练的视频打分模型）。

## 4. 资源与算力

- **训练模型**：基于Qwen2-VL-7B（7B参数），使用LoRA微调。
- **GPU配置**：4块RTX 3090（24G显存），训练10个epoch，学习率1×10⁻⁵，batch size每GPU 1，总batch size 4（gradient accumulation？原文未明确但推测如此）。
- **其他**：数据构建阶段使用GPT-4o生成CoT响应，推理阶段使用测试集和成对数据集时调用各MLLM的原生API（如GPT-4o、Gemini等），未提供具体算力需求。

## 5. 实验数量与充分性

- **主要实验（表2）**：在340样本测试集上对比10种方法（自动指标+多种MLLM）在7个维度上的SROCC/PLCC/Δ̅，每种方法计算三个指标，共7个维度，实验结果全面。
- **成对实验（表3）**：在4个数据集（T2VQA-DB、GenAI-Bench-Video、TVGE两子集）上对比6种MLLM+5种自动指标，共4×11=44组准确率数据。
- **消融实验（表4）**：5种设置（是否微调、是否含<Description>、<Overview>、全CoT、CNN基线），在每个维度上取平均ρ_srocc/ρ_plcc/Δ̅，共5组。
- **Benchmark（表5）**：8个T2V模型×7维度，共56个分数。
- **定性分析**：图4、5展示了Creativity和Rationality维度的示例输出对比。
- **充分性评估**：实验覆盖不同维度、不同模型、不同数据集，消融验证了CoT各组件的必要性。对比方法包括自动指标、开源/闭源MLLM（图像+视频），且在同一prompt/标准下比较（VideoScore除外，因原作者评分尺度不同做了映射）。实验设计客观公平，结论充分支撑论文主张。

## 6. 主要结论与发现

1. **GRADEO在所有维度上与人类评估的一致性显著优于现有方法**：在测试集上，GRADEO在7个维度的SROCC/PLCC均最高（例如质量维度SROCC 0.743 vs 最佳基线Gemini-1.5-Flash 0.617）。在成对数据集上，GRADEO准确率也最高（如T2VQA-DB上0.815 vs VideoScore 0.790）。
2. **多步推理（CoT）对提升性能关键**：消融表明，缺少<Description>或<Overview>均会显著降低表现；仅输出分数而不推理则会损失一致性。
3. **现有MLLM（即使GPT-4o、Gemini）在视频评估任务上表现不一致**：有些MLLM会拒绝回答或仅输出分数，缺乏可解释性；且在高层次维度（如理性、创意）上表现不稳定。
4. **T2V模型Benchmark结果**：当前模型在一致性维度得分较高（短时长不易失真），但在安全性、理性、创意上普遍较差；模型生成内容难以符合人类常识和复杂现实场景。
5. **指令遵循能力强的模型更易生成不安全内容**：强调需要加强安全对齐。

## 7. 优点：方法与实验设计的亮点

- **数据质量高**：人类标注通过严格一致性要求（50%以上一致、分差≤2），并利用GPT-4o将非结构化理由转化为结构化CoT，人工核验确保逻辑一致。
- **评估维度全面**：从低层感知（质量、美学）到高层语义（理性、安全、创意），填补了现有评估框架的空白。
- **可解释性强**：不仅输出分数，还输出完整的推理过程（Overview→Description→Analysis→Assessment），便于用户理解模型决策。
- **公平对比**：所有MLLM（除VideoScore因尺度问题）使用完全相同的prompt和评估标准；自动指标通过采样帧和映射到1-5分进行对齐。
- **实验充分**：包括测试集相关性、成对偏好准确性、消融、Benchmark、定性分析，多种指标和数据集交叉验证。
- **开源贡献**：计划公开数据集、模型和代码，促进社区研究。

## 8. 不足与局限

- **数据规模有限**：仅3.3k视频、16k标注，覆盖7个维度，可能不足以完全捕捉人类偏好的多样性；更多维度和更大规模标注可进一步提升。
- **标注者数量有限**：5名标注者可能存在偏差，未能充分代表多样人群（如不同文化背景对安全、创意的理解差异）。
- **CoT依赖GPT-4o生成**：存在引入GPT-4o自身偏差的风险；虽然人工验证了分数，但推理步骤可能不完全忠实于人类标注原因。
- **视频理解基模型局限**：基于Qwen2-VL-7B，该模型本身可能存在幻觉或错误描述，导致评估失败（如附录E所述）。
- **计算成本**：微调需要4×RTX 3090，而推理使用7B模型对资源有一定需求；但相比大型闭源MLLM仍较低。
- **应用限制**：仅评估单个视频维度（每维度一次评估），无法同时输出全部维度分数（需多次调用）；目前不支持实时评估。
- **实验覆盖**：未在更广泛的T2V模型（如Sora、Runway）上进行Benchmark（因闭源或无API），仅测试了8个较老的开源模型；成对数据集仅采样200 prompt，可能不足以代表全分布。

（完）
