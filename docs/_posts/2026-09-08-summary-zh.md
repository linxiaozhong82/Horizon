---
layout: default
title: "Horizon Summary: 2026-09-08 (ZH)"
date: 2026-09-08
lang: zh
---

> 从 34 条内容中筛选出 8 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：quantization、local-llm、LLM、efficient-ai、game-development。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[任务感知量化将 Qwen3.8-27B 压缩至 15%体积并保留 99%推理性能](https://www.reddit.com/r/LocalLLaMA/comments/1wa5dp9/my_qwen3827b_taskaware_quant_reaches_99_of_bf16/)**
2. **[《Warrior Quest》本地 LLM 驱动 NPC，游戏状态保持确定性的黑暗奇幻 RPG](https://www.reddit.com/r/LocalLLaMA/comments/1wa84sa/i_made_warrior_quest_a_local_llmpowered/)**
3. **[OpenBMB 发布 MiniCPM5-2B，成为 4B 以下开放模型中的智能指数第一](https://www.reddit.com/r/LocalLLaMA/comments/1w9skjz/minicpm52b_release_day/)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI 安全与软件治理

- **关联热点**: [Creepy crawlies](https://simonwillison.net/2026/Sep/7/creepy-crawlies/)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 2. 算力芯片与服务器

- **关联热点**: [任务感知量化将 Qwen3.8-27B 压缩至 15%体积并保留 99%推理性能](https://www.reddit.com/r/LocalLLaMA/comments/1wa5dp9/my_qwen3827b_taskaware_quant_reaches_99_of_bf16/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：任务感知量化将 Qwen3.8-27B 压缩至 15%体积并保留 99%推理性能

**关联新闻**: [任务感知量化将 Qwen3.8-27B 压缩至 15%体积并保留 99%推理性能](https://www.reddit.com/r/LocalLLaMA/comments/1wa5dp9/my_qwen3827b_taskaware_quant_reaches_99_of_bf16/)

**切入角度**: 开发者 ByteOtter 发布了任务感知量化流水线 TAK（Task Aware Knapsack）。其 Qwen3.8-27B 的 TAK 量化在推理基准上得分 82.81%，约为 BF16 基线（83.59%）的 99%，而体积仅为后者的约 15%。 这一结果表明，针对任务的精度分配可以在激进压缩下接近无损推理，使高质量本地大模型更有可能部署在消费级硬件上。它也为量化推理模型树立了效率基准，并表明该思路有望扩展到编码和数学等领域。 TAK 基于任务相关语料库构建 imatrix（重要性矩阵），并通过背包式分配在字节预算内对各张量进行升/降级，不涉及剪枝、微调或模型融合。作者称 TAK 在 Qwen3.5-4B、Gemma 4 E4B 和 Gemma 3 4B QAT 上均超过 Unsloth Dynamic，但编码任务可能出现重复循环。

**可延展方向**: 量化是将大语言模型的权重压缩为更少的比特来表示。在极低比特率下，通用的“一刀切”量化容易严重损害模型能力；IQ2_S 是 llama.cpp 等工具支持的一种约 2.5 bpw 的 GGUF 格式，常作为低比特量化基线。任务感知量化会根据校准数据或目标任务调整压缩策略，而 TAK 进一步在严格字节预算内按张量分配精度，把有限比特留给最容易受损的部分。

---

### 选题 2：《Warrior Quest》本地 LLM 驱动 NPC，游戏状态保持确定性的黑暗奇幻 RPG

**关联新闻**: [《Warrior Quest》本地 LLM 驱动 NPC，游戏状态保持确定性的黑暗奇幻 RPG](https://www.reddit.com/r/LocalLLaMA/comments/1wa84sa/i_made_warrior_quest_a_local_llmpowered/)

**切入角度**: 开发者 Rikkendo 在 Steam 上发布了《Warrior Quest》的可玩演示版。这是一款黑暗奇幻 RPG，完全离线运行，用本地 LLM 仅模拟 NPC 对话，而游戏状态、任务和剧情由确定性系统控制。演示包含约 60–90 分钟内容，需要至少 8 GB 显存的 GPU。 这种混合架构解决了 LLM 驱动游戏面临的一个关键可靠性问题：实际游戏状态保持确定性，可防止模型破坏逻辑或世界观，同时玩家仍能像在桌游中那样与 NPC 自由对话。它为希望在保持作者控制的同时实现沉浸式 AI 对话的独立开发者提供了一种实用范式。 所有美术、剧情、音乐、音效和基础配音均由开发者一人完成，NPC 对话使用基于其本人配音训练的 TTS 生成。游戏不需要 API key 或云端 LLM；该帖子是开发者本人的自荐帖，他同时也是桌游城主（DM）和软件工程师。

**可延展方向**: 本地 LLM 是完全在用户自有硬件上运行的大型语言模型，而非依赖云端服务器，从而带来隐私性好、可离线使用和延迟低等优点。在游戏设计中，生成式模型能创造动态对话，但也可能产生与游戏状态和剧情相矛盾的幻觉内容。《Warrior Quest》通过将模型限制在 NPC 角色扮演、让传统确定性系统掌管世界逻辑，从而规避了这一问题。

---

### 选题 3：OpenBMB 发布 MiniCPM5-2B，成为 4B 以下开放模型中的智能指数第一

**关联新闻**: [OpenBMB 发布 MiniCPM5-2B，成为 4B 以下开放模型中的智能指数第一](https://www.reddit.com/r/LocalLLaMA/comments/1w9skjz/minicpm52b_release_day/)

**切入角度**: OpenBMB 发布了 MiniCPM5-2B，这是一个 2.52B 参数的稠密开放权重模型。它在 Artificial Analysis Intelligence Index v4.2 上获得 15 分，是 4B 参数及以下开放权重模型中的最高分。 这表明紧凑的端侧模型无需数据中心 GPU 也能提供强大的推理和智能体性能。它为开发者在本地助手、编程智能体和工具调用流程上提供了一个强大的 Apache-2.0 选项。 MiniCPM5-2B 是一个稠密模型，拥有 19.8 亿非嵌入参数、131,072 token 的上下文窗口、混合 Think/No-Think 推理和原生工具调用能力。该模型 token 效率较高，每个智能指数任务约使用 19,000 个输出 token，而 Ling 3.0 Tiny 需要 56,000 个。

**可延展方向**: MiniCPM 是 OpenBMB 推出的端侧大语言模型系列，旨在运行在手机、笔记本电脑等边缘硬件上。Artificial Analysis Intelligence Index 是对涵盖智能体、编程、通用能力和科学推理的生产基准进行加权平均得到的分数，范围从 0 到 100。MiniCPM5-2B 延续了这一系列，以紧凑的稠密设计面向本地助手、编程智能体、工具调用和推理场景。

---

1. [任务感知量化将 Qwen3.8-27B 压缩至 15%体积并保留 99%推理性能](#item-1) ⭐️ 8.0/10
2. [《Warrior Quest》本地 LLM 驱动 NPC，游戏状态保持确定性的黑暗奇幻 RPG](#item-2) ⭐️ 8.0/10
3. [bzip3 压缩工具引发基准公平性与软件支持的讨论](#item-3) ⭐️ 7.0/10
4. [Creepy crawlies](#item-4) ⭐️ 7.0/10
5. [OpenBMB 发布 MiniCPM5-2B，成为 4B 以下开放模型中的智能指数第一](#item-5) ⭐️ 7.0/10
6. [DeepSeek-V4-Flash-Vision-Exp 用截图迭代创建游戏世界的演示](#item-6) ⭐️ 7.0/10
7. [exllamav3 在 CPU 卸载推理基准测试中胜过 llama.cpp](#item-7) ⭐️ 7.0/10
8. [非官方 llama.cpp 分支让 Strix Halo 解码速度达到 60 t/s](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [任务感知量化将 Qwen3.8-27B 压缩至 15%体积并保留 99%推理性能](https://www.reddit.com/r/LocalLLaMA/comments/1wa5dp9/my_qwen3827b_taskaware_quant_reaches_99_of_bf16/) ⭐️ 8.0/10

开发者 ByteOtter 发布了任务感知量化流水线 TAK（Task Aware Knapsack）。其 Qwen3.8-27B 的 TAK 量化在推理基准上得分 82.81%，约为 BF16 基线（83.59%）的 99%，而体积仅为后者的约 15%。 这一结果表明，针对任务的精度分配可以在激进压缩下接近无损推理，使高质量本地大模型更有可能部署在消费级硬件上。它也为量化推理模型树立了效率基准，并表明该思路有望扩展到编码和数学等领域。 TAK 基于任务相关语料库构建 imatrix（重要性矩阵），并通过背包式分配在字节预算内对各张量进行升/降级，不涉及剪枝、微调或模型融合。作者称 TAK 在 Qwen3.5-4B、Gemma 4 E4B 和 Gemma 3 4B QAT 上均超过 Unsloth Dynamic，但编码任务可能出现重复循环。

reddit · r/LocalLLaMA · /u/devildip · 9月7日 21:42

**背景**: 量化是将大语言模型的权重压缩为更少的比特来表示。在极低比特率下，通用的“一刀切”量化容易严重损害模型能力；IQ2_S 是 llama.cpp 等工具支持的一种约 2.5 bpw 的 GGUF 格式，常作为低比特量化基线。任务感知量化会根据校准数据或目标任务调整压缩策略，而 TAK 进一步在严格字节预算内按张量分配精度，把有限比特留给最容易受损的部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2609.01587">The Structure of Quantization Damage in LLMs: Why the Next Bit...</a></li>
<li><a href="https://kaitchup.substack.com/p/choosing-a-gguf-model-k-quants-i">GGUF Quantization Compared: Q4_K_M vs IQ4_XS vs IQ4_NL</a></li>

</ul>
</details>

**社区讨论**: 帖子作者提到，一些社区成员尝试用这种面向推理的量化模型跑编码任务时遇到重复循环，作者表示将复现并刻画这一失败模式。原始材料中没有提供更详细的顶层评论内容。

**标签**: `#quantization`, `#efficient-ai`, `#local-llm`, `#model-compression`, `#reasoning`

---

<a id="item-2"></a>
## [《Warrior Quest》本地 LLM 驱动 NPC，游戏状态保持确定性的黑暗奇幻 RPG](https://www.reddit.com/r/LocalLLaMA/comments/1wa84sa/i_made_warrior_quest_a_local_llmpowered/) ⭐️ 8.0/10

开发者 Rikkendo 在 Steam 上发布了《Warrior Quest》的可玩演示版。这是一款黑暗奇幻 RPG，完全离线运行，用本地 LLM 仅模拟 NPC 对话，而游戏状态、任务和剧情由确定性系统控制。演示包含约 60–90 分钟内容，需要至少 8 GB 显存的 GPU。 这种混合架构解决了 LLM 驱动游戏面临的一个关键可靠性问题：实际游戏状态保持确定性，可防止模型破坏逻辑或世界观，同时玩家仍能像在桌游中那样与 NPC 自由对话。它为希望在保持作者控制的同时实现沉浸式 AI 对话的独立开发者提供了一种实用范式。 所有美术、剧情、音乐、音效和基础配音均由开发者一人完成，NPC 对话使用基于其本人配音训练的 TTS 生成。游戏不需要 API key 或云端 LLM；该帖子是开发者本人的自荐帖，他同时也是桌游城主（DM）和软件工程师。

reddit · r/LocalLLaMA · /u/Rikkendo · 9月7日 23:37

**背景**: 本地 LLM 是完全在用户自有硬件上运行的大型语言模型，而非依赖云端服务器，从而带来隐私性好、可离线使用和延迟低等优点。在游戏设计中，生成式模型能创造动态对话，但也可能产生与游戏状态和剧情相矛盾的幻觉内容。《Warrior Quest》通过将模型限制在 NPC 角色扮演、让传统确定性系统掌管世界逻辑，从而规避了这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@arjunrao87/what-are-llms-local-llms-and-rag-0198868f8657">What are LLMs, Local LLMs and RAG? | by Arjun Rao | Medium</a></li>
<li><a href="https://scrapfly.io/blog/posts/guide-to-local-llm">Guide to Local LLMs</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#game-development`, `#llm-architecture`, `#deterministic-gameplay`, `#rpg`

---

<a id="item-3"></a>
## [bzip3 压缩工具引发基准公平性与软件支持的讨论](https://github.com/iczelia/bzip3) ⭐️ 7.0/10

一场高参与的 Hacker News 讨论聚焦于开源压缩工具 bzip3（自称 bzip2 的更强继承者）：支持者称赞其压缩率更高，但批评者认为其公开基准测试采用了不公平的参数设置。 压缩率和速度的选择直接影响存储成本与数据处理流程，因此这场争论对管理大型文本或代码档案以及 JSONL 数据集的开发者很重要。它也暴露出生态系统中一个反复出现的问题：像 lzma 和 bzip3 这样压缩率更高的算法，往往缺少 gzip 那样的透明工具支持。 批评者指出，bzip3 的基准测试将块大小设为 512 MB，而 zstd 仍使用默认的 8 MB 窗口；由多个 Perl 源码版本拼接成的语料库又特别有利于 BWT 的长距离匹配。bzip3 的压缩流程结合了 CRC32、RLE、LZP、BWT 与算术编码器，并且项目提供了多线程的压缩与解压实现。

hackernews · tosh · 9月7日 13:35 · [社区讨论](https://news.ycombinator.com/item?id=49598291)

**背景**: bzip3 是由 Kamila Szewczyk 开发的开源免费数据压缩工具，定位为 bzip2 的“精神继承者”。与 bzip2 一样，它基于 Burrows-Wheeler 变换（BWT），擅长压缩文本和代码；但 bzip3 在 BWT 前增加了 LZP、RLE 等预处理阶段，并使用算术编码器来获得更高的压缩率。该项目还提供了压缩和解压的多线程实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/iczelia/bzip3">GitHub - iczelia/bzip3: A better and stronger spiritual ...</a></li>
<li><a href="https://handwiki.org/wiki/Software:Bzip3">Software:Bzip3 - HandWiki</a></li>
<li><a href="https://deepwiki.com/iczelia/bzip3/2-compression-algorithm">Compression Algorithm | iczelia/bzip3 | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 评论者观点分歧：有人说这些基准测试“不诚实”，属于“挑数据”，因为 zstd 的窗口大小没有按 bzip3 的 512 MB 块大小调整；也有人强调实际软件支持比压缩率更重要，例如 DuckDB 能透明读取 gzip，却缺少 bzip3 或 lzma 支持。还有人建议用 bzip3 压缩其自身发布归档作为现实基准，并希望看到 zstd 使用更大窗口的对比。

**标签**: `#compression`, `#bzip3`, `#benchmarking`, `#open-source`, `#algorithms`

---

<a id="item-4"></a>
## [Creepy crawlies](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 7.0/10

Konstantin Ryabitsev reports that abusive crawlers force git.kernel.org to spend more CPU rendering commits for scrapers than on legitimate git clone traffic across all nodes.

rss · Simon Willison · 9月7日 23:08

**标签**: `#crawling`, `#web scraping`, `#Linux kernel`, `#server infrastructure`, `#security`

---

<a id="item-5"></a>
## [OpenBMB 发布 MiniCPM5-2B，成为 4B 以下开放模型中的智能指数第一](https://www.reddit.com/r/LocalLLaMA/comments/1w9skjz/minicpm52b_release_day/) ⭐️ 7.0/10

OpenBMB 发布了 MiniCPM5-2B，这是一个 2.52B 参数的稠密开放权重模型。它在 Artificial Analysis Intelligence Index v4.2 上获得 15 分，是 4B 参数及以下开放权重模型中的最高分。 这表明紧凑的端侧模型无需数据中心 GPU 也能提供强大的推理和智能体性能。它为开发者在本地助手、编程智能体和工具调用流程上提供了一个强大的 Apache-2.0 选项。 MiniCPM5-2B 是一个稠密模型，拥有 19.8 亿非嵌入参数、131,072 token 的上下文窗口、混合 Think/No-Think 推理和原生工具调用能力。该模型 token 效率较高，每个智能指数任务约使用 19,000 个输出 token，而 Ling 3.0 Tiny 需要 56,000 个。

reddit · r/LocalLLaMA · /u/Equivalent-Grass-527 · 9月7日 13:43

**背景**: MiniCPM 是 OpenBMB 推出的端侧大语言模型系列，旨在运行在手机、笔记本电脑等边缘硬件上。Artificial Analysis Intelligence Index 是对涵盖智能体、编程、通用能力和科学推理的生产基准进行加权平均得到的分数，范围从 0 到 100。MiniCPM5-2B 延续了这一系列，以紧凑的稠密设计面向本地助手、编程智能体、工具调用和推理场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/openbmb/MiniCPM5-2B">openbmb/MiniCPM5-2B · Hugging Face</a></li>
<li><a href="https://github.com/OpenBMB/MiniCPM">GitHub - OpenBMB/MiniCPM: MiniCPM5: SOTA on-device LLMs ... OpenBMB releases MiniCPM5-2B | Artificial Analysis MiniCPM5 - a openbmb Collection - Hugging Face OpenBMB Releases MiniCPM5-2B: A 2.52B Dense Model Averaging ... MiniCPM5-2B — a 2B open model that leads the… | AI/TLDR openbmb/MiniCPM5-2B | vLLM Recipes</a></li>
<li><a href="https://artificialanalysis.ai/articles/openbmb-releases-minicpm5-2b">OpenBMB releases MiniCPM5-2B | Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-weights`, `#small-model`, `#release`, `#benchmark`

---

<a id="item-6"></a>
## [DeepSeek-V4-Flash-Vision-Exp 用截图迭代创建游戏世界的演示](https://www.reddit.com/r/LocalLLaMA/comments/1wa06k3/deepseekv4flashvisionexp_is_amazing_at_creating/) ⭐️ 7.0/10

一位开发者报告称，DeepSeek-V4-Flash-Vision-Exp（DeepSeek V4-Flash 系列中首个支持视觉的模型）能够利用游戏截图来生成和修正素材、修复视觉故障并试玩测试机制。这套工作流在大约一个周末（两天的迭代）里便产出了一个完整的游戏世界。 这次亲身演示展示了一种实用工作流：本地多模态 LLM 为创意编程打通了视觉反馈回路。如果这套方法行之有效，将显著降低 AI 辅助游戏开发与素材制作所需的工作量。 据报道，该模型将 V4-Flash 的专家混合（MoE）主干与 32 层视觉塔相结合，支持 100 万 token 的上下文，并带有融合的 DSpark 草稿模块。作者在本地运行模型，没耐心时改用 API，并在发现笔记本上运行缓慢后补充了性能优化。

reddit · r/LocalLLaMA · /u/sloptimizer · 9月7日 18:27

**背景**: DeepSeek-V4-Flash-Vision-Exp 是 DeepSeek 首个实验性多模态模型，在原本仅支持文本的 V4-Flash 架构上增加了视觉理解能力。视觉语言模型（VLM）可同时接收图像与文本输入并输出文本，因此可以被用来读取截图以指导代码修改。作者此前曾用 Qwen3.8-Flash-Next 一次性生成 Cat-Hunt 游戏 demo，随后借助新的视觉模型对结果进行迭代改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek-ai/DeepSeek-V4-Flash-Vision-Exp · Hugging Face</a></li>
<li><a href="https://recipes.vllm.ai/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek-ai/DeepSeek-V4-Flash-Vision-Exp | vLLM Recipes</a></li>
<li><a href="https://huggingface.co/blog/vlms">Vision Language Models Explained</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#vision-language-model`, `#game-development`, `#AI-assisted-coding`, `#local-LLM`

---

<a id="item-7"></a>
## [exllamav3 在 CPU 卸载推理基准测试中胜过 llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1wa1jkb/exllamav3_comfortably_beats_llamacpp_running/) ⭐️ 7.0/10

在 Reddit 的帖子中，用户 Lowkey_LokiSN 报告称，exllamav3 在配备 CPU 卸载的双 RTX 3080 平台上运行 Qwen 3.8 Flash Next 时，解码速度约为 25 tps，预填充速度约为 870 tps；而 llama.cpp 的解码速度约 13 tps，预填充速度约 270 tps。用户还指出这种优势因模型而异，因为 GLM 5.3 Flash 的解码速度反而比 llama.cpp 慢约 2 倍。 这提供了具体的对比数据，表明在 CPU 卸载推理（一种常见的用于运行超出 GPU 显存容量的大模型的方案）中 exllamav3 可能优于 llama.cpp。同时这也说明用户应当针对不同模型分别测试推理引擎，因为没有任何一个推理库在各类模型上都是最快的。 用户强调该优势并不能推广到所有模型：在同一平台上，GLM 5.3 Flash 的 EXL3 量化版本解码速度比 llama.cpp 慢约 2 倍。用户还提醒，exllamav3 配合 TabbyAPI 的配置比 llama.cpp 更复杂，且解码速度需要经过数千个 token 的预热期才能达到峰值性能。

reddit · r/LocalLLaMA · /u/Lowkey_LokiSN · 9月7日 19:16

**背景**: 本地 LLM 推理通常借助量化来减小模型体积，使其适配消费级 GPU 显存。GGUF 是 llama.cpp 兼容引擎常用的量化格式，而 exllamav3 引入了基于 QTIP 的新 EXL3 格式，旨在提供更好的“体积—性能”权衡。当模型权重超过 GPU 显存时，就需要将部分模型交由系统内存和 CPU 处理，即 CPU 卸载，正如该帖子中双 RTX 3080 搭配 128GB DDR4 的平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/turboderp-org/exllamav3">GitHub - turboderp-org/ exllamav 3 : An optimized quantization and...</a></li>
<li><a href="https://ggufloader.github.io/what-is-gguf.html">What is GGUF? Complete Guide to GGUF Format & Quantization</a></li>
<li><a href="https://huggingface.co/collections/Volko76/exl3-quantizations-67f847ea38be0551016687dc">EXL 3 Quantizations - a Volko76 Collection</a></li>

</ul>
</details>

**标签**: `#exllamav3`, `#llama.cpp`, `#inference`, `#benchmark`, `#local LLM`

---

<a id="item-8"></a>
## [非官方 llama.cpp 分支让 Strix Halo 解码速度达到 60 t/s](https://www.reddit.com/r/LocalLLaMA/comments/1wa9m61/for_strix_halo_official_llamacpp_isnt_ideal_and/) ⭐️ 7.0/10

一位 Reddit 用户声称官方 llama.cpp 没有针对 AMD Strix Halo（gfx1150）优化，实际速度仅达到硬件理论性能的约 50%。该帖分享了三个替代分支，号称可将 Qwen3.8-Flash-Next 的解码速度提升到接近 60 tokens/s，预填速度提升到 600-1200 tokens/s，即理论吞吐量的 75%-90%。 这很重要，因为 Strix Halo 是适合本地运行大型模型的、性能最强的统一内存 AI 处理器之一，大幅提速能让本地推理变得实用得多。这也说明，针对新兴 GPU 架构定制修改的 llama.cpp 分支，能比官方版本带来非常大的性能提升。 帖子列出了三个分支：halogen-flash-server 仅针对 Strix Halo 和 Qwen3.8-Flash-Next 优化，被称为“Strix Halo 版 Ninfer”（约 90% 理论性能）；myhacsint 的 llama.cpp 实验分支（约 80% 理论性能）；以及 r/StrixHalo 最早出现、仍在持续更新的 strix-llama.cpp（约 75% 理论性能）。官方 llama.cpp 运行 Qwen38FN 时据称只有约 2 tokens/s 解码和约 20 tokens/s 预填，约为理论性能的 50%。

reddit · r/LocalLLaMA · /u/feelspeaceman · 9月8日 00:43

**背景**: AMD Strix Halo 以 Ryzen AI Max 品牌销售，是一款配备高性能 CPU、大型 Radeon 核显以及最高 128GB LPDDR5X 统一内存的 APU，因此非常适合在本地运行大型 LLM。llama.cpp 是一个广泛使用的本地 AI 模型 C++ 推理引擎，但其通用代码路径往往落后于针对特定架构的优化。Qwen3.8-Flash-Next 是一个开源权重多模态 MoE 模型，同时也是 Qwen4 架构的预览版本。Ninfer 是一个高性能单 GPU 推理项目，帖子中提到的其中一个 Strix Halo 分支以它为基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3.8-Flash-Next/">Qwen3.8-Flash-Next - GitHub</a></li>
<li><a href="https://github.com/Neroued/ninfer">GitHub - Neroued/ninfer: High-performance single-GPU ...</a></li>
<li><a href="https://www.amd.com/en/products/processors/desktops/ryzen/ryzen-ai-halo.html">AMD Ryzen™ AI Halo for AI Developers</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#Strix Halo`, `#performance optimization`, `#local LLM inference`, `#hardware-specific tuning`

---