---
title: "Stable Cinemetrics : Structured Taxonomy and Evaluation for Professional Video Generation"
title_zh: Stable Cinemetrics：专业视频生成的结构化分类与评估
authors: "Agneet Chatterjee, Rahim Entezari, Maksym Zhuravinskyi, Maksim Lapin, Reshinth Adithyan, Amit Raj, Chitta Baral, Yezhou Yang, Varun Jampani"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=JzOZkxa8Wd"
tags: ["query:vgen-metrics"]
score: 8.0
evidence: 视频生成的结构化评估框架
tldr: 该论文针对现有视频生成评估缺乏专业性的问题，提出了Stable Cinemetrics评估框架。该框架将电影制作控制分解为四个层次化分类（场景、事件、灯光、相机），定义76个细粒度控制节点，并构建了对应的基准测试和自动化评估管线。该工作为视频生成质量评估提供了系统化的指标和工具，直接匹配用户对视频生成评估指标的需求。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1439, \"height\": 753, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 734, \"height\": 431, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 703, \"height\": 660, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 703, \"height\": 369, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 702, \"height\": 283, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 709, \"height\": 535, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 698, \"height\": 350, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 694, \"height\": 348, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 730, \"height\": 412, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 723, \"height\": 320, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 697, \"height\": 353, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1310, \"height\": 425, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 705, \"height\": 356, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 702, \"height\": 398, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1437, \"height\": 701, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1441, \"height\": 966, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1441, \"height\": 671, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1230, \"height\": 485, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1360, \"height\": 711, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1440, \"height\": 694, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1436, \"height\": 692, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1228, \"height\": 482, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1441, \"height\": 1003, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1067, \"height\": 640, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1444, \"height\": 823, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1444, \"height\": 826, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1447, \"height\": 941, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1437, \"height\": 683, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1436, \"height\": 714, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 690, \"height\": 685, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 865, \"height\": 909, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 704, \"height\": 688, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 702, \"height\": 706, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 701, \"height\": 709, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-035.webp\", \"caption\": \"\", \"page\": 0, \"index\": 35, \"width\": 728, \"height\": 785, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-036.webp\", \"caption\": \"\", \"page\": 0, \"index\": 36, \"width\": 699, \"height\": 712, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-037.webp\", \"caption\": \"\", \"page\": 0, \"index\": 37, \"width\": 699, \"height\": 704, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-038.webp\", \"caption\": \"\", \"page\": 0, \"index\": 38, \"width\": 697, \"height\": 707, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-039.webp\", \"caption\": \"\", \"page\": 0, \"index\": 39, \"width\": 690, \"height\": 701, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-040.webp\", \"caption\": \"\", \"page\": 0, \"index\": 40, \"width\": 729, \"height\": 787, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-041.webp\", \"caption\": \"\", \"page\": 0, \"index\": 41, \"width\": 698, \"height\": 708, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-042.webp\", \"caption\": \"\", \"page\": 0, \"index\": 42, \"width\": 695, \"height\": 703, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-jzozkxa8wd/fig-043.webp\", \"caption\": \"\", \"page\": 0, \"index\": 43, \"width\": 1302, \"height\": 607, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1440, \"height\": 455, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 799, \"height\": 288, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1439, \"height\": 857, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1438, \"height\": 582, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1436, \"height\": 1936, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1438, \"height\": 783, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1444, \"height\": 708, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1432, \"height\": 358, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1448, \"height\": 1063, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1453, \"height\": 493, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1450, \"height\": 493, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1013, \"height\": 343, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-jzozkxa8wd/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1107, \"height\": 294, \"label\": \"Table\"}]"
motivation: 现有视频生成评估无法覆盖专业制作的复杂性，需要结构化评测框架。
method: 定义四层分类体系（场景、事件、灯光、相机），含76个控制节点，并构建自动评估管线。
result: 该框架能有效区分不同模型在专业控制上的表现。
conclusion: 提供了一个可复用的视频生成评估基准，对指标研究有直接贡献。
---

## Abstract
Recent advances in video generation have enabled high-fidelity video synthesis from user provided prompts. However, existing models and benchmarks fail to capture the complexity and requirements of professional video generation. Towards that goal, we introduce Stable Cinemetrics, a structured evaluation framework that formalizes filmmaking controls into four disentangled, hierarchical taxonomies: Setup, Event, Lighting, and Camera. Together, these taxonomies define 76 fine-grained control nodes grounded in industry practices. Using these taxonomies, we construct a benchmark of prompts aligned with professional use cases and develop an automated pipeline for prompt categorization and question generation, enabling independent evaluation of each control dimension. We conduct a large-scale human study spanning 10+ models and 20K videos, annotated by a pool of 80+ film professionals. Our analysis, both coarse and fine-grained reveal that even the strongest current models exhibit significant gaps, particularly in Events and Camera-related controls. To enable scalable evaluation, we train an automatic evaluator, a vision-language model aligned with expert annotations that outperforms existing zero-shot baselines. SCINE is the first approach to situate professional video generation within the landscape of video generative models, introducing taxonomies centered around cinematic controls and supporting them with structured evaluation pipelines and detailed analyses to guide future research.

