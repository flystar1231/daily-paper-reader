---
title: "WorldSimBench: Towards Video Generation Models as World Simulators"
title_zh: WorldSimBench：迈向将视频生成模型作为世界模拟器的评估
authors: "Yiran Qin, Zhelun Shi, Jiwen Yu, Xijun Wang, Enshen Zhou, Lijun Li, Zhenfei Yin, Xihui Liu, Lu Sheng, Jing Shao, LEI BAI, Ruimao Zhang"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=j9pVnmulQm"
tags: ["query:vgen-metrics"]
score: 6.0
evidence: 世界模拟器视频生成模型的双重评估框架
tldr: 现有基准无法有效评估高能力具身预测模型。本文提出WorldSimBench双重评估框架，包括显式感知评估和隐式操作评估，结合人类偏好评估，为视频生成模型作为世界模拟器提供系统评价方法。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1757, \"height\": 584, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1770, \"height\": 826, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1738, \"height\": 605, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1585, \"height\": 509, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1576, \"height\": 777, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1773, \"height\": 902, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1766, \"height\": 869, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1766, \"height\": 1008, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-j9pvnmulqm/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1769, \"height\": 750, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1646, \"height\": 366, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1770, \"height\": 448, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1775, \"height\": 223, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1769, \"height\": 228, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1139, \"height\": 185, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1771, \"height\": 160, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1195, \"height\": 1015, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1076, \"height\": 401, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 996, \"height\": 402, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1139, \"height\": 401, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 502, \"height\": 480, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1777, \"height\": 474, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1333, \"height\": 232, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1057, \"height\": 252, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-j9pvnmulqm/table-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1056, \"height\": 339, \"label\": \"Table\"}]"
motivation: 缺乏对视频生成模型作为世界模拟器的层次化评估方法。
method: 提出包含显式感知和隐式操作的双重评估框架。
result: 框架能有效区分不同模型的世界模拟能力。
conclusion: 为视频生成模型的具身评估提供新基准。
---

## Abstract
Recent advancements in predictive models have demonstrated exceptional capabilities in predicting the future state of objects and scenes. However, the lack of categorization based on inherent characteristics continues to hinder the progress of predictive model development. Additionally, existing benchmarks are unable to effectively evaluate higher-capability, highly embodied predictive models from an embodied perspective. In this work, we classify the functionalities of predictive models into a hierarchy and take the first step in evaluating World Simulators by proposing a dual evaluation framework called WorldSimBench. WorldSimBench includes Explicit Perceptual Evaluation and Implicit Manipulative Evaluation, encompassing human preference assessments from the visual perspective and action-level evaluations in embodied tasks, covering three representative embodied scenarios: Open-Ended Embodied Environment, Autonomous, Driving, and Robot Manipulation. In the Explicit Perceptual Evaluation, we introduce the HF-Embodied Dataset, a video assessment dataset based on fine-grained human feedback, which we use to train a Human Preference Evaluator that aligns with human perception and explicitly assesses the visual fidelity of World Simulater. In the Implicit Manipulative Evaluation, we assess the video-action consistency of World Simulators by evaluating whether the generated situation-aware video can be accurately translated into the correct control signals in dynamic environments. Our comprehensive evaluation offers key insights that can drive further innovation in video generation models, positioning World Simulators as a pivotal advancement toward embodied artificial intelligence.

---

## 论文详细总结（自动生成）

# 论文详细总结：WorldSimBench: Towards Video Generation Models as World Simulators

## 1. 核心问题与整体含义（研究动机和背景）

- **核心问题**：现有预测模型缺乏基于固有特性的层次化分类，且已有基准无法有效从具身视角评估高能力、高度具身的预测模型（特别是世界模拟器）。视频生成模型能否作为世界模拟器，在物理规则、动作可行性等方面尚未有系统评估方法。
- **整体含义**：该论文提出首个针对世界模拟器的双重评估框架WorldSimBench，旨在推动视频生成模型向具身人工智能发展，为后续模型改进提供标准化评价手段。

## 2. 方法论

### 核心思想
将预测模型的功能划分为四个层次（S0-S3：文本→图像→视频→可执行视频），并首次对S3级世界模拟器进行双视角评估：**显式感知评估**（基于人类偏好的视觉质量评价）和**隐式操作评估**（闭环比对，通过视频到动作的转换效果评价）。

### 关键技术细节
- **显式感知评估**：
  - 构建层次化评估维度（视觉质量、条件一致性、具身属性），针对三个场景定制（OE、AD、RM）。
  - 基于互联网视频和LLM扩展生成指令提示列表。
  - 使用多种视频生成模型生成大量视频，进行细粒度人工标注，构建**HF-Embodied数据集**（35,701个元组，多维度评分+理由）。
  - 基于Flash-VStream（VideoLLM）训练**人类偏好评估器**（仅LoRA参数），输入视频+提示，输出多维度得分。

- **隐式操作评估**：
  - 针对三个场景分别部署模拟环境（MineRL、CARLA、CALVIN）。
  - 训练视频到动作模型（逆动力学或基于目标的策略）：OE用Steve-1，AD用LMdrive，RM用Susie。
  - 闭环流程：世界模拟器基于当前观察和指令实时生成预测视频 → 视频-动作模型转换为控制信号 → 在模拟环境中执行并评估任务成功率。
  - 评估指标：OE用旅行距离、物品收集量等；AD用路线完成率、违章分数等；RM用任务链平均完成长度。

