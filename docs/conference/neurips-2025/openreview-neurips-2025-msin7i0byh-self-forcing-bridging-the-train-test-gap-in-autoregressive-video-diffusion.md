---
title: "Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion"
title_zh: 自强制：弥合自回归视频扩散中的训练-测试差距
authors: "Xun Huang, Zhengqi Li, Guande He, Mingyuan Zhou, Eli Shechtman"
date: 2025-09-18
pdf: "https://openreview.net/pdf?id=mSiN7i0BYH"
tags: ["query:vgen-metrics"]
score: 7.0
evidence: 视频级整体损失直接评估生成视频质量
tldr: 本文针对自回归视频扩散模型中的曝光偏差问题，提出自强制训练范式，通过在训练时进行自回归展开并引入视频级整体损失，直接评估整个生成序列的质量，从而有效缓解训练与推理之间的差异。该方法将质量评估融入训练过程，为视频生成评估提供了新的视角和工具。
source: NeurIPS-2025-Accepted
selection_source: conference_retrieval
figures_json: "[{\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1437, \"height\": 520, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1452, \"height\": 545, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1436, \"height\": 433, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 713, \"height\": 421, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1461, \"height\": 1036, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1459, \"height\": 488, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1425, \"height\": 772, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 873, \"height\": 857, \"label\": \"Figure\"}, {\"url\": \"assets/figures/openreview/openreview-neurips-2025-msin7i0byh/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 1437, \"height\": 494, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/openreview/openreview-neurips-2025-msin7i0byh/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 703, \"height\": 1102, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-msin7i0byh/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 712, \"height\": 1030, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-msin7i0byh/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1447, \"height\": 692, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-msin7i0byh/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 714, \"height\": 530, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-msin7i0byh/table-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 715, \"height\": 531, \"label\": \"Table\"}, {\"url\": \"assets/tables/openreview/openreview-neurips-2025-msin7i0byh/table-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1434, \"height\": 635, \"label\": \"Table\"}]"
motivation: 现有的自回归视频扩散模型在推理时因条件化自身不完美输出而导致质量下降，需要更好的训练策略。
method: 在训练时采用自回归展开和KV缓存，使模型基于自身生成结果进行条件化，并引入视频级整体损失监督。
result: 该方法有效弥合了训练-测试差距，提升了生成视频的整体质量。
conclusion: 自强制训练范式为视频生成模型提供了一种将质量评估内置于训练过程的有效途径。
---

## Abstract
We introduce Self Forcing, a novel training paradigm for autoregressive video diffusion models. It addresses the longstanding issue of exposure bias, where models trained on ground-truth context must generate sequences conditioned on their own imperfect outputs during inference. Unlike prior methods that denoise future frames based on ground-truth context frames, Self Forcing conditions each frame's generation on previously self-generated outputs by performing autoregressive rollout with key-value (KV) caching during training. This strategy enables supervision through a holistic loss at the video level that directly evaluates the quality of the entire generated sequence, rather than relying solely on traditional frame-wise objectives. To ensure training efficiency, we employ a few-step diffusion model along with a stochastic gradient truncation strategy, effectively balancing computational cost and performance. We further introduce a rolling KV cache mechanism that enables efficient autoregressive video extrapolation. Extensive experiments demonstrate that our approach achieves real-time streaming video generation with sub-second latency on a single GPU, while matching or even surpassing the generation quality of significantly slower and non-causal diffusion models.

---

## 论文详细总结（自动生成）

# 论文总结：Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion

## 1. 核心问题与整体含义（研究动机和背景）

- **暴露偏差（Exposure Bias）**：自回归视频扩散模型在训练时使用真实上下文帧（Teacher Forcing 或 Diffusion Forcing），但推理时必须依赖自身生成的、可能不完美的历史帧作为条件。这种分布不匹配导致误差随时间累积，生成质量逐步退化。
- **现有方法不足**：Teacher Forcing 和 Diffusion Forcing 虽然设计了不同的条件方式（清洁帧 vs. 带噪帧），但训练输出与推理时模型自身生成的分布仍存在差异，无法从根本上解决暴露偏差。
- **目标**：提出一种新的训练范式 Self Forcing，使训练过程紧密模拟推理场景，从而弥合训练-测试分布差距，提升长序列生成质量，并支持实时流式视频生成。

## 2. 方法论：核心思想与关键技术细节

- **核心思想**：在训练时进行**自回归自我展开（Autoregressive Self-Rollout）**——每个帧的生成基于模型之前**自己生成的**帧（而非真实帧），并使用**视频级整体损失（Holistic Distribution-Matching Loss）** 对整个生成序列进行监督。
- **关键技术细节**：
  - **Few-step 扩散模型**：采用 4 步扩散过程近似每个条件分布，降低展开的计算成本。
  - **梯度截断策略**：仅对每帧的最后一个去噪步骤进行反向传播，并将前帧的 KV 缓存梯度分离（stop-gradient），避免梯度爆炸和内存爆炸。
  - **随机去噪步骤采样**：在训练中随机选择一个去噪步骤 `s`（1~T），并仅对第 `s` 步输出计算损失，确保所有去噪步骤都能得到监督信号。
  - **滚动 KV 缓存（Rolling KV Cache）**：在长视频生成中维护固定大小的 KV 缓存，新的帧仅与缓存中最新的 L 帧进行注意力计算，避免重复计算，复杂度为 O(TL)，支持无限长视频外推。
  - **训练中的局部注意力窗口**：为防止滚动缓存中模型过度依赖第一帧（图像潜码）导致闪烁，训练时限制注意力窗口，使模型在生成末尾帧时无法看到第一帧。