---

## 论文详细总结（自动生成）

# Stable Cinemetrics：专业视频生成的结构化分类与评估——论文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）
- **研究动机**：现有视频生成模型（如文本到视频）在“业余”场景（如“宇航员骑马”）上已有不错效果，但**无法满足专业电影制作对精确控制的需求**——例如对镜头构图、灯光位置、角色动作时序等细节的精细调控。当前缺乏对“专业级视频生成”的明确定义和标准化评估协议。
- **核心问题**：当前视频生成模型是否已准备好用于专业电影制作？如何在生成视频中评估电影级别的控制能力？
- **整体含义**：论文旨在弥合生成式视觉与专业视频制作之间的鸿沟，通过构建结构化分类体系和评估套件，系统性地揭示当前模型的缺陷，并为未来研究提供可扩展的基准。

## 2. 论文提出的方法论：核心思想、关键技术细节
### 2.1 核心思想
- 将电影制作控制分解为四个**层次化、可解耦的分类体系**（Taxonomies），每个分类包含从粗粒度到细粒度的控制节点，共 **76 个细粒度控制节点**。
- 基于这些分类，构建**提示词基准**（SCINE Scripts 和 SCINE Visuals），自动分类提示词并生成**定向评估问题**，实现每个控制维度的独立评估。
- 训练**视觉-语言模型（VLM）自动评估器**，与人类专家标注对齐，替代昂贵的人工评估。

### 2.2 四个分类体系
| 分类 | 作用 | 示例细节点 |
|------|------|------------|
| **Setup（场景设置）** | 画面内所有可见元素：场景、主体、文字生成 | 纹理、几何、道具、服装、表情、时间、背景等 |
| **Events（事件）** | 镜头中的叙事内容：动作、情绪、对话 | 动作类型（独立/交互）、情绪显式/隐式、对话节奏 |
| **Lighting（灯光）** | 镜头中的照明控制：光源、色温、效果、位置 | 自然光/人工光、硬/软阴影、背光、颜色凝胶 |
| **Camera（相机）** | 镜头相关的所有参数：内部参数、外部参数、运动、创意意图 | 景深、焦距、镜头角度、运动轨迹、帧尺寸 |

### 2.3 关键技术细节
- **提示词生成**：
  - **SCINE-Scripts**：基于专业编剧的种子提示词和 Events 分类节点，使用 LLM 生成叙事性提示词（单镜头、<10秒）。
  - **SCINE-Visuals**：在 SCINE-Scripts 基础上，通过采样 Camera/Lighting/Setup 分类节点，注入视觉设置，模拟“从剧本到镜头”的过程。
  - 提示词自动分类：将提示词中的每个控制元素映射回分类树，并生成对应的评估问题（例如：“视频中是否使用了浅景深？”）。
- **自动评估器**：
  - 基于 Qwen2.5-VL-7B 微调，使用 Bradley-Terry 目标函数进行偏好学习。
  - 输入：单视频 + 相应提示词 + 评估问题；输出：1-5 分标量评分。
  - 训练数据：44,062 样本（训练），12,763 样本（验证），batch size 8，学习率 6e-5，训练 1 epoch。

## 3. 实验设计
- **基准（Benchmark）**：
  - **SCINE 基准** 包含 2,089 个提示词，分为：
    - SCINE-Scripts（事件叙事，1,133 个提示词，平均 2.57 个问题/提示词）
    - SCINE-Visuals（视觉风格，按角色分为 Cinematographer、Production Designer、Director，共 956 个提示词，平均 4-10 个问题/提示词）
  - 提示词多样性：通过 Plutchik 情绪模型、不同动作/对话结构、类型等保证多样性；t-SNE 可视化显示与真实剧本高度重叠。
- **对比方法**：
  - **13 个 T2V 模型**：开源（WAN 14B/1B, HunyuanVideo, StepVideo, CogVideoX 5B, LTX-Video, Pyramid Flow, Easy Animate 5.1, Mochi, VChitect-2.0）和闭源（Minimax, Luma Ray 2, Pika 2.2）。
  - **自动评估基线**：零样本 VLM（Qwen2.5-VL 7B/32B/72B, Gemini-2.0-Flash, Gemini-2.5-Pro）。
