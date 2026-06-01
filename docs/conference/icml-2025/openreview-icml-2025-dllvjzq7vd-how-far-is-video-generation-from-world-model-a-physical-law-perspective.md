---
title: "How Far Is Video Generation from World Model: A Physical Law Perspective"
title_zh: 视频生成离世界模型有多远：一个物理定律视角
authors: "Bingyi Kang, Yang Yue, Rui Lu, Zhijie Lin, Yang Zhao, Kaixin Wang, Gao Huang, Jiashi Feng"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=DLlVjZQ7vD"
tags: ["query:vgen-metrics"]
score: 6.0
evidence: 视频生成模型物理定律遵循评估
tldr: 视频生成模型是否真正学习了物理定律尚存疑问。本文在分布内、分布外和组合泛化三种场景下，利用2D物理仿真测试集评估扩散视频生成模型，揭示模型在物理规律遵循上的局限，为评估生成质量提供新视角。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1401, \"height\": 375, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 739, \"height\": 485, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1729, \"height\": 450, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 705, \"height\": 653, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 470, \"height\": 501, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1775, \"height\": 422, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 869, \"height\": 219, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 843, \"height\": 399, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 852, \"height\": 478, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 855, \"height\": 187, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1561, \"height\": 1050, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1409, \"height\": 576, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1138, \"height\": 585, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1737, \"height\": 521, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1430, \"height\": 610, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1356, \"height\": 512, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 772, \"height\": 1045, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1075, \"height\": 654, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 1047, \"height\": 1075, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1046, \"height\": 1077, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-021.webp\", \"caption\": \"\", \"page\": 0, \"index\": 21, \"width\": 1762, \"height\": 793, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-022.webp\", \"caption\": \"\", \"page\": 0, \"index\": 22, \"width\": 1495, \"height\": 2120, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-023.webp\", \"caption\": \"\", \"page\": 0, \"index\": 23, \"width\": 1646, \"height\": 576, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-024.webp\", \"caption\": \"\", \"page\": 0, \"index\": 24, \"width\": 1683, \"height\": 582, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-025.webp\", \"caption\": \"\", \"page\": 0, \"index\": 25, \"width\": 1684, \"height\": 550, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-026.webp\", \"caption\": \"\", \"page\": 0, \"index\": 26, \"width\": 1683, \"height\": 557, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-dllvjzq7vd/fig-027.webp\", \"caption\": \"\", \"page\": 0, \"index\": 27, \"width\": 1680, \"height\": 551, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-dllvjzq7vd/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 652, \"height\": 207, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dllvjzq7vd/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1397, \"height\": 260, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dllvjzq7vd/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1026, \"height\": 207, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-dllvjzq7vd/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 788, \"height\": 242, \"label\": \"Table\"}]"
motivation: 探究视频生成模型能否从视觉数据中发现并遵循物理定律。
method: 构建2D物理仿真测试集，评估模型在三种泛化场景下的表现。
result: 模型在分布外和组合泛化场景下表现不佳。
conclusion: 表明当前视频生成模型尚未真正掌握底层物理规律。
---

## Abstract
Scaling video generation models is believed to be promising in building world models that adhere to fundamental physical laws. However, whether these models can discover physical laws purely from vision can be questioned. 
A world model learning the true law should give predictions robust to nuances and correctly extrapolate on unseen scenarios.
In this work, we evaluate across three key scenarios: in-distribution, out-of-distribution, and combinatorial generalization.
We developed a 2D simulation testbed for object movement and collisions to generate videos deterministically governed by one or more classical mechanics laws.
We focus on the scaling behavior of training
diffusion-based video generation models to predict object movements based on initial frames.
Our scaling experiments show perfect generalization within the distribution, measurable scaling behavior for combinatorial generalization, but failure in out-of-distribution scenarios.
Further experiments reveal two key insights about the generalization mechanisms of these models: (1) the models fail to abstract general physical rules and instead exhibit "case-based" generalization behavior, i.e., mimicking the closest training example; (2) when generalizing to new cases, models are observed to prioritize different factors when referencing training data: color $>$ size $>$ velocity $>$ shape.
Our study suggests that scaling alone is insufficient for video generation models to uncover fundamental physical laws.

---

## 论文详细总结（自动生成）

### 论文核心问题与整体含义（研究动机和背景）

- **研究动机**：视频生成模型（如Sora）被视作构建世界模型（world model）的潜在途径，但尚不清楚这些模型能否从纯视觉观察中真正发现并遵循物理定律。真正的世界模型应当能够稳健预测并外推到未见场景，而不仅仅是记忆训练数据。
- **背景**：现有研究倾向于通过缩放数据和模型规模来提升视频生成效果，但缺乏对模型是否掌握底层物理规律的严谨评估。本文从物理定律的角度，系统考察视频生成模型的泛化能力。

### 论文提出的方法论：核心思想、关键技术细节

- **核心思想**：设计一个2D物理仿真测试台，生成由经典力学定律（如惯性定律、动量守恒、牛顿第二定律）严格控制的确定性视频。训练扩散视频生成模型，以初始几帧为条件预测后续帧，并评估其在不同泛化场景下的表现。
- **关键技术细节**：
  - **视频生成模型**：采用VAE（(2+1)D-VAE压缩视频为潜空间）+ DiT（Diffusion Transformer）架构，遵循Sora的设计。VAE预训练后固定，只训练扩散模型。
  - **条件机制**：以前若干帧（例如1或3帧）作为输入，通过零填充和二进制掩码标记条件帧。
  - **物理定律验证**：定义三种泛化场景：
    - **分布内（ID）**：训练与测试数据同分布。
    - **分布外（OOD）**：测试数据中潜在参数（如速度、半径）超出训练范围。
    - **组合泛化（combinatorial）**：训练中见过单个概念，但测试需组合未见过的概念。
  - **评估指标**：对于简单场景（ID/OOD），通过像素解析物体位置和速度，计算速度误差；对于复杂组合场景，使用FVD、SSIM、PSNR、LPIPS以及人工标注的“异常比例”（违反物理规律）。
