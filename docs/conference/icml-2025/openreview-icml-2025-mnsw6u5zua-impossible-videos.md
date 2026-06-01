---
title: Impossible Videos
title_zh: 不可能视频
authors: "Zechen Bai, Hai Ci, Mike Zheng Shou"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=MNSW6U5zUA"
tags: ["query:vgen-metrics"]
score: 6.0
evidence: 视频生成评估基准
tldr: 针对当前视频生成模型遵循提示生成超现实内容的能力以及视频理解模型识别超现实内容的能力，提出了IPV-Bench基准。该基准包含4个领域14个类别，评估生成视频在物理、生物、地理和社会规则违反方面的质量，为视频生成评估提供了新维度。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1112, \"height\": 1389, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1702, \"height\": 508, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 772, \"height\": 693, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 749, \"height\": 623, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 784, \"height\": 757, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 773, \"height\": 425, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 769, \"height\": 744, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1604, \"height\": 1061, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1753, \"height\": 455, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1143, \"height\": 175, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1145, \"height\": 219, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1372, \"height\": 204, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1368, \"height\": 203, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1369, \"height\": 204, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1367, \"height\": 204, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1373, \"height\": 201, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1367, \"height\": 204, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1369, \"height\": 192, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1361, \"height\": 205, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1366, \"height\": 201, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1374, \"height\": 205, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1373, \"height\": 206, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1381, \"height\": 204, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1378, \"height\": 205, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1380, \"height\": 208, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1380, \"height\": 205, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1376, \"height\": 206, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-028.webp\", \"caption\": \"\", \"page\": 0, \"index\": 28, \"width\": 1382, \"height\": 206, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-029.webp\", \"caption\": \"\", \"page\": 0, \"index\": 29, \"width\": 1657, \"height\": 242, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-030.webp\", \"caption\": \"\", \"page\": 0, \"index\": 30, \"width\": 1651, \"height\": 242, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-031.webp\", \"caption\": \"\", \"page\": 0, \"index\": 31, \"width\": 1643, \"height\": 249, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-032.webp\", \"caption\": \"\", \"page\": 0, \"index\": 32, \"width\": 1654, \"height\": 245, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-033.webp\", \"caption\": \"\", \"page\": 0, \"index\": 33, \"width\": 1654, \"height\": 244, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-mnsw6u5zua/fig-034.webp\", \"caption\": \"\", \"page\": 0, \"index\": 34, \"width\": 1649, \"height\": 244, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-mnsw6u5zua/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1721, \"height\": 492, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-mnsw6u5zua/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1601, \"height\": 502, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-mnsw6u5zua/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1595, \"height\": 551, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-mnsw6u5zua/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 737, \"height\": 482, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-mnsw6u5zua/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1415, \"height\": 393, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-mnsw6u5zua/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 814, \"height\": 239, \"label\": \"Table\"}]"
motivation: 探索视频生成模型能否生成并理解反现实视频概念。
method: 构建基于分类学的IPV-Bench基准，涵盖4领域14类别异常场景。
result: 基准能有效区分不同视频生成和理解的性能差异。
conclusion: 为视频生成评估提供了覆盖超现实内容的补充基准。
---

## Abstract
Synthetic videos nowadays is widely used to complement data scarcity and diversity of real-world videos.
Current synthetic datasets primarily replicate real-world scenarios, leaving impossible, counterfactual and anti-reality video concepts underexplored. This work aims to answer two questions: 1) Can today's video generation models effectively follow prompts to create impossible video content? 2) Are today's video understanding models good enough for understanding impossible videos?
To this end, we introduce *IPV-Bench*, a novel benchmark designed to evaluate and foster progress in video understanding and generation. *IPV-Bench* is underpinned by a comprehensive taxonomy, encompassing 4 domains, 14 categories.
It features diverse scenes that defy physical, biological, geographical, or social laws. Based on the taxonomy, a prompt suite is constructed to evaluate video generation models, challenging their prompt following and creativity capabilities. In addition, a video benchmark is curated to assess Video-LLMs on their ability of understanding impossible videos, which particularly requires reasoning on temporal dynamics and world knowledge. Comprehensive evaluations reveal limitations and insights for future directions of video models, paving the way for next-generation video models.

---

## 论文详细总结（自动生成）

### 1. 论文的核心问题与整体含义（研究动机和背景）

- **研究动机**：当前合成视频数据集主要用于复制真实世界场景，但忽略了**不可能、反事实和反现实（impossible, counterfactual, anti-reality）** 的视频概念。这类内容在电影、广告等创意领域有重要应用价值，同时能测试模型的**泛化和推理能力**（而非简单记忆真实数据）。
- **核心问题**：
  1. 现有视频生成模型能否有效遵循文本提示生成不可能视频？
  2. 现有视频理解模型（特别是 Video-LLM）能否准确理解不可能视频中的异常？
- **背景**：现有基准（如 VBench、VideoPhy、TempCompass 等）多侧重真实世界视频或物理合理性评估，缺乏对反物理、反常识内容的系统评测。

