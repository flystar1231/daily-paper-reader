---
title: Reliable Image Quality Evaluation and Mitigating Quality Bias in Generative Models
title_zh: 可靠图像质量评估与生成模型中的质量偏差缓解
authors: "Hoin Jung, Shenyu Lu, De Wang, Xiaoqian Wang"
date: 2025-05-06
pdf: "https://openreview.net/pdf?id=nFmq9z7Mdq"
tags: ["query:vgen-metrics"]
score: 6.0
evidence: 提出DQA分数评估图像质量度量可靠性，可迁移到视频生成评估
tldr: 该论文针对图像生成模型中质量评估指标（如FID）存在的人群偏差问题，提出了差异质量评估（DQA）分数，通过严格可控条件下评估不同人群间的质量差异来衡量指标可靠性。实验表明DQA能有效揭示指标偏差，为更公平的生成模型评估提供了新工具。该方法有望推广至视频生成评估领域。
source: NeurIPS-2025-Rejected-Public
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 707, \"height\": 245, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 721, \"height\": 261, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1440, \"height\": 635, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1212, \"height\": 655, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1349, \"height\": 774, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1412, \"height\": 380, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1439, \"height\": 687, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1333, \"height\": 793, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1297, \"height\": 1708, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1442, \"height\": 548, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1354, \"height\": 477, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1125, \"height\": 415, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1444, \"height\": 935, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-nfmq9z7mdq/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1447, \"height\": 354, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-nfmq9z7mdq/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1464, \"height\": 266, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nfmq9z7mdq/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1491, \"height\": 373, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nfmq9z7mdq/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1431, \"height\": 591, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nfmq9z7mdq/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 832, \"height\": 184, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nfmq9z7mdq/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 712, \"height\": 263, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-nfmq9z7mdq/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1463, \"height\": 265, \"label\": \"Table\"}]"
motivation: 现有图像生成质量指标（如FID）在评估不同人群时存在偏差，影响评估可靠性。
method: 提出DQA分数，通过严格控制条件比较不同人群间的质量评估差异来量化指标可靠性。
result: 实验证实了DQA能有效检测指标偏差，并帮助缓解生成模型中的质量不公平问题。
conclusion: DQA为生成模型的质量评估提供了可靠性度量，是现有指标的重要补充。
---

## Abstract
Discrepancies in generation quality across demographic groups pose a substantial and critical challenge in image generative models. However, the Fréchet Inception Distance (FID) score, which is widely used as an image quality evaluation metric for generative models, introduces unintended bias when assessing quality across sensitive attributes. This undermines the reliability of the evaluation procedure. This paper addresses this limitation by introducing the Difference in Quality Assessment (DQA) score, a novel approach that quantifies the reliability of existing evaluation metrics, e.g. FID. DQA assesses discrepancies in evaluated quality across demographic groups under strictly controlled conditions to effectively gauge metric reliability. Our findings reveal that traditional quality evaluation metrics can yield biased assessments across groups due to inappropriate reference set selection and inherent biases in image encoder in FID. Furthermore, we propose DQA-Guidance within diffusion model sampling to reduce quality disparities across groups. Experimental results demonstrate the utility of the DQA score in identifying biased evaluation metrics and present effective strategies to mitigate these biases. This work contributes to the development of reliable and fair evaluation metrics for generative models and provides actionable methods to address quality disparities in image generation across groups.

---

## 论文详细总结（自动生成）

# 论文详细总结

## 1. 核心问题与整体含义（研究动机和背景）

- **问题背景**：图像生成模型（如GAN、扩散模型）在不同人口统计群体（性别、种族、职业等）之间存在生成质量差异，即“质量偏差”（quality bias）。例如，对于“护士”职业，模型生成女性图像质量高，生成男性图像却出现肢体扭曲、灰度化等缺陷。
- **现有指标缺陷**：广泛使用的生成质量评估指标——Fréchet Inception Distance（FID）在跨群体评估时存在不可靠性，原因有二：
  1. **参考数据集选择不当**：FID使用统一参考集，掩盖或放大偏差，导致质量偏差的方向被误判。
  2. **图像编码器固有偏差**：InceptionV3、CLIP等编码器对同一质量水平的图像在不同群体上产生不一致的嵌入，甚至将低质量图像误嵌入到错误群体的聚类中。
- **研究目标**：提出一种评估指标可靠性（特别是公平性）的方法，并设计策略缓解生成模型中的质量偏差。

## 2. 方法论

### 2.1 核心思想
- **DQA分数（Difference in Quality Assessment）**：衡量现有评估指标（如FID）在不同人口群体间评估质量差异的可靠性。通过严格可控的数据集，量化编码器带来的偏差。
- **DQA-Guidance**：利用DQA作为能量函数，在扩散模型采样阶段引导生成，以降低群体间质量差异，同时提升整体质量。

### 2.2 关键技术细节

#### DQA分数定义
设群体A和B有参考集$A_{ref}, B_{ref}$，生成集$A_{gen}, B_{gen}$，图像编码器$f$，距离度量$D$（本文使用MMD）。DQA定义为：
$$
DQA = \frac{D(f(A_{gen}), f(A_{ref})) - D(f(B_{gen}), f(B_{ref}))}{D(f(I_{gen}), f(I_{ref}))}
$$
其中$I_{ref}=A_{ref}\cup B_{ref}$，$I_{gen}=A_{gen}\cup B_{gen}$。分子衡量群体间质量差异，分母衡量全局生成质量。低DQA表示评估公平，高DQA表示编码器存在偏差。
- 对于多个群体，使用平均DQA（AvgDQA）聚合所有成对DQA。