- **视频级分布匹配损失**：支持三种方式：
  - **DMD**：最小化逆KL散度，利用真实分布和模型分布的得分函数差。
  - **SiD**：最小化 Fisher 散度。
  - **GAN**：采用 R3GAN（相对配对 + R1+R2 正则化）进行对抗训练。
- **算法流程**：
  - 训练（Algorithm 1）：逐帧进行多步去噪，仅在最后一步启用梯度，更新 KV 缓存，对整个序列计算整体损失。
  - 推理（Algorithm 2）：使用滚动 KV 缓存，生成每一帧时执行完整 4 步去噪，并更新/淘汰缓存。

## 3. 实验设计

- **数据集与场景**：
  - 训练提示：使用 VidProM 的过滤和 LLM 扩展版本（约 25 万提示）。
  - 生成训练数据：用 Wan2.1-T2V-14B 生成 7 万段视频作为 GAN 训练数据。
  - 评估：VBench 基准（16项指标）和用户偏好研究（MovieGenBench 1003 提示）。
- **对比方法**：
  - 双向扩散模型：Wan2.1-1.3B、LTX-Video（1.9B）。
  - 自回归扩散模型（逐块/逐帧）：SkyReels-V2、MAGI-1、CausVid、Pyramid Flow、NOVA。
- **主要指标**：
  - 吞吐量（FPS）、第一帧延迟（秒）、VBench总分（质量+语义）、用户偏好率。

## 4. 资源与算力

- **训练硬件**：64 块 NVIDIA H100 GPU（80GB 显存每块），单卡 batch size 1，梯度累积实现有效 batch size 64（DMD/SiD）或 768（GAN）。
- **训练时长**：
  - DMD 训练约 1.5 小时收敛。
  - SiD/GAN 训练 2-3 小时。
- **预训练模型**：Wan2.1-T2V-1.3B（初始化权重）和 Wan2.1-T2V-14B（生成 ODE 解和训练数据）。

## 5. 实验数量与充分性

- **主要对比实验**（表1）：7 个模型在相似规模下的全指标对比。
- **用户研究**（图4）：4 组成对偏好比较（Ours vs MAGI-1, SkyReels-V2, Wan2.1, CausVid），各约 1000 提示。
- **消融实验**（表2、图6、附录B）：
  - 不同训练范式（Teacher Forcing, Diffusion Forcing, Self Forcing） × 不同损失（DMD, SiD, GAN）。
  - 逐个 vs. 逐块自回归模式。
  - 多步（50步） vs. 少步（4步）对比。
  - 滚动 KV 缓存消融（有/无局部注意力训练）。
  - 训练效率对比（每个迭代时间+质量 vs. 壁钟时间）。
- **VBench 全维度**（附录C）：16项指标雷达图。
- **公平性**：CausVid 使用相同基础模型（Wan-1.3B）重新实现；所有基线在同一评估协议下测试。

综合来看，实验覆盖了主要维度（质量、效率、消融、人类偏好），对照组设计合理，数量充足，结论可信。

## 6. 主要结论与发现

- Self Forcing 在所有分布匹配损失（DMD、SiD、GAN）下均稳定优于 Teacher Forcing 和 Diffusion Forcing 训练的基线，尤其在逐帧自回归模式下（更易误差累积）优势明显。
- 生成质量显著超过 CausVid（DF + DMD），并匹配/超越原始慢速双向扩散模型 Wan2.1-1.3B。
- 实现真实时视频生成：
  - 逐模型：17 FPS 吞吐量，0.69s 延迟（逐帧模式 8.9 FPS, 0.45s 延迟）。
- 训练效率意外高：Self Forcing 的每个迭代时间与并行范式相当，且在相同壁钟时间内达到更高质量。
- 滚动 KV 缓存结合局部注意力训练可有效避免长视频外推时的闪烁伪影。

## 7. 优点

- **方法论创新**：首次在视频扩散模型训练中引入完全自回归自我展开，直接从源头上解决暴露偏差。
- **视频级整体损失**：更符合生成任务目标（评估整个序列质量），而非仅帧级局部损失。
- **高效性**：利用 few-step 扩散、梯度截断和滚动 KV 缓存，在实现高质量的同时达到实时推理，训练成本甚至低于并行基线。
- **模块化损失设计**：支持 DMD、SiD、GAN 等多种分布匹配方法，灵活性强。
- **泛化性**：框架可应用于其他连续序列域（如图像、音频、语言），具有推广潜力。

## 8. 不足与局限

- **外推能力有限**：在生成远超过训练上下文长度（如>10秒）的视频时，质量仍会下降（如闪烁、误差累积）。
- **梯度截断**：为内存效率限制了梯度流过过去帧的 KV 缓存，可能削弱模型对长程依赖的学习能力。
- **长视频评估缺失**：实验中仅评估固定长度（5s）视频，缺乏对超长视频（>30s）的量化度量。
- **依赖预训练模型**：初始化权重来自 Wan2.1，且需要预先生成 ODE 解和 GAN 训练数据（需大模型），对计算资源仍有较高要求。
- **未测试多条件输入**：实验仅针对文本到视频，未探索图像/视频条件控制场景。
- **社会影响**：实时生成能力降低了滥用门槛，需配套检测机制和伦理规范（论文附录D提及，但未提供具体缓解措施）。

（完）