- **人类标注**：84 名电影专业人士（平均 6.5 年经验），对每对视频-问题收集 3 个评分（1-5 分），共 248,536 个标注。
- **评估指标**：
  - 人类评估：1-5 评分，聚合后计算模型平均分；通过 Wilcoxon 符号秩检验判断模型间显著性。
  - 自动评估：人类偏好准确率（VLM 选出的更高分视频与人类一致的比例）。

## 4. 资源与算力
- 文中 **未明确说明** 用于训练自动评估 VLM 或生成视频的具体 GPU 型号、数量及总耗时。
- 仅提及训练 VLM 使用 1 epoch，batch size 8，学习率 6e-5，未提供更多硬件细节。
- 提示词生成和视频生成使用 LLM 和现有模型，但未提供计算开销。

## 5. 实验数量与充分性
- **实验组数**：非常充分。
  - 对 13 个模型在 2,089 个提示词上生成视频（约 20K 视频）。
  - 人类标注覆盖 13,457 个独特问题，每个问题 3 次评分。
  - 统计检验：对 45 个模型对进行 Wilcoxon 检验，其中 37 对有显著差异；ICC 组内相关系数达 80.4%（模型对级别）和 95.5%（单模型级别）。
  - 消融分析：按分类（四大支柱）、事件子类型（动作/情绪/对话）、灯光子节点、相机角度、提示难度（基本/高级）、角色（导演/摄影师/设计师）等维度进行了细粒度对比。
- **充分性**：实验设计全面，覆盖了多种模型、多种控制维度、多种提示难度，并使用严格的统计检验确保结果可靠性。但只使用英文提示词，未评估其他语言或跨文化差异。

## 6. 论文的主要结论与发现
1. **模型整体表现**：WAN-14B 和 Minimax 是当前最强的模型，但所有模型在专业控制方面均有显著不足。
2. **最难控制的维度**：**Events（事件）** 和 **Camera（相机）** 表现最差；**Setup（场景设置）** 和 **Lighting（灯光）** 相对较好。
3. **具体薄弱环节**：
   - 事件：互动动作、显式情绪、多轮对话、因果/重叠/循环事件处理困难。
   - 相机：外部参数（角度）和运动轨迹（3D 运动）表现最弱；景深、帧大小等也有差距。
   - 灯光：灯光位置（背光等）是主要瓶颈；硬阴影、颜色凝胶等高级控制困难。
   - 场景设置：主体个性、化妆、环境风格等表现差；但头发、配件、背景整体较好。
4. **自动评估**：微调后的 7B VLM 达到 72.36% 准确率，优于所有零样本 VLM（包括 72B 模型和 Gemini-2.5-Pro），且在不同模型生成视频上表现稳定。
5. **专业角色差异**：当所有控制维度同时指定（导演角色）时，模型性能普遍下降，进一步凸显多维度控制挑战。

## 7. 优点
- **结构化分类体系**：基于电影制作实践，层次化、可扩展，支持多级抽象评估（粗粒度到细粒度），易于添加新节点。
- **细粒度评估**：通过自动生成每个控制节点的独立问题，实现了真正解耦的评估，而非仅高层面提示词匹配。
- **大规模人类标注**：超过 80 名专业人士、20K 视频、248K 标注，保证了评估的可靠性和专业性。
- **自动评估对齐**：训练的 VLM 在有限数据下显著优于零样本基线，提供了可扩展的评估方案。
- **提示词设计**：结合叙事脚本和视觉注入，更贴近真实电影制作流程，比现有基准（如 VBench）更具专业真实性。
- **公开性**：作者承诺公开分类体系和评估工具，有利于社区复现和扩展。

## 8. 不足与局限
- **专家网络有限**：分类体系受限于合作专家群体的地域和经验范围，可能未覆盖全球电影制作惯例。
- **节点抽象化**：一些细粒度值（如具体 ISO 800 或 2000K 色温）被抽象为“低/中/高”等类别，可能丢失精确性。
- **LLM 偏差**：提示词生成依赖 LLM，其训练数据可能存在语言或文化偏差，影响提示词的代表性。
- **零样本 VLM 实验局限**：受限于计算资源，未探索更大规模模型或更多训练样本对自动评估器性能的影响。
- **未披露算力细节**：缺少训练和推理阶段的具体 GPU 型号、数量、时长等，影响可复现性。
- **单镜头限制**：评估仅针对单镜头（<10秒），未覆盖多镜头叙事或长视频控制。
- **仅文本输入**：论文仅评估文本到视频，未覆盖图像到视频等模态，也未考虑音频同步（对话输出无声音）。
- **性别/种族偏差**：未分析模型在不同主体性别、种族、文化背景上的表现差异，可能存在偏见风险。

---

（完）