#### 评估数据集构造
- 使用Stable Diffusion XL生成10种职业、2种性别、4种种族的图像，每种子集250张，共20000张/场景。
- 设计6种质量退化场景：基线（良好质量）、弱引导、减少采样步数、强噪声、无精炼器、组合退化。基线作为参考集，其他作为生成集。

#### DQA-Guidance公式
在扩散模型去噪过程中，将DQA梯度加入噪声预测：
$$
\tilde{\epsilon}_\theta(z_t) = \epsilon_\theta(z_t) + \sigma_t \nabla_{z_t} \left[ \lambda_1 DQA(g(z_{At}), g(z_{Bt}); f^*) + \lambda_2 D(f^*(I_{gen}), f^*(I_{ref})) \right]
$$
其中$f^*$是可靠编码器（如DINO-RN50），$\lambda_1,\lambda_2$为超参数。第一项降低质量差异，第二项提升整体质量。

## 3. 实验设计

### 3.1 数据集与场景
- **人类图像生成**：使用Stable Diffusion XL，构造6种质量退化场景（基线、弱引导、少步数、强噪声、无精炼、组合）。共20000张/场景。
- **医学图像**：使用NIH ChestX-ray14数据集，ROCO数据集训练的ImageGen模型生成合成X光图像。模拟生成故障（如变换）构建评估集。

### 3.2 Benchmark与对比方法
- **评估指标可靠性**：对比12种预训练图像编码器（InceptionV3、VGG、ResNet-50、ViT-B/16、Swin Transformer、MoCo、MSN、DINO、CLIP等），训练方式（监督、自监督）、架构（CNN、Transformer）、数据集大小（IN-1K、IN-21K）。
- **质量偏差缓解（DQA-Guidance）**：与基线（无引导）对比，无其他现有方法（论文称首次从质量角度缓解偏差）。

### 3.3 下游任务验证
- 使用DQA分数构建公平/不公平子集（基于影响函数采样），用于数据增强，在Chest X-ray分类任务（ResNet-50）上验证公平性（AUC差异）。

## 4. 资源与算力
- **硬件**：CPU为AMD EPYC 7313 16核处理器，GPU为NVIDIA RTX A5000（附录L）。
- **训练时长**：未明确报告具体训练/推理时间。仅指出DQA-Guidance需要辅助编码器和梯度计算，增加内存开销。

## 5. 实验数量与充分性

- **可靠性分析**：对12种编码器在6种退化场景下计算DQA，涵盖性别和种族两个属性，实验数量约12×6=72组（图5(b)）。
- **DQA-Guidance**：在人类图像生成中测试不同$\lambda_1,\lambda_2$组合（表1、图9），消融研究表明参数敏感但有效。在医学图像上也进行了类似实验（图11、附录H）。
- **下游任务**：使用Chest X-ray分类任务，对比基线、全增强、公平子集、不公平子集（表2、表3），以及DQA-Guidance增强（3个$\lambda_1$值），共约10组。
- **其他验证**：t-SNE可视化（图4、图7）、不同质量评估类型（VQA、IQA）的DQA适配（附录I）、Fréchet Distance替代MMD（附录K）。
- **充分性评价**：实验覆盖了主要贡献点（可靠性诊断、缓解策略、下游应用），且进行了消融和敏感性分析。但缺乏与其他缓解方法的对比（因领域空白），部分实验仅报告单次或少量重复（未提供置信区间）。

## 6. 主要结论与发现

1. **FID等传统指标不可靠**：在跨群体质量评估中存在因参考集选择和编码器偏差导致的系统性偏差。
2. **DQA可有效诊断指标偏差**：自监督方法（DINO-RN50、MoCo-RN50）的DQA最低，最可靠；CNN架构优于ViT；增大训练数据集规模不一定降低偏差。
3. **DQA-Guidance能缓解质量偏差**：在扩散模型采样中加入DQA梯度，可同时提升整体质量和群体公平性。
4. **DQA有实际应用价值**：通过DQA选择公平/不公平子集，可改善或恶化下游分类的公平性。

## 7. 优点

- **创新性强**：首次系统研究生成质量公平性，提出可靠性诊断工具（DQA）和缓解策略（DQA-Guidance）。
- **方法论严谨**：通过严格受控的数据集（6种退化场景）隔离编码器偏差，公式定义清晰合理（分组距离归一化）。
- **实验设计全面**：涵盖多种编码器架构、训练范式、下游任务，并验证了DQA的实际效用。
- **开放可复现**：提供了数据集构造细节和算法流程（Algorithm 1）。

## 8. 不足与局限

- **缺乏基线对比**：在质量偏差缓解部分无其他现有方法对比（论文自承，表1无对照组）。
- **计算开销**：DQA-Guidance需每步计算梯度，内存和推理时间增加。
- **数据集局限性**：受控退化场景可能不完全反映真实生成模型的质量变化；未进行人类感知验证（如通过调查确认质量）。
- **实验重复性**：部分表格（如表1、图9）未报告多次运行的误差棒，统计显著性不明。
- **群体划分有限**：仅考虑性别、种族、职业三个属性，未覆盖年龄、地域等更多维度。
- **医学应用泛化性**：仅使用单一数据集（ChestX-ray14），其他医学领域（如MRI、CT）未验证。

（完）
