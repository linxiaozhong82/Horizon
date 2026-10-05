---
layout: default
title: "Horizon Summary: 2026-10-05 (ZH)"
date: 2026-10-05
lang: zh
---

> 从 20 条内容中筛选出 4 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：local-llm-inference、ARC-AGI、macOS、quantization、AI benchmarks。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Strata 在单张 RTX 4090 上以约 124 tokens/秒运行 125B 的 Qwen3.8-Flash-Next](https://github.com/Niko1221/Strata)**
2. **[ARC-AGI-3 的 Kaggle 分数在 30 天内从 7% 飙升至 56%](https://www.reddit.com/r/MachineLearning/comments/1wxcd4k/top_arc%CE%B1gi3_scores_on_kaggle_just_went_from_7_to/)**
3. **[RemoveMacAI 工具可从 macOS 中剥离 Apple Intelligence 以回收磁盘空间](https://github.com/omlahore/RemoveMacAI)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [RemoveMacAI 工具可从 macOS 中剥离 Apple Intelligence 以回收磁盘空间](https://github.com/omlahore/RemoveMacAI)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. 算力芯片与服务器

- **关联热点**: [Strata 在单张 RTX 4090 上以约 124 tokens/秒运行 125B 的 Qwen3.8-Flash-Next](https://github.com/Niko1221/Strata)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Strata 在单张 RTX 4090 上以约 124 tokens/秒运行 125B 的 Qwen3.8-Flash-Next

**关联新闻**: [Strata 在单张 RTX 4090 上以约 124 tokens/秒运行 125B 的 Qwen3.8-Flash-Next](https://github.com/Niko1221/Strata)

**切入角度**: GitHub 项目 Strata（Niko1221/Strata）展示了如何在单张消费级 RTX 4090 上运行 Qwen 开放权重的 Qwen3.8-Flash-Next——一个约 125B 参数的多模态混合专家（MoE）模型；有用户在 4090 搭配 128GB DDR5 内存与 Ryzen 7950X3D 的机器上实测达到 124 tokens/秒。 如果这些数字站得住脚，这将标志着本地大模型推理的一个重要里程碑：原本需要服务器级硬件才能承载的模型，如今可以在许多爱好者已拥有的设备上实现交互式服务。同时，这也给 llama.cpp 等成熟本地推理运行时带来了更大的竞争压力，社区普遍将 llama.cpp 视为端侧推理的事实标准。 该成绩依赖激进的 4-bit 以下量化以及对系统内存的卸载，因此引发了对质量损失的质疑；一位用户在同一份 GGUF 与视觉适配器权重上做的独立视觉基准显示，Strata 的坐标中位误差为 154.8 像素，而 llama.cpp 仅为 46.5 像素；另有用户报告在租用的 RTX Pro 6000 上吞吐表现强劲（约 1 美元/小时可产出约 120 万 tokens，另一套栈的解码速度达 255 tokens/秒）。

**可延展方向**: Qwen3.8-Flash-Next 是阿里 Qwen 团队发布的开放权重稀疏混合专家多模态模型，作为 Qwen4 架构的早期预览版，原生支持 262,144 token 上下文，并能处理文本、代码与图像。混合专家模型在生成每个 token 时只激活一部分参数，这正是 125B 级模型能跑出远超其体量预期速度的原因，但仍需要足够内存容纳全部权重。量化技术会压缩这些权重——常见为 4 bit，Strata 更是压到更低——以牺牲数值精度换取大幅降低的显存占用和更高的速度。Strata 的卖点是这一切完全在本地 PC 上完成，数据不出本机。

---

### 选题 2：ARC-AGI-3 的 Kaggle 分数在 30 天内从 7% 飙升至 56%

**关联新闻**: [ARC-AGI-3 的 Kaggle 分数在 30 天内从 7% 飙升至 56%](https://www.reddit.com/r/MachineLearning/comments/1wxcd4k/top_arc%CE%B1gi3_scores_on_kaggle_just_went_from_7_to/)

**切入角度**: r/MachineLearning 上的一篇 Reddit 帖子称，ARC-AGI-3 在 Kaggle 排行榜上的最高分在过去 30 天内从 7% 上升到 56%，取得该成绩的是被「harness」包裹的小型本地模型，而不是前沿大规模模型。发帖人还提到，他分享的排行榜截图已经有些过时，因此这个数字可能已经不再是最新状态。 如果这一说法属实，那么这对于一个刻意设计成「人类容易、AI 困难」的基准测试而言是一次惊人的跃升，意味着小型本地模型加上脚手架（scaffolding）可能已经在交互式推理任务上超过普通人类的水平。同时，它也会让一个争论更加尖锐：基准分数究竟反映的是真实的推理能力，还是外围 harness 与搜索策略的有效性。 该说法几乎没有附带任何技术细节——只有一张排行榜截图和一段简短评论——并且依赖 Kaggle 比赛对参赛者只能使用相对小型本地模型的规则限制，这让结果更加出人意料，但也更难以验证。harness 式的脚手架（提示工程、反复重试、搜索或工具调用循环）往往会把表面分数推高到远超底层模型单次推理所能达到的水平。

**可延展方向**: ARC-AGI（Abstraction and Reasoning Corpus，抽象与推理语料库）是由 François Chollet 提出的一系列基准测试，用于衡量 AI 系统的流体智力。前两个版本考察的是被动的解题能力，而 ARC-AGI-3 是一个交互式基准：智能体必须探索陌生的环境、即时推断目标、构建可适应的世界模型并持续学习；拿到 100% 意味着智能体能像人类一样高效地通关每一个游戏。Kaggle 曾举办过与 ARC Prize 相关的竞赛，在此语境下，「harness」指的是驱动模型的外围代码——负责喂入输入、重试、管理搜索——而不是模型本身。小型本地模型在此值得一提，是因为比赛规则禁止参赛者使用大型托管的前沿模型。

---

### 选题 3：RemoveMacAI 工具可从 macOS 中剥离 Apple Intelligence 以回收磁盘空间

**关联新闻**: [RemoveMacAI 工具可从 macOS 中剥离 Apple Intelligence 以回收磁盘空间](https://github.com/omlahore/RemoveMacAI)

**切入角度**: 一个名为 RemoveMacAI 的 GitHub 项目发布了脚本，用于从 macOS 中移除 Apple Intelligence 相关组件，从而让用户回收这些本地模型和资源所占用的磁盘空间。该工具在 Hacker News 上引发了热烈讨论（361 分、222 条评论），话题围绕用户控制权、隐私以及 Apple 的产品决策展开。 这说明即使在长期以干净、精选体验著称的 macOS 上，用户如今也觉得有必要运行第三方“去臃肿”脚本来夺回对自己系统的控制权，这与 Windows 上的常见做法如出一辙。由于 Apple Intelligence 在受支持的 Mac 上默认开启，且并没有一个能一次性关闭全部相关资源的全局开关，该工具折射出 Apple 的 AI 战略与用户自主权之间更广泛的张力。 macOS 上的 Apple Intelligence 仅在 Apple 芯片的 Mac（M1 及更新型号）上运行，Intel Mac 不受影响，而且其本地模型体量相对较小，并非前沿规模。删除操作是非官方的、基于脚本的，这意味着它可能导致 AI 功能失效、可能干扰系统更新，并且在重大系统升级后需要重新运行。

**可延展方向**: Apple Intelligence 是 Apple 于 2024 年 6 月 10 日在 WWDC 上发布的一系列 AI 功能，作为 iOS 18、iPadOS 18 和 macOS Sequoia 的内置特性推出；它对受支持的设备免费，结合了本地处理与服务器端模型。其功能包括写作工具、图像生成、通知摘要、Photos 修图以及可选的 ChatGPT 集成。“去臃肿（debloating）”指的是移除厂商默认预装的软件和后台组件，这种做法长期以来与 O&O ShutUp10、Winhance 等 Windows 工具联系在一起。

---

1. [Strata 在单张 RTX 4090 上以约 124 tokens/秒运行 125B 的 Qwen3.8-Flash-Next](#item-1) ⭐️ 8.0/10
2. [ARC-AGI-3 的 Kaggle 分数在 30 天内从 7% 飙升至 56%](#item-2) ⭐️ 8.0/10
3. [RemoveMacAI 工具可从 macOS 中剥离 Apple Intelligence 以回收磁盘空间](#item-3) ⭐️ 7.0/10
4. [Nolan Lawson 追问：开发者为何仍不愿“使用平台”原生 API](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Strata 在单张 RTX 4090 上以约 124 tokens/秒运行 125B 的 Qwen3.8-Flash-Next](https://github.com/Niko1221/Strata) ⭐️ 8.0/10

GitHub 项目 Strata（Niko1221/Strata）展示了如何在单张消费级 RTX 4090 上运行 Qwen 开放权重的 Qwen3.8-Flash-Next——一个约 125B 参数的多模态混合专家（MoE）模型；有用户在 4090 搭配 128GB DDR5 内存与 Ryzen 7950X3D 的机器上实测达到 124 tokens/秒。 如果这些数字站得住脚，这将标志着本地大模型推理的一个重要里程碑：原本需要服务器级硬件才能承载的模型，如今可以在许多爱好者已拥有的设备上实现交互式服务。同时，这也给 llama.cpp 等成熟本地推理运行时带来了更大的竞争压力，社区普遍将 llama.cpp 视为端侧推理的事实标准。 该成绩依赖激进的 4-bit 以下量化以及对系统内存的卸载，因此引发了对质量损失的质疑；一位用户在同一份 GGUF 与视觉适配器权重上做的独立视觉基准显示，Strata 的坐标中位误差为 154.8 像素，而 llama.cpp 仅为 46.5 像素；另有用户报告在租用的 RTX Pro 6000 上吞吐表现强劲（约 1 美元/小时可产出约 120 万 tokens，另一套栈的解码速度达 255 tokens/秒）。

hackernews · snehesht · 10月4日 12:51 · [社区讨论](https://news.ycombinator.com/item?id=49953495)

**背景**: Qwen3.8-Flash-Next 是阿里 Qwen 团队发布的开放权重稀疏混合专家多模态模型，作为 Qwen4 架构的早期预览版，原生支持 262,144 token 上下文，并能处理文本、代码与图像。混合专家模型在生成每个 token 时只激活一部分参数，这正是 125B 级模型能跑出远超其体量预期速度的原因，但仍需要足够内存容纳全部权重。量化技术会压缩这些权重——常见为 4 bit，Strata 更是压到更低——以牺牲数值精度换取大幅降低的显存占用和更高的速度。Strata 的卖点是这一切完全在本地 PC 上完成，数据不出本机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen/Qwen3.8-Flash-Next · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论既热情又尖锐：多位评论者怀疑 4-bit 以下量化能否保住模型质量，其中一人给出了量化视觉基准，显示在相同权重下 Strata 的误差是 llama.cpp 的三倍以上。也有人分享了在租用 RTX Pro 6000 上的正面吞吐与成本数据，同时至少有一位评论者警告说该模型在各 LLM 论坛被大量刷屏，最终评价仍有待时间检验。

**标签**: `#local-llm-inference`, `#quantization`, `#qwen`, `#gpu-optimization`, `#llm-serving`

---

<a id="item-2"></a>
## [ARC-AGI-3 的 Kaggle 分数在 30 天内从 7% 飙升至 56%](https://www.reddit.com/r/MachineLearning/comments/1wxcd4k/top_arc%CE%B1gi3_scores_on_kaggle_just_went_from_7_to/) ⭐️ 8.0/10

r/MachineLearning 上的一篇 Reddit 帖子称，ARC-AGI-3 在 Kaggle 排行榜上的最高分在过去 30 天内从 7% 上升到 56%，取得该成绩的是被「harness」包裹的小型本地模型，而不是前沿大规模模型。发帖人还提到，他分享的排行榜截图已经有些过时，因此这个数字可能已经不再是最新状态。 如果这一说法属实，那么这对于一个刻意设计成「人类容易、AI 困难」的基准测试而言是一次惊人的跃升，意味着小型本地模型加上脚手架（scaffolding）可能已经在交互式推理任务上超过普通人类的水平。同时，它也会让一个争论更加尖锐：基准分数究竟反映的是真实的推理能力，还是外围 harness 与搜索策略的有效性。 该说法几乎没有附带任何技术细节——只有一张排行榜截图和一段简短评论——并且依赖 Kaggle 比赛对参赛者只能使用相对小型本地模型的规则限制，这让结果更加出人意料，但也更难以验证。harness 式的脚手架（提示工程、反复重试、搜索或工具调用循环）往往会把表面分数推高到远超底层模型单次推理所能达到的水平。

reddit · r/MachineLearning · /u/we_are_mammals · 10月4日 10:24 · [社区讨论](https://www.reddit.com/r/MachineLearning/comments/1wxcd4k/top_arcαgi3_scores_on_kaggle_just_went_from_7_to/)

**背景**: ARC-AGI（Abstraction and Reasoning Corpus，抽象与推理语料库）是由 François Chollet 提出的一系列基准测试，用于衡量 AI 系统的流体智力。前两个版本考察的是被动的解题能力，而 ARC-AGI-3 是一个交互式基准：智能体必须探索陌生的环境、即时推断目标、构建可适应的世界模型并持续学习；拿到 100% 意味着智能体能像人类一样高效地通关每一个游戏。Kaggle 曾举办过与 ARC Prize 相关的竞赛，在此语境下，「harness」指的是驱动模型的外围代码——负责喂入输入、重试、管理搜索——而不是模型本身。小型本地模型在此值得一提，是因为比赛规则禁止参赛者使用大型托管的前沿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arcprize.org/leaderboard">ARC-AGI-3 Leaderboard - ARC Prize</a></li>
<li><a href="https://github.com/EleutherAI/lm-evaluation-harness">GitHub - EleutherAI/lm-evaluation-harness: A framework for ...</a></li>

</ul>
</details>

**标签**: `#ARC-AGI`, `#AI benchmarks`, `#reasoning`, `#Kaggle`, `#local models`

---

<a id="item-3"></a>
## [RemoveMacAI 工具可从 macOS 中剥离 Apple Intelligence 以回收磁盘空间](https://github.com/omlahore/RemoveMacAI) ⭐️ 7.0/10

一个名为 RemoveMacAI 的 GitHub 项目发布了脚本，用于从 macOS 中移除 Apple Intelligence 相关组件，从而让用户回收这些本地模型和资源所占用的磁盘空间。该工具在 Hacker News 上引发了热烈讨论（361 分、222 条评论），话题围绕用户控制权、隐私以及 Apple 的产品决策展开。 这说明即使在长期以干净、精选体验著称的 macOS 上，用户如今也觉得有必要运行第三方“去臃肿”脚本来夺回对自己系统的控制权，这与 Windows 上的常见做法如出一辙。由于 Apple Intelligence 在受支持的 Mac 上默认开启，且并没有一个能一次性关闭全部相关资源的全局开关，该工具折射出 Apple 的 AI 战略与用户自主权之间更广泛的张力。 macOS 上的 Apple Intelligence 仅在 Apple 芯片的 Mac（M1 及更新型号）上运行，Intel Mac 不受影响，而且其本地模型体量相对较小，并非前沿规模。删除操作是非官方的、基于脚本的，这意味着它可能导致 AI 功能失效、可能干扰系统更新，并且在重大系统升级后需要重新运行。

hackernews · privacyisntdead · 10月4日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=49957116)

**背景**: Apple Intelligence 是 Apple 于 2024 年 6 月 10 日在 WWDC 上发布的一系列 AI 功能，作为 iOS 18、iPadOS 18 和 macOS Sequoia 的内置特性推出；它对受支持的设备免费，结合了本地处理与服务器端模型。其功能包括写作工具、图像生成、通知摘要、Photos 修图以及可选的 ChatGPT 集成。“去臃肿（debloating）”指的是移除厂商默认预装的软件和后台组件，这种做法长期以来与 O&O ShutUp10、Winhance 等 Windows 工具联系在一起。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence</a></li>
<li><a href="https://www.apple.com/apple-intelligence/">Apple Intelligence and Siri - Apple</a></li>
<li><a href="https://winhance.net/">Winhance - Windows Enhancement Utility</a></li>

</ul>
</details>

**社区讨论**: 社区情绪褒贬不一，但总体上对 Apple 持批评态度：多位评论者将这一情况类比为 Windows 的去臃肿和 O&O ShutUp10，并抱怨 iOS 不像竞争对手那样提供简单的开关来禁用这些 AI 功能。也有人持相反意见，认为删除那些体量不大、表现均衡且能让推理不必上云的本地模型并不合理；还有评论者好奇 Apple 究竟如何权衡增加的磁盘占用与用户的烦恼，并回忆起当年用户不得不从 OS X 中删除数 GB 打印机驱动的往事。

**标签**: `#macOS`, `#Apple Intelligence`, `#privacy`, `#debloating`, `#system-tools`

---

<a id="item-4"></a>
## [Nolan Lawson 追问：开发者为何仍不愿“使用平台”原生 API](https://nolanlawson.com/2026/10/03/why-dont-more-developers-use-the-platform/) ⭐️ 7.0/10

Nolan Lawson 在其博客 nolanlawson.com 上发表了题为《Why don't more developers 'use the platform'?》的文章，探讨开发者为何依然偏爱框架和库，而不是浏览器原生平台 API。该文在 Hacker News 上引发了热烈讨论，获得约 278 分和 288 条评论。 这个问题触及前端开发中长期存在的矛盾：Web 平台不断加入原生能力，但生态的势能却持续流向 React 这类框架。如果平台 API 在争夺采用率的较量中反复落败，浏览器厂商和标准制定者或许需要重新思考这些 API 的设计与推广方式，而这又会反过来影响数以百万计 Web 应用的构建方式。 争论围绕具体案例展开：Web Components 往往不是被直接使用，而是通过 Lit 之类的封装库来使用；原生 HTML 的 `<datalist>` 元素则被批评为各大浏览器实现参差不齐、几乎无法实际使用。评论者还反驳了文中“自己动手构建只是更有趣”的说法，认为真正的原因是在处理实际任务时，平台 API 既繁琐又不可靠。

hackernews · vinhnx · 10月4日 04:10 · [社区讨论](https://news.ycombinator.com/item?id=49950554)

**背景**: “使用平台”（use the platform）是一句由来已久的口号，倡导开发者直接基于标准化的浏览器 API 来构建应用，例如 HTML、CSS、DOM、自定义元素和 Shadow DOM，而不是依赖第三方框架。Facebook 于 2013 年发布的 React 推广了基于组件、声明式的 UI 构建方式，并成为前端开发的主流选择。Web Components 是一组标准（Custom Elements、Shadow DOM、HTML Templates 和 ES Modules），目的是让开发者能原生地提供可复用、可封装的自定义元素；Lit 则是 Google 支持的一个轻量库，让编写这些组件更加容易。

**社区讨论**: 评论者普遍质疑“原生方案更快更好”这一前提，以 `<datalist>` 在多数浏览器中无法使用为例，并称 Web Components 是一个设计糟糕、难以上手的 API，几乎没有人会在不使用 Lit 或更大型框架的情况下采用它。也有人为 React 辩护，认为它设计相对良好、并不算臃肿，并指出这种选择本质上是主观的；此外，有从通用编程视角出发的评论者认为，Web API 不断增多却缺乏像 `read()`/`write()` 或 `epoll()` 那样可组合的抽象。

**标签**: `#web-platform`, `#javascript`, `#web-components`, `#react`, `#frontend-development`

---