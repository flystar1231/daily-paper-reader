---
title: Direct Motion Models for Assessing Generated Videos
title_zh: 直接运动模型用于评估生成视频
authors: "Kelsey R Allen, Carl Doersch, Guangyao Zhou, Mohammed Suhail, Danny Driess, Ignacio Rocco, Yulia Rubanova, Thomas Kipf, Mehdi S. M. Sajjadi, Kevin Patrick Murphy, Joao Carreira, Sjoerd van Steenkiste"
date: 2025-05-01
pdf: "https://openreview.net/pdf?id=qpi7NiaCYj"
tags: ["query:vgen-metrics"]
score: 9.0
evidence: 基于运动的视频评估指标
tldr: 针对生成视频评估中运动质量难以衡量的问题，提出了基于自编码点轨迹的评估指标。该指标不仅可用于比较视频分布，还可评估单个视频的运动质量。实验表明，相比像素重建或动作识别特征，该指标对时序失真更为敏感，能够更好地捕捉物体交互和合理运动，弥补了FVD的不足。
source: ICML-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 824, \"height\": 317, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 831, \"height\": 309, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1770, \"height\": 460, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 860, \"height\": 297, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1311, \"height\": 277, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1588, \"height\": 567, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 597, \"height\": 466, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1708, \"height\": 333, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1603, \"height\": 287, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 925, \"height\": 398, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-011.webp\", \"caption\": \"\", \"page\": 0, \"index\": 11, \"width\": 1346, \"height\": 414, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-012.webp\", \"caption\": \"\", \"page\": 0, \"index\": 12, \"width\": 1437, \"height\": 581, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-013.webp\", \"caption\": \"\", \"page\": 0, \"index\": 13, \"width\": 1437, \"height\": 579, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-014.webp\", \"caption\": \"\", \"page\": 0, \"index\": 14, \"width\": 1593, \"height\": 332, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-015.webp\", \"caption\": \"\", \"page\": 0, \"index\": 15, \"width\": 1592, \"height\": 333, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-016.webp\", \"caption\": \"\", \"page\": 0, \"index\": 16, \"width\": 1596, \"height\": 334, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-017.webp\", \"caption\": \"\", \"page\": 0, \"index\": 17, \"width\": 1241, \"height\": 1873, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-018.webp\", \"caption\": \"\", \"page\": 0, \"index\": 18, \"width\": 1240, \"height\": 1873, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-019.webp\", \"caption\": \"\", \"page\": 0, \"index\": 19, \"width\": 658, \"height\": 559, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-icml-2025-qpi7niacyj/fig-020.webp\", \"caption\": \"\", \"page\": 0, \"index\": 20, \"width\": 1783, \"height\": 1085, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1484, \"height\": 424, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 830, \"height\": 352, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 850, \"height\": 280, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 457, \"height\": 210, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 808, \"height\": 313, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1407, \"height\": 412, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1255, \"height\": 335, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 854, \"height\": 225, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-icml-2025-qpi7niacyj/table-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1456, \"height\": 242, \"label\": \"Table\"}]"
motivation: 现有FVD等指标不能很好地衡量生成视频中的运动质量。
method: 基于自编码点轨迹提取运动特征，用于视频分布比较和单视频评估。
result: 新指标对时序失真更敏感，优于基于像素或动作识别的方法。
conclusion: 为生成视频的运动质量评估提供了有效新工具。
---

## Abstract
A current limitation of video generative video models is that they generate plausible looking frames, but poor motion --- an issue that is not well captured by FVD and other popular methods for evaluating generated videos. Here we go beyond FVD by developing a metric which better measures plausible object interactions and motion. Our novel approach is based on auto-encoding point tracks and yields motion features that can be used to not only compare distributions of videos (as few as one generated and one ground truth, or as many as two datasets), but also for evaluating motion of single videos. We show that using point tracks instead of pixel reconstruction or action recognition features results in a metric which is markedly more sensitive to temporal distortions in synthetic data, and can predict human evaluations of temporal consistency and realism in generated videos obtained from open-source models better than a wide range of alternatives. We also show that by using a point track representation, we can spatiotemporally localize generative video inconsistencies, providing extra interpretability of generated video errors relative to prior work. An overview of the results and link to the code can be found on the project page: trajan-paper.github.io.

---

## 论文详细总结（自动生成）

# 论文详细中文总结

## 1. 论文的核心问题与整体含义（研究动机和背景）

当前生成视频模型（如扩散模型、Transformer）虽然在生成逼真单帧方面进步显著，但在运动连贯性方面存在严重缺陷（如物体变形、手指消失、跳跃等）。现有主流评估指标（如FVD及其变体）主要基于帧级内容（如I3D、VideoMAE特征），对运动质量不敏感，且只能用于分布比较，无法评估单个视频或视频对。此外，人类评估成本高、不可扩展。因此，亟需一种能够直接衡量运动质量、支持多场景（单视频、视频对、分布）评估的自动指标。

## 2. 论文提出的方法论

**核心思想**：利用点轨迹（point tracks）作为运动表征，通过自编码器（TRAJAN）学习稠密运动特征，并基于重建误差或特征距离来评估视频运动质量。