- **公式与算法**：物理过程由微分方程 \(\dot{z}=F(z)\) 描述，渲染函数 \(R(\cdot)\) 将潜状态映射为图像。训练目标为最大化条件对数似然 \(\log p_\theta(I_{c+1},...,I_L | I_1,...,I_c)\)。

### 实验设计：数据集/场景、基准、对比方法

- **数据集与场景**：
  - **ID/OOD实验**：三个基本物理场景：
    1. **匀速直线运动**（惯性定律）。
    2. **完全弹性碰撞**（能量与动量守恒）。
    3. **抛物线运动**（牛顿第二定律）。
    每个场景包含2-4个自由度（如速度、质量、半径），训练数据规模为30K/300K/3M，测试数据分为ID和OOD（参数范围外）。
  - **组合泛化实验**：基于PHYRE模拟器，包含8种物体类型（球、罐、杆、墙等），每次选取4种物体生成视频，共70种组合（\(C_8^4\)）。使用60种组合训练，10种测试。训练数据量：600K/3M/6M。
- **基准（Baseline）**：对比由模拟器生成的地面真值视频解析得到的速度误差（即系统最小误差），以及不同模型尺寸（DiT-S/B/L/XL，参数量22M~456M）。
- **对比方法**：主要对比自身不同规模模型，也尝试了Stable Video Diffusion（SVD）微调，以及条件输入中加入数值和文本的多模态变体。

### 资源与算力

- 论文中明确说明：所有实验使用Nvidia A100 GPU。
  - ID/OOD实验：32块A100，批量大小256，训练100K步（已收敛）。
  - 组合实验：64块A100，批量大小256，训练1000K步。
- 未提及具体训练总时长，但指出更高分辨率（256×256 vs 128×128）会显著减慢训练。

### 实验数量与充分性

- **数量**：进行了多组系统实验，包括：
  - 3种物理场景 × 3种数据规模 × 3种模型尺寸（部分场景还有DiT-XL）的ID/OOD对比。
  - 组合泛化中，3种模板数量（6/30/60） × 2种模型尺寸（DiT-B/XL），并进行了人工评估。
  - 额外的消融实验：缺失速度范围的训练、属性优先级（颜色/大小/速度/形状）的成对比较6组、空间/时间组合分析、多模态条件对比等。
- **充分性与公平性**：
  - ID/OOD实验覆盖了不同参数组合，OOD测试包含6种类型，结论一致。
  - 组合泛化实验通过控制模板数量排除数据量混淆，人工评估有10名标注员。
  - 实验设计较为全面，结论稳健。但未在真实复杂视频上验证，仅限于2D物理仿真。

### 论文的主要结论与发现

1. **ID泛化完美，OOD泛化失败**：缩放数据量和模型大小显著提升ID性能（误差接近系统极限），但对OOD几乎没有改善，甚至随机波动。
2. **组合泛化存在缩放定律**：增加模板覆盖（从6到60）显著降低异常比例（67%→10%），表明数据多样性是关键。
3. **模型表现“案例式”泛化**：模型倾向于模仿训练中最接近的示例，而非学习抽象规则。例如，训练中引入翻转的匀速运动数据后，模型会错误地让慢速球反转方向。
4. **属性优先级：颜色 > 大小 > 速度 > 形状**：当测试样本与训练样本存在属性冲突时，模型优先保留高优先级属性（如颜色），改变低优先级属性（如形状）。这解释了为何视频模型常出现形状不一致问题。
5. **视觉模糊性限制物理建模**：当物体大小差异在像素级别时，模型可能产生看似合理但实际错误的物理结果（如错误判断球能否通过间隙）。

### 优点：方法或实验设计上的亮点

- **系统性泛化分类**：清晰区分ID、OOD、组合泛化，为评估视频模型物理理解提供了框架。
- **可控且干净的实验环境**：使用2D物理仿真，避免真实视频中的纹理、光影等混淆因素，能够精确定量化评估。
- **丰富的消融分析**：深入探究模型内部机制（案例匹配、属性优先级、插值外推、空间/时间组合），揭示模型行为的底层原因。
- **综合评估指标**：结合客观指标（FVD、SSIM、PSNR、LPIPS）和人工评估（异常比例），覆盖视频质量和物理正确性。
- **对比不同条件模态**：考察了数值和文本输入对OOD泛化的影响，发现反而带来过拟合，具有指导意义。

### 不足与局限

- **场景限制**：所有实验基于2D简单图形，未在真实复杂视频（如3D、非刚体、光照变化）上验证，结论的泛化性需进一步测试。
- **硬件与时间消耗**：大型模型（DiT-XL）在组合场景上训练需64块A100训练1000K步，资源开销大，可能限制了更广泛的缩放研究。
- **评估局限**：组合泛化场景中因物体复杂，无法使用自动速度误差，依赖人工评估（可能主观），且未提供标注者间一致性指标。
- **未涉及其他生成范式**：论文仅关注扩散模型，未对比自回归模型（如VideoPoet）或GAN的方法，结论的通用性有待验证。
- **潜在偏差**：属性优先级顺序（颜色>大小>速度>形状）可能受VAE潜空间距离影响，论文虽做了初步验证，但未给出理论证明或更本质的解释。

（完）
