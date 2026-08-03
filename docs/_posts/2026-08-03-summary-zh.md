---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 51 条内容中筛选出 20 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：local-llm、DeepSeek、inference、voice-ai、prompt caching。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Parlor v2：本地 GPT-Live 克隆采用级联架构](https://www.reddit.com/r/LocalLLaMA/comments/1vdrb0y/parlor_v2_besteffort_fully_local_gptlive_clone_on/)**
2. **[DeepSeek V4 Flash 提醒：system 角色消息会破坏提示缓存，请改用 latest_reminder](https://www.reddit.com/r/LocalLLaMA/comments/1vdbgw5/psa_for_deepseekv4flash0731_users_dont_blow_out/)**
3. **[在 8GB 内存 CPU 上跑通 1.56TB 的 Kimi K3 MoE 模型](https://www.reddit.com/r/LocalLLaMA/comments/1vd874t/i_pushed_kimi_k3_onto_one_cpu_with_8_gb_of_ram/)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [Parlor v2：本地 GPT-Live 克隆采用级联架构](https://www.reddit.com/r/LocalLLaMA/comments/1vdrb0y/parlor_v2_besteffort_fully_local_gptlive_clone_on/)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [F*：用于程序验证的通用面向证明语言](https://fstar-lang.org/)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [在 8GB 内存 CPU 上跑通 1.56TB 的 Kimi K3 MoE 模型](https://www.reddit.com/r/LocalLLaMA/comments/1vd874t/i_pushed_kimi_k3_onto_one_cpu_with_8_gb_of_ram/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Parlor v2：本地 GPT-Live 克隆采用级联架构

**关联新闻**: [Parlor v2：本地 GPT-Live 克隆采用级联架构](https://www.reddit.com/r/LocalLLaMA/comments/1vdrb0y/parlor_v2_besteffort_fully_local_gptlive_clone_on/)

**切入角度**: Parlor v2 是一个完全本地化的 GPT-Live 克隆，可在 M3 Pro Mac 上运行，并已作为开源项目发布在 GitHub 上。开发者在多次尝试创建全双工模型失败后，从微调转向了经典的级联架构。 该项目为在消费级硬件上复制 GPT-Live 风格的实时语音交互提供了一条实用的开源路径，对本地大语言模型社区的开发者很有价值。它也凸显了当前开源权重模型在全双工语音方面的局限，强调了前沿 AI 公司发布具有竞争力的全双工模型的必要性。 开发者最初的方法是对 Gemma 4 12B 进行微调，通过嫁接决策 tick 和语音头使其表现类似全双工模型，但在多次尝试后失败了。Parlor v2 转而使用级联系统——很可能是由独立的语音识别、语言模型和语音合成组件组成的流水线——作者认为这是在前沿全双工模型出现前更好的做法。

**可延展方向**: GPT-Live 是 OpenAI 推出的新一代语音模型，基于全双工架构，可以同时听和说，使对话更加自然。语音 AI 中的级联架构通常将自动语音识别、文本生成和文本转语音分别用独立模型串联起来，而端到端全双工模型则在单一集成系统中完成这些任务。M3 Pro 是苹果的 ARM 芯片，用于 MacBook Pro 等设备，能够在本地运行大型语言模型。Parlor v2 的发布展示了开发者在不想依赖云 API 的情况下获得类似 GPT-Live 功能的一种实用替代方案。

---

### 选题 2：DeepSeek V4 Flash 提醒：system 角色消息会破坏提示缓存，请改用 latest_reminder

**关联新闻**: [DeepSeek V4 Flash 提醒：system 角色消息会破坏提示缓存，请改用 latest_reminder](https://www.reddit.com/r/LocalLLaMA/comments/1vdbgw5/psa_for_deepseekv4flash0731_users_dont_blow_out/)

**切入角度**: r/LocalLLaMA 上的一则 PSA 警告：DeepSeek V4 Flash 会把对话中途的每条 system 角色消息都提升到提示词顶部，从而导致提示缓存失效。解决办法是改用 latest_reminder 角色，llama.cpp 可以正常透传该角色。 无论是本地还是通过托管 API 使用 DeepSeek V4 Flash 的开发者，在提示缓存悄然失效时都会浪费时间和金钱，因为被缓存的前缀 token 更便宜也更快。这条提示能帮助用户保持提示词前缀稳定，避免意外的高成本和高延迟。 DeepSeek V4 Flash 是一个面向效率优化的混合专家（MoE）模型，总参数 284B，激活参数 13B，支持 1M token 上下文。该模型未附带 Jinja 模板，但凡是按 DeepSeek 聊天模板 Python 逻辑重建的分发版都会把所有 system 消息提升到顶部，因此对话中途放入的任何 system 文本都会破坏已缓存的前缀，而不是保持在注入点附近。

**可延展方向**: 提示缓存（prompt caching）允许大模型服务商在不同请求之间复用提示词的静态前缀，从而降低重复内容（如指令和文档）的成本和延迟。DeepSeek 的聊天模板把顶层的 system 角色视为全局指令的位置，本身不支持对话中途的 system 轮次，因此这些消息会被移动到提示词开头。latest_reminder 是 DeepSeek 为对话内部消息训练使用的角色，使用它可以保持前缀不变，继续享受缓存带来的收益。

---

### 选题 3：在 8GB 内存 CPU 上跑通 1.56TB 的 Kimi K3 MoE 模型

**关联新闻**: [在 8GB 内存 CPU 上跑通 1.56TB 的 Kimi K3 MoE 模型](https://www.reddit.com/r/LocalLLaMA/comments/1vd874t/i_pushed_kimi_k3_onto_one_cpu_with_8_gb_of_ram/)

**切入角度**: 一位开发者用 C99 编写了一个推理引擎，从 NVMe 流式读取 1.56TB 的 Kimi K3 混合专家（MoE）权重，仅将打包为 4-bit 的专家数据留在内存中，在 CPU 上以约 33 秒/词元的速度运行，峰值内存占用 8.24GB。代码已开源在 GitHub，并用一个 13 层小型测试模型对照 PyTorch 参考实现验证了正确性。 这说明 Kimi K3 这样的前沿开源模型可以在没有 GPU 的普通硬件上运行，大幅降低了本地实验的门槛。同时也展示了 MoE 稀疏性结合 4-bit 量化如何用磁盘带宽换取内存，为 CPU 和边缘端推理优化提供了新思路。 Kimi K3 共有 896 个专家，每个词元只激活其中 16 个；这些被路由到的专家会从 NVMe 读取，并直接以打包的 4-bit 格式参与矩阵乘运算，无需反量化。稠密主干被重打包为单个文件，每层有固定偏移量；内存占用可以调节，128GB 内存时约 20 秒/词元，且不同内存预算下输出完全一致。

**可延展方向**: Kimi K3 是 Moonshot AI 推出的 2.8 万亿参数开源混合专家（MoE）模型，采用了 Kimi Delta Attention（KDA）和 Attention Residuals（AttnRes）技术，并具备原生视觉能力。在 MoE 模型中，每个词元只激活总参数中的一小部分，因此推理系统只需将活跃专家留在内存里，其余权重可从存储设备流式读取。4-bit 量化进一步降低了每个权重所需的内存和带宽，这也是让 1.56TB 权重能在 CPU 上推理的关键。

---

1. [Kakehashi：实验性用户态在 Linux ARM 上运行 macOS 二进制文件](#item-1) ⭐️ 8.0/10
2. [F*：用于程序验证的通用面向证明语言](#item-2) ⭐️ 8.0/10
3. [EU Age Verification Project Mandates Hardware-Bound Attestation](#item-3) ⭐️ 8.0/10
4. [微软牵头发布公开信力挺开放权重 AI 模型](#item-4) ⭐️ 8.0/10
5. [开源模型 Laguna S2.1、Inkling 与 Kimi K3 展现帕累托前沿实用价值](#item-5) ⭐️ 8.0/10
6. [在 8GB 内存 CPU 上跑通 1.56TB 的 Kimi K3 MoE 模型](#item-6) ⭐️ 8.0/10
7. [在 Mac 上仅用约 5.3GB 内存流式运行 284B DeepSeek-V4-Flash](#item-7) ⭐️ 8.0/10
8. [Karpathy’s Pelican](#item-8) ⭐️ 7.0/10
9. [NixOS-DGX-Spark：让 NVIDIA DGX Spark 与 Asus GX10 用上 Nix/NixOS](#item-9) ⭐️ 7.0/10
10. [eBay 骚扰案：安全高管获刑并支付 5600 万美元赔偿](#item-10) ⭐️ 7.0/10
11. [个人 AI 基准测试：让模型用 SVG 画一只带哈布斯堡下巴的青蛙](#item-11) ⭐️ 7.0/10
12. [中国 DFSX 声称内存带宽为 NVIDIA GB200 的两倍](#item-12) ⭐️ 7.0/10
13. [DeepSeek-V4-Flash-0731 在国际象棋基准测试中超越 Fable-5、Sol 和 Kimi-K3](#item-13) ⭐️ 7.0/10
14. [llama.cpp 为 DeepSeek V4 Flash 添加 MTP/DSpark 支持](#item-14) ⭐️ 7.0/10
15. [Vacuum 16T：空壳 16.5 万亿参数模型暴露 Hugging Face 排名漏洞](#item-15) ⭐️ 7.0/10
16. [DeepSeek V4 Flash 请勿量化 KV Cache：质量明显下降](#item-16) ⭐️ 7.0/10
17. [llama.cpp 官方 Mac 应用与 llama serve 命令简化本地大模型使用](#item-17) ⭐️ 7.0/10
18. [Parlor v2：本地 GPT-Live 克隆采用级联架构](#item-18) ⭐️ 7.0/10
19. [通过 CUDA 降级或 Fork 提升 DeepSeek v4 Flash 预填充速度](#item-19) ⭐️ 7.0/10
20. [DeepSeek V4 Flash 提醒：system 角色消息会破坏提示缓存，请改用 latest_reminder](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Kakehashi：实验性用户态在 Linux ARM 上运行 macOS 二进制文件](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi 是一个实验性用户态翻译层，能够在 Linux aarch64 上加载 Darwin Mach-O 二进制文件。目前已有 7-Zip、curl 和 Xcode Git 的工作原型，其中 7-Zip 已在包含 8k 个文件的文件树上通过多线程压缩测试。 该项目可能将 WINE/Proton 式的兼容方法扩展到 ARM 上的 macOS，使 macOS 命令行工具无需虚拟机或类似 Darling 的完整环境即可在 Linux 上原生运行。尽管仍处于早期阶段，它对系统研究和 ARM 生态的二进制兼容性具有重要意义。 该项目以命令行工具为先，不使用 JIT；它映射了一个 freestanding libSystem 并翻译 BSD 系统调用。当前性能显示 7-Zip 比原生 Linux 执行慢约 5.2 倍，但作者已有明确的优化计划来缩小这一差距。

hackernews · vlad_kalinkin · 8月2日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**背景**: Mach-O 是苹果 macOS 和 iOS 用于可执行文件、库和对象代码的二进制格式。要在 Linux 上运行 macOS 二进制文件，必须处理 Mach-O 加载、库依赖和系统调用翻译，而无法依赖苹果的内核。Darling 是一个更早的开源项目，旨在 Linux 上提供类似的 macOS 二进制兼容性，并且它有一个开放中的 ARM64 支持 PR。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">GitHub - wie-project/kakehashi: Userspace macOS translation layer for ...</a></li>
<li><a href="https://news.mcan.sh/item/49145937">Show HN: Kakehashi - Experimental userspace to run macOS binaries on ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach - O - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对此充满热情，并将 Kakehashi 与 Darling 项目进行比较，建议在 ARM64 支持方面进行合作。也有人提醒说该解决方案仍处于早期阶段，还有人希望未来能通过类似 yabridge 的封装程序在 Linux 上运行 AU 插件。

**标签**: `#macOS`, `#Linux`, `#ARM`, `#binary compatibility`, `#userspace`

---

<a id="item-2"></a>
## [F*：用于程序验证的通用面向证明语言](https://fstar-lang.org/) ⭐️ 8.0/10

本次新闻聚焦 F*——一种用于编写和验证程序的通用面向证明编程语言。Hacker News 上的讨论集中在其语法展示、C 语言集成以及工业采用情况。 F* 是少数具有实际影响力的面向证明语言之一，尤其在 HACL* 等已验证密码学库中发挥重要作用。通过让开发者证明安全关键代码的正确性属性，F* 有助于提高必须抵御错误和攻击的软件的可信度。 F* 将依赖类型、单子效果和精化类型与基于 SMT 的证明自动化及基于策略的交互式证明相结合。默认编译为 OCaml，部分片段可提取为 F#、C、WebAssembly（通过 KaRaMeL）或汇编语言（通过 Vale）。

hackernews · ducktective · 8月2日 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49143925)

**背景**: F* 是微软研究院与法国国家信息与自动化研究所（Inria）的联合项目，受 ML、Caml 和 OCaml 启发，旨在进行程序验证。形式化验证使用数学方法，依据形式化规范证明或否定系统的正确性，典型例子包括 CompCert 和 seL4。F* 的类型检查器利用 SMT 求解和手动证明来确保程序满足其规范。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language) - Wikipedia</a></li>
<li><a href="https://fstar-lang.org/">F*: A Proof-Oriented Programming Language</a></li>
<li><a href="https://github.com/FStarLang/FStar">FStarLang/FStar: A Proof-oriented Programming Language - GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者希望主页上能立即展示基本的语法示例，并将其比作没有截图或视频的游戏网站。一位用户称赞 F* 在将现有 C 代码库迁移到 F* 时能简洁地表达对外部库的调用，另一位则询问 F* 是否在工业界使用以及用于何种软件。还有一位开玩笑说，没有副作用就无法实现响应式样式表。

**标签**: `#programming languages`, `#formal verification`, `#proof-oriented`, `#functional programming`, `#security`

---

<a id="item-3"></a>
## [EU Age Verification Project Mandates Hardware-Bound Attestation](https://linuxiac.com/eu-age-verification-project-mandates-hardware-bound-attestation/) ⭐️ 8.0/10

The EU's age verification project requiring hardware-bound attestation raises major privacy and digital sovereignty concerns, with community debate over its impact on Linux users and competition.

hackernews · RobotToaster · 8月2日 20:44 · [社区讨论](https://news.ycombinator.com/item?id=49148128)

**标签**: `#EU regulation`, `#privacy`, `#age verification`, `#hardware attestation`, `#digital identity`

---

<a id="item-4"></a>
## [微软牵头发布公开信力挺开放权重 AI 模型](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

7 月 24 日，微软牵头发布了一封开放信，得到包括英伟达、亚马逊、Y Combinator、Linux 基金会以及后来的 OpenAI 在内的 235 家 AI 相关企业联署，主张不应限制开放权重模型。Anthropic 拒绝签署并发布了自身立场，另一封由 1324 名前沿 AI 员工签署的《Pacing the Frontier》公开信则呼吁对自动化 AI 发展进行有意识的节奏控制。 这标志着主要 AI 企业在 AI 政策问题上难得地形成了一致立场，直接反对美国政府可能对开放权重模型的限制。结果将影响先进 AI 能力是保持广泛可及，还是集中于少数封闭提供方手中。 微软牵头的信件明确为蒸馏（利用其他模型的输出来训练或改进模型）辩护，称政策制定者不应将其与盗用混为一谈。Anthropic 在 7 月 27 日由 CEO Dario Amodei 主导的回应中警告威权政府滥用风险及工业级蒸馏操作，但表示 Anthropic 从未主张禁止开放权重模型。

rss · Simon Willison · 8月2日 04:16

**背景**: 开放权重模型公开其训练后的参数，任何人都可以下载、运行和微调，但训练数据和代码可能保持私有。这与要求数据和代码透明的完全开源 AI 不同，也不同于只能通过 API 访问的封闭模型。这些公开信反映了关于开放还是限制更能解决安全、竞争和国家安全问题的更广泛政策辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://telnyx.com/resources/open-weight-models">Open Weight Models What They Are and How to Use Them</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights : not quite what you’ve been told – Open Source Initiative</a></li>
<li><a href="https://medium.com/@bhagyarana80/why-open-weight-models-matter-more-than-you-think-1d1d8787a4fe">Why Open - Weight Models Matter (More Than You Think) | Medium</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open weights`, `#AI regulation`, `#open source`, `#industry letter`

---

<a id="item-5"></a>
## [开源模型 Laguna S2.1、Inkling 与 Kimi K3 展现帕累托前沿实用价值](https://www.interconnects.ai/p/latest-open-artifacts-23-laguna-s21) ⭐️ 8.0/10

Interconnects 的开放产物系列第 23 期聚焦新发布的开源权重模型 Laguna S2.1、Inkling 和 Kimi K3，指出它们展示了开源模型在帕累托前沿上的实用价值。这一期反映出训练有竞争力开源模型的能力正在增强。 强大的开源权重模型日益普及，为研究人员和工程师提供了更高效、更具竞争力的专有系统替代品，减少了对少数封闭提供商的依赖。识别哪些模型位于帕累托前沿，有助于从业者根据能力和资源消耗做出最佳权衡。 帕累托前沿表示一组最优权衡方案，其中改善一个目标（如模型质量）通常会恶化另一个目标（如推理成本）。开放权重模型会公开其训练参数，但修改或再分发的权利则取决于各模型的具体许可证。

rss · Interconnects · 8月2日 13:01

**背景**: 在机器学习中，帕累托前沿描述的是帕累托最优的模型，即在所有目标（通常包括质量、延迟和成本）上没有其他模型能全面超越它们。开放权重模型是将其学习参数（权重）公开释出的人工智能模型，允许他人下载，并根据许可证进行微调或再分发。Interconnects 通讯定期追踪新的开放产物，以帮助社区了解开放人工智能的发展状况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pareto_front">Pareto front - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open-weight_model">Open-weight model</a></li>

</ul>
</details>

**标签**: `#open models`, `#AI`, `#machine learning`, `#model releases`, `#Pareto frontier`

---

<a id="item-6"></a>
## [在 8GB 内存 CPU 上跑通 1.56TB 的 Kimi K3 MoE 模型](https://www.reddit.com/r/LocalLLaMA/comments/1vd874t/i_pushed_kimi_k3_onto_one_cpu_with_8_gb_of_ram/) ⭐️ 8.0/10

一位开发者用 C99 编写了一个推理引擎，从 NVMe 流式读取 1.56TB 的 Kimi K3 混合专家（MoE）权重，仅将打包为 4-bit 的专家数据留在内存中，在 CPU 上以约 33 秒/词元的速度运行，峰值内存占用 8.24GB。代码已开源在 GitHub，并用一个 13 层小型测试模型对照 PyTorch 参考实现验证了正确性。 这说明 Kimi K3 这样的前沿开源模型可以在没有 GPU 的普通硬件上运行，大幅降低了本地实验的门槛。同时也展示了 MoE 稀疏性结合 4-bit 量化如何用磁盘带宽换取内存，为 CPU 和边缘端推理优化提供了新思路。 Kimi K3 共有 896 个专家，每个词元只激活其中 16 个；这些被路由到的专家会从 NVMe 读取，并直接以打包的 4-bit 格式参与矩阵乘运算，无需反量化。稠密主干被重打包为单个文件，每层有固定偏移量；内存占用可以调节，128GB 内存时约 20 秒/词元，且不同内存预算下输出完全一致。

reddit · r/LocalLLaMA · /u/FareedKhan557 · 8月2日 04:26

**背景**: Kimi K3 是 Moonshot AI 推出的 2.8 万亿参数开源混合专家（MoE）模型，采用了 Kimi Delta Attention（KDA）和 Attention Residuals（AttnRes）技术，并具备原生视觉能力。在 MoE 模型中，每个词元只激活总参数中的一小部分，因此推理系统只需将活跃专家留在内存里，其余权重可从存储设备流式读取。4-bit 量化进一步降低了每个权重所需的内存和带宽，这也是让 1.56TB 权重能在 CPU 上推理的关键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://www.kdnuggets.com/why-the-newest-llms-use-a-moe-mixture-of-experts-architecture">Why the Newest LLMs use a MoE ( Mixture of Experts ) Architecture</a></li>
<li><a href="https://huggingface.co/blog/4bit-transformers-bitsandbytes">Making LLMs even more accessible with bitsandbytes, 4-bit quantization and QLoRA</a></li>

</ul>
</details>

**标签**: `#inference`, `#MoE`, `#CPU`, `#optimization`, `#local-llm`

---

<a id="item-7"></a>
## [在 Mac 上仅用约 5.3GB 内存流式运行 284B DeepSeek-V4-Flash](https://www.reddit.com/r/LocalLLaMA/comments/1vdbix4/deepseekv4flash_284b_on_53gb_of_memory/) ⭐️ 8.0/10

开发者 u/Blahblahblakha 发布了 Mference 推理引擎，通过在 SSD 上流式加载稀疏专家，让 284B-A13B 的 DeepSeek-V4-Flash 模型在 24GB 内存的 Mac M5 Pro 上仅占用约 5.3GB 常驻内存（峰值 6.8GB）即可运行。在 2 位动态量化下，生成速度最高可达每秒 4.8 个 token。 这表明，通过用磁盘带宽换取内存，大规模 MoE 模型可以在消费级硬件上运行，从而让更多人能在本地运行前沿开源模型。这可能会加速本地 AI 开发，并降低实验所需的硬件门槛。 Mference 还支持 Gemma 4 26B-A4B（约 2GB，31–35 tok/s）和 Qwen 3.6 35B-A3B（约 1.45GB，19–23 tok/s），并提供了原生 Mac 应用，带有 OpenAI 兼容服务器和文档附件功能。该模型磁盘占用约 91GB，当前解码约 53%的耗时在 I/O 上，上下文长度限制为 4K token。

reddit · r/LocalLLaMA · /u/Blahblahblakha · 8月2日 07:28

**背景**: 混合专家（MoE）模型会让每个 token 只经过一小部分参数，因此 284B 的模型每次 token 可能只激活约 13B 参数。这使得推理引擎可以将共享层和 KV 缓存保留在内存中，同时按需从 SSD 读取被选中的专家权重，Flash-MoE 也采用了类似思路。KV 缓存用于存储此前生成的 token 的键/值张量，避免自回归生成时的重复计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://www.mindstudio.ai/blog/ssd-streaming-ai-models-ram-dial">SSD Streaming for AI Models: How to Turn RAM from a Wall into a Dial | MindStudio</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#MoE`, `#inference-optimization`, `#SSD-streaming`, `#Mac`

---

<a id="item-8"></a>
## [Karpathy’s Pelican](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Karpathy notes that frontier LLMs still struggle with creating truly playable pinball games, suggesting a useful benchmark for understanding the physical world.

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**标签**: `#LLM`, `#benchmark`, `#physical reasoning`, `#AI evaluation`, `#Karpathy`

---

<a id="item-9"></a>
## [NixOS-DGX-Spark：让 NVIDIA DGX Spark 与 Asus GX10 用上 Nix/NixOS](https://github.com/graham33/nixos-dgx-spark) ⭐️ 7.0/10

NixOS-DGX-Spark 仓库提供了 USB 镜像和一个 NixOS 模块，让 NVIDIA DGX Spark 和 Asus Ascent GX10 可以使用 Nix 与 NixOS。该仓库既支持在原有 DGX OS 上运行 Nix playbook，也支持直接安装完整的 NixOS 系统。 该项目把 Nix 可复现、声明式的包管理能力带到了 NVIDIA 的个人 AI 超算上，让 AI 工作流更容易定义、版本化并复现。对于希望在专用 AI 硬件上使用 CUDA 部署模型、同时又想获得一致环境的 Nix 用户和 AI 开发者来说，这很重要。 该项目明确支持 NVIDIA DGX Spark 和 Asus Ascent GX10 两款设备，并提供包含系统配置的 NixOS 模块。社区用户反馈已经在上面运行 k3s 集群和 DeepSeek 模型。

hackernews · graham33 · 8月2日 17:05 · [社区讨论](https://news.ycombinator.com/item?id=49146267)

**背景**: Nix 是一个包管理器，它用纯函数式语言中的可复现、声明式指令来构建软件，从而避免依赖冲突，并支持原子升级和回滚。NixOS 是围绕 Nix 构建的 Linux 发行版，整个系统配置都通过一个声明式的功能配置来定义。DGX Spark 是 NVIDIA 基于 Blackwell 架构推出的紧凑型个人 AI 超算，面向需要本地运行 AI 推理和实验的开发者与团队。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>
<li><a href="https://en.wikipedia.org/wiki/NixOS">NixOS - Wikipedia</a></li>
<li><a href="https://nixos.org/">Nix & NixOS | Declarative builds and deployments</a></li>

</ul>
</details>

**社区讨论**: 评论者态度积极，有用户反馈该项目在 Asus GX10 上配合 k3s 和 DeepSeek 运行良好，其他人则感谢作者让 DGX Spark 管理变得更容易。还有人提到相关的生态项目，比如用于 Firecracker 沙箱的 microvm.nix，以及 Flox 关于 Nix/CUDA 在资本市场应用的案例研究；也有评论指出 Claude Code 在编写 Nix 代码方面出奇地高效。

**标签**: `#NixOS`, `#Nix`, `#DGX Spark`, `#NVIDIA`, `#AI hardware`

---

<a id="item-10"></a>
## [eBay 骚扰案：安全高管获刑并支付 5600 万美元赔偿](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay 前安全高管因策划针对批评性新闻通讯作者的骚扰活动而被判刑，并导致公司支付 5600 万美元赔偿。相关判决包括监禁、监督释放和罚款。 此案凸显了企业安全团队滥用权力压制批评者的风险，引发了对科技伦理和企业问责制的严重质疑。它开创了让高管个人为此类不当行为承担责任的先例。 eBay 前安全与安保高级总监 Jim Baugh 被判入狱 57 个月。Brian Gilbert 被判处已服刑期、一年监督释放及 2 万美元罚款，安全团队的其他成员也参与了此案。

hackernews · JumpCrisscross · 8月2日 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**背景**: 斯坦纳夫妇（The Steiners）经营一份批评 eBay 的新闻通讯，成为 eBay 全球安全团队主导的骚扰活动的目标。检方称，包括前警察队长在内的七名安全团队成员联手骚扰和恐吓这对夫妇。此案成为企业不当行为的典型案例，并促成了 5600 万美元的和解协议。

**社区讨论**: 评论者对该骚扰行为仅限于一对批评者表示怀疑，呼吁对 eBay 安全团队及相关前警察队长进行更广泛的调查。还有人提出了 eBay 高额卖家费用等其他问题，另有人引用了关于不受监督的权力导致不良行为的普遍原则。

**标签**: `#eBay`, `#corporate-accountability`, `#tech-ethics`, `#legal`, `#harassment`

---

<a id="item-11"></a>
## [个人 AI 基准测试：让模型用 SVG 画一只带哈布斯堡下巴的青蛙](https://frogs.vaguespac.es/) ⭐️ 7.0/10

一位开发者发起了一项个人基准测试，要求多个 AI 模型“生成一个带有哈布斯堡下巴的青蛙 SVG”，并发布了测试结果。该网站因流量过大而一度不堪重负，作者随后表示正在努力提升其稳定性。 这项基准测试提供了一种轻量、富有创意的比较方式，用于评估多模态大语言模型在矢量图形任务上的表现，从中可以看出模型对生物解剖结构和历史文化概念的理解程度。它还表明，即便是领先的模型，在空间关系和姿势选择上仍然存在困难，而不仅仅是事实记忆问题。 该任务要求生成 SVG 图像，这是一种基于 XML 定义的矢量格式，因此输出是代码而非像素图。评论者指出，几乎所有模型都选择了青蛙的正面视角，而不是侧面轮廓，这使得突出的哈布斯堡下巴更难被逼真地呈现；一些模型还为下巴生成了一个与蛙脸脱节的“块状物”。

hackernews · thebigship · 8月2日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=49147622)

**背景**: “哈布斯堡下巴”指的是下颌前突（mandibular prognathism），即下颌明显向前突出的状况，历史上与哈布斯堡家族成员密切相关。SVG（可缩放矢量图形）是一种基于 XML 的开放标准图像格式，它使用矢量形状而非固定像素网格来描述图像，因此与分辨率无关。AI 需要将这种历史文化与生物学知识结合基本绘画能力，才能满足该提示要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Habsburg_jaw">Habsburg jaw</a></li>
<li><a href="https://docs.fileformat.com/page-description-language/svg/">Learn about SVG file format and APIs that can create and open SVG ...</a></li>

</ul>
</details>

**社区讨论**: 评论者们认为这项基准测试既有趣又富有启发性，有人称 Opus 5 是唯一接近通过的模型。好几个人注意到一个意外现象：没有模型从侧面绘制青蛙，尽管侧面轮廓会让下巴形状更加明显；网站作者感谢了社区，为访问中断道歉，并分享了自己的通讯订阅链接。

**标签**: `#AI`, `#benchmarking`, `#LLM`, `#SVG`, `#image-generation`

---

<a id="item-12"></a>
## [中国 DFSX 声称内存带宽为 NVIDIA GB200 的两倍](https://www.reddit.com/r/LocalLLaMA/comments/1vduej3/chinas_dfsx_offers_2x_the_memory_bandwidth_of/) ⭐️ 7.0/10

Reddit 上 r/LocalLLaMA 版块的一篇帖子声称，中国的 DFSX 芯片提供的内存带宽是 NVIDIA GB200 的两倍。帖子中没有提供官方规格或基准测试，因此该说法未经证实。 如果属实，内存带宽达到 GB200 两倍将是中国本土 AI 芯片行业的一个重大里程碑。内存带宽是大语言模型推理的关键瓶颈，这一说法可能影响 AI/ML 社区对硬件选型的决策。 该帖子没有提供任何基准测试、技术文档或来源来验证这一 2 倍性能的说法。DFSX 是一家中国初创公司，近期推出了 DF1000，这是一款通过完全本土供应链生产的 14nm AI 加速器，可能正是该说法所指的芯片。

reddit · r/LocalLLaMA · /u/MundanePercentage674 · 8月2日 21:39

**背景**: DFSX 是一家中国芯片初创公司，近期发布了其首款 AI 加速器 DF1000，采用 14nm 制程工艺并通过完全本土供应链制造。NVIDIA GB200 是 Blackwell 架构的 AI 超级芯片，以其高内存带宽而闻名。内存带宽是指数据从内存读取或写入内存的速率，是影响 AI 模型性能的关键因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nvidia_GB200">Nvidia GB200</a></li>
<li><a href="https://www.qore.com/big-tech/el-chip-de-14nm-con-el-que-china-busca-desafiar-a-nvidia/">El chip de 14nm con el que China busca desafiar a Nvidia | Qore</a></li>
<li><a href="https://wpnews.pro/news/chinas-14nm-ai-chip-wager">China ’s 14nm AI Chip Wager — Web Pulse</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#China`, `#memory bandwidth`, `#NVIDIA GB200`, `#chip`

---

<a id="item-13"></a>
## [DeepSeek-V4-Flash-0731 在国际象棋基准测试中超越 Fable-5、Sol 和 Kimi-K3](https://www.reddit.com/r/LocalLLaMA/comments/1vdq8en/deepseekv4flash0731_surpasses_fable5_sol_kimik3/) ⭐️ 7.0/10

Reddit 用户 mrwang89 发帖称，DeepSeek 新发布的模型版本 DeepSeek-V4-Flash-0731 在国际象棋基准测试中超越了 Fable-5、Sol 和 Kimi-K3。该帖子未提供具体的基准测试分数或方法细节。 国际象棋基准测试考察模型在动态、多步策略环境中的推理、规划和指令跟随能力，而这些正是大语言模型传统的弱项。这一结果说明 DeepSeek 的高效 MoE 架构在复杂推理任务上具备与其它领先模型竞争的实力，也预示着小而廉价、却能在重推理任务上表现出色的模型可能成为趋势。 DeepSeek-V4-Flash-0731 是一个稀疏混合专家（MoE）模型，总参数 284B，其中激活参数仅 13B，官方描述其非常适合编码、推理和智能体工作流。根据 OpenRouter 的信息，0731 版本是在此前版本基础上重新训练后的迭代版本；此处提及的基准测试很可能指的是基于 Elo 等级分的国际象棋评测体系，如 ChessBench 或 LLM Chess。

reddit · r/LocalLLaMA · /u/mrwang89 · 8月2日 18:54

**背景**: 近年来，国际象棋已成为评测大语言模型推理与指令跟随能力的热门测试场景，例如 NeurIPS'25 上提出的 LLM Chess 基准以及按 Elo 等级分排名的 ChessBench。这些基准测试超越了传统的数学和编程任务，要求模型处理动态棋盘状态并遵循复杂的多轮指令。DeepSeek V4 Flash 定位为一款面向实际应用的高性价比模型，而其在象棋上的出色表现说明，无需扩增激活参数也能获得较强的推理能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek-ai/ DeepSeek - V 4 - Flash - 0731 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash-0731">DeepSeek V 4 Flash 0731 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://arxiv.org/html/2512.01992">LLM Chess : Benchmarking Reasoning and Instruction-Following in...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#LLM`, `#benchmark`, `#chess`, `#AI`

---

<a id="item-14"></a>
## [llama.cpp 为 DeepSeek V4 Flash 添加 MTP/DSpark 支持](https://www.reddit.com/r/LocalLLaMA/comments/1vdhgq9/llamacpp_just_added_mtp_dspark_support_for/) ⭐️ 7.0/10

llama.cpp 已为 DeepSeek V4 Flash 增加 MTP（多 token 预测）和 DSpark 投机解码支持，用户可以在本地硬件上以更快的推理速度运行该模型。 这一更新对本地 LLM 实践者很重要，因为 MTP 和 DSpark 能显著降低推理延迟，使 DeepSeek V4 Flash 更适合在消费级和专业级 GPU 上的实时应用。这也表明 llama.cpp 始终站在采用新解码技术的前沿。 MTP 使模型能够在一次前向传播中预测多个未来 token，而 DSpark 采用基于置信度调度的投机解码和半自回归生成。Hugging Face 上的 'DeepSeek-V4-Flash-DSpark' 模型卡片声称，在配备 2-4 块 RTX Pro 6000 GPU 的系统上，DSpark 比 MTP 更快。

reddit · r/LocalLLaMA · /u/rmhubbert · 8月2日 12:58

**背景**: 大型语言模型以自回归方式逐 token 生成文本，这限制了吞吐量。多 token 预测（MTP）训练模型联合预测多个未来 token，而投机解码则使用较小的草稿模型提出 token，再由目标模型并行验证。llama.cpp 是一个被广泛使用的开源 C/C++ 项目，用于在本地 CPU、GPU 及其他硬件上运行 LLM。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/fraserprice/DeepSeek-V4-Flash-DSpark">fraserprice/DeepSeek-V4-Flash- DSpark · Hugging Face</a></li>
<li><a href="https://www.alphaxiv.org/overview/2607.05147">DSpark : Confidence-Scheduled Speculative Decoding with... | alphaXiv</a></li>
<li><a href="https://arxiv.org/html/2509.18362">FastMTP: Accelerating LLM Inference with Enhanced Multi - Token ...</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#DeepSeek V4`, `#MTP`, `#DSpark`, `#local LLM inference`

---

<a id="item-15"></a>
## [Vacuum 16T：空壳 16.5 万亿参数模型暴露 Hugging Face 排名漏洞](https://www.reddit.com/r/LocalLLaMA/comments/1vdh1us/vacuum_16t/) ⭐️ 7.0/10

用户在 Hugging Face 上发布了“Vacuum 16T”，这个模型声明有 16.5 万亿参数，但实际上不包含任何可用信息。Hugging Face 仅根据 safetensors 头部计算参数量，因此这个空声明足以让它在参数排行榜上登顶。 这证明 Hugging Face 的模型规模排名可以被低成本操纵，削弱了参数量作为模型规模信号的有效性。它还暴露了存储计费上的漏洞：该仓库占用 8.25 TB 配额，但实际传输量仅约 692 KB。 该模型在 385 个分片中使用 3,841 个形状为[65536, 65536]的 FP4 张量，外加一个[4294967296, 1]的嵌入张量，声明的参数量为 16,501,264,351,232。Xet 的内容定义分块会对相同的 64 KiB 零块进行去重，因此上传带宽大幅缩小，但 Hugging Face 的存储配额仍按完整的 8.25 TB 逻辑大小计费。

reddit · r/LocalLLaMA · /u/alerikaisattera · 8月2日 12:39

**背景**: safetensors 是一种安全的张量存储格式，其头部为每个张量声明形状、数据类型和偏移量；Hugging Face 通过对声明形状求乘积来显示仓库的参数量，而不会读取张量数据。参数量被广泛用来粗略衡量 LLM 的规模和能力，因此排行榜排名备受关注。这个空模型表明，这一显示的指标可以完全通过元数据来操纵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.fileformat.com/data/safetensors/">SAFETENSORS - Stable Diffusion Model - What is SAFETENSORS ...</a></li>
<li><a href="https://medium.com/@nishthakukreti.01/safetensors-efficient-serialization-format-for-deep-learning-57364317be43">SafeTensors : Efficient Serialization Format for Deep Learning | Medium</a></li>

</ul>
</details>

**标签**: `#safetensors`, `#huggingface`, `#parameter-count`, `#llm`, `#exploit`

---

<a id="item-16"></a>
## [DeepSeek V4 Flash 请勿量化 KV Cache：质量明显下降](https://www.reddit.com/r/LocalLLaMA/comments/1vduxth/you_really_should_not_quantize_kv_cache_for/) ⭐️ 7.0/10

一位 Reddit 用户的实测显示，将 DeepSeek V4 Flash 的 KV Cache 从 BF16 量化到 8-bit 会带来明显的质量下降，平均困惑度从 5.840 上升到 5.877，平均 KL 散度达到 0.146。相比之下，Qwen 397B 在同样量化下几乎无变化（PPL 3.747 对 3.748，平均 KLD 0.0036）。 KV Cache 量化被广泛用于降低内存占用并加速本地 LLM 推理，但这一发现表明它并非对所有模型都无损。服务 DeepSeek V4 Flash 的用户在启用 8-bit KV Cache 前应测试质量影响，因为输出可靠性可能明显受损。 该分析报告了困惑度、KL 散度、token 概率变化以及 same-top-p 比例。DeepSeek V4 Flash 的尾部表现尤其糟糕——最大 KL 散度达到 12.47，最大 token 概率变化达到 99.5%，而 same-top-p 降至 87.2%，Qwen 则为 97.9%。

reddit · r/LocalLLaMA · /u/erazortt · 8月2日 22:01

**背景**: KV Cache 保存已生成 token 的 key 和 value 张量，使自回归生成无需重复计算，将其从 16-bit 量化到 8-bit 大约可以减半内存占用。困惑度衡量模型对下一个 token 的不确定性，KL 散度则量化量化后模型输出分布与原始分布的偏移程度。这一对比很重要，因为不同架构对量化的敏感度差异很大，对某个大模型有效的方法未必适用于另一个模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2402.12065">WKVQuant: Quantizing Weight and Key/Value Cache for Large ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Perplexity">Perplexity - Wikipedia</a></li>

</ul>
</details>

**标签**: `#KV cache`, `#quantization`, `#DeepSeek`, `#LLM inference`, `#local LLMs`

---

<a id="item-17"></a>
## [llama.cpp 官方 Mac 应用与 llama serve 命令简化本地大模型使用](https://www.reddit.com/r/LocalLLaMA/comments/1vdt1i2/psa_llamaapp_mac_app_and_llama_serve_from_llamacpp/) ⭐️ 7.0/10

llama.cpp 团队发布了官方 Mac 菜单栏应用 llama.app，提供 DMG 安装包，并推出了替代 llama-server 的新命令 llama serve。该命令无需传参即可调用，llama.cpp 会根据传入请求自动加载合适的模型。 这降低了运行本地大模型的门槛，让原本需要命令行的非专业用户也能轻松使用 llama.cpp。它也使得 llama.cpp 成为 Ollama、LM Studio 等易用工具的更强竞争者，有望扩大本地 AI 的普及度。 llama.app 以 DMG 形式面向 macOS 分发，可在菜单栏显示 API URL、已安装模型和模型推荐。此外还有一条无需 Homebrew 或 winget 的一键安装命令，供命令行用户使用。

reddit · r/LocalLLaMA · /u/rm-rf-rm · 8月2日 20:44

**背景**: llama.cpp 是一个开源的 C/C++ 推理引擎，可在本地运行 Llama 等大语言模型，通常使用 GGUF 格式的模型。它被视为几乎所有本地推理工具（包括 Ollama 和 LM Studio）的事实标准核心。该项目历来以命令行操作为主，因此这次推出官方 GUI 应用和简化后的服务命令，是向更广泛用户群体迈出的重要一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://huggingface.co/docs/inference-endpoints/engines/llama_cpp">llama . cpp · Hugging Face</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#LLM`, `#Mac app`, `#local inference`, `#tooling`

---

<a id="item-18"></a>
## [Parlor v2：本地 GPT-Live 克隆采用级联架构](https://www.reddit.com/r/LocalLLaMA/comments/1vdrb0y/parlor_v2_besteffort_fully_local_gptlive_clone_on/) ⭐️ 7.0/10

Parlor v2 是一个完全本地化的 GPT-Live 克隆，可在 M3 Pro Mac 上运行，并已作为开源项目发布在 GitHub 上。开发者在多次尝试创建全双工模型失败后，从微调转向了经典的级联架构。 该项目为在消费级硬件上复制 GPT-Live 风格的实时语音交互提供了一条实用的开源路径，对本地大语言模型社区的开发者很有价值。它也凸显了当前开源权重模型在全双工语音方面的局限，强调了前沿 AI 公司发布具有竞争力的全双工模型的必要性。 开发者最初的方法是对 Gemma 4 12B 进行微调，通过嫁接决策 tick 和语音头使其表现类似全双工模型，但在多次尝试后失败了。Parlor v2 转而使用级联系统——很可能是由独立的语音识别、语言模型和语音合成组件组成的流水线——作者认为这是在前沿全双工模型出现前更好的做法。

reddit · r/LocalLLaMA · /u/ffinzy · 8月2日 19:36

**背景**: GPT-Live 是 OpenAI 推出的新一代语音模型，基于全双工架构，可以同时听和说，使对话更加自然。语音 AI 中的级联架构通常将自动语音识别、文本生成和文本转语音分别用独立模型串联起来，而端到端全双工模型则在单一集成系统中完成这些任务。M3 Pro 是苹果的 ARM 芯片，用于 MacBook Pro 等设备，能够在本地运行大型语言模型。Parlor v2 的发布展示了开发者在不想依赖云 API 的情况下获得类似 GPT-Live 功能的一种实用替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT - Live | OpenAI</a></li>
<li><a href="https://www.stork.ai/blog/openais-ai-voice-just-got-a-brain">OpenAI GPT - Live : A New AI Voice with Full-Duplex... | Stork. AI</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#voice-ai`, `#real-time`, `#open-source`, `#GPT-Live`

---

<a id="item-19"></a>
## [通过 CUDA 降级或 Fork 提升 DeepSeek v4 Flash 预填充速度](https://www.reddit.com/r/LocalLLaMA/comments/1vdm4z8/deepseek_v4_flash_100150_faster_ts_in_prefillpp/) ⭐️ 7.0/10

一位 Reddit 用户报告说，将 CUDA 从 13.3 降级到 13.1（或使用社区 fork）可以修复 DeepSeek v4 Flash 的预填充/PP 性能，使提示处理速度提升 100-150 tokens/s。使用该 fork 时，提示处理速度可达 1.3K tokens/s。 这为 CUDA 13.2+中的真实性能回退提供了一个实用且影响显著的工作区，帮助本地 LLM 用户在等待官方修复之前就能大幅提升 DeepSeek v4 Flash 的提示处理速度。这也凸显了库层面的细微变化（如 DeviceTopK 与 argsort）会对推理性能产生显著影响。 核心问题在于 CUDA 13.2 将基于 argsort 的 top-k 实现替换为 DeviceTopK，导致 DeepSeek v4 Flash 的预填充/PP 吞吐量下降。首选修复方案是降级到 CUDA 13.1 并重新编译；另一个位于 github.com/vektorprime/working_ds4_speed 的 fork 适用于 CUDA 13.3，可实现 1.3K tokens/s 的提示处理速度。

reddit · r/LocalLLaMA · /u/fragment_me · 8月2日 16:13

**背景**: 在 LLM 推理中，预填充（prefill）阶段会在自回归生成（decode）开始之前，以并行方式处理整个输入提示，以填充 KV 缓存。DeviceTopK 是 CUDA 中用于在设备内存中查找最大或最小 K 个元素的并行原语；在 CUDA 13.2 中，它取代了先前用于 top-k 采样的基于 argsort 的方法。尽管两者产生相同的结果，但 DeviceTopK 实现对于 DeepSeek v4 Flash 的预填充/PP 工作负载（尤其是在全模型卸载推理中）明显更慢。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvidia.github.io/cccl/cub/api/structcub_1_1DeviceTopK.html">cub:: DeviceTopK — CUDA Core Compute Libraries</a></li>
<li><a href="https://insertchat.com/glossary/prefill">What is Prefill in LLM Inference ? Definition & - InsertChat</a></li>
<li><a href="https://developer.nvidia.com/blog/cuda-13-2-introduces-enhanced-cuda-tile-support-and-new-python-features/">CUDA 13.2 Introduces Enhanced CUDA Tile Support and New Python...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#CUDA`, `#LLM inference`, `#Performance optimization`, `#LocalLLaMA`

---

<a id="item-20"></a>
## [DeepSeek V4 Flash 提醒：system 角色消息会破坏提示缓存，请改用 latest_reminder](https://www.reddit.com/r/LocalLLaMA/comments/1vdbgw5/psa_for_deepseekv4flash0731_users_dont_blow_out/) ⭐️ 7.0/10

r/LocalLLaMA 上的一则 PSA 警告：DeepSeek V4 Flash 会把对话中途的每条 system 角色消息都提升到提示词顶部，从而导致提示缓存失效。解决办法是改用 latest_reminder 角色，llama.cpp 可以正常透传该角色。 无论是本地还是通过托管 API 使用 DeepSeek V4 Flash 的开发者，在提示缓存悄然失效时都会浪费时间和金钱，因为被缓存的前缀 token 更便宜也更快。这条提示能帮助用户保持提示词前缀稳定，避免意外的高成本和高延迟。 DeepSeek V4 Flash 是一个面向效率优化的混合专家（MoE）模型，总参数 284B，激活参数 13B，支持 1M token 上下文。该模型未附带 Jinja 模板，但凡是按 DeepSeek 聊天模板 Python 逻辑重建的分发版都会把所有 system 消息提升到顶部，因此对话中途放入的任何 system 文本都会破坏已缓存的前缀，而不是保持在注入点附近。

reddit · r/LocalLLaMA · /u/CharlesStross · 8月2日 07:24

**背景**: 提示缓存（prompt caching）允许大模型服务商在不同请求之间复用提示词的静态前缀，从而降低重复内容（如指令和文档）的成本和延迟。DeepSeek 的聊天模板把顶层的 system 角色视为全局指令的位置，本身不支持对话中途的 system 轮次，因此这些消息会被移动到提示词开头。latest_reminder 是 DeepSeek 为对话内部消息训练使用的角色，使用它可以保持前缀不变，继续享受缓存带来的收益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V2-Chat">deepseek -ai/ DeepSeek -V2- Chat · Hugging Face</a></li>
<li><a href="https://www.linkedin.com/pulse/making-llms-work-smarter-understanding-prompt-caching-faisal-feroz-4mwpf">Making LLMs Work Smarter: Understanding Prompt Caching</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#prompt caching`, `#LLM`, `#llama.cpp`, `#system prompts`

---