### 算法流程（文字说明）
1. 分类预测模型为S0–S3。
2. 对S3世界模拟器：
   - 显式：生成指令视频 → 人类偏好评估器打分（平均各维度）。
   - 隐式：构建闭环环境 → 实时生成视频 → 视频-动作模型 → 执行并统计任务表现。

## 3. 实验设计

### 数据集/场景
- **开放式具身环境（OE）**：Minecraft，使用VPT数据集和自制探索轨迹，任务包括收集木材/泥土/种子、探索、挖掘。
- **自动驾驶（AD）**：CARLA模拟器，nuScenes训练集，LangAuto-Tiny基准（短路线），指令如“左转”、“直行”。
- **机器人操作（RM）**：CALVIN基准，训练环境A/B/C，测试环境D，任务链含5个子任务（如“按下按钮打开LED”）。

### Benchmark
- 显式：自定义层次化维度（见表2），每个维度5条指令，每个模型生成5个视频。
- 隐式：OE用5个任务×10个种子；AD用8个标准指标；RM用20/100条轨迹的任务完成率。

### 对比方法
8个流行视频生成模型：Open-Sora-Plan（T2V和TI2V）、Lavie、ModelScope、OpenSora、AnimateDiff、DynamicCrafter、EasyAnimate。所有模型均在对应场景数据集上微调。

## 4. 资源与算力

- 论文明确提及：**人类偏好评估器**训练使用4张A100 80GB GPU，训练4个epoch，学习率2e-5，warmup比率0.03，LoRA设置与Flash-VStream一致。
- 其他视频生成模型的微调算力未详细说明，但提到遵循官方实现设置，训练短视频（~16帧）和长视频（~60帧）。总体算力描述不充分，仅部分可量化。

## 5. 实验数量与充分性

- **显式评估**：三个场景共约21个维度×5个指令×5个视频，每个模型每场景得到平均得分，结果呈现在表8-10。还比较了人类偏好评估器与GPT-4o的零样本/微调性能（表3/7）。
- **隐式评估**：OE：5任务×10 trials（表12）；AD：8指标（表13）；RM：20 trials（表14）和100 trials（表15）均有报告。还进行了定性样例分析（图7-10）。
- **消融/泛化实验**：零样本跨模型评估（如OpenSora、Lavie）验证人类偏好评估器泛化性；对比UniPi（表15）显示优势。
- **充分性**：实验覆盖三个关键具身场景，对比了多个主流模型，有定量和定性分析，但缺少对更多模型（如Sora闭源）的比较，且仅测试了文本/图像条件，未探索其他条件形式。整体较为充分，公平性方面：显式评估使用统一人类偏好评估器，隐式评估使用统一视频-动作模型，避免了模型自带的策略差异。

## 6. 主要结论与发现

- **当前视频生成模型仍无法有效模拟物理规则**，在具身交互、轨迹合理性、指令对齐等方面存在显著不足，距离成为真正的世界模拟器还有很大差距。
- **显式与隐式评估结果基本一致**：在轨迹生成好的模型（如DynamicCrafter）在AD和RM隐式评估中也表现好，但在高频交互任务（如OE长序列）中Open-Sora-Plan更鲁棒。
- **关键瓶颈**：OE中交互合理性差；AD中3D深度感和行人/车辆渲染质量差；RM中指令对齐最弱，模型常生成无目的动作。
- **人类偏好评估器**比GPT-4o更贴近人类判断，尤其在零样本设置下表现稳定。
- **建议**：未来应结合两种评估视角全面评价世界模拟器。

## 7. 优点

- **首次提出面向世界模拟器的层次化分类和系统评估**，填补了S3级模型评估空白。
- **双重评估框架**：兼顾视觉质量与动作可行性，更全面反映模型在具身任务中的真实能力。
- **构建了大规模细粒度人类反馈数据集**（HF-Embodied，35K+元组，20个维度），不仅可用于评估，还可用于模型对齐（如DPO训练提升效果）。
- **闭环交互评估**避免了静态评价的局限，更贴近实际应用。
- **实验设计规范**：多场景、多模型、多任务，消融和泛化验证充分。

## 8. 不足与局限

- **场景覆盖有限**：仅包含三个场景（Minecraft、自动驾驶、机器人操作），更多具身场景（如家庭服务、医疗）未涉及，物理规则表示也需扩展。
- **人类偏好评估器**可能受HF-Embodied数据集分布偏差影响（如模型生成视频质量分布不均），且训练仅用了LoRA，可能未充分利用大模型潜力。
- **隐式评估依赖视频-动作模型质量**：如果视频-动作模型本身不够鲁棒，会影响对世界模拟器的公平评价。
- **未比较闭源顶级模型**（如Sora、Genie），结果仅代表开源模型水平。
- **算力消耗未全面报告**，部分模型微调细节（如训练步数、批量大小）缺失，使复现成本不明确。
- **评估指令主要依赖LLM扩展+人工筛选**，可能引入语义偏差或覆盖不足。

（完）