**关键技术细节**：
- **点轨迹提取**：使用BootsTAPIR模型从视频中提取一组点轨迹（含位置和遮挡标志）。
- **TRAJAN架构**：
  - 编码器：对每条轨迹进行正弦位置嵌入，添加readout token，使用自注意力（遮挡掩码忽略不可见点）得到每条轨迹的定长表示；再通过Perceiver风格交叉注意力将所有轨迹编码为固定大小的128×64运动潜在向量φ_S。
  - 解码器：给定查询点（x_q, y_q, t_q），从φ_S中解码出该点对应的完整轨迹（位置和遮挡），使用Huber损失和交叉熵损失训练。
  - 关键设计：编码器对输入点集是排列不变的，解码器必须重建未输入的支持点，从而学习稠密运动场。
- **评估方式**：
  - 单视频：使用Average Jaccard（AJ）衡量重建精度，AJ越高表示运动越真实。
  - 视频对：计算TRAJAN潜在向量的L2距离。
  - 分布比较：计算两个分布潜在向量的Fréchet距离（类似FVD）。
- **替代方法对比**：
  - 运动类：运动直方图、光流（RAFT）扭曲误差、MooG预测PSNR。
  - 外观类：I3D熵、VideoMAE-v2（预训练和SSv2微调）重建损失/熵。

## 3. 实验设计

**使用的数据集/场景**：
- **单视频评估**：VideoPhy（8个模型生成视频）、EvalCrafter（11个模型生成视频），配合新收集的人类评分（一致性、交互、真实感、速度）。
- **视频对比较**：WALT模型在Kinetics-600上训练后的生成-真实视频对。
- **分布比较**：UCF101数据集，施加五种弹性变形（空间/时空维度），检验指标对时序失真的敏感性。

**Benchmark**：与多种现有指标对比（I3D、VideoMAE、RAFT、MooG、运动直方图等），并对比人类评分。

**对比方法**：见上述替代方法列表。

## 4. 资源与算力

论文**未明确说明**使用的具体GPU型号、数量及训练时长。仅提及TRAJAN使用Adam优化器训练1M步，批量大小64，学习率2e-4，基于大型公开视频数据集（150帧剪辑，共1500万视频片段）。训练细节在附录B.2.1中给出，但未涉及硬件信息。

## 5. 实验数量与充分性

**主要实验组**：
1. **单视频评估**：在VideoPhy和EvalCrafter两个数据集上，计算与人类评分的Spearman秩相关系数，涵盖4个维度（运动一致性、外观一致性、真实感、交互），并控制运动量进行子集分析。
2. **视频对比较**：对WALT生成视频，比较TRAJAN潜在距离与PSNR/SSIM的相关性（2364个样本），并展示定性示例。
3. **分布比较**：在UCF101上计算Fréchet距离和平均单视频分数，评估对时空失真的灵敏度（5种变形级别，空间vs时空模式）。
4. **消融/附加实验**：
   - 使用MMD替代Fréchet距离（附录A.1）。
   - 跟踪WALT训练过程中指标变化（附录A.2）。
   - 在原始EvalCrafter和VideoPhy标签上进行验证（表3、图6）。
   - 人类评分一致性分析（inter-rater σ）。
   - 空间-时间定位示例（图5）。

**充分性评价**：实验覆盖了三种评估场景（单视频、视频对、分布），对比了多种主流方法，使用了两个人类评分数据集（含自采数据），并进行了控制实验（区分运动量）。实验设计较为全面，但分布比较仅使用UCF101单一数据集，且弹性变形是合成失真，真实生成视频的分布评估有待补充。

## 6. 论文的主要结论与发现

- TRAJAN在**单视频评估**中比所有对比方法（包括光流、VideoMAE、I3D等）更好地与人类评分相关，尤其在运动一致性、外观一致性、真实感方面。
- TRAJAN在**分布比较**中对时序失真灵敏度最高（ST/S比值最高），运动直方图和外观方法表现较差。
- TRAJAN的**潜在空间距离**与像素级指标（PSNR/SSIM）低相关，表明它捕捉的是运动相似性而非外观相似性。
- TRAJAN可用于**时空错误定位**，通过逐点AJ可视化指出帧间不一致区域。
- 人类评分者自身一致性有限（inter-rater σ约0.5），提示人类评判作为金标准需谨慎。

## 7. 优点

- **运动专注**：通过点轨迹自然解耦运动与外观，避免内容偏差。
- **多场景统一**：支持单视频、视频对、分布三种评估模式，无需参考分布。
- **可解释性**：能逐点、逐帧定位不自然运动。
- **高性能**：无需人工标注，即可在多个基准上超越或媲美人类评分。
- **简洁架构**：基于自编码和点轨迹，训练数据来自公共模型BootsTAPIR，易于复现。

## 8. 不足与局限

- **无法评估物理合理性**：对“物体不应凭空消失”等违反物理常识的运动仍可能给出高分（图4例子）。
- **依赖点跟踪质量**：若视频质量差或运动极端，BootsTAPIR可能失败。
- **训练数据偏差**：TRAJAN仅在有限类别的公开视频上训练，可能对非自然运动（如动画）表现不佳。
- **人类评分噪声**：不同评判者对“真实感”“一致性”理解差异大，导致标签噪声大，限制了指标的上限。
- **计算开销**：提取点轨迹和运行TRAJAN编码器需额外计算，虽小于人类评估，但可能比简单I3D特征更耗时。
- **实验覆盖**：分布比较仅使用UCF101（动作类视频），未在更多样化的视频生成数据集上验证。
- **资源信息缺失**：未报告训练所需GPU数量、型号及时间，不利于比较效率。

（完）
