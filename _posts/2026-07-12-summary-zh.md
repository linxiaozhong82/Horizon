---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> 从 50 条内容中筛选出 19 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：LLM、GPU performance、ollama、code generation、LLM inference。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Qwen3.6 35B-A3B 单提示生成飞行模拟器](https://www.reddit.com/r/LocalLLaMA/comments/1utb6io/qwen36_35ba3b_q8_0_no_kv_quant_single_prompt_in/)**
2. **[RTX 5090 vs 6000 Pro：分流改装基准测试结果](https://www.reddit.com/r/LocalLLaMA/comments/1utvbey/performance_comparison_on_full_compute/)**
3. **[Ollama v0.32.0-rc0 新增 Qwen3.5 解析器和代理界面](https://github.com/ollama/ollama/releases/tag/v0.32.0-rc0)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [Rasbt 在 LLMs-from-Scratch 仓库中创建新分支](https://github.com/rasbt/LLMs-from-scratch)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [Grok Build CLI 将整个仓库上传至 xAI 云端](https://www.reddit.com/r/LocalLLaMA/comments/1ut7tis/grok_build_cli_uploads_your_whole_repo_full_git/)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [vLLM v0.25.0：Model Runner V2 成为默认，移除了 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Qwen3.6 35B-A3B 单提示生成飞行模拟器

**关联新闻**: [Qwen3.6 35B-A3B 单提示生成飞行模拟器](https://www.reddit.com/r/LocalLLaMA/comments/1utb6io/qwen36_35ba3b_q8_0_no_kv_quant_single_prompt_in/)

**切入角度**: 一位 Reddit 用户展示，Qwen3.6 35B-A3B 在采用 Q8_0 CPU 量化后，能够根据单个提示在 opencode 中生成包含山脉、云朵和无限程序化地形的完整飞行模拟器 HTML 文件。该用户指出，从 GPU 上的 Q4_K_M 切换至 CPU 上的 Q8_0 后性能显著提升。 这表明，采用适当量化的本地 LLM 在复杂代码生成方面可与云端模型媲美，使个人开发者和爱好者更容易获得先进的 AI 能力。同时，这也凸显了量化选择对特定任务性能的重要性。 该用户首先使用了计划模式，然后指示模型无需更改即实现。他们强调，尽管速度较慢，但 CPU 上的 Q8_0 量化相比 GPU 上的 Q4_K_M 显著提升了输出质量。

**可延展方向**: Qwen3.6 35B-A3B 是一种稀疏混合专家（MoE）模型，总参数量为 350 亿，但仅有 30 亿活跃参数，专为高效代理编码而设计。量化通过降低数值精度来减小模型大小并加速推理，但像 Q8_0 这样的高精度格式比 Q4_K_M 等低精度格式保留了更多准确性。此演示表明，对于某些创意任务，采用更高精度的 CPU 推理可以胜过 GPU 加速的低精度推理。

---

### 选题 2：RTX 5090 vs 6000 Pro：分流改装基准测试结果

**关联新闻**: [RTX 5090 vs 6000 Pro：分流改装基准测试结果](https://www.reddit.com/r/LocalLLaMA/comments/1utvbey/performance_comparison_on_full_compute/)

**切入角度**: 一位 Reddit 用户对分流改装并水冷的 RTX 6000 PRO MaxQ 与常规及超频的 RTX 5090 和 RTX 6000 PRO WS 进行了详细的 LLM 推理和完整计算（Anima）性能对比。改装后的 MaxQ 在 600W 功耗下性能最佳，比 RTX 5090 快 12.8%。 该对比为希望通过分流改装和水冷等硬件修改最大化 AI 工作负载 GPU 性能的爱好者和专业人士提供了宝贵的实证数据。它表明，去除功耗限制后，经过筛选的专业 GPU 可以显著超越消费旗舰产品，挑战高端消费显卡的性价比。 分流改装涉及更换电阻（R002），使 RTX 6000 PRO MaxQ 功耗达到 600W，水冷将温度控制在 60°C。测试使用了特定软件版本（Torch 2.14.0、Sageattention 2.1、Forge Neo），并包含使用 llama.cpp 在 Kimi K2 2.5 和 GLM 5.1 等模型上的 LLM 基准测试。

**可延展方向**: 分流改装是一种硬件修改，通过添加电阻让 GPU 误以为功耗更低，从而实现更高功耗和超频。水冷用于管理增加的热量。RTX 6000 PRO MaxQ 是一款经过筛选的工作站 GPU，在低功耗下具有高时钟频率，而 RTX 5090 是消费旗舰。Anima 基准测试可能指计算密集型任务，LLM 测试通过将模型层卸载到 CPU 使 GPU 成为计算瓶颈。

---

### 选题 3：Ollama v0.32.0-rc0 新增 Qwen3.5 解析器和代理界面

**关联新闻**: [Ollama v0.32.0-rc0 新增 Qwen3.5 解析器和代理界面](https://github.com/ollama/ollama/releases/tag/v0.32.0-rc0)

**切入角度**: 该候选版本引入了针对 Qwen3.5 模型系列的专用解析器和渲染器、新的代理用户界面，以及对过时代理模型的警告提示。 这些新增功能使用户更容易正确渲染运行 Qwen3.5，并通过内置界面与 AI 代理交互，从而提升本地大语言模型的可用性。 代理界面是命令行界面的一部分，对旧代理模型的警告有助于用户避免兼容性问题。该版本还包括其他修复和改进（详见完整变更日志）。

**可延展方向**: Ollama 是一款流行的开源工具，可在个人电脑上本地运行大语言模型（LLM）。Qwen3.5 是阿里云开发的开源大语言模型系列。代理界面允许用户通过可视化界面与 AI 代理（例如用于工具使用和多步推理）进行交互。

---

1. [vLLM v0.25.0：Model Runner V2 成为默认，移除了 PagedAttention](#item-1) ⭐️ 9.0/10
2. [Grok Build CLI 将整个仓库上传至 xAI 云端](#item-2) ⭐️ 9.0/10
3. [Nvidia、CoreWeave 与 Nebius 间的循环融资](#item-3) ⭐️ 8.0/10
4. [UPI 支付交易架构深度解析](#item-4) ⭐️ 8.0/10
5. [奇异值分解的早期历史 (1993)](#item-5) ⭐️ 8.0/10
6. [躲避致命无人机：伪装无效](#item-6) ⭐️ 8.0/10
7. [Qwen3.6 35B-A3B 单提示生成飞行模拟器](#item-7) ⭐️ 8.0/10
8. [100 美元超预算 20GB 显存方案](#item-8) ⭐️ 8.0/10
9. [美国科技业对中国开源 AI 模型的崛起感到焦虑](#item-9) ⭐️ 8.0/10
10. [RTX 5090 vs 6000 Pro：分流改装基准测试结果](#item-10) ⭐️ 8.0/10
11. [Qwen3 30B A3B 在 RTX 5060 Ti 上达到 50 tok/s](#item-11) ⭐️ 8.0/10
12. [SQLite/FTS5 专利数据库从 350 万条扩展到 536 万条的优化经验](#item-12) ⭐️ 8.0/10
13. [Rasbt 在 LLMs-from-Scratch 仓库中创建新分支](#item-13) ⭐️ 7.0/10
14. [Ollama v0.32.0-rc0 新增 Qwen3.5 解析器和代理界面](#item-14) ⭐️ 7.0/10
15. [别再叫我去问 LLM 了](#item-15) ⭐️ 7.0/10
16. [ClickHouse 通过 SO_REUSEPORT 和 Peering 将 PgBouncer 吞吐量提升 4 倍](#item-16) ⭐️ 7.0/10
17. [在 SQLite 中优先使用 STRICT 表](#item-17) ⭐️ 7.0/10
18. [llama.cpp b9966 缓存正则表达式以提升性能](#item-18) ⭐️ 7.0/10
19. [双 GPU PCIe 传输基准测试：张量并行与流水线并行对比](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，移除了 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有稠密模型的默认执行路径，并移除了旧的 PagedAttention 实现，同时带来了性能提升和新模型支持。 这一版本标志着 vLLM 架构的重大转变，简化了推理流程，有望在多种大语言模型服务场景中提升性能。移除 PagedAttention 使代码库更简洁，而 Model Runner V2 为未来优化铺平了道路。 Model Runner V2 现支持 EVS、实时嵌入、Mamba 混合模型的前缀缓存以及全 CUDA 图的动态推测解码。Transformers 建模后端经过优化，速度已与原生 vLLM 持平，并新增了 LLaVA-OneVision-2 和 GLM-5 系列等模型。

github · khluu · 7月11日 20:06

**背景**: vLLM 是由加州大学伯克利分校最初开发的开源大语言模型推理与服务引擎，以其通过 PagedAttention 实现的高性能而闻名。PagedAttention 是一种内存高效的注意力算法，将键值缓存管理在非连续的内存块中。Model Runner V2 是新一代执行后端，取代了基于 PagedAttention 的旧流水线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2023-06-20-vllm">vLLM: Easy, Fast, and Cheap LLM Serving with PagedAttention</a></li>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#open source`, `#model serving`, `#AI`

---

<a id="item-2"></a>
## [Grok Build CLI 将整个仓库上传至 xAI 云端](https://www.reddit.com/r/LocalLLaMA/comments/1ut7tis/grok_build_cli_uploads_your_whole_repo_full_git/) ⭐️ 9.0/10

研究人员演示了 Grok Build CLI v0.2.93 会将用户的整个代码仓库（包括完整的 Git 历史记录和 .env 机密文件）上传至 xAI 的 Google Cloud 基础设施，即使关闭了用于模型改进的退出开关，上传仍会进行。 这对使用 Grok Build CLI 的开发人员构成了严重的安全和隐私风险，因为敏感凭据和专有代码在未经用户同意的情况下被传输，可能泄露 API 密钥、密码和知识产权。 该上传行为通过 mitmproxy 捕获，一个从未被代理读取的植入文件依然出现在恢复的 Git 捆绑包中，证实了无论打开或读取了什么内容，整个 Git 历史记录都会被上传。

reddit · r/LocalLLaMA · /u/TastyLeadership2757 · 7月11日 02:34

**背景**: Grok Build CLI 是 xAI 推出的终端原生 AI 编码代理，用于在终端中协助编码任务。该工具包含一个“改进模型”开关，用户可关闭以退出基于模型训练的数据收集。然而，此开关并不影响仓库数据的自动上传，后者似乎是用于调试或分析的独立机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build Beta | xAI</a></li>
<li><a href="https://grokipedia.com/page/mitmproxy">mitmproxy</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#data leak`, `#CLI`, `#xAI`

---

<a id="item-3"></a>
## [Nvidia、CoreWeave 与 Nebius 间的循环融资](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

这种循环性引发了对 AI 基础设施投资可持续性的担忧，因为它可能人为地夸大需求，掩盖潜在的盈利能力问题。 Nvidia 对 CoreWeave 的 20 亿美元投资仅占 CoreWeave 2026 年计划资本支出 350 亿美元的 5.7%，其余资金来自其他投资者，表明这一循环并非完全封闭。

hackernews · adletbalzhanov · 7月11日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: 循环融资是指公司之间相互投资，以营造增长和需求的假象，常常推高估值。在 GPU 热潮中，Nvidia 投资于 CoreWeave 和 Nebius 等云服务提供商，后者再将资金用于购买 Nvidia 的硬件，形成反馈循环。这种做法可能掩盖真实的市场需求，并导致过度建设。

**社区讨论**: 社区评论对循环的程度进行了辩论：一些人认为 Nvidia 的持股相对于 CoreWeave 的总支出很小，而另一些人则关注 GPU 投资的盈利能力和潜在的过度建设。还有关于 Yandex 与 Nebius 的区别以及地缘政治影响的讨论。

**标签**: `#GPU`, `#AI Infrastructure`, `#Financing`, `#Nvidia`, `#Cloud Computing`

---

<a id="item-4"></a>
## [UPI 支付交易架构深度解析](https://timeseriesofindia.com/economy/reads/upi-architecture/) ⭐️ 8.0/10

一篇关于 UPI 支付交易架构的详细技术概述发布，解释了其设计、实际影响和可扩展性。文章剖析了 UPI 如何无缝处理数十亿笔交易。 UPI 彻底改变了印度的数字支付方式，甚至让老年人也能完全实现无现金支付。理解其架构有助于欣赏支撑每月超过 180 亿笔交易系统的工程能力。 NPCI 的 UPI 交换中心在每年 220 亿笔交易中平均约 700 QPS，但峰值可能高得多。该系统使用中心化、与 KYC 关联的私有网络，引发了对中心化和隐私的担忧。

hackernews · prtk25 · 7月11日 16:33 · [社区讨论](https://news.ycombinator.com/item?id=48873457)

**背景**: UPI（统一支付接口）是由印度国家支付公司（NPCI）开发并于 2016 年 8 月推出的实时支付系统。它允许通过智能手机使用虚拟支付地址（VPA）和 MPIN 进行身份验证，实现银行账户间的即时资金转账。UPI 全天候运行，已成为印度数字支付的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unified_Payments_Interface">Unified Payments Interface - Wikipedia</a></li>
<li><a href="https://medium.com/@avinashkariya05910/deep-dive-system-design-of-upi-unified-payments-interface-eff3b0334b0d">Deep Dive: System Design of UPI (Unified Payments Interface) | by Avinash Kariya | Medium</a></li>
<li><a href="https://razorpay.com/blog/what-is-upi-and-how-it-works/">What is UPI?: Unified Payments Interface Meaning, Features ... Designing UPI - System Design - GeeksforGeeks How Does UPI Work? - GeeksforGeeks Deep Dive: System Design of UPI (Unified Payments Interface) How UPI Works Internally (Backend + NPCI Explained) - Oflox</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞 UPI 让所有年龄段的人都能够使用数字支付，有人称其为‘举世无双的壮举’。其他人将其与中国的支付宝进行比较并讨论可扩展性，指出平均 700 QPS 相对于纳斯达克 10 万+ QPS 峰值来说并不算高。少数人提出了对中心化和隐私的担忧，质疑中心化、KYC 关联的系统是否可取。

**标签**: `#UPI`, `#payment systems`, `#architecture`, `#digital payments`, `#India`

---

<a id="item-5"></a>
## [奇异值分解的早期历史 (1993)](https://www.math.ucdavis.edu/~saito/courses/229A/stewart-svd.pdf) ⭐️ 8.0/10

G.W. Stewart 在 1993 年发表的一篇论文追溯了奇异值分解从 Beltrami 和 Jordan 的起源到 Golub 和 Kahan 的现代算法工作的历史发展。 了解 SVD 的历史有助于理解其在现代计算中的普遍作用，从 PCA 到神经网络优化。 论文献给了 Gene Golub 的 60 岁生日，社区讨论强调了 SVD 在 Muon 和 Adam 等优化器中的使用，以及 Eckart-Young-Mirsky 定理用于低秩近似。

hackernews · wolfi1 · 7月11日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=48872858)

**背景**: 奇异值分解（SVD）将任意实或复矩阵分解为三个部分：左奇异向量、奇异值和右奇异向量。它将特征分解推广到非方阵，并广泛应用于机器学习中的数据压缩和降噪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Singular_value_decomposition">Singular value decomposition</a></li>
<li><a href="https://math.mit.edu/classes/18.095/2016IAP/lec2/SVD_Notes.pdf">Chapter 7 The Singular Value Decomposition (SVD) ✬ ✫ ✩ ✪</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了技术见解，如奇异值为'广义特征值'以及与 Muon 和 Adam 等优化器的联系。一位评论者指出论文献给了 Gene Golub，他的生日是 2 月 29 日，另一位推荐了 Sheldon Axler 关于 SVD 的章节。总体情绪积极，认为该论文是宝贵的历史资源。

**标签**: `#linear algebra`, `#singular value decomposition`, `#numerical analysis`, `#machine learning`, `#history of mathematics`

---

<a id="item-6"></a>
## [躲避致命无人机：伪装无效](https://www.economist.com/science-and-technology/2026/07/08/how-to-hide-from-killer-drones) ⭐️ 8.0/10

《经济学人》文章探讨了用伪装躲避无人机的方法，但社区评论指出，现代机器视觉使这些技术失效，并建议改用主动防御系统如近程防御系统（CIWS）。 这场辩论突显了战争中的关键转变：AI 驱动的无人机探测正在超越传统伪装，迫使军队和平民重新考虑生存策略。讨论也凸显了反无人机技术日益增长的重要性。 社区指出，历史上用于迷惑人类视觉的炫目伪装可以迷惑民用大语言模型，但无法骗过专用机器视觉模型，这些模型能轻松锁定方形轮廓。有人提议使用能够覆盖整个半球并同时攻击多个无人机的近程防御系统。

hackernews · pseudolus · 7月11日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=48874357)

**背景**: 无人机，尤其是小型四轴飞行器，在战场上构成日益增长的威胁，并已被用于攻击。传统伪装针对人眼设计，但基于 AI 的探测器利用深度学习通过形状、运动和热信号识别目标。主动防御系统（APS）已用于装甲车辆拦截火箭和导弹，类似技术可被改造用于反无人机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mdpi.com/2504-446X/8/11/643">Vision-Based Drone Detection in Complex Environments: A Survey</a></li>
<li><a href="https://ipsjcva.springeropen.com/articles/10.1186/s41074-019-0059-x">Deep learning-based strategies for the detection and tracking of drones using several cameras | IPSJ Transactions on Computer Vision and Applications | Full Text</a></li>
<li><a href="https://www.twz.com/tank-active-protection-systems-could-be-used-shoot-down-drones">Tank Active Protection Systems Could Be Used To Shoot Down Drones</a></li>

</ul>
</details>

**社区讨论**: 评论对伪装的有效性持怀疑态度。网友 orthoxerox 认为炫目伪装无效，因为机器视觉锁定形状。iFire 分享了一个项目，展示无人机能看穿墙壁。不过，也有评论开玩笑说斑马条纹能驱赶马蝇。总体而言，大家认为主动防御比躲藏更可行。

**标签**: `#drones`, `#military technology`, `#computer vision`, `#countermeasures`

---

<a id="item-7"></a>
## [Qwen3.6 35B-A3B 单提示生成飞行模拟器](https://www.reddit.com/r/LocalLLaMA/comments/1utb6io/qwen36_35ba3b_q8_0_no_kv_quant_single_prompt_in/) ⭐️ 8.0/10

一位 Reddit 用户展示，Qwen3.6 35B-A3B 在采用 Q8_0 CPU 量化后，能够根据单个提示在 opencode 中生成包含山脉、云朵和无限程序化地形的完整飞行模拟器 HTML 文件。该用户指出，从 GPU 上的 Q4_K_M 切换至 CPU 上的 Q8_0 后性能显著提升。 这表明，采用适当量化的本地 LLM 在复杂代码生成方面可与云端模型媲美，使个人开发者和爱好者更容易获得先进的 AI 能力。同时，这也凸显了量化选择对特定任务性能的重要性。 该用户首先使用了计划模式，然后指示模型无需更改即实现。他们强调，尽管速度较慢，但 CPU 上的 Q8_0 量化相比 GPU 上的 Q4_K_M 显著提升了输出质量。

reddit · r/LocalLLaMA · /u/_TheWolfOfWalmart_ · 7月11日 05:24

**背景**: Qwen3.6 35B-A3B 是一种稀疏混合专家（MoE）模型，总参数量为 350 亿，但仅有 30 亿活跃参数，专为高效代理编码而设计。量化通过降低数值精度来减小模型大小并加速推理，但像 Q8_0 这样的高精度格式比 Q4_K_M 等低精度格式保留了更多准确性。此演示表明，对于某些创意任务，采用更高精度的 CPU 推理可以胜过 GPU 加速的低精度推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qwen.ai/blog?id=qwen3.6-35b-a3b">Qwen3.6-35B-A3B: Agentic Coding Power, Now Open to All</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-35B-A3B">Qwen/Qwen3.6-35B-A3B · Hugging Face</a></li>
<li><a href="https://medium.com/@paul.ilvez/demystifying-llm-quantization-suffixes-what-q4-k-m-q8-0-and-q6-k-really-mean-0ec2770f17d3">Demystifying LLM Quantization Suffixes: What Q4_K_M, Q8_0, and ... - Medium</a></li>

</ul>
</details>

**标签**: `#LLM`, `#code generation`, `#local AI`, `#Qwen`

---

<a id="item-8"></a>
## [100 美元超预算 20GB 显存方案](https://www.reddit.com/r/LocalLLaMA/comments/1utwqf8/ultra_budget_20gb_vram_with_448gbs_for_100_bucks/) ⭐️ 8.0/10

一位 Reddit 用户展示了一种双 NVIDIA P102-100 GPU 配置，仅需 100 美元即可提供 20GB 显存和 448GB/s 带宽，支持最多三个并发用户进行高效的本地大语言模型推理。 该方案提供了极高的显存价格比，使预算有限的用户能够进行本地大语言模型推理，可能让原本需要昂贵硬件的模型变得更加普及。 P102-100 是 2018 年发布的专业 GPU，每张卡配备 5GB GDDR5X 显存，合计 448GB/s 的带宽可与更昂贵的消费级显卡媲美。该方案使用 llama.cpp 运行，支持 3 个槽位和 32768 token 的上下文长度。

reddit · r/LocalLLaMA · /u/Boricua-vet · 7月11日 21:49

**背景**: NVIDIA P102-100 是一款基于 GP102 架构的专业挖矿 GPU，拥有 3200 个 CUDA 核心和 250W TDP。由于其挖矿专用设计缺乏视频输出接口，在二手市场上价格低廉。双卡配置可通过 NVLink 或 PCIe 桥接，在推理场景中实现显存池化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techpowerup.com/gpu-specs/p102-100.c3100">NVIDIA P102-100 Specs | TechPowerUp GPU Database</a></li>

</ul>
</details>

**标签**: `#budget build`, `#local LLM`, `#GPU`, `#inference`, `#VRAM`

---

<a id="item-9"></a>
## [美国科技业对中国开源 AI 模型的崛起感到焦虑](https://www.reddit.com/r/LocalLLaMA/comments/1uthozd/the_us_tech_industry_is_increasingly_anxious/) ⭐️ 8.0/10

美国科技行业日益担忧中国开源 AI 模型不断增强的实力和极具竞争力的价格，并质疑特朗普政府是否会通过新的行政命令来应对。 这一发展可能重塑全球 AI 格局，因为中国廉价而强大的开源模型挑战了美国的领先地位，并可能引发影响整个开源 AI 生态系统的监管行动。 Politico 的报道指出，担忧不仅涉及技术能力，还包括定价——中国模型以更低成本提供具有竞争力的性能，并且业界正关注类似以往 AI 相关指令的潜在行政命令。

reddit · r/LocalLLaMA · /u/Nunki08 · 7月11日 11:34

**背景**: 开源 AI 模型是任何人都可以使用、修改和分发的公开软件。中国近期发布了几个高性能的开源模型，如 DeepSeek，其效率和低成本令全球 AI 界惊讶。特朗普政府此前曾发布关于 AI 安全与竞争力的行政命令，针对开源模型的新命令可能影响全球这类技术的共享与开发。

**标签**: `#AI`, `#open-source`, `#US-China competition`, `#policy`, `#Trump administration`

---

<a id="item-10"></a>
## [RTX 5090 vs 6000 Pro：分流改装基准测试结果](https://www.reddit.com/r/LocalLLaMA/comments/1utvbey/performance_comparison_on_full_compute/) ⭐️ 8.0/10

一位 Reddit 用户对分流改装并水冷的 RTX 6000 PRO MaxQ 与常规及超频的 RTX 5090 和 RTX 6000 PRO WS 进行了详细的 LLM 推理和完整计算（Anima）性能对比。改装后的 MaxQ 在 600W 功耗下性能最佳，比 RTX 5090 快 12.8%。 该对比为希望通过分流改装和水冷等硬件修改最大化 AI 工作负载 GPU 性能的爱好者和专业人士提供了宝贵的实证数据。它表明，去除功耗限制后，经过筛选的专业 GPU 可以显著超越消费旗舰产品，挑战高端消费显卡的性价比。 分流改装涉及更换电阻（R002），使 RTX 6000 PRO MaxQ 功耗达到 600W，水冷将温度控制在 60°C。测试使用了特定软件版本（Torch 2.14.0、Sageattention 2.1、Forge Neo），并包含使用 llama.cpp 在 Kimi K2 2.5 和 GLM 5.1 等模型上的 LLM 基准测试。

reddit · r/LocalLLaMA · /u/panchovix · 7月11日 20:49

**背景**: 分流改装是一种硬件修改，通过添加电阻让 GPU 误以为功耗更低，从而实现更高功耗和超频。水冷用于管理增加的热量。RTX 6000 PRO MaxQ 是一款经过筛选的工作站 GPU，在低功耗下具有高时钟频率，而 RTX 5090 是消费旗舰。Anima 基准测试可能指计算密集型任务，LLM 测试通过将模型层卸载到 CPU 使 GPU 成为计算瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/shunt-modded-air-cooled-rtx-5090-achieves-top-rankings-in-3dmark-tests/">Shunt Modded Air-Cooled RTX 5090 Achieves Top Rankings In...</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/nvidia-rtx-5090-beats-rtx-pro-6000-in-tests-after-shunt-mod-to-a-staggering-800w-consumer-flagship-barely-scrapes-past-the-usd10-000-pro-despite-eye-watering-power-modification">Nvidia RTX 5090 beats RTX Pro 6000 in tests after shunt mod to...</a></li>
<li><a href="https://github.com/BlackSnowSkill/ANIMA_BOOSTER">GitHub - BlackSnowSkill/ANIMA_BOOSTER: High-performance optimization ...</a></li>

</ul>
</details>

**标签**: `#GPU performance`, `#LLM inference`, `#hardware modding`, `#AI compute`, `#benchmarking`

---

<a id="item-11"></a>
## [Qwen3 30B A3B 在 RTX 5060 Ti 上达到 50 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1utefpr/running_qwen3_30b_a3b_at_50_toks_on_rtx_5060_ti/) ⭐️ 8.0/10

一个自定义的 CUDA/C++ 推理引擎 garlic-inference 在 RTX 5060 Ti（16GB VRAM）上以 float8 精度运行 Qwen3-30B-A3B 时，达到了 50-54 tok/s 的速度，比 llama.cpp 快了 50%。 这表明大型 MoE 模型可以在消费级硬件上高效运行，从而实现私有、低成本、节能的本地推理，无需依赖云端数据中心。 加速来源于结合了 NeurIPS、ICML 和 EuroSys 论文中的最新技术。Qwen3-30B-A3B 模型共有 30.5B 参数，但由于其混合专家（MoE）架构，每个 token 仅激活约 3.3B 参数。

reddit · r/LocalLLaMA · /u/Azazelionide · 7月11日 08:29

**背景**: 像 Qwen3-30B-A3B 这样的混合专家（MoE）模型通过稀疏激活来减少计算量，但高效推理仍需优化内核。Float8（FP8）精度可将内存使用减半并提高吞吐量，同时精度损失很小。llama.cpp 通常通过 --n-cpu-moe 标志将 MoE 专家层卸载到 CPU，但自定义 CUDA 代码可以更好地利用 GPU 显存和算力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3-30B-A3B">Qwen/Qwen3-30B-A3B · Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/floating-point-8-an-introduction-to-efficient-lower-precision-ai-training/">Floating-Point 8: An Introduction to Efficient, Lower-Precision AI ...</a></li>
<li><a href="https://dev.to/someoddcodeguy/understanding-moe-offloading-5co6">Understanding MoE Offloading - DEV Community</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#inference-optimization`, `#cuda`, `#moe`, `#qwen3`

---

<a id="item-12"></a>
## [SQLite/FTS5 专利数据库从 350 万条扩展到 536 万条的优化经验](https://www.reddit.com/r/LocalLLaMA/comments/1utl6r5/followup_what_i_learned_scaling_a_sqlitefts5/) ⭐️ 8.0/10

一位专利律师记录了将 SQLite/FTS5 全文搜索专利数据库从 350 万条扩展到 536 万条的实用优化技巧，包括使用 ANALYZE、避免宽行更新，以及在 BM25 查询中优先使用 AND 而非 OR。 这为任何管理大规模 SQLite 全文搜索数据库的人员提供了可操作的见解，展示了精心优化即使在消费级硬件上也能显著提升查询性能。 批量加载后运行 ANALYZE，将一个包含 1.08 亿行引文表的相关 EXISTS 查询从 34 秒优化到 0.16 秒。平均 19KB 的宽行导致批量更新重写整个 119GB 表，因此推荐使用侧表加 JOIN 的方式。

reddit · r/LocalLLaMA · /u/Impressive_Tower_550 · 7月11日 14:11

**背景**: SQLite 是一种轻量级嵌入式 SQL 数据库引擎，FTS5 是其全文搜索扩展，使用 BM25 排序算法。ANALYZE 命令创建统计信息，帮助查询优化器选择更好的索引。BM25 是一种基于词频和逆文档频率对文档进行评分的排序函数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sqlite.org/docs.html">SQLite Documentation</a></li>
<li><a href="https://arrizza.com/test-bm25.html">A discussion and project showing how to use BM 25 for page ranking</a></li>

</ul>
</details>

**标签**: `#SQLite`, `#FTS5`, `#database optimization`, `#patents`, `#full-text search`

---

<a id="item-13"></a>
## [Rasbt 在 LLMs-from-Scratch 仓库中创建新分支](https://github.com/rasbt/LLMs-from-scratch) ⭐️ 7.0/10

Sebastian Raschka（rasbt）在 GitHub 上的 LLMs-from-Scratch 仓库中创建了一个新分支，表明正在进行开发或实验。 该仓库提供了从零开始用 PyTorch 构建类似 ChatGPT 的大语言模型的分步指南，是深度学习从业者的宝贵教育资源。 该仓库位于 https://github.com/rasbt/LLMs-from-scratch，分支创建可能包含新功能、错误修复或替代实现。

github · rasbt · 7月11日 15:05

**背景**: LLMs-from-scratch 是一个教程仓库，教授如何使用 PyTorch 实现类似 ChatGPT 的大语言模型（LLM）。它涵盖从数据准备到训练和推理的各个阶段，使复杂概念对学习者易于理解。在仓库中创建分支通常允许在不影响主代码库的情况下进行并行开发。

**标签**: `#LLM`, `#PyTorch`, `#tutorial`, `#deep learning`

---

<a id="item-14"></a>
## [Ollama v0.32.0-rc0 新增 Qwen3.5 解析器和代理界面](https://github.com/ollama/ollama/releases/tag/v0.32.0-rc0) ⭐️ 7.0/10

该候选版本引入了针对 Qwen3.5 模型系列的专用解析器和渲染器、新的代理用户界面，以及对过时代理模型的警告提示。 这些新增功能使用户更容易正确渲染运行 Qwen3.5，并通过内置界面与 AI 代理交互，从而提升本地大语言模型的可用性。 代理界面是命令行界面的一部分，对旧代理模型的警告有助于用户避免兼容性问题。该版本还包括其他修复和改进（详见完整变更日志）。

github · github-actions[bot] · 7月11日 01:03

**背景**: Ollama 是一款流行的开源工具，可在个人电脑上本地运行大语言模型（LLM）。Qwen3.5 是阿里云开发的开源大语言模型系列。代理界面允许用户通过可视化界面与 AI 代理（例如用于工具使用和多步推理）进行交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/library/qwen3.5">qwen3.5</a></li>
<li><a href="https://cohorte.co/blog/deep-dive-building-a-self-hosted-ai-agent-with-ollama-and-open-webui">Build a Self-Hosted AI Agent: Ollama + Open WebUI in 30 Minutes — Cohorte</a></li>

</ul>
</details>

**标签**: `#ollama`, `#LLM`, `#release-candidate`, `#agent`, `#Qwen`

---

<a id="item-15"></a>
## [别再叫我去问 LLM 了](https://blog.yaelwrites.com/stop-telling-me-to-ask-an-llm/) ⭐️ 7.0/10

作者认为，当对方已经问过 LLM 时，再叫他们去问 LLM 是一种敷衍的态度，并建议更有效的回应方式，比如询问他们得到的答案或直接提供帮助。 这揭示了技术社区中日益严重的沟通问题：默认建议对方去问 LLM 可能会削弱真正的知识共享，并让已经做过研究的人感到沮丧。 文章强调，回应者应假设提问者已经尝试过查询 LLM，并针对他们仍然存在的疑问或具体背景进行交流。

hackernews · theorchid · 7月11日 22:28 · [社区讨论](https://news.ycombinator.com/item?id=48876441)

**背景**: LLM（大型语言模型）如 ChatGPT 和 Claude 能生成类似人类的文本，常被用作快速获取答案的工具。在技术社区中，人们常以“去问 LLM”来回复问题，但如果提问者已经问过，这种回应就显得敷衍。本文呼吁更尊重和协作的回应方式。

**社区讨论**: HN 评论者大多赞同作者观点，并提出了实用建议：先说明自己已做过研究，用“LLM 怎么说的？”这样的跟进问题代替命令式回复，并承认有时 LLM 确实能给出最佳答案。

**标签**: `#LLM`, `#communication`, `#tech community`, `#AI assistance`, `#knowledge sharing`

---

<a id="item-16"></a>
## [ClickHouse 通过 SO_REUSEPORT 和 Peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 7.0/10

ClickHouse 工程师通过启用 SO_REUSEPORT 实现多进程套接字监听，并实施连接 Peering 以正确转发取消请求，从而将 PostgreSQL 连接池 PgBouncer 的吞吐量提升了 4 倍。 这项优化显著提高了 PgBouncer 的可扩展性，对高流量 PostgreSQL 部署至关重要，并且所展示的技术可应用于其他连接池以提升性能。 SO_REUSEPORT 允许多个 PgBouncer 进程监听同一端口，由内核分配传入连接；而 Peering 确保取消请求能被转发到拥有该会话的正确进程。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是 PostgreSQL 的轻量级连接池，用于减少频繁新建连接的开销。传统上它以单进程运行，在高负载下可能成为瓶颈。SO_REUSEPORT 是 Linux 套接字选项，允许多个服务器进程绑定到同一端口；而 Peering 则允许在进程间协调取消请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.f5.com/company/blog/nginx/socket-sharding-nginx-release-1-9-1">Socket Sharding in NGINX Release 1.9.1 | F5</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://www.mankier.com/1/pgbouncer">pgbouncer : lightweight connection pooler for PostgreSQL | ManKier</a></li>

</ul>
</details>

**社区讨论**: 评论者提到了 Odyssey 和 pgdog 等替代连接池，并对 Peering 的配置表示兴趣。有人询问 PostgreSQL 是否有内置的 Peering 支持，也有人指出在 Kubernetes 中运行多个 PgBouncer 进程很方便。

**标签**: `#postgresql`, `#connection-pooling`, `#performance`, `#pgbouncer`

---

<a id="item-17"></a>
## [在 SQLite 中优先使用 STRICT 表](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

Evan Hahn 的一篇博客文章主张在 SQLite 中使用 STRICT 表来强制执行类型安全，为希望提高数据完整性的开发者提供了实用建议。 STRICT 表解决了 SQLite 灵活类型这一长期缺陷，使其更适合需要严格数据验证和一致性的应用。 STRICT 表在 SQLite 3.37.0 版本（2021 年 11 月）中引入，强制执行静态类型，如果数据无法无损转换为声明的列类型，则会报错。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 传统上使用类型亲和力，允许将不同类型的值存储在同一列中，这可能导致数据完整性问题。STRICT 表提供了一种可选机制来强制执行类型，类似于其他 SQL 数据库，同时保持向后兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables - SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了争论：一些开发者强烈希望将 STRICT 设为默认，而另一些人引用 SQLite 官方'flextypegood'文档，认为灵活类型对某些用例有益。评论者还指出 STRICT 表缺少 DATE 等数据类型，这可能是一个限制。

**标签**: `#SQLite`, `#Database`, `#Strict Tables`, `#Type Enforcement`, `#Software Engineering`

---

<a id="item-18"></a>
## [llama.cpp b9966 缓存正则表达式以提升性能](https://www.reddit.com/r/LocalLLaMA/comments/1utyzbl/llamacpp_b9966_for_smtensor/) ⭐️ 7.0/10

llama.cpp b9966 的修复缓存了正则表达式，从而避免了解码线程上每个张量每个 token 的 29 次重复编译，减少了 CPU 浪费。 对于使用 -sm tensor 标志的生产部署，此优化通过消除解码线程上冗余的正则表达式编译开销来提高推理效率，这对吞吐量至关重要。 正则表达式曾为每个 token 的每个张量从头重建；修复将其缓存一次，保持相同行为同时减少解码线程上的 CPU 使用。

reddit · r/LocalLLaMA · /u/Bulky-Priority6824 · 7月11日 23:28

**背景**: llama.cpp 是一个用 C/C++ 编写的项目，用于在各种硬件上本地运行 LLM 推理。-sm tensor 标志可使用 NCCL 实现跨多 GPU 的张量并行。在逐个 token 生成过程中，解码线程处理张量，而重复的正则表达式编译是最近一次变更中引入的低效问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/docs/multi-gpu.md">llama.cpp/docs/multi-gpu.md at master · ggml-org/llama.cpp</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/issues/22268">Eval bug: llama-server crash on generation using "-sm tensor" · Issue #22268 · ggml-org/llama.cpp</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#performance optimization`, `#regex caching`, `#LLM inference`, `#local LLM`

---

<a id="item-19"></a>
## [双 GPU PCIe 传输基准测试：张量并行与流水线并行对比](https://www.reddit.com/r/LocalLLaMA/comments/1utz50z/measuring_pcie_transfer_under_dual_gpu_with/) ⭐️ 7.0/10

一位 Reddit 用户使用两块 GPU（RTX 3090 和 Titan RTX）在 llama.cpp 中测量了张量并行和流水线并行下的 PCIe 传输速率。张量并行解码速度为 47 t/s，流水线为 30 t/s；而流水线预填充速度为 1250 t/s，张量为 650 t/s。 这些实测数据有助于多 GPU 大模型推理用户在并行策略之间做出选择，并评估 PCIe 延长线是否成为瓶颈。结果表明 PCIe 3.0 x16 并未饱和，支持使用更便宜的延长线。 测试使用 Qwen3.6-27B-UD-Q4_K_XL.gguf 模型，上下文长度 180k，系统为 Ubuntu 24.04。通过 nvidia-smi dmon -s t 监控 PCIe 带宽。张量并行在解码期间有持续传输，而流水线并行传输量非常低。

reddit · r/LocalLLaMA · /u/nick_ziv · 7月11日 23:35

**背景**: 张量并行将模型层拆分到多个 GPU 上，需要频繁的 GPU 间通信。流水线并行也将模型层拆分，但通信频率较低。PCIe 带宽对大模型推理中的多 GPU 性能至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/deploy/nvidia-smi/index.html">docs.nvidia.com/deploy/ nvidia - smi /index.html</a></li>
<li><a href="https://www.microway.com/hpc-tech-tips/nvidia-smi_control-your-gpus/">nvidia - smi : Control Your GPUs - Microway</a></li>
<li><a href="https://bentoml.com/llm/inference-optimization/data-tensor-pipeline-expert-hybrid-parallelism">Data, tensor, pipeline, expert and hybrid parallelisms | LLM Inference Handbook</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#PCIe`, `#multi-GPU`, `#tensor parallelism`, `#pipeline parallelism`

---