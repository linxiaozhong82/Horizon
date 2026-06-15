---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> 从 47 条内容中筛选出 20 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：LLM comparison、LLM inference、LLM、local LLM、Xiaomi。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Nemotron Super 在深度上下文中击败竞争对手 LLM 基准测试](https://www.reddit.com/r/LocalLLaMA/comments/1u5vqpl/nemotron_king_of_the_deep_comparison_of_4_models/)**
2. **[小米 MiMo V2.5 采用 DFlash 和持久内核实现 1000-3000 tps](https://www.reddit.com/r/LocalLLaMA/comments/1u5jtr8/xiaomi_is_now_serving_mimo_v25_at_10003000tps/)**
3. **[里约热内卢'自研'大模型被发现是模型合并产物](https://github.com/nex-agi/Nex-N2/issues/4)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [Anthropic 的 AI 安全立场被批虚伪](https://www.verysane.ai/p/did-anthropic-ask-for-this)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [Anthropic 的 AI 安全立场被批虚伪](https://www.verysane.ai/p/did-anthropic-ask-for-this)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [小米 MiMo V2.5 采用 DFlash 和持久内核实现 1000-3000 tps](https://www.reddit.com/r/LocalLLaMA/comments/1u5jtr8/xiaomi_is_now_serving_mimo_v25_at_10003000tps/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Nemotron Super 在深度上下文中击败竞争对手 LLM 基准测试

**关联新闻**: [Nemotron Super 在深度上下文中击败竞争对手 LLM 基准测试](https://www.reddit.com/r/LocalLLaMA/comments/1u5vqpl/nemotron_king_of_the_deep_comparison_of_4_models/)

**切入角度**: 一位用户对四个高达 120B 参数的大语言模型在深度上下文（约 10 万 token）下的提示处理速度进行了基准测试，发现 Nemotron Super 优于 GPT-OSS 和 Qwen 模型，即使在 40 万 token 上下文深度下仍保持可用速度。 该基准测试为依赖大型模型进行代码分析等需要深度上下文任务的本地 LLM 用户提供了实用见解。它强调了常被忽略的提示处理速度可能成为关键瓶颈，并且 Nemotron Super 为此类用例提供了强大选择。 基准测试在配备 128GB 共享内存的 AMD Strix Halo APU 上运行，使用 Lemonade Server 和 Vulkan 后端，以及 llama-bench。作者采用了主观阈值：提示处理 100 TPS，token 生成 10/20 TPS 作为可用性指标。

**可延展方向**: 参数数量多（例如 120B）的大语言模型常用于复杂任务，但由于内存和处理需求，在处理长上下文时可能会遇到困难。提示处理（PP）速度衡量模型摄入输入 token 的速度，而 token 生成（TG）速度衡量输出速度。AMD Strix Halo APU 是一种高性能芯片，拥有大统一内存，适合本地运行大型模型。Lemonade Server 是一个本地 LLM 服务工具，支持 Vulkan 等多种后端。

---

### 选题 2：小米 MiMo V2.5 采用 DFlash 和持久内核实现 1000-3000 tps

**关联新闻**: [小米 MiMo V2.5 采用 DFlash 和持久内核实现 1000-3000 tps](https://www.reddit.com/r/LocalLLaMA/comments/1u5jtr8/xiaomi_is_now_serving_mimo_v25_at_10003000tps/)

**切入角度**: 小米宣布其 MiMo V2.5 模型采用 DFlash 和持久内核技术，实现了每秒 1000-3000 tokens 的推理速度，DFlash 模型已发布，并承诺即将开源。 这代表了 LLM 推理服务的重大突破，因为实现如此高的吞吐量（1000-3000 tps）可以大幅降低生产部署的延迟和成本，使大规模 AI 应用更加实用和普及。 MiMo V2.5 是一个 1.02 万亿参数的混合专家（MoE）模型，拥有 420 亿活跃参数和 100 万 token 的上下文窗口，基于混合注意力架构。DFlash 模型已可供使用，而服务栈的开源版本承诺即将发布。

**可延展方向**: 混合专家（MoE）模型每个 token 只激活部分参数，从而在较低计算量下实现高容量。持久内核技术（如 Mirage Persistent Kernel）将多个 GPU 操作融合为一次内核启动，减少开销并降低延迟。DFlash（可能是小米的另一项优化）进一步提升了吞吐量。这些进步对于高效服务大型模型至关重要。

---

### 选题 3：里约热内卢'自研'大模型被发现是模型合并产物

**关联新闻**: [里约热内卢'自研'大模型被发现是模型合并产物](https://github.com/nex-agi/Nex-N2/issues/4)

**切入角度**: 里约热内卢市政府发布了 Rio-3.5-Open-397B 模型，声称是自研微调版本，但分析表明它实际上是 Nex-N2 Pro 和 Qwen3.5-397B-A17B 的线性合并（比例约为 60%与 40%），且未进行适当披露。 这一争议凸显了开源 AI 中透明度和归属的重要性，虚假宣称会侵蚀公众信任，并为道德标准树立不良先例。 Rio 模型的每个权重张量在所有 60 层和组件中都与 Nex-N2 Pro 和 Qwen 的 0.6/0.4 混合比例完全一致，表明是简单的线性插值而非微调或蒸馏。

**可延展方向**: 模型合并是一种将多个预训练大语言模型的权重组合以提升性能的技术，无需额外训练。线性合并是其最简单形式，对对应权重求平均。Nex-N2 Pro 是一个 397B 开源模型，本身可能基于 Qwen。Rio 模型被宣传为专有微调版本，但实际上似乎是直接合并而未作修改。

---

1. [小米 MiMo V2.5 采用 DFlash 和持久内核实现 1000-3000 tps](#item-1) ⭐️ 9.0/10
2. [里约热内卢'自研'大模型被发现是模型合并产物](#item-2) ⭐️ 8.0/10
3. [Anthropic 的 AI 安全立场被批虚伪](#item-3) ⭐️ 8.0/10
4. [形式方法与编程的未来](#item-4) ⭐️ 8.0/10
5. [Yserver：用 Rust 编写的现代 X11 服务器](#item-5) ⭐️ 8.0/10
6. [《JavaScript 的诞生与死亡》（2014）：一场预言性的演讲](#item-6) ⭐️ 8.0/10
7. [为何 AI 不会取代软件工程师](#item-7) ⭐️ 8.0/10
8. [基于 Qwen3.5-397B 的实时本地语音聊天机器人](#item-8) ⭐️ 8.0/10
9. [Deepseek 4 Flash 可在 M3 Max Mac（96GB）上运行](#item-9) ⭐️ 8.0/10
10. [Kage：将任何网站打包成单个二进制文件供离线查看](#item-10) ⭐️ 7.0/10
11. [Zeroserve 实现 Caddy 兼容性，速度大幅提升](#item-11) ⭐️ 7.0/10
12. [艾伦·珀利斯的编程箴言（1982）](#item-12) ⭐️ 7.0/10
13. [保罗·格雷厄姆探讨亿万财富的道德性](#item-13) ⭐️ 7.0/10
14. [Linux 7.1 发布，AI 驱动移除旧驱动](#item-14) ⭐️ 7.0/10
15. [AI 采用并不普遍，许多人使用频率低](#item-15) ⭐️ 7.0/10
16. [OpenAI 推出 1.5 亿美元合作伙伴网络，加速企业 AI 应用](#item-16) ⭐️ 7.0/10
17. [EAGLE 投机解码合并入 llama.cpp](#item-17) ⭐️ 7.0/10
18. [Nemotron Super 在深度上下文中击败竞争对手 LLM 基准测试](#item-18) ⭐️ 7.0/10
19. [双 DGX Spark 在 Deepseek V4 Flash 上达到 40 tk/s](#item-19) ⭐️ 7.0/10
20. [Strix Halo 与 DGX Spark：本地大模型台式机对决](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [小米 MiMo V2.5 采用 DFlash 和持久内核实现 1000-3000 tps](https://www.reddit.com/r/LocalLLaMA/comments/1u5jtr8/xiaomi_is_now_serving_mimo_v25_at_10003000tps/) ⭐️ 9.0/10

小米宣布其 MiMo V2.5 模型采用 DFlash 和持久内核技术，实现了每秒 1000-3000 tokens 的推理速度，DFlash 模型已发布，并承诺即将开源。 这代表了 LLM 推理服务的重大突破，因为实现如此高的吞吐量（1000-3000 tps）可以大幅降低生产部署的延迟和成本，使大规模 AI 应用更加实用和普及。 MiMo V2.5 是一个 1.02 万亿参数的混合专家（MoE）模型，拥有 420 亿活跃参数和 100 万 token 的上下文窗口，基于混合注意力架构。DFlash 模型已可供使用，而服务栈的开源版本承诺即将发布。

reddit · r/LocalLLaMA · /u/Dany0 · 6月14日 12:26

**背景**: 混合专家（MoE）模型每个 token 只激活部分参数，从而在较低计算量下实现高容量。持久内核技术（如 Mirage Persistent Kernel）将多个 GPU 操作融合为一次内核启动，减少开销并降低延迟。DFlash（可能是小米的另一项优化）进一步提升了吞吐量。这些进步对于高效服务大型模型至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/mimo-v2-5-pro">MiMo - V 2 . 5 -Pro | Xiaomi</a></li>
<li><a href="https://huggingface.co/XiaomiMiMo/MiMo-V2.5">XiaomiMiMo/ MiMo - V 2 . 5 · Hugging Face</a></li>
<li><a href="https://github.com/mirage-project/mirage">GitHub - mirage-project/mirage: Mirage Persistent Kernel : Compiling...</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#Xiaomi`, `#MiMo`, `#DFlash`, `#open source`

---

<a id="item-2"></a>
## [里约热内卢'自研'大模型被发现是模型合并产物](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

里约热内卢市政府发布了 Rio-3.5-Open-397B 模型，声称是自研微调版本，但分析表明它实际上是 Nex-N2 Pro 和 Qwen3.5-397B-A17B 的线性合并（比例约为 60%与 40%），且未进行适当披露。 这一争议凸显了开源 AI 中透明度和归属的重要性，虚假宣称会侵蚀公众信任，并为道德标准树立不良先例。 Rio 模型的每个权重张量在所有 60 层和组件中都与 Nex-N2 Pro 和 Qwen 的 0.6/0.4 混合比例完全一致，表明是简单的线性插值而非微调或蒸馏。

hackernews · unrvl22 · 6月14日 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48528371)

**背景**: 模型合并是一种将多个预训练大语言模型的权重组合以提升性能的技术，无需额外训练。线性合并是其最简单形式，对对应权重求平均。Nex-N2 Pro 是一个 397B 开源模型，本身可能基于 Qwen。Rio 模型被宣传为专有微调版本，但实际上似乎是直接合并而未作修改。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/nex-agi/Nex-N2-Pro">nex-agi/ Nex - N 2 - Pro · Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：有人推测上传的检查点遗漏了蒸馏步骤，也有人批评缺乏归属。评论者指出类似做法可能在全球初创企业中普遍存在，引发对学术诚信的广泛担忧。

**标签**: `#LLM`, `#open-source`, `#controversy`, `#attribution`, `#AI ethics`

---

<a id="item-3"></a>
## [Anthropic 的 AI 安全立场被批虚伪](https://www.verysane.ai/p/did-anthropic-ask-for-this) ⭐️ 8.0/10

Hacker News 上的社区讨论批评 Anthropic 可能存在的虚伪行为，认为该公司一边倡导严格的 AI 监管，一边推广自己的强大 AI 模型，并设置只有自己才能达到的监管门槛。 这场辩论凸显了 AI 治理中的一个核心矛盾：公司在倡导安全监管的同时，是否还能可靠地竞争构建最强大的系统，并可能影响政策以利于自己的产品。 评论者将 Anthropic 类比为卖危险产品却呼吁监管的'末日设备公司'，并指出 Anthropic CEO Dario Amodei 可能设定了竞争对手无法达到的高安全标准，以构建'护城河'。

hackernews · ad8e · 6月14日 22:23 · [社区讨论](https://news.ycombinator.com/item?id=48533504)

**背景**: Anthropic 是一家由前 OpenAI 员工创立的 AI 公司，专注于 AI 安全和负责任的发展。该公司发布了 Claude 等强大模型，同时一直敦促政府对高级 AI 系统进行监管。批评者认为这种双重角色造成了利益冲突。

**社区讨论**: 评论者对 Anthropic 的动机表示怀疑，有人将其比作末日设备公司以说明其虚伪。另一位评论者指出，拥有非凡权力往往会导致傲慢，并暗示 Anthropic 的 CEO 可能正在构建监管护城河。还有评论者认为 Anthropic 真正担心存在风险，应在此背景下评估其行为，并将其与 OpenAI 更激进的游说活动进行对比。

**标签**: `#AI safety`, `#Anthropic`, `#AI governance`, `#ethics`, `#existential risk`

---

<a id="item-4"></a>
## [形式方法与编程的未来](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

简街（Jane Street）发布了一篇博客文章，讨论了形式方法在编程中的实际应用和未来潜力，强调了它们在软件验证中的作用以及自动化的挑战。 这很重要，因为形式方法可以大幅提高软件可靠性，尤其是在 AI 生成代码日益普及的背景下，将人类的精力从编写代码转移到验证代码的正确性上。 博客讨论了历史上正确性证明的工作，包括使用 SAT 求解器和 Boyer-Moore 证明器，并指出像 Scala 3 的表达性类型这样的现代系统可以携带编译时证明。

hackernews · eatonphil · 6月14日 12:35 · [社区讨论](https://news.ycombinator.com/item?id=48526633)

**背景**: 形式方法是用于规范、开发和验证软件与硬件系统的数学严格技术。与测试不同，它们可以在执行前证明正确性。然而，它们需要大量人类努力来引导定理证明器和构建引理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Software_verification">Software verification - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论包括关于形式规范是否只是另一种测试形式的辩论，有人认为证明也可能有错误。另一些人强调了形式方法在 AI 辅助编码中的价值，因为此时验证变得至关重要。

**标签**: `#formal methods`, `#verification`, `#programming languages`, `#Jane Street`, `#AI-assisted programming`

---

<a id="item-5"></a>
## [Yserver：用 Rust 编写的现代 X11 服务器](https://github.com/joske/yserver) ⭐️ 8.0/10

Yserver 是一个用 Rust 编写的新 X11 服务器实现，目前已能与 XFCE4 等桌面环境配合使用，但需要禁用合成器才能稳定运行。 该项目展示了使用现代系统语言 Rust 来提升 X Window System（类 Unix 操作系统的关键组件）的内存安全性和性能的潜力。 Yserver 明确放弃了对多显示器的支持，视其为遗留负担，并且目前与 LightDM 等显示管理器集成不佳，需要从 TTY 手动启动。

hackernews · Venn1 · 6月14日 19:10 · [社区讨论](https://news.ycombinator.com/item?id=48531394)

**背景**: X Window System（X11）是广泛应用于类 Unix 系统的位图窗口系统，X.Org Server 是其参考实现。Rust 是一种提供内存安全性且无需垃圾回收的系统编程语言。用 Rust 重写 X11 组件可能减少安全漏洞并提高可维护性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X11_server">X11 server</a></li>
<li><a href="https://en.wikipedia.org/wiki/Direct_Rendering_Infrastructure">Direct Rendering Infrastructure - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些人称赞项目的进展，而另一些人则批评移除多显示器支持的做法忽视了实际使用场景。还讨论了网络透明性，一些用户更倾向于 X11 的网络能力而非 Wayland 的方案。

**标签**: `#Rust`, `#X11`, `#Window System`, `#Open Source`, `#Systems Programming`

---

<a id="item-6"></a>
## [《JavaScript 的诞生与死亡》（2014）：一场预言性的演讲](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 8.0/10

Gary Bernhardt 在 2014 年的演讲《JavaScript 的诞生与死亡》幽默地预言了 JavaScript 将成为一个无处不在的编译目标，这一预言随着 TypeScript、asm.js 和 WebAssembly 的兴起在很大程度上已成为现实。 这场演讲准确预见了 JavaScript 作为编译目标的角色，影响了开发者对 Web 技术的思考方式，并突显了转译的趋势。随着 WebAssembly 和其他编译到 JavaScript 的语言不断发展，它仍然具有现实意义。 该演讲在一次会议上发表，现可在 Destroy All Software 上观看。它引入了 asm.js 等概念，后来被 WebAssembly 取代。演讲还开玩笑地预测了 2020-2025 年间的一场全球灾难，评论者指出这与 COVID-19 大流行惊人地接近。

hackernews · subset · 6月14日 12:38 · [社区讨论](https://news.ycombinator.com/item?id=48526661)

**背景**: JavaScript 最初被设计为 Web 浏览器的脚本语言。随着时间的推移，开发者希望在网上使用其他语言，导致了像 Emscripten 这样的工具，将 C/C++编译为 JavaScript。Asm.js 是 JavaScript 的一个严格子集，能够为这类编译后的代码提供接近原生的性能。WebAssembly 是一种二进制指令格式，此后成为 Web 首选的编译目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asm.js">Asm.js</a></li>
<li><a href="https://betterstack.com/community/guides/scaling-nodejs/typescript-target-compiler/">Understanding TypeScript's Target Compiler Option</a></li>
<li><a href="https://grokipedia.com/page/Asm.js">asm.js</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这场演讲是杰作，指出它准确预测了 JavaScript 作为编译目标的趋势。一些人指出 WebAssembly 进展不如预期快，仍然需要 JavaScript 进行 DOM 操作，而另一些人则庆祝 TypeScript 和 Electron 的兴起。关于全球灾难的预测也被认为具有惊人的先见之明。

**标签**: `#JavaScript`, `#WebAssembly`, `#programming languages`, `#predictions`

---

<a id="item-7"></a>
## [为何 AI 不会取代软件工程师](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 指出，数据并不支持 AI 导致软件工程大规模裁员的说法——纽约州在 WARN 法案申报中增设 AI 披露复选框的第一年里，没有任何一家公司勾选了该框。 这一分析为 AI 导致失业的普遍担忧提供了基于数据的反驳，表明软件工程所需的人类深度理解（如代码库和业务背景）使该职业比通常认为的更具韧性。 作者指出软件工程中难以自动化的三个真正瓶颈：决定构建什么、验证交付物，以及两者所需的深度人类理解。他们指出，即使有 AI 辅助，工程师的价值仍取决于他们对问题和解决方案的理解深度。

rss · Simon Willison · 6月14日 23:54

**背景**: 《工人调整和再培训通知法案》（WARN Act）要求 100 人以上雇主在大规模裁员前提前 60 天通知。2025 年 3 月，纽约州成为首个在 WARN 申报中增加 AI 披露复选框的州，询问“技术创新或自动化”是否导致裁员。第一年内没有任何公司勾选此框，为反对 AI 裁员叙事提供了经验证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WARN_Act">WARN Act</a></li>
<li><a href="https://www.hunton.com/hunton-employment-labor-perspectives/new-york-warn-act-no-ai-related-layoffs-reported-in-first-year-of-adding-ai-related-disclosure-to-the-system">New York WARN Act: No AI-Related Layoffs Reported in First Year of Adding AI-Related Disclosure to the System</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#job displacement`, `#economics`, `#labor market`

---

<a id="item-8"></a>
## [基于 Qwen3.5-397B 的实时本地语音聊天机器人](https://www.reddit.com/r/LocalLLaMA/comments/1u5uqsc/voicetovoice_chatbot_update/) ⭐️ 8.0/10

一位开发者构建了一个实时、可打断、完全本地的语音对话聊天机器人，集成了 Qwen3.5-397B、Whisper-small 语音识别和 Orpheus TTS，并使用了自定义 SNAC 解码器，在 24 GB GPU 上实现了接近实时的性能。 这表明像 Qwen3.5-397B 这样的大型开源模型可以在消费级硬件上实际部署用于实时语音交互，有望实现完全私密和可定制的语音助手。 在 24 GB GPU 上 VRAM 占用保持在 21.3 GB，系统 RAM 约 150 GB 用于 Qwen 的 MoE 专家层；系统使用 bf16 KV 缓存，支持 131,072 个 token，并通过 SSE 流式传输实现低延迟。

reddit · r/LocalLLaMA · /u/Responsible_Fig_1271 · 6月14日 19:45

**背景**: Qwen3.5-397B 是阿里巴巴推出的大型混合专家（MoE）语言模型，总参数量 397B（激活 17B）。Orpheus TTS 是基于 Llama 的开源文本转语音模型，而 SNAC（多尺度神经音频编解码器）可将音频压缩为离散编码以实现高效生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://build.nvidia.com/qwen/qwen3.5-397b-a17b/modelcard">qwen3.5-397b-a17b Model by Qwen | NVIDIA NIM</a></li>
<li><a href="https://github.com/canopyai/Orpheus-TTS">GitHub - canopyai/ Orpheus - TTS : Towards Human-Sounding Speech</a></li>
<li><a href="https://github.com/hubertsiuzdak/snac">GitHub - hubertsiuzdak/ snac : Multi-Scale Neural Audio Codec ...</a></li>

</ul>
</details>

**标签**: `#voice chatbot`, `#local LLM`, `#real-time`, `#Qwen3.5`, `#open-source`

---

<a id="item-9"></a>
## [Deepseek 4 Flash 可在 M3 Max Mac（96GB）上运行](https://www.reddit.com/r/LocalLLaMA/comments/1u5mfaq/you_can_run_deepseek_4_flash_on_mac_m3_max_96gb/) ⭐️ 8.0/10

一位用户成功在配备 96GB 内存的 M3 Max Mac 上使用 antirez 的 ds4 引擎和 SSD 流式加载运行了 DeepSeek V4 Flash（一个 284B 参数的 MoE 模型），达到了约 12-13 tokens/秒的速度。 这表明超大语言模型可以在消费级硬件上运行，使本地 LLM 推理对爱好者和开发者更加可及，无需昂贵的服务器 GPU。 设置需要使用 --ssd-streaming 标志并通过 iogpu.wired_limit_mb=86016 将 Metal 分配限制提高到 86016 MB。冷启动预填充约需 10 秒，但持续生成保持在 12 t/s 左右；一个 36k token 的提示需要 2.5 分钟预填充。

reddit · r/LocalLLaMA · /u/Zeeplankton · 6月14日 14:20

**背景**: DeepSeek V4 Flash 是一个 284B 参数的混合专家（MoE）模型，激活参数 13B，支持 1M token 上下文窗口。Antirez 的 ds4 引擎是一个开源本地推理引擎，支持 Metal、CUDA 和 ROCm。SSD 流式加载受 Apple 的“LLM in a Flash”研究启发，按需从存储加载模型权重，使得大于 RAM 的模型能在 Apple Silicon 上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek -V 4 - Flash · Hugging Face</a></li>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash and PRO local inference engine for Metal, CUDA and ROCm · GitHub</a></li>
<li><a href="https://build.nvidia.com/deepseek-ai/deepseek-v4-flash">deepseek -v 4 - flash Model by Deepseek -ai | NVIDIA NIM</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#local-llm`, `#mac`, `#performance`, `#guide`

---

<a id="item-10"></a>
## [Kage：将任何网站打包成单个二进制文件供离线查看](https://github.com/tamnd/kage) ⭐️ 7.0/10

Kage 是一款新的开源命令行工具，它捕获完整的交互式网站快照，并将其打包成单个可执行二进制文件，无需任何依赖即可离线查看。 该工具简化了离线共享和访问网页内容的过程，适用于需要在低连通性环境下进行离线文档、原型审查或协作的团队。 Kage 使用无头 Chrome 渲染页面并剥离 JavaScript，然后将内容打包成一个独立的二进制文件，该文件内置 HTTP 服务器，用于提供离线站点服务。

hackernews · tamnd · 6月14日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=48529990)

**背景**: 离线网页归档工具如 HTTrack 或 SingleFile 将网页保存为文件，而 Kage 生成包含服务器的单个二进制文件，使其便携且易于共享。它使用无头 Chrome 忠实捕获页面在 JavaScript 执行后的视觉状态，但随后剥离脚本以确保安全性和简洁性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tamnd/kage">GitHub - tamnd/kage: Shadow any website for offline viewing, with the JavaScript stripped out · GitHub</a></li>
<li><a href="https://cybermediacreations.com/show-hn-kage-shadow-any-website-to-a-single-binary-for-offline-viewing/">Show HN: Kage – Shadow any website to a single binary for offline...</a></li>

</ul>
</details>

**社区讨论**: 社区评论注意到了使用 ascii-gif 生成演示 GIF、HTTP 站点导致获取错误的问题，以及对离线维基和 AI 原型的潜在用途。用户还质疑内置服务器的必要性，更倾向于直接浏览器打开。

**标签**: `#offline`, `#web-archiving`, `#tool`, `#open-source`, `#static-site`

---

<a id="item-11"></a>
## [Zeroserve 实现 Caddy 兼容性，速度大幅提升](https://su3.io/posts/zeroserve-caddy-compat) ⭐️ 7.0/10

基于 eBPF 的 Web 服务器 Zeroserve 现已声称与 Caddy 兼容，吞吐量提升 3 倍，延迟降低 70%，但缺少 ACME 支持并引发 io_uring 安全担忧。 这一性能飞跃可能挑战 Nginx 和 Caddy 等成熟服务器，但缺少核心功能（ACME）和安全问题限制了其在生产 HTTPS 服务中的实际采用。 Zeroserve 使用 io_uring 实现异步 I/O，提升了性能但被认为不如 libuv 等替代方案安全；兼容性不包括 Caddy 的 ACME 或插件系统。

hackernews · losfair · 6月14日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=48527145)

**背景**: Zeroserve 是一款零配置、高性能的 HTTPS 服务器，使用 eBPF 进行脚本编写，并采用 io_uring 实现异步 I/O。Caddy 因其通过 ACME 自动管理 HTTPS 而广受欢迎。io_uring 是 Linux 内核中用于高效异步 I/O 的接口，但其安全模型备受质疑，特别是对于面向网络的服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sesamedisk.com/zeroserve-ebpf-web-server-infrastructure/">Zeroserve : An eBPF-Powered Web Server Without... - Sesame Disk</a></li>
<li><a href="https://su3.io/posts/introducing-zeroserve">zeroserve : a zero -config web server you can script with eBPF</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_uring">Io uring</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调缺少 ACME 是一个致命问题，codingjoe 称其为'去除所有关键功能的 Caddy 兼容'。有用户报告了 Chrome 针对 zeroserve 域名弹出奇怪的证书选择框，pbohun 则质疑 io_uring 在 Web 服务器中的安全性，指出安全资料建议避免使用。

**标签**: `#web server`, `#performance`, `#io_uring`, `#Caddy`, `#zeroserve`

---

<a id="item-12"></a>
## [艾伦·珀利斯的编程箴言（1982）](https://www.cs.yale.edu/homes/perlis-alan/quotes.html) ⭐️ 7.0/10

一篇收录艾伦·珀利斯（Alan Perlis）133 条编程语录的文章被在线分享和讨论，这些语录最初发表于 1982 年的《编程警句》一书中，展现了计算机科学的永恒智慧。 珀利斯的语录与现代编程辩论（包括关于 AI 生成代码和语言设计的讨论）密切相关，证明了计算机科学的基本原则跨越时代。 这些语录涵盖了从语言设计到软件工程的主题，一些评论指出它们在自然语言编程和大语言模型等当代问题上的先见之明。

hackernews · tosh · 6月14日 14:56 · [社区讨论](https://news.ycombinator.com/item?id=48527820)

**背景**: 艾伦·珀利斯（Alan Perlis）是一位图灵奖得主、计算机科学家，也是编程语言领域的先驱。他的《编程警句》是一系列简洁而有洞察力的陈述，对编程和软件开发实践进行了批判和反思，已成为计算机科学文献中的经典参考。

**社区讨论**: 社区评论对珀利斯的语录表示赞赏，特别是关于语言影响思维和自然语言编程挑战的语句。用户还分享了相关资源，如一个虚构的 Perl 程序员的视频和一个专门展示这些语录的域名。

**标签**: `#programming-quotes`, `#computer-science`, `#alan-perlis`, `#software-engineering`, `#programming-philosophy`

---

<a id="item-13"></a>
## [保罗·格雷厄姆探讨亿万财富的道德性](https://paulgraham.com/earn.html) ⭐️ 7.0/10

保罗·格雷厄姆的文章《如何赚取十亿美元》探讨了赚取与获取巨额财富的概念，挑战了对亿万富翁的常见道德批评。 这篇文章引发了关于财富创造、创业以及初创企业社会价值的重要讨论，在科技和创业社区中引起了强烈共鸣。 文章认为，通过创造有价值的产品或服务赚取十亿美元，与通过剥削或寻租攫取财富在道德上是不同的。

hackernews · kingstoned · 6月14日 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48526360)

**背景**: 保罗·格雷厄姆是著名风险投资家、散文家及 Y Combinator 联合创始人。他常撰写关于创业和技术的文章。此文回应了常见的批评——亿万富翁必然以不道德方式致富。

**社区讨论**: 评论高度两极分化。一些人赞同格雷厄姆对赚取与攫取的区分，而另一些人则认为巨额财富本质上涉及对劳动力的剥削或市场操纵。

**标签**: `#wealth creation`, `#startups`, `#entrepreneurship`, `#Paul Graham`, `#morality`

---

<a id="item-14"></a>
## [Linux 7.1 发布，AI 驱动移除旧驱动](https://lore.kernel.org/lkml/CAHk-=wi4BF4bMhZNZ1tqs+FFV4OuZRe3ZqdWB+LxRLmRweUzQw@mail.gmail.com/T/#u) ⭐️ 7.0/10

Linux 7.1 内核已发布，显著特点是移除了 ISDN 及其他过时网络驱动代码，此举源于 AI 辅助的 bug 报告让维护者不堪重负。 减少遗留代码有助于内核维护者专注于当前硬件，也反映出利用 AI 识别并消除大型开源项目技术债务的趋势。 移除针对很少使用的过时硬件驱动，减少 bug 报告噪音。此外，Linux 7.1 引入了新的 NTFS 驱动，取代了 Paragon 老旧的 ntfs3。

hackernews · berlianta · 6月14日 16:01 · [社区讨论](https://news.ycombinator.com/item?id=48528729)

**背景**: 近期，Linux 内核维护者被大量 AI 生成的 bug 报告淹没，许多是重复或低质量的。为减轻负担，Linus Torvalds 等人决定清理无人使用的死代码，例如已过时的 ISDN 驱动。此举不仅减轻维护压力，也使内核更精简。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://systemadministration.net/ai-is-starting-to-overwhelm-linux-maintainers-with-duplicate-bug-reports/">AI is starting to overwhelm Linux maintainers with duplicate bug reports</a></li>
<li><a href="https://www.omgubuntu.co.uk/2026/06/linux-7-1-kernel-features">Linux 7.1 brings new NTFS driver , Steam Deck OLED... - OMG! Ubuntu</a></li>
<li><a href="https://logicity.in/en/blog/ai-bug-reports-overwhelm-linux-security-list-torvalds-says">AI Bug Reports Overwhelm Linux Security List, Torvalds Says | Logicity</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍赞赏 AI 驱动的清理，一位评论者称这是‘AI 带来的最好后果之一’。其他人对新 NTFS 驱动和 Arch Linux 即将更新到 7.1 表示兴奋。

**标签**: `#Linux`, `#kernel`, `#AI`, `#bug reporting`, `#open source`

---

<a id="item-15"></a>
## [AI 采用并不普遍，许多人使用频率低](https://gabrielweinberg.com/p/people-are-consuming-ai-like-they) ⭐️ 7.0/10

一篇文章指出 AI 采用并不普遍，超过 50%的人每周使用 AI 不到一次，挑战了“人人都在使用 AI”的说法。 这很重要，因为它提供了 AI 采用的现实视角，反驳了炒作，帮助企业和开发者专注于实际整合，而非假设普遍使用。 文章引用了一项研究，显示超过 50%的人每周使用 AI 不到一次，社区讨论认为 AI 的增长将来自融入现有软件，而非独立的聊天界面。

hackernews · yegg · 6月14日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=48527700)

**背景**: 像聊天机器人这样的人工智能工具已被快速采用，但关于它们实际使用范围和使用频率存在争议。一些人认为 AI 正变得无处不在，而另一些人则指出调查数据显示其常规使用有限。讨论常常集中在 AI 是保持小众工具还是深度融入日常软件。

**社区讨论**: 评论者指出，AI 融入现有软件（如搜索、电子邮件）比单独使用聊天更重要。有人分享了求职面试中雇主询问 LLM 使用情况的挑战，需要小心措辞。其他人表示怀疑，称尽管有炒作，但他们日常工作几乎没有受到影响。

**标签**: `#AI`, `#technology adoption`, `#software engineering`, `#community discussion`, `#Hacker News`

---

<a id="item-16"></a>
## [OpenAI 推出 1.5 亿美元合作伙伴网络，加速企业 AI 应用](https://openai.com/index/introducing-openai-partner-network) ⭐️ 7.0/10

OpenAI 宣布推出 OpenAI 合作伙伴网络，投入 1.5 亿美元支持全球合作伙伴加速企业 AI 的采用和部署。 这一举措标志着 OpenAI 向企业市场战略推进，提供资源以扩大 AI 在各行业的整合，并可能扩展其生态系统。 1.5 亿美元的投资将用于合作伙伴赋能、联合营销和技术支持，以推动企业转型。

rss · OpenAI News · 6月14日 17:00

**背景**: 企业采用 AI 通常需要专业知识和集成支持。合作伙伴网络在云和企业软件中很常见，以扩展覆盖范围并提供本地化服务。OpenAI 的网络旨在建立由顾问、系统集成商和经销商组成的生态系统。

**标签**: `#OpenAI`, `#enterprise AI`, `#partnership`, `#AI adoption`

---

<a id="item-17"></a>
## [EAGLE 投机解码合并入 llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1u5z4j0/eagle_support_merged_into_llamacpp/) ⭐️ 7.0/10

EAGLE 投机解码支持已被合并到 llama.cpp 仓库中，使得用户能够利用这项先进技术加速本地 LLM 推理。 此次合并将最先进的投机解码算法引入最广泛使用的本地 LLM 推理引擎之一，可能在不牺牲输出质量的情况下，将许多用户的推理速度提升一倍或两倍。 EAGLE 在目标模型的隐藏状态上附加一个轻量级的自回归预测头，每个步骤生成多个候选 token，相比标准自回归解码降低了延迟。

reddit · r/LocalLLaMA · /u/Diablo-D3 · 6月14日 22:45

**背景**: 投机解码是一种推理时优化技术，由一个小型草案模型提出一系列 token，再由较大的目标模型通过一次前向传播进行验证，同时保持原始输出分布。EAGLE（Extrapolation Algorithm for Greater Language-model Efficiency）在此基础上使用从目标模型隐藏状态外推的草案头，提供了更高的接受率和加速效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://grokipedia.com/page/EAGLE_speculative_decoding">EAGLE (speculative decoding)</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#EAGLE`, `#speculative decoding`, `#LLM inference`, `#open-source`

---

<a id="item-18"></a>
## [Nemotron Super 在深度上下文中击败竞争对手 LLM 基准测试](https://www.reddit.com/r/LocalLLaMA/comments/1u5vqpl/nemotron_king_of_the_deep_comparison_of_4_models/) ⭐️ 7.0/10

一位用户对四个高达 120B 参数的大语言模型在深度上下文（约 10 万 token）下的提示处理速度进行了基准测试，发现 Nemotron Super 优于 GPT-OSS 和 Qwen 模型，即使在 40 万 token 上下文深度下仍保持可用速度。 该基准测试为依赖大型模型进行代码分析等需要深度上下文任务的本地 LLM 用户提供了实用见解。它强调了常被忽略的提示处理速度可能成为关键瓶颈，并且 Nemotron Super 为此类用例提供了强大选择。 基准测试在配备 128GB 共享内存的 AMD Strix Halo APU 上运行，使用 Lemonade Server 和 Vulkan 后端，以及 llama-bench。作者采用了主观阈值：提示处理 100 TPS，token 生成 10/20 TPS 作为可用性指标。

reddit · r/LocalLLaMA · /u/Reasonable_Goat · 6月14日 20:25

**背景**: 参数数量多（例如 120B）的大语言模型常用于复杂任务，但由于内存和处理需求，在处理长上下文时可能会遇到困难。提示处理（PP）速度衡量模型摄入输入 token 的速度，而 token 生成（TG）速度衡量输出速度。AMD Strix Halo APU 是一种高性能芯片，拥有大统一内存，适合本地运行大型模型。Lemonade Server 是一个本地 LLM 服务工具，支持 Vulkan 等多种后端。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://d33gy59ovltp76.cloudfront.net/news/amd-s-game-changing-strix-halo-apu-formally-known-as-the-ryzen-ai-max-poses-for-new-die-shots-and-gets-annotated">AMD 's game-changing Strix Halo APU , formally known as</a></li>
<li><a href="https://lemonade-server.ai/docs/guide/concepts/">Local LLM Server Concepts - Lemonade Server Documentation</a></li>
<li><a href="https://github.com/eugr/llama-benchy">eugr/llama-benchy: llama-benchy - llama - bench style benchmarking ...</a></li>

</ul>
</details>

**标签**: `#LLM comparison`, `#local LLM`, `#prompt processing`, `#Nemotron`, `#deep context`

---

<a id="item-19"></a>
## [双 DGX Spark 在 Deepseek V4 Flash 上达到 40 tk/s](https://www.reddit.com/r/LocalLLaMA/comments/1u5g9pr/dual_dgx_sparks_40tks_single_1m_350_tks_agg/) ⭐️ 7.0/10

一位用户通过 200 Gb/s ConnectX-7 电缆连接两台 Nvidia DGX Spark，对 Deepseek V4 Flash 进行了基准测试，单请求达到约 40 tokens/s，在 32 个并发请求、256K 上下文长度下聚合速度达 350 tokens/s。 该配置表明，价格适中的双 DGX Spark 硬件能够以适合智能体使用的速度运行大型 MoE 模型，挑战了对昂贵数据中心 GPU 的需求。 DGX Spark 采用 Nvidia Grace Blackwell 平台，通过 vLLM 支持 FP8，200 Gb/s 互连电缆售价 180 美元，是实现此速度的关键。

reddit · r/LocalLLaMA · /u/elsung · 6月14日 09:07

**背景**: Nvidia DGX Spark 是一款紧凑型 AI 超级计算机，专为本地开发和大型模型推理设计。ConnectX-7 是一款高性能网络适配器，提供高达 400 Gb/s 的带宽。vLLM 是一个开源推理引擎，支持 FP8 量化，可减少内存使用并提高吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DGX_Spark">DGX Spark</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/quantization/fp8.html">FP 8 W8A8 — vLLM</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区赞扬了详细的基准测试和实用指南，但也有人指出额外 180 美元的电缆成本和两台设备的需求可能限制可及性。用户讨论了 Mac Studio M2 Ultra 和 RTX Pro 6000 等替代配置的比较。

**标签**: `#hardware`, `#benchmarking`, `#MOE models`, `#Deepseek`, `#LLM inference`

---

<a id="item-20"></a>
## [Strix Halo 与 DGX Spark：本地大模型台式机对决](https://www.reddit.com/r/LocalLLaMA/comments/1u59ibr/strix_halo_desktop_trying_to_compete_against_dgx/) ⭐️ 7.0/10

Reddit 上的一篇帖子将 AMD 的 Strix Halo APU 与 NVIDIA 的 DGX Spark 作为本地运行大语言模型的台式机方案进行了对比，突出了它们的统一内存架构。 这一比较有助于实践者在两款针对本地 AI 推理优化的新兴设备中做出选择，从而在没有云依赖的情况下普及强大 LLM 的使用。 Strix Halo 在 NUC 形态中提供高达 128GB 的统一内存，而 DGX Spark 则配备 20 核 Grace CPU 和 Blackwell GPU 及统一内存，两者均面向本地 AI 工作负载。

reddit · r/LocalLLaMA · /u/SkyFeistyLlama8 · 6月14日 02:53

**背景**: 本地 LLM 推理需要高内存带宽和容量，传统上由昂贵的服务器 GPU 满足。AMD 的 Strix Halo 和 NVIDIA 的 DGX Spark 是紧凑型桌面系统，集成了 CPU 和 GPU 并采用统一内存，适合本地运行 LLaMA 等模型。这些设备旨在为个人用户带来 AI 超级计算能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=vMGX35mzsWg">AMD 's Most Powerful APU Yet - Strix Halo /Ryzen AI Max+... - YouTube</a></li>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nvidia_RTX_Spark">Nvidia RTX Spark</a></li>

</ul>
</details>

**标签**: `#hardware`, `#LLM inference`, `#AMD`, `#NVIDIA`, `#local AI`

---