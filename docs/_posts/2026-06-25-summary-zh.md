---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> 从 37 条内容中筛选出 19 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：reinforcement learning、open source、AI、self-play、AI infrastructure。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[通过自对弈强化学习、JAX 和 ViT 实现超人类 Generals.io 智能体](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/)**
2. **[Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks](https://www.latent.space/p/databricks)**
3. **[Claude Slackbot 升级：支持多人协作、主动和持久化智能体](https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [通过自对弈强化学习、JAX 和 ViT 实现超人类 Generals.io 智能体](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [Rust 社区推动将 crates.io 从 GitHub 发布解耦](https://infosec.exchange/@mttaggart/116806641273303255)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [OpenAI 发布首款定制芯片 Jalapeño，由博通制造](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：通过自对弈强化学习、JAX 和 ViT 实现超人类 Generals.io 智能体

**关联新闻**: [通过自对弈强化学习、JAX 和 ViT 实现超人类 Generals.io 智能体](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/)

**切入角度**: 开发者创建了一个用于 Generals.io 的自对弈强化学习智能体，在人类 1v1 排行榜上达到#1 排名，超越了顶级人类玩家。该智能体使用 JAX 进行可扩展计算，并采用 Vision Transformer 作为神经网络架构，整个流程已开源。 这项工作表明，通过 JAX 和 Vision Transformer 扩展计算和模型容量，可以在复杂的不完全信息游戏中实现超人类表现，减少对人工特征的依赖。模拟器和智能体的开源为游戏 AI 和强化学习社区提供了宝贵的资源。 该智能体从早期的 NumPy/Torch 版本完全重构为 JAX 实现，并将 CNN 替换为 Vision Transformer 以更好地捕捉空间关系。开发者的博客文章详细介绍了项目中遇到的死胡同、设计决策以及获得的实用见解。

**可延展方向**: Generals.io 是一款具有不完全信息的即时战略游戏，玩家控制军队夺取敌方将军。自对弈强化学习是指智能体通过与自己对战来不断学习改进。JAX 是一个用于高性能机器学习的数值计算库，支持快速模拟和梯度计算。Vision Transformer（ViT）是一种将 Transformer 注意力机制应用于图像补丁的神经网络架构，提供了卷积神经网络的替代方案。

---

### 选题 2：Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks

**关联新闻**: [Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks](https://www.latent.space/p/databricks)

**切入角度**: Databricks leaders argue for an open ecosystem to enable every company to build Agent Clouds.

---

### 选题 3：Claude Slackbot 升级：支持多人协作、主动和持久化智能体

**关联新闻**: [Claude Slackbot 升级：支持多人协作、主动和持久化智能体](https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive)

**切入角度**: Anthropic 对 Claude 的 Slack 集成进行了升级，支持多人协作、主动式和持久化智能体，使团队能够在 Slack 频道中与多个持续独立运行的 AI 智能体协同工作。 此次升级将 Claude 从简单的聊天机器人转变为跨对话持久的主动团队成员，有望提高团队在 Slack 工作流中的生产力和自动化水平。 新功能包括支持并发交互的多智能体协作、无需提示即可主动发起操作的主动式智能体能力，以及跨会话和频道保留上下文的持久化记忆。

**可延展方向**: 多智能体系统由多个交互的 AI 智能体组成，可以协作解决复杂问题。主动式智能体独立监控环境并主动发起操作，而持久化智能体则能跨会话保持记忆。此次升级将这些概念整合到 Slack 集成中。

---

1. [OpenAI 发布首款定制芯片 Jalapeño，由博通制造](#item-1) ⭐️ 9.0/10
2. [通过自对弈强化学习、JAX 和 ViT 实现超人类 Generals.io 智能体](#item-2) ⭐️ 9.0/10
3. [高通收购 AI 初创公司 Modular](#item-3) ⭐️ 8.0/10
4. [开源 PR 垃圾信息堪比早期邮件垃圾信息](#item-4) ⭐️ 8.0/10
5. [英伟达 45°C 液冷设计近乎零水耗](#item-5) ⭐️ 8.0/10
6. [Nub：一个类似 Bun 的全能 Node.js 工具包](#item-6) ⭐️ 8.0/10
7. [Rust 社区推动将 crates.io 从 GitHub 发布解耦](#item-7) ⭐️ 8.0/10
8. [Gemini 3.5 Flash 新增电脑操控能力](#item-8) ⭐️ 8.0/10
9. [LLM 推理定价对比揭示惊人缓存成本差异](#item-9) ⭐️ 8.0/10
10. [Bunny DNS 免费提供最多 500 个域名](#item-10) ⭐️ 7.0/10
11. [卡马克反思 id Software 早期管理失误](#item-11) ⭐️ 7.0/10
12. [大型 AI 实验室正聘用哲学家](#item-12) ⭐️ 7.0/10
13. [NVIDIA NeMo AutoModel 加速 Transformer 微调](#item-13) ⭐️ 7.0/10
14. [Tom MacWright 批评由 LLM 生成的求职申请](#item-14) ⭐️ 7.0/10
15. [Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks](#item-15) ⭐️ 7.0/10
16. [Claude Slackbot 升级：支持多人协作、主动和持久化智能体](#item-16) ⭐️ 7.0/10
17. [Papers with Code 汇总顶尖开源 OCR 模型与基准](#item-17) ⭐️ 7.0/10
18. [HDD-RoPE：动态旋转位置嵌入提升收敛速度](#item-18) ⭐️ 7.0/10
19. [DeepSWE：针对编码智能体的全新无污染基准测试](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 发布首款定制芯片 Jalapeño，由博通制造](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 发布了其首款定制 AI 推理芯片 Jalapeño，该芯片由博通合作设计、台积电制造。该芯片专门针对大语言模型推理进行了优化，从设计到生产用时九个月，部分环节通过 OpenAI 自身的 AI 模型加速完成。 这标志着 OpenAI 进军定制芯片领域，可能减少对 NVIDIA GPU 的依赖，并实现更高效、更具成本效益的大规模 AI 推理。此举也可能影响更广泛的 AI 硬件格局，促使更多公司开发专用芯片。 该芯片名为 Jalapeño，专为大语言模型推理设计。它基于 OpenAI 对 LLM 底层原理的深刻理解从零开始设计，开发过程中利用 OpenAI 自身模型加速了部分流程。制造由台积电负责。

hackernews · jamdesk · 6月24日 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 推理芯片是专门用于高效运行已训练模型的特种硬件，侧重于低延迟和高吞吐量。与训练芯片（如 GPU）不同，推理芯片优先考虑速度和能效。此前 OpenAI 依赖 NVIDIA GPU 和云服务提供商进行推理。像 Jalapeño 这样的定制芯片旨在针对特定模型和工作负载优化性能，有望降低成本并改善用户体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/">OpenAI unveils its first custom chip, built by Broadcom</a></li>

</ul>
</details>

**社区讨论**: 一些评论者对 AI 模型加速芯片设计的说法表示怀疑，认为可能只是营销噱头。其他人确认了台积电是制造商，还有少数人讨论了将权重直接烧录到硅片中以实现极致效率的可行性，并提及了 Taalas 等公司。

**标签**: `#openai`, `#hardware`, `#ai-chip`, `#inference`, `#broadcom`

---

<a id="item-2"></a>
## [通过自对弈强化学习、JAX 和 ViT 实现超人类 Generals.io 智能体](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

开发者创建了一个用于 Generals.io 的自对弈强化学习智能体，在人类 1v1 排行榜上达到#1 排名，超越了顶级人类玩家。该智能体使用 JAX 进行可扩展计算，并采用 Vision Transformer 作为神经网络架构，整个流程已开源。 这项工作表明，通过 JAX 和 Vision Transformer 扩展计算和模型容量，可以在复杂的不完全信息游戏中实现超人类表现，减少对人工特征的依赖。模拟器和智能体的开源为游戏 AI 和强化学习社区提供了宝贵的资源。 该智能体从早期的 NumPy/Torch 版本完全重构为 JAX 实现，并将 CNN 替换为 Vision Transformer 以更好地捕捉空间关系。开发者的博客文章详细介绍了项目中遇到的死胡同、设计决策以及获得的实用见解。

reddit · r/MachineLearning · /u/shrekofspeed · 6月24日 16:18

**背景**: Generals.io 是一款具有不完全信息的即时战略游戏，玩家控制军队夺取敌方将军。自对弈强化学习是指智能体通过与自己对战来不断学习改进。JAX 是一个用于高性能机器学习的数值计算库，支持快速模拟和梯度计算。Vision Transformer（ViT）是一种将 Transformer 注意力机制应用于图像补丁的神经网络架构，提供了卷积神经网络的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vision_transformer">Vision transformer</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#self-play`, `#vision transformer`, `#JAX`, `#game AI`

---

<a id="item-3"></a>
## [高通收购 AI 初创公司 Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

2026 年 6 月 24 日，高通宣布收购 AI 初创公司 Modular，后者是 Mojo 编程语言和 AI 基础设施的开发商，据报道交易价值 40 亿美元。 此次收购增强了高通在 AI 软硬件集成方面的能力，可能挑战英伟达在 AI 推理领域的主导地位。同时，它将创新的 Mojo 语言纳入高通旗下，可能重塑 AI 编程生态系统。 据报道，此次收购价值 40 亿美元。Mojo 专为高性能 AI 工作负载设计，通过 MLIR 编译器框架支持多种硬件加速器，与传统语言形成区别。

hackernews · timmyd · 6月24日 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Mojo 是一种基于 Python 的专有编程语言，旨在结合 Python 的易用性与 C++和 Rust 的性能。它构建在 MLIR 编译器框架之上，可以编译到 CPU、GPU、TPU 和 ASIC，非常适合 AI 应用。高通一直在将 AI 产品线从手机芯片扩展到数据中心和边缘 AI，此次收购符合这一战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人质疑高通在高端 AI 推理领域的竞争力，而另一些人则认为这是对抗英伟达的更大胆战略的一部分。一个值得关注的担忧是，Modular 创始人此前曾批评硬件公司在 AI 软件栈方面的不足。

**标签**: `#Qualcomm`, `#Modular`, `#acquisition`, `#AI`, `#Mojo`

---

<a id="item-4"></a>
## [开源 PR 垃圾信息堪比早期邮件垃圾信息](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 8.0/10

PR 垃圾信息浪费维护者时间并可能抑制贡献，威胁开源项目的健康；应对此问题需要新工具和社区规范。 GitHub 最近为维护者引入了可配置的 PR 限制以缓解垃圾信息。一些项目要求新贡献者在合并第一个 PR 前以非文本形式与维护者会面，还出现了使用捐赠代币积分的建议。

hackernews · dakshgupta · 6月24日 14:32 · [社区讨论](https://news.ycombinator.com/item?id=48660579)

**背景**: Pull request（PR）垃圾信息是指向开源仓库提交低质量或自动化的 PR，通常用于自我推广或测试。这类似于早期电子邮件垃圾信息（未经请求的批量消息淹没收件箱），后来催生了过滤解决方案。开源维护者随着项目受欢迎程度增长面临类似的规模化挑战。

**社区讨论**: 评论者指出 GitHub 新推出的可配置 PR 限制是部分解决方案。有人强调与邮件垃圾信息的关键区别——后者依赖于服务器级别的信誉，而 PR 垃圾信息针对单个用户。其他人分享了非文本验证等个人方法，并建议使用代币积分作为替代方案。

**标签**: `#open-source`, `#spam`, `#pull-request`, `#maintainer`, `#github`

---

<a id="item-5"></a>
## [英伟达 45°C 液冷设计近乎零水耗](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

Nvidia 发布了针对 AI 数据中心的 45°C 液冷设计，将用水量降至接近零。 这一创新使 AI 基础设施更可持续，减少环境影响，并允许在缺水地区部署。 该设计采用直接芯片液冷，冷却液温度达 45°C，比传统系统更高，从而可使用干式冷却，消除水蒸发。

hackernews · nitin_flanker · 6月24日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 数据中心传统上采用蒸发冷却散热，消耗大量水。液冷通过冷却液回路直接吸收芯片热量，但通常需要冷却水。更高的冷却液温度可使用干式冷却器，通过环境空气散热而不损失水。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers">NVIDIA Unveils 45°C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45°C Liquid Cooling Redefines AI Data Center ...</a></li>
<li><a href="https://datacenters.lbl.gov/liquid-cooling">Liquid Cooling | Center of Expertise for Data Center Efficiency</a></li>

</ul>
</details>

**社区讨论**: 评论探讨了实际影响，如区域供暖潜力和与现有 NASA 设施的对比。部分读者质疑创新性，而其他人则指出全液冷服务器的维护挑战。总体态度积极，辩论有建设性。

**标签**: `#liquid cooling`, `#data center`, `#sustainability`, `#AI`, `#energy efficiency`

---

<a id="item-6"></a>
## [Nub：一个类似 Bun 的全能 Node.js 工具包](https://github.com/nubjs/nub) ⭐️ 8.0/10

Zod 的创造者 Colin McDonnell 发布了 Nub，这是一个面向 Node.js 的全能工具包，通过--require 预加载钩子集成了基于 oxc 的编译器、模块解析钩子以及针对 Worker 和 Temporal 等 API 的 polyfill，所有功能均在标准 Node.js 上运行。 Nub 在保持 Node 生态系统的同时，提供了类似 Bun 的开发体验（TypeScript 支持、polyfill），有望弥合 Bun 的开发体验与 Node 的稳定性和生态系统之间的差距。 Nub 使用以 Rust 编写的 oxc 编译器，打包成 Node-API 插件，并通过 Node 的 module.register API 注册模块解析钩子。它仅在需要时注入 polyfill，确保代码最终在 Node 的实际引擎和标准库上运行。

hackernews · colinmcd · 6月24日 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Node.js 传统上缺乏内置的 TypeScript 编译和现代 API polyfill（例如 Temporal）。Bun 提供了这些开箱即用的功能，但作为独立的运行时。Nub 利用 Node 的--require 钩子（在应用启动前运行代码）和模块解析钩子（自定义模块加载方式）来添加这些功能。oxc 编译器是一个高性能的 Rust 工具，用于转换 JavaScript/TypeScript。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance ...</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal">Temporal - JavaScript - MDN Web Docs</a></li>
<li><a href="https://nodejs.org/api/module.html">Modules: `node:module` API | Node.js v26.3.1 Documentation</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，pier25 认为这个想法很有意义，并提到了作者的背景。ssalbdivad 报告说将大型 monorepo 迁移到 Nub 很顺利。eyelidlessness 对使用--require 而非--import 的 ESM 支持表示担忧，vmsp 则质疑在 Node 已能运行 TypeScript 的情况下是否需要编译器。此外还有关于名称'nub'的幽默评论。

**标签**: `#Node.js`, `#TypeScript`, `#Bun`, `#developer-experience`, `#transpiler`

---

<a id="item-7"></a>
## [Rust 社区推动将 crates.io 从 GitHub 发布解耦](https://infosec.exchange/@mttaggart/116806641273303255) ⭐️ 8.0/10

Rust 社区正在积极讨论并致力于将 crates.io 从 GitHub 发布解耦，最近合并的 RFC 3963 为此扫清了障碍，实现工作已经开始。 这一变化对供应链安全至关重要，因为它减少了对单一平台的依赖，降低了因 GitHub 停运或政策变化带来的风险。同时，通过让社区对包发布拥有更多控制权，增强了 Rust 生态系统的基础设施。 解耦工作是一项重大的工程挑战，因为 crates.io 与 GitHub 在身份验证和发布工作流上紧密集成。这项工作由志愿者推动，进展取决于资金和审查人员的可用性。

hackernews · speckx · 6月24日 19:40 · [社区讨论](https://news.ycombinator.com/item?id=48664733)

**背景**: crates.io 是 Rust 的官方包注册中心，托管着成千上万的 crate，开发者依赖它们来构建项目。目前，发布 crate 需要 GitHub 账户并通过 GitHub 进行 OAuth 认证，这形成了一个单点故障。Rust 项目多年来一直意识到这一依赖，但重新设计认证系统的复杂性导致了努力的延迟。近期供应链安全问题加剧了解耦的紧迫性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://crates.io/">crates.io: Rust Package Registry</a></li>
<li><a href="https://github.com/rust-lang/crates.io">GitHub - rust-lang/crates.io: The Rust package registry</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍支持解耦，但承认任务艰巨。评论指出 Rust 主要由志愿者驱动，枯燥但关键的基础设施工作往往缺乏资金。一些人提到其他生态系统如 PHP 的 Packagist 可以借鉴，而另一些人则强调需要建设性地加固生态系统，而不是指责 GitHub。

**标签**: `#Rust`, `#crates.io`, `#GitHub`, `#supply chain security`, `#open source infrastructure`

---

<a id="item-8"></a>
## [Gemini 3.5 Flash 新增电脑操控能力](https://deepmind.google/blog/introducing-computer-use-in-gemini-3-5-flash/) ⭐️ 8.0/10

Google DeepMind 宣布 Gemini 3.5 Flash 现在支持电脑使用，使 AI 代理能够通过直接操作图形用户界面来执行任务。 这一能力标志着向能够像人类一样操作电脑的自主 AI 代理迈出了重要一步，可能彻底改变任务自动化和人机交互。 Gemini 3.5 Flash 针对代理任务进行了优化，具有持续的前沿级智能、更低的成本和更快的速度，支持子代理部署和长期工作流。

rss · Google DeepMind Blog · 6月24日 16:30

**背景**: AI 模型的电脑使用能力指的是在电脑屏幕上执行操作的能力，例如点击按钮、输入文本和浏览应用程序，类似于人类用户。这是构建无需预先集成 API 即可执行复杂任务的自主代理的关键特性。Google 的 Gemini 多模态大语言模型家族发展迅速，其中 Flash 变体强调效率和速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.5 Flash — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models/gemini-3.5-flash">Gemini 3.5 Flash | Gemini API | Google AI for Developers</a></li>
<li><a href="https://openai.com/index/computer-using-agent/">Computer-Using Agent - OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户对这一能力印象深刻，但其他用户报告了准确性和任务完成方面的问题。几位评论者指出，Gemini 仍然缺乏 MCP 支持和编码代理功能，而 Claude 和 GPT 等竞争模型已具备这些功能。还有人对基于截图的电脑使用方式持怀疑态度，认为它不如 API 逆向工程或可访问性树高效。

**标签**: `#AI agents`, `#Gemini`, `#automation`, `#human-computer interaction`, `#Google DeepMind`

---

<a id="item-9"></a>
## [LLM 推理定价对比揭示惊人缓存成本差异](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 8.0/10

一位 Reddit 用户将 7 家供应商（OpenRouter、DeepSeek、Together AI、Fireworks、Groq 等）的公开 LLM 推理定价数据整理成电子表格，发现缓存输入 token 成本存在巨大差异——对于 DeepSeek V4 Pro 等模型，缓存命中的价格可比缓存未命中便宜数十倍。 这一对比很重要，因为对于智能体、RAG 流水线和多轮对话而言，缓存成本可能主导总价格，使得提供商的缓存策略与实际 token 定价对许多实际 AI 应用同等重要。 电子表格追踪了每家供应商的输入/输出 token 定价、上下文窗口、缓存输入定价及支持模型。用户指出，即使是同一模型（如 DeepSeek V4 Pro），不同供应商的缓存成本也差异显著，有些供应商清晰公开了缓存策略，而另一些则几乎没有文档说明。

reddit · r/MachineLearning · /u/Technomadlyf · 6月24日 11:28

**背景**: LLM 推理定价通常按输入和输出 token 计费，但许多提供商对重复内容（如系统提示、文档前缀）提供更便宜的缓存输入 token，这些内容通过 KV 缓存来自早先的计算。DeepSeek V4 Pro 是一个大型混合专家（MoE）模型，拥有 1.6 万亿总参数，支持 100 万 token 上下文和三种推理模式。OpenRouter 是一个 API 聚合器，提供对 300 多个 LLM 模型的统一访问，通常会加收少量费用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://knightli.com/en/2026/04/25/llm-token-pricing-principles/">Why LLM APIs Charge by Tokens: A Clear Guide to Input, Output, and Context Costs</a></li>
<li><a href="https://ngrok.com/blog/prompt-caching">Prompt caching: 10x cheaper LLM tokens, but how? | ngrok blog</a></li>
<li><a href="https://build.nvidia.com/deepseek-ai/deepseek-v4-pro/modelcard">deepseek-v4-pro Model by Deepseek-ai | NVIDIA NIM</a></li>

</ul>
</details>

**标签**: `#LLM`, `#pricing`, `#caching`, `#inference`, `#providers`

---

<a id="item-10"></a>
## [Bunny DNS 免费提供最多 500 个域名](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 7.0/10

Bunny DNS 宣布每个账户最多可免费托管 500 个域名，并取消了所有 DNS 查询费用和按次计费。 此举使 Bunny DNS 成为 Cloudflare 和 Amazon Route 53 的有力欧盟替代品，在地缘政治担忧下可能吸引寻求欧洲云服务的用户。 免费层包括智能记录和健康监控，无查询限制，也无隐藏在企业计划中的功能。Bunny 是一家私人公司，仅在 2022 年进行过一轮 600 万美元的小额融资。

hackernews · dabinat · 6月24日 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48657030)

**背景**: DNS 托管是一种管理域名解析的服务，将人类可读的域名转换为 IP 地址。Bunny.net 是一家总部位于欧盟的全球边缘平台，提供 CDN、存储和 DNS 服务，将自己定位为美国主要云提供商的竞争者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bunny.net/dns/">Bunny DNS | The #1 Scriptable DNS Platform | bunny .net</a></li>
<li><a href="https://bunny.net/">bunny.net - The Global Edge Platform that truly Hops</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论对欧盟替代 Cloudflare 的方案表示赞赏，但一些人担心潜在的突然收费和跨产品计费保障不足。其他人注意到 Bunny 的有机增长方式和小额融资，认为是积极信号。

**标签**: `#DNS`, `#free hosting`, `#cloud services`, `#EU tech`, `#alternative to Cloudflare`

---

<a id="item-11"></a>
## [卡马克反思 id Software 早期管理失误](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 7.0/10

约翰·卡马克公开承认，他在 id Software 早期对团队施加了过大压力，未能随着公司成熟调整管理风格，他认为这最终掏空了公司。 这位传奇程序员的坦诚反思，为创业强度与可持续管理提供了宝贵教训，对软件工程和游戏开发领域的领导者具有参考价值。 卡马克表示‘持续以创业强度要求员工会让他们疲惫不堪’，并质疑《雷神之锤》的成功是否值得 id Software 付出的代价，不过他最终认为考虑到游戏的影响力，这是值得的。

hackernews · shadowtree · 6月24日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=48661825)

**背景**: 约翰·卡马克是 id Software 的联合创始人，以《毁灭战士》和《雷神之锤》等开创性游戏闻名。该公司以高强度工作文化著称，但随着公司壮大，许多关键创意人员离职，导致后期作品质量下滑。这条推文是对科技初创公司管理挑战的反思的一部分。

**社区讨论**: 评论者大多认同卡马克的反思，指出许多公司可以从他的承认中学习。有人指出《雷神之锤 3：竞技场》仍展现了强大的技术创新，另有人分享了桑迪·彼得森的访谈链接，提供了创意人才流失的更多背景。

**标签**: `#john-carmack`, `#id-software`, `#software-engineering-management`, `#startup-culture`, `#game-development`

---

<a id="item-12"></a>
## [大型 AI 实验室正聘用哲学家](https://www.economist.com/science-and-technology/2026/06/24/why-big-ai-labs-are-hiring-so-many-philosophers) ⭐️ 7.0/10

OpenAI、DeepMind 等大型 AI 实验室正在招聘哲学家，以应对关于人工智能意识、推理及社会影响等的伦理和概念挑战。 这表明 AI 开发越来越需要超越工程学的跨学科视角，标志着向更审慎的 AI 治理转变，并可能影响 AI 系统的设计方式和监管方向。 文章指出，哲学系人才正大量流向产业界，Floridi 博士称之为'人才流失'；哲学家通常担任伦理研究员等职务，但其实际影响力难以衡量。

hackernews · Brajeshwar · 6月24日 16:40 · [社区讨论](https://news.ycombinator.com/item?id=48662452)

**背景**: 哲学长期以来探讨意识、伦理和逻辑等问题，这些现在都成为 AI 的核心议题。随着 AI 系统能力增强，机器道德、偏见、智能本质等问题需要哲学分析。聘用哲学家有助于以严谨态度处理工程师难以独自解决的概念性问题。

**社区讨论**: 评论呈现复杂情绪：YuechenLi 注意到 LLM 对哲学化提示反应更好；Scalene2 和 why_at 表示怀疑，why_at 质疑学术界流失的规模；Hard_Space 分享了实际经验但效果有限；elphinstone 认为此举相比高价聘请知名设计师是更廉价的公关。

**标签**: `#AI ethics`, `#philosophy`, `#AI labs`, `#employment trends`

---

<a id="item-13"></a>
## [NVIDIA NeMo AutoModel 加速 Transformer 微调](https://huggingface.co/blog/nvidia/accelerating-fine-tuning-nvidia-nemo-automodel) ⭐️ 7.0/10

Hugging Face 发布了一篇博客，介绍 NVIDIA NeMo AutoModel，该模型与 Hugging Face AutoModel 集成，可以加速 Transformer 模型的微调。 这种集成为实践者简化了微调流程，降低了时间和计算成本，并使先进的分布式训练技术更易于深度学习社区使用。 NeMo AutoModel 是一个 PyTorch DTensor 原生 SPMD 开源库，旨在用于 LLM、VLM、扩散模型和检索模型的分布式训练和微调。它可以通过 PyPI、Docker 或从源码安装。

rss · Hugging Face Blog · 6月24日 16:00

**背景**: 微调大型 Transformer 模型通常需要大量计算资源和专用基础设施。NeMo AutoModel 利用 SPMD（单程序多数据）等分布式训练策略，在多个 GPU 上高效扩展微调，降低了部署自定义模型的门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/nemo/automodel/latest/index.html">NeMo AutoModel Documentation — NeMo-AutoModel</a></li>
<li><a href="https://github.com/NVIDIA-NeMo/Automodel">GitHub - NVIDIA-NeMo/Automodel: Pytorch Distributed native ...</a></li>

</ul>
</details>

**标签**: `#transformers`, `#fine-tuning`, `#nvidia-nemo`, `#deep-learning`, `#huggingface`

---

<a id="item-14"></a>
## [Tom MacWright 批评由 LLM 生成的求职申请](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright 指出一种逐渐蔓延的趋势：求职申请、作品集网站乃至 GitHub 项目完全由 LLM 生成，导致招聘者无法评估候选人的真实能力，只能看出他们使用了 AI 工具。 这一趋势通过剥夺个人真实性和可识别的信号（评估候选人匹配度和技能的关键要素），削弱了招聘流程。它还引发了关于求职申请中 AI 滥用对雇主和求职者影响的深刻问题。 MacWright 描述了一些申请：它们 '明显由 LLM 合写'，链接到 LLM 生成的作品集网站和带有 LLM 生成提交信息的 GitHub 项目，最终得到的是泛泛而谈、毫无个性的简历，仅能反映出工具的使用。

rss · Simon Willison · 6月24日 18:13

**背景**: 像 GPT-4 这样的 LLM 现在可以生成逼真的简历、求职信和代码。这使一些求职者过度依赖这些工具而不加入个人特色，造成了 MacWright 所称的 '意外匿名'——候选人消失在生成内容之后。

**标签**: `#ai`, `#careers`, `#software-engineering`, `#authenticity`

---

<a id="item-15"></a>
## [Why the Frontier Ecosystem must be Open — Matei Zaharia and Reynold Xin, Databricks](https://www.latent.space/p/databricks) ⭐️ 7.0/10

Databricks leaders argue for an open ecosystem to enable every company to build Agent Clouds.

rss · Latent Space · 6月24日 18:53

**标签**: `#open source`, `#AI infrastructure`, `#agent clouds`, `#Databricks`, `#cloud computing`

---

<a id="item-16"></a>
## [Claude Slackbot 升级：支持多人协作、主动和持久化智能体](https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive) ⭐️ 7.0/10

Anthropic 对 Claude 的 Slack 集成进行了升级，支持多人协作、主动式和持久化智能体，使团队能够在 Slack 频道中与多个持续独立运行的 AI 智能体协同工作。 此次升级将 Claude 从简单的聊天机器人转变为跨对话持久的主动团队成员，有望提高团队在 Slack 工作流中的生产力和自动化水平。 新功能包括支持并发交互的多智能体协作、无需提示即可主动发起操作的主动式智能体能力，以及跨会话和频道保留上下文的持久化记忆。

rss · Latent Space · 6月24日 07:14

**背景**: 多智能体系统由多个交互的 AI 智能体组成，可以协作解决复杂问题。主动式智能体独立监控环境并主动发起操作，而持久化智能体则能跨会话保持记忆。此次升级将这些概念整合到 Slack 集成中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multi-agent_system">Multi-agent system - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/Always-On_Proactive_Agent">Always-On Proactive Agent</a></li>
<li><a href="https://medium.com/@iniyarajan/building-persistent-ai-agent-memory-systems-that-actually-work-fa37508080fa">Building Persistent AI Agent Memory Systems That Actually Work | by Iniyarajan S. | AI × Developer Productivity | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#Slack`, `#Agents`, `#Collaboration`

---

<a id="item-17"></a>
## [Papers with Code 汇总顶尖开源 OCR 模型与基准](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

Papers with Code 上新推出了一个页面，汇总了顶尖开源 OCR 模型和基准，重点推荐了百度的 Unlimited OCR（30 亿参数，引入参考滑动窗口注意力机制）和 Mistral 的 OCR 4 API。 OCR 对于将文档数字化以支持智能体检索增强生成至关重要，这份精选列表帮助开发者在 Hugging Face 上众多新发布中选出最佳模型。 百度的 Unlimited OCR 基于 DeepSeek OCR 并引入了参考滑动窗口注意力（R-SWA）。Mistral OCR 4 仅通过 API 提供。推荐的主要基准包括 OlmOCRBench 和 OmniDocBench。

reddit · r/MachineLearning · /u/NielsRogge · 6月24日 16:26

**背景**: 光学字符识别（OCR）将扫描文档或 PDF 转换为机器可读文本。智能体检索增强生成（Agentic RAG）利用这些文本来驱动回答问题或执行任务的 AI 智能体。滑动窗口注意力将注意力限制在固定窗口内，从而降低计算成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/swa/">Sliding Window Attention (SWA) | Sebastian Raschka, PhD</a></li>
<li><a href="https://weaviate.io/blog/what-is-agentic-rag">What Is Agentic RAG? From LLM RAG to AI Agents | Weaviate</a></li>

</ul>
</details>

**社区讨论**: 该帖子没有评论，因此社区 sentiment 未知。

**标签**: `#OCR`, `#open-source`, `#benchmarks`, `#Hugging Face`, `#retrieval-augmented generation`

---

<a id="item-18"></a>
## [HDD-RoPE：动态旋转位置嵌入提升收敛速度](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 7.0/10

一种名为 HDD-RoPE（高维动态旋转位置嵌入）的新型位置嵌入方法被提出，它采用更大的分块尺寸和数据依赖的旋转，在 TinyStories 数据集上比 xPos 更快收敛。 HDD-RoPE 挑战了位置是一维的标准假设，可能使 Transformer 学习到更丰富的位置结构，如段落或句子。若经验证，它可能带来更高效的训练和更好的长上下文任务表现。 HDD-RoPE 将 query/key 分块拆分为大小为 4 的组（而非 2），从而产生 6 个旋转轴（4 选 2）。每个轴的旋转量依赖于数据，允许模型根据层激活动态调整位置编码。

reddit · r/MachineLearning · /u/mikayahlevi · 6月24日 18:16

**背景**: 旋转位置嵌入 (RoPE) 通过旋转 query 和 key 的元素对来编码 token 位置，提供相对位置信息。xPos 是 RoPE 的扩展，调整旋转频率以改善长度外推。HDD-RoPE 将 RoPE 推广到更高维度的旋转，并使旋转速度可学习。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/mikayahlevi/hdd-rope/">GitHub - mikayahlevi/hdd-rope</a></li>
<li><a href="https://kaggle.curtischong.me/techniques/xpos-positional-encoding">xpos positional encoding</a></li>

</ul>
</details>

**标签**: `#positional embedding`, `#transformer`, `#rotary position encoding`, `#NLP`, `#machine learning`

---

<a id="item-19"></a>
## [DeepSWE：针对编码智能体的全新无污染基准测试](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 7.0/10

DeepSWE 是一个新的开源基准，用于评估前沿编码智能体，其任务从零编写以避免数据污染，涵盖 5 种语言共 91 个仓库，并要求长周期解决方案。 通过提供无污染且真实的任务，DeepSWE 能更准确地衡量 AI 编码智能体在实际软件工程中的表现，帮助社区区分炒作与真正进展。 尽管提示长度约为 SWE-bench Pro 的一半，解决方案却需要 5.5 倍多的代码和约 2 倍的输出 token，且验证器为手工编写以测试软件行为而非实现细节。

reddit · r/MachineLearning · /u/we_are_mammals · 6月24日 02:03

**背景**: 基准污染是指评估样本出现在模型训练数据中，导致分数虚高。现有基准如 SWE-bench 和 SWE-bench Pro 常从真实提交或拉取请求中改编任务，存在污染风险。DeepSWE 通过创建原创任务避免这一问题。AI 编码智能体是能自主完成软件工程任务的系统，准确的基准测试对衡量其进展至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.lol/">DeepSWE — Long-Horizon Software Engineering Benchmark</a></li>
<li><a href="https://mbrenndoerfer.com/writing/benchmark-contamination-llm-detection-mitigation">Benchmark Contamination in LLMs: Detection & Mitigation ...</a></li>

</ul>
</details>

**标签**: `#benchmark`, `#code generation`, `#AI agents`, `#open-source`, `#evaluation`

---