### 2. 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：构建一个结构化分类体系（Taxonomy），覆盖物理、生物、地理、社会四大领域的 14 个子类别，以此为基础构建**提示套件（IPV-Txt）** 和**视频数据集（IPV-Vid）**，分别用于评估视频生成和理解模型。
- **关键技术细节**：
  - **IPV-Txt**：包含 260 个高质量文本提示，描述反事实场景（如“牛奶倒入半满杯子，水位不变”）。通过 LLM、众包、人工审核、语言增强等迭代生成。
  - **IPV-Vid**：包含 902 个高质量视频（来自 10 个 T2V 模型生成、网络收集和真实视频检索），经人工筛选和标注（空间/时间异常、分类、解释）。
  - **评估任务**：
    - 生成评估：使用 **IPV-Score**（视觉质量 × 提示遵循），由人工标注。
    - 理解评估：三个层级任务——**判断任务**（AI 生成判断）、**多选问答（MCQA）**（识别正确异常描述，使用 GPT-4o 生成干扰项）、**开放式问答（OpenQA）**（自由解释异常，用 LLM 评估者打分，采用“理由-评分”两步法避免不稳定）。
  - **自动评估替代**：针对生成，提出自动策略：VBench 子指标组合计算视觉质量，GPT-4o + 三步推理链评估提示遵循。

### 3. 实验设计：数据集 / 场景、Benchmark 与对比方法

- **生成评估**：
  - 数据集：IPV-Txt (260 prompts)
  - 对比模型：开源（LTX, Open-Sora, Pyramid-Flow, CogVidX-1.5, Mochi 1, HunyuanVideo）和闭源（Luma, Sora, Kling, Hailuo）共 10 个。
  - 指标：视觉质量、提示遵循、IPV-Score。
- **理解评估**：
  - 数据集：IPV-Vid (902 个视频，含合成/真实各 50%)
  - 对比模型：开源（Video-LLaVA, Oryx, Intern-VL-2.5, NVILA, LongVU, Qwen2-VL, LLaVA-Next）和闭源（Gemini-1.5-Flash, GPT-4o）。
  - 任务与指标：判断（Accuracy, F1）、MCQA（Accuracy）、OpenQA（LLM 打分 0-1）。
  - 额外分析：按领域（Physical, Biological, Social, Geographical）和异常类型（空间/时间）拆分结果。

### 4. 资源与算力

- **文中未明确说明**训练或推理所用的 GPU 型号、数量、时长等具体算力信息。仅在数据集构建中提到使用 10 个 T2V 模型生成视频，但未给出生成成本。
- 理解模型评估中，GPT-4o 使用 1 FPS 采样，但仍未提及推理资源。
- **需指出**：论文未提供算力细节，这在复现和能耗分析上存在不足。

### 5. 实验数量与充分性

- **数量**：
  - 生成：10 个模型 × 260 prompts = 2600 个生成视频，经人工筛选保留，最终用于评估。
  - 理解：9 个视频理解模型在 3 个任务上评测，报告了各领域、空间/时间拆分的子结果。
  - 额外：自动评估与人工评分的一致性分析（Spearman ρ > 0.8），人类基线（MCQA 94%, OpenQA 82.7%）。
- **充分性与公平性**：
  - 覆盖了主流开源/闭源模型，类别全面。
  - 理解任务中，OpenQA 使用独立评估者 Claude 3.5 避免 GPT-4o 自评偏差；MCQA 干扰项设计禁止简单视觉匹配。
  - 限制：生成评估依赖人工标注（可能主观），OpenQA 打分虽有两步法但仍受 LLM 偏好影响；未见跨数据集迁移或更多消融（如不同分辨率、帧率影响）。

### 6. 论文的主要结论与发现

- **生成方面**：当前最佳模型（Mochi 1）的 IPV-Score 仅 **37.3%**，视觉质量与提示遵循严重不平衡（如 Luma 质量高但遵循差，Mochi 1 反之）。失败原因：反事实提示导致视觉伪影（out-of-distribution），或模型过度遵守物理定律而忽略异常。
- **理解方面**：
  - 判断任务：Qwen2-VL 准确率最高（76.2%），但部分模型存在严重偏见（如 Intern-VL 93.5% 答“Yes”）。
  - MCQA：LLaVA-Next 最佳（86.4%），但多数开源模型接近随机；物理领域最难。
  - OpenQA：GPT-4o 最高（49.1%），仍远低于人类（82.7%）。时间异常理解普遍更差。
- 关键挑战：**时间动态推理** 与 **世界知识推理**；当前模型更擅长空间异常检测。

### 7. 优点：方法或实验设计上的亮点

- **首创性**：首次系统提出并定义“不可能视频”概念，构建结构化分类体系（4 领域 14 子类），为反事实视频理解与生成提供标准化测试平台。
- **多层次任务设计**：从判别到多选再到自由解释，难度递增，能细粒度诊断模型能力。
- **数据质量保证**：
  - 众包 + LLM + 人工审查的提示迭代。
  - 视频筛选（视觉质量 + 语义异常）和详细标注（空间/时间、分类、解释）。
  - 加入真实视频平衡评估偏差。
- **评估严谨性**：OpenQA 采用“理由-评分”两步法，并使用独立评估者（Claude）避免自评估偏差；自动生成评估策略与人类标注 Spearman ρ > 0.8。

### 8. 不足与局限

- **实验覆盖**：
  - 生成评估仅基于 260 个提示，可能未覆盖所有不可能类型（如更复杂的因果违反）。
  - 理解模型仅评估 902 个视频，样本量有限，可能遗漏长尾异常场景。
- **偏差风险**：
  - 人工标注主观性，尤其 OpenQA 打分依赖 LLM，虽用 Claude 仍可能受语言风格影响。
  - MCQA 干扰项由 GPT-4o 生成，可能隐含自身偏好，影响公平性。
- **应用限制**：
  - 基准主要面向科研，直接用于工业部署需考虑成本（生成大量视频）和泛化性（仅覆盖英文提示）。
  - 未探讨模型在**零样本** vs **少样本** 下的表现，也未分析不同帧率/分辨率的影响。
- **算力缺失**：未提供训练/推理资源消耗，不利于社区复现和能耗评估。

（完）
