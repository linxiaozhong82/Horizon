---
layout: default
title: "Horizon Summary: 2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 49 条内容中筛选出 15 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：LLM、OpenAI、agents、code-generation、ChatGPT。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Cognition 发布 SWE-2 编程模型，宣称对标 Fable 5.1 与 GPT-Astra](https://cognition.com/blog/swe-2)**
2. **[OpenAI 推出金融服务版 ChatGPT，搭载 GPT-6 Astra](https://openai.com/index/introducing-chatgpt-financial-services)**
3. **[OpenAI 推出托管式 Agents API，提供受管 agent harness](https://developers.openai.com/api/docs/guides/agents-api/overview)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [Shopify 将移动应用从 React Native 迁回原生 Swift 与 Kotlin](https://shopify.engineering/back-to-native)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [Calif Research 演示 WeWorm：借 AI 打造的微信通话零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [Shopify 将移动应用从 React Native 迁回原生 Swift 与 Kotlin](https://shopify.engineering/back-to-native)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Cognition 发布 SWE-2 编程模型，宣称对标 Fable 5.1 与 GPT-Astra

**关联新闻**: [Cognition 发布 SWE-2 编程模型，宣称对标 Fable 5.1 与 GPT-Astra](https://cognition.com/blog/swe-2)

**切入角度**: Cognition 发布了 SWE-2，这是一个面向编程任务的大语言模型，基于 Moonshot AI 的开源权重模型 Kimi K3 进行后训练，官方宣称其性能可与 Fable 5.1 和 GPT-Astra 相抗衡。该消息在 Hacker News 上获得 343 分和 141 条评论，讨论主要集中在其基准测试的可信度以及模型权重是否开放。 这次发布重新点燃了大模型生态中的一个核心争论：基准测试分数究竟反映真实的泛化能力，还是仅仅对公开测试集过拟合；以及像 Cognition 这样的闭源权重厂商，能否与日益强大的开源权重对手（如 DeepSeek Flash 4.1）竞争。如果在一个已有的开源基座模型上做后训练就足以达到前沿编程水平，那么斥巨资从零训练模型的价值就会受到质疑。 被引用最多的警示信号是 SWE-2 在 Terminal Bench 2.1 上取得 92.8%，而在几周前才发布的较新版本 Terminal Bench 4 上仅得 27.3%，差距巨大。该模型是在 Kimi K3 之上做后训练，而非基于全新架构，且目前尚不清楚 Cognition 是否会公开模型权重。

**可延展方向**: Kimi K3 是 Moonshot AI 的开源权重前沿模型，参数规模达 2.8 万亿，原生支持视觉，并具备 100 万 token 的上下文窗口，于 2026 年 7 月发布。Terminal Bench 一类的测试集属于智能体编程基准，要求模型完成真实的命令行任务，而较新的版本会加入未见过的题目以检验泛化能力。基准过拟合是一个已被充分记录的现象：模型有意或无意地被调优以迎合广为流传的评测集的特定模式，从而抬高分数却无助于真实场景的实用性。开源权重与闭源权重的区别在于：模型的训练参数是否公开发布、允许任何人运行、修改并自行部署，还是被隐藏在 API 之后保密。

---

### 选题 2：OpenAI 推出金融服务版 ChatGPT，搭载 GPT-6 Astra

**关联新闻**: [OpenAI 推出金融服务版 ChatGPT，搭载 GPT-6 Astra](https://openai.com/index/introducing-chatgpt-financial-services)

**切入角度**: OpenAI 宣布推出面向金融服务行业的 ChatGPT，该产品将内置金融数据与全新的旗舰模型 GPT-6 Astra 相结合，用于研究分析、财务建模以及生成可直接交付客户的材料。此次发布将其定位为一套打包好的行业垂直解决方案，而非通用聊天机器人。 这标志着 OpenAI 从横向的模型 API 供应，进一步迈向面向特定行业的打包式企业产品，瞄准的是经济中价值最高、监管也最严格的领域之一。如果被广泛采用，它可能重塑投资、银行与咨询工作流使用 AI 的方式，并使 OpenAI 与现有金融数据和分析平台形成更直接的竞争。 此次公告本身只是一段简短的宣传文字：没有披露技术基准测试、定价、上线日期，也没有说明数据授权、合规管控或客户数据处理方式等细节，而这些在受监管的金融行业中至关重要。其他渠道公布的模型信息则将 GPT-6 Astra 描述为 OpenAI 面向复杂推理、编程、计算机操作以及长时间多步骤智能体工作流的旗舰模型，在公开的 BenchAlign 排行榜上于约 232 个模型中排名第二，估计得分约为 81/100。

**可延展方向**: 行业垂直型 AI 产品会把通用基础模型与专有数据、数据连接器和预置工作流相结合，使之适配单一行业；在金融领域，这通常意味着行情数据、监管文件、财报电话会议记录，以及与电子表格和建模工具的集成。OpenAI 此前已朝这一方向迈进：ChatGPT 中推出了个人理财功能，允许用户关联账户并获得预算与规划方面的帮助；同时它也有面向企业的金融服务方案，客户反馈称研究与尽职调查流程因此提速。GPT-6 Astra 正是这些产品所依托的旗舰模型。金融等受监管行业高度重视数据来源、可审计性与保密性，因此本次公告未提及合规细节格外值得注意。

---

### 选题 3：OpenAI 推出托管式 Agents API，提供受管 agent harness

**关联新闻**: [OpenAI 推出托管式 Agents API，提供受管 agent harness](https://developers.openai.com/api/docs/guides/agents-api/overview)

**切入角度**: OpenAI 发布了一个托管式的 Agents API，开发者可以把自有工具接入由 OpenAI 托管的 agent harness，由平台负责编排、状态管理和执行循环，而不必自行搭建。该发布在 Hacker News 上引发了 71 条评论的讨论，焦点集中在抽象层设计、沙箱自托管以及厂商锁定等问题上。 这是主流模型厂商向快速增长的 agent 基础设施领域发起的一次平台级进军，而目前大量开源 harness 都运行在开发者自己的机器上。如果托管式 harness 成为交付 agent 的主流方式，竞争格局可能向那些把模型、工具链与执行环境打包在一起的厂商倾斜，同时也会给基于其构建的团队带来锁定风险。 据阅读了文档的评论者指出，该服务允许开发者选择自托管自己的沙箱，这降低了对 OpenAI 执行环境的依赖，也让更换供应商更容易。值得注意的是，harness 本身——即编排与状态层——仍由 OpenAI 托管，因此锁定争议更多集中在控制流和状态管理上，而非代码在哪里运行。

**可延展方向**: Agent harness 是围绕语言模型的一层控制框架：它负责管理推理、工具调用、记忆与权限的循环，这些都是原始模型无法独立完成的，某种程度上相当于 agent 的操作系统。在生产环境中运行 harness 通常还需要配套一个沙箱，即在隔离环境中安全执行 agent 生成的代码，而沙箱的运维难度很高，涉及冷启动、资源管理和环境共享等问题。因此，自行搭建 harness 是一项相当庞大的工程，而这正是此类托管服务试图填补的空白。

---

1. [OpenAI 的 Navier-Stokes 论断附带 Lean 4 形式化证明](#item-1) ⭐️ 9.0/10
2. [Calif Research 演示 WeWorm：借 AI 打造的微信通话零点击蠕虫](#item-2) ⭐️ 9.0/10
3. [Shopify 将移动应用从 React Native 迁回原生 Swift 与 Kotlin](#item-3) ⭐️ 8.0/10
4. [研究人员能放心把未发表的数学成果交给 OpenAI 吗？](#item-4) ⭐️ 8.0/10
5. [Forgejo 16.0.4 修复模板仓库变量展开导致的严重 RCE 漏洞](#item-5) ⭐️ 8.0/10
6. [trynix.dev 借助 qemu-wasm 在浏览器中启动任意 Nix 软件包](#item-6) ⭐️ 8.0/10
7. [OpenAI 推出托管式 Agents API，提供受管 agent harness](#item-7) ⭐️ 7.0/10
8. [Cognition 发布 SWE-2 编程模型，宣称对标 Fable 5.1 与 GPT-Astra](#item-8) ⭐️ 7.0/10
9. [NASA 的去相关拉伸技术让褪色古代岩画重现](#item-9) ⭐️ 7.0/10
10. [PlanetScale 发布 Neki：分片式 PostgreSQL 服务](#item-10) ⭐️ 7.0/10
11. [微软将 Rust 列为内部开发的 Tier-1 语言](#item-11) ⭐️ 7.0/10
12. [布朗大学报告审视大型科技公司如何重塑军工复合体](#item-12) ⭐️ 7.0/10
13. [Raymond Chen 揭秘 Windows XP 如何挑选初始用户头像](#item-13) ⭐️ 7.0/10
14. [维基页面汇总索尼"拥有"数字游戏的说法，数字所有权诉讼持续发酵](#item-14) ⭐️ 7.0/10
15. [OpenAI 推出金融服务版 ChatGPT，搭载 GPT-6 Astra](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 的 Navier-Stokes 论断附带 Lean 4 形式化证明](https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/) ⭐️ 9.0/10

2026 年 9 月 8 日，OpenAI 宣称找到了一个反例，表明三维欧几里得空间中 Navier-Stokes 方程的解会发生爆破（blow-up），并且该发布据称附带了用 Lean 4 编写的形式化证明。根据相关报道，这个反例由约 1 万个运行内部前沿模型的 AI 智能体集群生成，其形态类似一个不断收紧、速度发散直至形成奇点的旋转陀螺。 Navier-Stokes 方程解的存在性与光滑性问题是七大千禧年大奖难题之一，因此一个由机器生成、并配有机器可检验 Lean 证明的反例，将成为 AI 驱动数学研究的真正里程碑。这也把形式化验证推到了聚光灯下：如果 AI 能生成前沿级别的证明，那么瓶颈就会转移到人类能以多快、多低的成本独立检验这些证明上。 该反例尚未经过外部数学家或 Clay 数学研究所的验证，OpenAI 也表示不会为其申领 100 万美元的千禧年大奖。此次发布还伴随着一场优先权争议：就职于竞争对手 AI 公司 Anthropic 的 Levent Alpöge 与 Tristan Buckmaster 此前已得出关于 Euler 方程的一系列密切相关结果；而所用方法则建立在 Diego Córdoba 与 Luis Martínez-Zoroa 于 2023 年提出的、用于在相关流体方程中寻找爆破现象的方法之上。

hackernews · ibobev · 9月10日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=49650326)

**背景**: Navier-Stokes 方程是一组描述流体运动的偏微分方程；三维空间中是否始终存在光滑解，是 Clay 数学研究所于 2000 年提出的七大千禧年大奖难题之一。Lean 4 是一个开源的证明助手兼函数式编程语言，基于归纳构造演算（Calculus of Inductive Constructions），可以让计算机逐行检查数学证明是否正确。形式化验证是指用形式化数学方法证明某个系统满足特定形式化规范，而证明助手正是用来构建和检验这类证明的交互式工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_existence_and_smoothness_problem">Navier-Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant)</a></li>
<li><a href="https://lean-lang.org/">Lean Programming Language</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论主要围绕成本与验证性能，而非数学结果本身：有人按文中数字重新估算，人类一侧的成本约为 88 万小时 × 150 美元/小时 ≈ 1.32 亿美元，而 OpenAI 的智能体成本估计约为 4000 万美元，因此认为两者差距并非所暗示的“四个数量级”。也有人指出 Lean 验证本身就十分昂贵——费马大定理的验证据称耗时 15 小时、占用 230GB 内存，仅比智能体生成 Lean 代码快一个数量级左右；还有人抱怨讨论避开了真正令人震惊之处：一个通用程序竟解决了如此量级的问题，同时担心未来某个 AI 证明可能完全无法被人类验证。

**标签**: `#AI theorem proving`, `#Lean 4`, `#formal verification`, `#Navier-Stokes`, `#OpenAI`

---

<a id="item-2"></a>
## [Calif Research 演示 WeWorm：借 AI 打造的微信通话零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research 发布了 WeWorm 的演示，称其为首个通过微信通话在 iOS 和 Android 上传播的零点击蠕虫。该团队表示，借助 AI 在约两天内就找到了漏洞并写出首个远程代码执行（RCE）利用程序，随后又用了一周时间构建出完整的蠕虫。 微信拥有超过十亿用户，且绝大多数位于中国，因此一个无需用户任何交互即可劫持账号并自我传播的蠕虫一旦被证实真实可用，潜在影响面极大。这同时也被视为 AI 领域的一个里程碑：过去需要更大团队花费数月完成的漏洞利用开发，据说被压缩到大约九天。 受害者无需接听电话，即使接听也听不到任何声音、利用依然成功；唯一失效的情况是受害者在几秒内主动拒接，但攻击者可以再次拨打。该利用针对微信的语音通话（VoIP）栈，可实现完全的账号接管（读取和发送消息、拨打电话），并把每个被感染的账号变成新的攻击源——不过目前它只是一个演示，尚无在野利用的证据。

rss · Simon Willison · 9月10日 00:56

**背景**: 零点击攻击指无需用户任何操作即可入侵设备，通常利用会自动处理不可信数据的应用，例如接听 VoIP 通话时的建立流程。蠕虫则是一种能自我复制的恶意软件：每个新被感染的设备都会成为攻击更多目标的新源头，这正是通信类应用中被认为「可蠕虫化」的漏洞如此危险的原因。微信是一款集消息、支付和社交等功能于一体、用户超过十亿的中国「超级应用」，而近期的研究已显示，AI 辅助的漏洞利用开发能把从发现漏洞到拿出可用利用程序的时间从数月或数周缩短到数天甚至数小时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">"Zero-click" WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm - First 0-Click Worm Spreading Through WeChat Calls Across iOS and Android</a></li>
<li><a href="https://cloud.google.com/blog/topics/threat-intelligence/ai-vulnerability-exploitation-initial-access/">Adversaries Leverage AI for Vulnerability Exploitation ...</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#cybersecurity`, `#zero-click-exploit`, `#wechat`, `#ai-assisted-exploit`

---

<a id="item-3"></a>
## [Shopify 将移动应用从 React Native 迁回原生 Swift 与 Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 在其工程博客上发文《Native is now the future of mobile at Shopify》，宣布其移动应用将放弃 React Native，重新转向原生开发，即 iOS 使用 Swift、Android 使用 Kotlin。该消息在 Hacker News 上引发了约 748 个赞、499 条评论的大型讨论，聚焦跨平台与原生开发的取舍。 Shopify 是使用 React Native 最受关注的公司之一，因此这次“回头”为长期存在的观点提供了佐证：跨平台框架在调试、性能和团队职责上存在隐性成本。这一决定很可能影响其他产品公司在“单一共享代码库”与“两支专职原生团队”之间如何抉择。 有评论者指出，跨 JavaScript、C++ 与原生线程排查崩溃的成本，可能高于维护两套独立代码库；也有人分享说，借助 LLM 辅助重写（例如用 Codex 配合 Maestro UI 测试工具），一个 15-20 个页面的应用可以在一夜之间完成双平台移植，再用几天做细节打磨。值得注意的是，多位工程师认为这类迁移在 LLM 代码生成普及之前就已可行，因此“AI 才让迁移变得划算”的说法可能被夸大。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**背景**: React Native 是 Meta 开源的一套框架，开发者用 React/JavaScript 编写代码，即可在 iOS 和 Android 上渲染原生 UI 组件，从而用一套代码库同时服务两个平台，Meta、微软和 Shopify 都曾在生产环境使用它。Swift 是苹果为其平台推出的、基于 LLVM 的编译型语言；Kotlin 则是 JetBrains 开发的静态类型语言，谷歌在 2019 年将其定为 Android 的首选语言，它也能通过 LLVM 编译为原生代码。是选择共享的跨平台代码库，还是维护两套原生代码库，一直是移动工程领域最常被反复讨论的架构问题之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native</a></li>
<li><a href="https://en.wikipedia.org/wiki/Swift_(programming_language)">Swift (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kotlin_programming_language">Kotlin programming language</a></li>

</ul>
</details>

**社区讨论**: 整体情绪偏向支持原生开发，不少 iOS 工程师表示这一决定印证了他们长期以来对共享代码库的质疑。关于 AI 的作用则存在明显分歧：一位亲自主导过中型 React Native 应用到原生重写的评论者强调，其中的大部分工作发生在任何 LLM 辅助之前；而另一位评论者认为，既然如今代码很大程度上由模型生成，React Native 最初的吸引力——让 Web 开发者也能交付移动应用——已基本消失。

**标签**: `#React Native`, `#Mobile Development`, `#Swift`, `#Kotlin`, `#Cross-Platform`

---

<a id="item-4"></a>
## [研究人员能放心把未发表的数学成果交给 OpenAI 吗？](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

Hacker News 上一条获得约 638 个赞、616 条评论的讨论帖，围绕“数学家能否放心把未发表的工作交给 OpenAI”展开，起因是 Andreas Thom 在 Mastodon 上的系列帖子以及 X、Bluesky 上的相关评论。争论的核心是：OpenAI 的模型是否可能在与研究人员对话的过程中接受了未发表的想法，随后却发表了与该合作方向相近的成果，且未给出署名。 如果研究人员无法确信未发表的想法会被保密并得到应有的署名，那么把前沿模型当作数学合作者的做法就可能难以为继，这不仅影响学术署名的惯例，也会影响数学家与 AI 实验室合作的意愿。在各家实验室宣称在公开难题上取得超越人类的进展之际，这一争议还牵出了用户对话如何进入模型训练与强化学习流程的更广泛问题。 有评论者指出，两种解释并不互斥：模型既可能在预训练阶段从对话中吸收了对某个问题的直觉，也可能在大规模算力下、基于可验证数学问题的强化学习中真正发现了新颖技巧。也有人列举了具体细节，例如 OpenAI 据称向约 10 万名研究人员提供免费访问，以及一种怀疑：在得知某重大数学证明可能存在于模型训练数据中之后不久，OpenAI 就用一个仍在训练中的模型生成了约 3000 亿个输出 token。

hackernews · pred_ · 9月10日 06:49 · [社区讨论](https://news.ycombinator.com/item?id=49639408)

**背景**: 前沿 AI 实验室近年来不断拉拢数学家，提供免费或优惠的模型访问权限，让研究者用 Codex 之类的工具攻坚难题，同时据称其内部模型正以惊人的速度解决公开问题。与此相关的训练流程主要有两个阶段：一是对大规模文本语料（可能包含用户对话）的预训练，二是在答案可验证的问题（如形式化或数值数学题）上做强化学习，让模型自行搜索解题策略。而学术数学界依靠的是署名规范，以及未经允许不得使用同行未发表想法的默契——这正是讨论中反复出现“人类合作者”类比的原因。

**社区讨论**: 整体情绪偏向怀疑。一个被广泛引用的类比是：如果 OpenAI 是一位人类合作者，拿了研究者的想法却不加署名地发表相关成果，那显然是不道德的；另一种观点则认为两件事可以同时成立——预训练可能提升了模型的直觉，而强化学习发现的技术与某段具体对话无关；还有人形容这一连串事件“像是平行构造”，也有评论者对人们竟然如此信任企业来保护个人数据感到不安。

**标签**: `#OpenAI`, `#AI ethics`, `#research collaboration`, `#mathematics`, `#trust`

---

<a id="item-5"></a>
## [Forgejo 16.0.4 修复模板仓库变量展开导致的严重 RCE 漏洞](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo 发布了 16.0.4 版本（并为旧分支提供了对应的 15.0.8 回补版本），修复了一个严重的远程代码执行漏洞：恶意模板仓库可以读取 Forgejo 宿主机上的任意数据，并在宿主机上执行任意进程。该修复被描述为“防止模板展开干扰 git 仓库初始化”。 由于漏洞利用成功即可在宿主机上执行任意代码，任何会处理用户提供的模板生成仓库的自建 Forgejo 实例都可能面临整台服务器被完全攻陷的风险，包括所有托管的源代码、凭证和 CI 密钥被泄露。由于该漏洞被定为严重级别且技术细节已公开，自建用户被建议立即升级。 易受攻击的流程是这样的：Forgejo 克隆模板仓库、删除其 .git 目录、对 .forgejo/template 中列出的文件执行变量模板展开，然后初始化一个新的 git 仓库——而模板展开过程可能重建一个 .git 目录，从而干扰这次初始化。因此补丁的做法是在变量展开完成之后、初始化新仓库之前，删除任何已存在的 .git 目录。

hackernews · weierstass · 9月10日 15:57 · [社区讨论](https://news.ycombinator.com/item?id=49645907)

**背景**: Forgejo 是 Gitea 的社区治理分支，被广泛用作轻量级的自建“Git 托管平台”，即用于托管代码仓库、issue 和 CI 的 Web 服务，其最知名的部署是公开实例 Codeberg。它的“模板仓库”功能允许用户把某个仓库标记为模板，其他人可据此生成新项目；模板文件中可以包含变量，在创建副本时会被替换为新仓库名称等取值。正是这个便利功能在此次事件中演变成了代码执行路径，因为变量展开是在仓库重新初始化之前对攻击者可控的内容执行的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1093671/">Forgejo 16.0.4 and 15.0.8 address critical security ...</a></li>
<li><a href="https://codeberg.org/forgejo/forgejo/issues/14300">#14300 - 2026-09-10 security patches - forgejo/forgejo ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49645907">Forgejo <= 16 . 0 . 3 Critical RCE | Hacker News</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者指出，由于 Codeberg 的速率限制，发布说明页面无法打开，于是直接引用了公告原文，同时有人以维护者身份纠正称应指向 milestone 链接。一位 Gitea 项目负责人表示 Gitea 对这两个问题都免疫（并披露了自己的身份），还补充说安全事件人人都会遇到，不应苛责报告者，否则会导致未来问题被报告得更少。还有人围绕 Forgejo 禁止 LLM 生成贡献的规定展开争论，认为防御方放弃用 AI 寻找漏洞、而攻击者却在用 AI，会让 Forgejo 处于劣势。

**标签**: `#security`, `#vulnerability`, `#forgejo`, `#git`, `#self-hosted`

---

<a id="item-6"></a>
## [trynix.dev 借助 qemu-wasm 在浏览器中启动任意 Nix 软件包](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Farid Zakaria 称这是他在 Nix 领域的“巅峰之作”：他推出了 trynix.dev，通过 qemu-wasm（WebAssembly）在浏览器内完整运行一台 x86_64 Linux 虚拟机，并能启动过去 13 年间的任意 Nix 软件包。每个包都可以用 URL 寻址——例如访问 trynix.dev/?pkg=python3%403.6.2 并点击“Load”，即可获得一个运行 2017 年 Python 3.6.2 的交互式 shell。他还发布了 trynix-preview，这是一个 GitHub Action，会在 Pull Request 下评论一个链接，让评审者直接在浏览器中启动该 PR 的构建产物。 它把 Nix 的核心承诺——可复现性——变成了可以即时分享、且无需服务器的东西：某个特定软件包或构建可以直接固化在一个 URL 里，在评审者自己的机器上运行，无需准备任何基础设施。这对代码评审、缺陷复现和教学都立刻有用，也预示着一个未来：可复现环境以链接的形式传递，而不是靠容器镜像或安装文档。 整个技术栈都运行在客户端：这台虚拟机是 QEMU 的 x86_64 系统模拟器，经由 ktock/qemu-wasm 项目编译成 WebAssembly，因此做到了“没有服务器，只有浏览器”；但这也意味着访问者的浏览器需要下载体积可观的 WASM 二进制文件和磁盘镜像，而且模拟执行相比原生执行会有性能开销。可启动软件包能覆盖 13 年，反映的是 Nix 软件包集合 nixpkgs 漫长的修订历史。

rss · Simon Willison · 9月10日 23:44

**背景**: Nix 是面向类 Unix 系统的纯函数式包管理器，由 Eelco Dolstra 于 2003 年创建，它把软件包视为不可变的值，专为可复现、声明式的构建而设计，其软件包集合称为 nixpkgs。QEMU 是广泛使用的开源机器模拟器和虚拟化工具，而 qemu-wasm 项目把它的 x86_64 系统模拟功能编译成了 WebAssembly。WebAssembly 是一种可移植的二进制指令格式，能让接近原生速度的代码在浏览器沙箱中运行，这正是整台 Linux 虚拟机可以跑在浏览器标签页里的前提。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/ qemu - wasm : QEMU on browser · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nix_(package_manager)">Nix (package manager)</a></li>
<li><a href="https://nixos.org/">Nix & NixOS | Declarative builds and deployments</a></li>

</ul>
</details>

**标签**: `#Nix`, `#WebAssembly`, `#qemu`, `#virtualization`, `#developer-tools`

---

<a id="item-7"></a>
## [OpenAI 推出托管式 Agents API，提供受管 agent harness](https://developers.openai.com/api/docs/guides/agents-api/overview) ⭐️ 7.0/10

OpenAI 发布了一个托管式的 Agents API，开发者可以把自有工具接入由 OpenAI 托管的 agent harness，由平台负责编排、状态管理和执行循环，而不必自行搭建。该发布在 Hacker News 上引发了 71 条评论的讨论，焦点集中在抽象层设计、沙箱自托管以及厂商锁定等问题上。 这是主流模型厂商向快速增长的 agent 基础设施领域发起的一次平台级进军，而目前大量开源 harness 都运行在开发者自己的机器上。如果托管式 harness 成为交付 agent 的主流方式，竞争格局可能向那些把模型、工具链与执行环境打包在一起的厂商倾斜，同时也会给基于其构建的团队带来锁定风险。 据阅读了文档的评论者指出，该服务允许开发者选择自托管自己的沙箱，这降低了对 OpenAI 执行环境的依赖，也让更换供应商更容易。值得注意的是，harness 本身——即编排与状态层——仍由 OpenAI 托管，因此锁定争议更多集中在控制流和状态管理上，而非代码在哪里运行。

hackernews · aquir · 9月10日 19:43 · [社区讨论](https://news.ycombinator.com/item?id=49649213)

**背景**: Agent harness 是围绕语言模型的一层控制框架：它负责管理推理、工具调用、记忆与权限的循环，这些都是原始模型无法独立完成的，某种程度上相当于 agent 的操作系统。在生产环境中运行 harness 通常还需要配套一个沙箱，即在隔离环境中安全执行 agent 生成的代码，而沙箱的运维难度很高，涉及冷启动、资源管理和环境共享等问题。因此，自行搭建 harness 是一项相当庞大的工程，而这正是此类托管服务试图填补的空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.snowflake.com/en/artificial-intelligence/agents/harness/">Agent Harness : The Operating Layer for AI Agents | Snowflake</a></li>
<li><a href="https://medium.com/@rajithaeye/what-is-an-agent-harness-how-ai-agents-get-tools-memory-and-control-cb61ea87f94b">What Is an Agent Harness ? How AI Agents Get Tools... | Medium</a></li>
<li><a href="https://northflank.com/blog/self-hosted-ai-sandboxes">Self-hosted AI sandboxes: Guide to secure code execution in ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为，把 agent 作为产品出售的合适抽象方式仍未有定论，有人指出托管服务解决了诸如 Cloudflare Worker 这类没有文件系统的环境下状态该存放在哪里的问题。也有人强调，沙箱可自托管让这一服务吸引力大增，并让切换供应商变得更容易；还有开发者表示，自己在普通 QEMU 虚拟机中运行 Codex 并以手机远程控制，作为个人助理效果很好。最强烈的批评来自认为这是在推动厂商锁定的人，其中一条评论直言 OpenAI 应该直接提供用户付费购买的推理 token。

**标签**: `#agents`, `#openai`, `#api`, `#llm-infrastructure`, `#vendor-lock-in`

---

<a id="item-8"></a>
## [Cognition 发布 SWE-2 编程模型，宣称对标 Fable 5.1 与 GPT-Astra](https://cognition.com/blog/swe-2) ⭐️ 7.0/10

Cognition 发布了 SWE-2，这是一个面向编程任务的大语言模型，基于 Moonshot AI 的开源权重模型 Kimi K3 进行后训练，官方宣称其性能可与 Fable 5.1 和 GPT-Astra 相抗衡。该消息在 Hacker News 上获得 343 分和 141 条评论，讨论主要集中在其基准测试的可信度以及模型权重是否开放。 这次发布重新点燃了大模型生态中的一个核心争论：基准测试分数究竟反映真实的泛化能力，还是仅仅对公开测试集过拟合；以及像 Cognition 这样的闭源权重厂商，能否与日益强大的开源权重对手（如 DeepSeek Flash 4.1）竞争。如果在一个已有的开源基座模型上做后训练就足以达到前沿编程水平，那么斥巨资从零训练模型的价值就会受到质疑。 被引用最多的警示信号是 SWE-2 在 Terminal Bench 2.1 上取得 92.8%，而在几周前才发布的较新版本 Terminal Bench 4 上仅得 27.3%，差距巨大。该模型是在 Kimi K3 之上做后训练，而非基于全新架构，且目前尚不清楚 Cognition 是否会公开模型权重。

hackernews · seelos · 9月10日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49645443)

**背景**: Kimi K3 是 Moonshot AI 的开源权重前沿模型，参数规模达 2.8 万亿，原生支持视觉，并具备 100 万 token 的上下文窗口，于 2026 年 7 月发布。Terminal Bench 一类的测试集属于智能体编程基准，要求模型完成真实的命令行任务，而较新的版本会加入未见过的题目以检验泛化能力。基准过拟合是一个已被充分记录的现象：模型有意或无意地被调优以迎合广为流传的评测集的特定模式，从而抬高分数却无助于真实场景的实用性。开源权重与闭源权重的区别在于：模型的训练参数是否公开发布、允许任何人运行、修改并自行部署，还是被隐藏在 API 之后保密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://github.com/MoonshotAI/Kimi-K3">GitHub - MoonshotAI/Kimi-K3: Open Frontier Intelligence</a></li>
<li><a href="https://nearform.com/digital-community/open-vs-closed-navigating-the-critical-llm-decision-for-enterprise-ai/">Open vs. closed: Navigating the critical LLM decision for enterprise AI | Nearform</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍持怀疑态度而非兴奋情绪：最高赞观点指出，Terminal Bench 上 92.8% 对 27.3% 的巨大落差，恰好说明 SWE-2 被“刷榜”刷到了什么程度，泛化能力可能很差。有人质疑该模型是否真的开放权重，并反问相比 DeepSeek Flash 4.1 为何要选它；也有人翻出 Cognition 早年的自主智能体演示，称其当时并未真正完成所宣称的任务。少数评论认为积极的一面是，对 Kimi K3 做强化学习后训练似乎确实能接近 Fable 5 级别的能力；另有一位批评者则直接因 Devin 产品体验糟糕而否定这家公司。

**标签**: `#LLM`, `#code-generation`, `#benchmarking`, `#open-weights`, `#AI-models`

---

<a id="item-9"></a>
## [NASA 的去相关拉伸技术让褪色古代岩画重现](https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images) ⭐️ 7.0/10

NASA Spinoff 在 2025 年的一篇文章中介绍，最初为处理多波段卫星照片而开发去相关拉伸（decorrelation stretch）图像处理技术，如今被用于揭示肉眼几乎看不见的褪色古代岩画。Hacker News 上的讨论还给出了在 GIMP 中复现类似效果的具体做法：将图像分解为 LAB 通道，再对 A、B 色度通道做自动色阶拉伸。 这是技术转移的一个典型案例：为地球观测卫星打造的工具，最终在考古与文化遗产领域发挥作用，帮助研究者辨认传统摄影无法捕捉的模糊岩画。讨论还表明，这类遥感方法正通过普通修图软件逐渐走向爱好者群体。 去相关拉伸的原理是先消除通道之间高度的波段间相关性，再拉伸剩余的色差，因此它需要多波段传感器数据而不能仅靠普通 RGB 照片，输出也是刻意夸张的假彩色图像。社区成员指出，在 GIMP 中可以粗略近似该效果（颜色 > 组件 > 分解 > LAB，对 A/B 通道执行自动输入色阶，再重新组合），但目前还没有现成的 ImageMagick 一条命令实现。

hackernews · gumby · 9月10日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49645437)

**背景**: 在遥感领域，卫星会采集多个彼此高度相关的光谱波段（包括红外波段），直接合成出的图像往往灰暗平淡。去相关拉伸通过抑制这种冗余、放大细微色差，得到色彩鲜艳的假彩色图像，常用于区分岩石类型或植被等任务。而褪色的岩画往往只残留极淡的颜料痕迹，放大这些微小的光谱差异就能让图案重新可辨——这正是该原理被应用于考古的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Decorrelation">Decorrelation - Wikipedia</a></li>
<li><a href="https://www.mathworks.com/help/images/enhance-color-separation-using-decorrelation-stretching.html">Enhance Color Separation Using Decorrelation Stretching - MATLAB & Simulink</a></li>
<li><a href="https://www.dstretch.com/DecorrelationStretch.pdf">Algorithm Theoretical Basis Document for Decorrelation Stretch</a></li>

</ul>
</details>

**社区讨论**: 评论整体热情高涨：Waterluvian 把假彩色合成描述为高中和本科阶段的“顿悟时刻”，认为它重塑了自己对传感器与信号处理的理解（“植被是红色的，不是绿色的”）；matja 分享了具体的 GIMP LAB 操作流程，mlmonkey 则询问是否存在对应的 ImageMagick 实现。其他人补充了背景：dylan604 感叹古代创作者付出的巨大努力，qurren 则讲述了自己在吴哥窟用多组带通滤光片并放大交叉光谱差异寻找隐藏岩画却未能成功的经历。

**标签**: `#image-processing`, `#remote-sensing`, `#archaeology`, `#color-compositing`, `#nasa-spinoff`

---

<a id="item-10"></a>
## [PlanetScale 发布 Neki：分片式 PostgreSQL 服务](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale 发布了 Neki，这是一款由 Vitess 原班团队打造的分片式 PostgreSQL 产品，目前已进入平台预览（platform preview）阶段。官方宣称 Neki 可以将原生 PostgreSQL 扩展到每秒数亿次查询（QPS）和 PB 级数据量，并支持零停机重新分片（resharding）。 PostgreSQL 的水平扩展一直是数据库领域最热门的方向之一，因为 Postgres 在单机之外的分片能力一向较难实现。Neki 把 Vitess 式的分片经验带到了 Postgres，但由于该产品是闭源的，它引发了关于厂商锁定的担忧，并与 Supabase 的 multigres 等开源方案形成鲜明对比。 Neki 目前处于平台预览阶段，PlanetScale 表示正在与大规模运行 Postgres 的设计合作伙伴紧密协作。除了扩展能力之外，这篇发布公告也因未清楚说明 Neki 究竟是什么样的产品、以及它如何处理一致性而遭到批评，使得围绕高可用分布式 Postgres 的最终一致性（eventual consistency）与 CAP 定理取舍问题仍悬而未决。

hackernews · simon_weber · 9月10日 15:43 · [社区讨论](https://news.ycombinator.com/item?id=49645686)

**背景**: 分片（sharding）是指把单个数据库拆分到多台服务器上，每台服务器运行各自独立的 Postgres 实例，并由路由层负责转发查询、在分片之间迁移数据，从而让应用基本可以像使用单一数据库一样继续运行。Vitess 是 PlanetScale 打造并曾开源的、被广泛采用的 MySQL 分片系统，而 Neki 本质上就是把这一套方法复制到 Postgres 上。CAP 定理指出，分布式系统无法同时保证一致性（Consistency）、可用性（Availability）和分区容错性（Partition tolerance）三者，这也正是评论者追问 PlanetScale：Neki 在故障期间究竟如何处理一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://planetscale.com/blog/introducing-neki">Introducing Neki — PlanetScale</a></li>
<li><a href="https://planetscale.com/neki">Neki — PlanetScale</a></li>
<li><a href="https://neki.dev/">Neki | Sharded Postgres by PlanetScale</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论明显偏批评性：最高赞评论（gk1）指出这篇发布文章反复解释问题背景、替代方案和架构，却始终没有清楚说明 Neki 到底是什么、用来做什么。也有人赞扬底层技术本身，但抨击 CEO 的态度，以及 Neki 在公开贬低 Supabase 开源项目 multigres 的同时自身却保持闭源；还有评论者提出了实际担忧：最终一致性会让许多高可用分布式 Postgres 方案无法适用于某些工作负载，并追问 Neki 如何解决这一 CAP 取舍问题。

**标签**: `#postgres`, `#databases`, `#sharding`, `#planetscale`, `#distributed-systems`

---

<a id="item-11"></a>
## [微软将 Rust 列为内部开发的 Tier-1 语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 7.0/10

微软在 Rust 基金会博客上发表客座文章，宣布 Rust 如今已与 C++、C# 和 TypeScript 并列，成为公司内部开发中享受最高级别支持的“Tier-1 语言”。这一正式定位意味着 Rust 已从试验性选项升级为微软内部系统级新项目开发完全支持的语言。 微软是 C 和 C++ 语言工具链最重要的维护者之一，它的背书强烈表明 Rust 已成熟为被主流接受的重要系统编程语言，而非小众实验。这也意味着所有维护 C/C++ 工具链的主流操作系统厂商如今都为新项目提供了多样化的内存安全选择，将影响整个行业的工具链、人才招聘与长期平台决策。 微软公开了一个雄心勃勃的目标：借助自动化工具在 2030 年前将约 10 亿行 C/C++ 代码转换为 Rust，并将其描述为可实现“1 名工程师、1 个月、100 万行代码”。自动化迁移研究正从多个方向推进，包括 DARPA 资助的六个团队以不同方法攻克 C 到 Rust 的转换，以及 GrammaTech 的 CRAM 等开源半自动 C++ 转 Rust 工具，但完全自动化且符合习惯用法的翻译仍是一个未解难题。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**背景**: Rust 是一门通用系统编程语言，由 Graydon Hoare 于 2006 年在 Mozilla 任职期间创建，Mozilla 自 2009 年起正式赞助该项目；Rust 1.0 于 2015 年 5 月发布首个稳定版，自 2021 年 2 月起由独立的 Rust 基金会负责管理。其核心特性是在不使用垃圾回收器的情况下实现内存安全：编译期的“借用检查器”会追踪引用的生命周期，从而防止内存错误和数据竞争。在微软这样的公司内部，“Tier-1 语言”是一种工程支持等级，意味着该语言在内部开发中得到完全支持、配套工具齐全并被推荐使用，而不只是为兼容遗留代码而被勉强接受。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_Foundation">Rust Foundation</a></li>
<li><a href="https://www.grammatech.com/publication/cram-c-to-rust-assisted-migration/">CRAM: C++ to Rust Assisted Migration | GrammaTech</a></li>

</ul>
</details>

**社区讨论**: Hacker News 讨论帖（592 分、336 条评论）总体积极但内容扎实：有评论者认为这证明 Rust 不再是“迭代快、常出问题”的“初生语言”；一位拥有五年 Rust 专业开发经验的工程师表示，从高层应用开发的角度看，如今找不到选择其他语言的技术理由。反复出现的保留意见包括 Rust 在 WebAssembly 方面尚不成熟、缺少 macOS/Windows/Android/iOS 原生 UI 支持，以及与 Zig、Odin 等更新的“更好的 C/C++”语言的比较；也有评论者指出，所有主流操作系统厂商如今都在为新项目多元化其系统编程语言选项。

**标签**: `#rust`, `#microsoft`, `#programming-languages`, `#memory-safety`, `#systems-programming`

---

<a id="item-12"></a>
## [布朗大学报告审视大型科技公司如何重塑军工复合体](https://costsofwar.watson.brown.edu/paper/how-big-tech-and-silicon-valley-are-transforming-military-industrial-complex) ⭐️ 7.0/10

布朗大学“战争成本”（Costs of War）项目发布的一篇报告，分析了大型科技公司与硅谷如何重塑当代军工复合体，认为科技行业与美国国防体系之间的联系正以新的方式不断加深。该文被提交到 Hacker News，引发了长篇讨论，围绕科技与国防合作的历史渊源与伦理争议展开辩论。 这一话题直接影响大量供职于承接国防合同公司的工程师和研究人员，并引出令人不安的问题：参与军事相关工作是个人选择，还是整个行业难以回避的特征。它也反映出更广泛的趋势——由风险投资支持的初创公司和云服务商正进入过去由传统主承包商主导的国防市场。 “战争成本”项目是布朗大学沃森国际与公共事务学院下属的无党派研究项目，始于 2011 年，由约 35 位学者、法律专家、人权实践者和医生组成，旨在记录美国“9·11”后战争在人员和经济上的直接与间接代价。该报告的核心论点是：硅谷的角色不是脱离军工复合体，而是对其的一次改造。

hackernews · paimapi · 9月10日 15:47 · [社区讨论](https://news.ycombinator.com/item?id=49645754)

**背景**: “军工复合体”一词因美国总统艾森豪威尔 1961 年的告别演说而广为人知，他警告国防承包商与军方对国家政策的影响力。硅谷与国防的联系并非新鲜事：早在 20 世纪 50 至 60 年代，仙童半导体（Fairchild Semiconductor）等公司就为导弹系统向军方供应集成电路，而该地区的早期发展也深受二战期间政府资助项目（如雷达研究）的影响。Hacker News 是由孵化器 Y Combinator 运营的科技与创业讨论网站，其评论区常将工程细节与政策、伦理讨论交织在一起。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://costsofwar.watson.brown.edu/">Costs of War | Brown University</a></li>
<li><a href="https://en.wikipedia.org/wiki/Costs_of_War_Project">Costs of War Project - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上反驳了该报告“揭示新现象”的框架，指出美国国防部“从一开始”就在资助硅谷，并援引 Steve Blank 的《硅谷秘史》，将这一地区的起源追溯到二战时期的雷达研究。也有人把问题视为个人的伦理抉择：一位评论者称自己因不愿参与战争相关业务而辞去微软的工作，另一位则尖锐地反问，企业是否应当拒绝本国国防部的合同，还是仅仅针对美国才应如此。

**标签**: `#military-industrial complex`, `#Silicon Valley`, `#tech ethics`, `#defense contracts`, `#policy`

---

<a id="item-13"></a>
## [Raymond Chen 揭秘 Windows XP 如何挑选初始用户头像](https://devblogs.microsoft.com/oldnewthing/20260909-00/?p=112683) ⭐️ 7.0/10

微软工程师 Raymond Chen 在其博客 The Old New Thing 上详细解释了 Windows XP 为新建用户账户分配默认头像所用的算法：系统使用伪随机数生成器 RtlRandomEx，并以 GetTickCount() 的当前值作为初始种子，再通过一次遍历的随机选择算法从可用的图片文件中挑出一张。该文章在 Hacker News 上引发了热烈讨论（337 分、165 条评论），内容既有网友贴出实际的 NT5 源码链接，也有对“计算机随机挑选有多难”的思考。 这篇文章是一个精炼的案例，说明像“给新用户显示哪张内置照片”这样看似微不足道的产品决策，仍然需要认真的算法设计，也凸显了人类对“随机”的直觉与软件实际实现方式之间长期存在的差距。对工程师而言，它还提醒我们，即便是纯装饰性功能也包含设计取舍，例如在结果只关乎观感时选用廉价、非加密级的随机源。 关键技术细节在于“一次遍历”的随机选择算法：它无需先统计目录下的文件总数，就能以均匀概率挑出一项；同时配合以 GetTickCount() 为种子的 RtlRandomEx，而该时钟值分辨率低且完全可预测，用于任何安全相关场景都是不可接受的。换句话说，这一设计刻意追求轻量，之所以可行，仅仅是因为选错头像的唯一后果不过是换一张缩略图而已。

hackernews · soheilpro · 9月10日 09:04 · [社区讨论](https://news.ycombinator.com/item?id=49640646)

**背景**: Windows XP 是首个为每个用户账户提供专属头像的消费级 Windows 版本，这些头像取自系统内置的一组图库图片；据 Windows Wallpaper Wiki 记载，这些图片来自免版税的 Corbis 和 PhotoDisc 图库，挑选时力求体现“全球视野”，同时避免带有政治或种族色彩。Raymond Chen 是微软的资深工程师，他的博客 The Old New Thing 是了解 Windows 内部机制设计思路的重要来源，而 RtlRandomEx 则是操作系统内部用于生成伪随机数的原生 Windows API 之一。调用 RtlRandomEx 前需要一个种子，Windows XP 就用 GetTickCount()（系统启动以来经过的毫秒数）来充当这个种子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://devblogs.microsoft.com/oldnewthing/20260909-00/?p=112683">What algorithm did Windows XP use to choose your initial user picture? - The Old New Thing</a></li>
<li><a href="https://windowswallpaper.miraheze.org/wiki/Windows_XP">Windows XP - Windows Wallpaper Wiki - Miraheze</a></li>

</ul>
</details>

**社区讨论**: 评论者总体反应非常正面，有人称 Raymond Chen 每一篇关于 Windows 内部机制的文章都“像过圣诞节一样令人开心”，但也有人好奇他发布这些细节前是否需要获得许可。多位读者贴出了 GitHub 上真实的 NT5 源码链接，还有人借这篇文章反思编程所需的认知转换：人类几乎不费力气就能随机抓取一样东西，而计算机没有直接对应的做法，必须先计数、编号再抽样——mawadev 也指出，这种意识和纪律往往会被日常繁重的工作淹没。

**标签**: `#Windows XP`, `#Windows internals`, `#algorithms`, `#random selection`, `#UI design`

---

<a id="item-14"></a>
## [维基页面汇总索尼"拥有"数字游戏的说法，数字所有权诉讼持续发酵](https://consumerrights.wiki/w/Sony_PlayStation_digital_game_ownership_lawsuit) ⭐️ 7.0/10

consumerrights.wiki 上的一篇页面汇总了索尼及其 PlayStation Store 在多个场合告诉玩家他们"拥有"所购买数字游戏的说法。这份材料被用于一场正在加州进行的集体诉讼，该诉讼指控商店的"Buy Now（立即购买）"措辞误导消费者，让人误以为获得了所有权，而实际上只是获得可撤销的使用许可。 此案的核心在于：数字商店能否继续用"拥有"这类措辞来描述可撤销的许可。这一问题影响所有销售游戏、影视、音乐和电子书的数字平台。若判决对索尼不利，可能迫使整个行业采用更清晰的告知标准，并改变消费者对"自己花钱到底买到了什么"的理解。 索尼的抗辩逻辑是：如果买家真的"拥有"游戏，那么第二位顾客就不可能再购买同一款作品——其文件援引原告 Edward Heycock 于 2026 年 2 月 25 日以 69.99 美元买下《Resident Evil Requiem》，而原告 Jason Mendoza 早在 2026 年 2 月 14 日就已购买该游戏。文件还提到 PlayStation 服务条款第 14 条，其中规定了强制仲裁与集体诉讼弃权条款，用户若想退出必须在 30 天内以书面形式通知索尼。

hackernews · haunter · 9月10日 12:18 · [社区讨论](https://news.ycombinator.com/item?id=49642531)

**背景**: 数字商店通常出售的是访问内容的许可，而非实体拷贝，这意味着一旦服务关停或账号被封，平台就可以撤销访问权。consumerrights.wiki 是一个由社区共建的维基，专门记录维修权限制、计划性淘汰、订阅陷阱等反消费者做法，它与消费者权益倡导者 Louis Rossmann 以及他在 2025 年联合创立的 FULU 基金会相关。此次诉讼是一项拟议的集体诉讼，覆盖在加州 PlayStation Store 点击过"Buy Now"购买数字游戏的消费者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Consumer_Rights_Wiki">Consumer Rights Wiki</a></li>
<li><a href="https://cybernews.com/tech/sony-digital-game-ownership-lawsuit/">Sony Digital Game Ownership Fight: You Can’t Own Games, It ...</a></li>
<li><a href="https://openclassactions.com/lawsuits/consumer-protection/sony-playstation-digital-game-license-class-action-lawsuit.php">Do You Own Digital Games You Buy? Sony Lawsuit Explained</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者普遍对第 14 条的强制仲裁和集体诉讼弃权条款持反对态度，其中一位直言针对个人的强制仲裁"就该被彻底认定为非法"，因为它唯一的作用就是剥夺消费者和劳动者的权利。不少人用买书作类比：买一本书就拥有那一本，朋友买同一本书则拥有另一本，因此索尼的抗辩可能反而在无意中承认了某种形式的所有权。还有人表达了对索尼这家公司的不信任，并提及 2005 年索尼在用户电脑中植入 rootkit 的事件。

**标签**: `#digital-ownership`, `#consumer-rights`, `#licensing`, `#legal`, `#gaming`

---

<a id="item-15"></a>
## [OpenAI 推出金融服务版 ChatGPT，搭载 GPT-6 Astra](https://openai.com/index/introducing-chatgpt-financial-services) ⭐️ 7.0/10

OpenAI 宣布推出面向金融服务行业的 ChatGPT，该产品将内置金融数据与全新的旗舰模型 GPT-6 Astra 相结合，用于研究分析、财务建模以及生成可直接交付客户的材料。此次发布将其定位为一套打包好的行业垂直解决方案，而非通用聊天机器人。 这标志着 OpenAI 从横向的模型 API 供应，进一步迈向面向特定行业的打包式企业产品，瞄准的是经济中价值最高、监管也最严格的领域之一。如果被广泛采用，它可能重塑投资、银行与咨询工作流使用 AI 的方式，并使 OpenAI 与现有金融数据和分析平台形成更直接的竞争。 此次公告本身只是一段简短的宣传文字：没有披露技术基准测试、定价、上线日期，也没有说明数据授权、合规管控或客户数据处理方式等细节，而这些在受监管的金融行业中至关重要。其他渠道公布的模型信息则将 GPT-6 Astra 描述为 OpenAI 面向复杂推理、编程、计算机操作以及长时间多步骤智能体工作流的旗舰模型，在公开的 BenchAlign 排行榜上于约 232 个模型中排名第二，估计得分约为 81/100。

rss · OpenAI News · 9月10日 07:00

**背景**: 行业垂直型 AI 产品会把通用基础模型与专有数据、数据连接器和预置工作流相结合，使之适配单一行业；在金融领域，这通常意味着行情数据、监管文件、财报电话会议记录，以及与电子表格和建模工具的集成。OpenAI 此前已朝这一方向迈进：ChatGPT 中推出了个人理财功能，允许用户关联账户并获得预算与规划方面的帮助；同时它也有面向企业的金融服务方案，客户反馈称研究与尽职调查流程因此提速。GPT-6 Astra 正是这些产品所依托的旗舰模型。金融等受监管行业高度重视数据来源、可审计性与保密性，因此本次公告未提及合规细节格外值得注意。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/solutions/industries/financial-services/">AI for Financial Services | OpenAI</a></li>
<li><a href="https://openai.com/index/personal-finance-chatgpt/">A new personal finance experience in ChatGPT | OpenAI</a></li>
<li><a href="https://www.cometapi.com/models/openai/gpt-6-astra/">GPT - 6 Astra API - Access OpenAI GPT - 6 Astra at Best... | CometAPI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#financial-services`, `#GPT-6`, `#enterprise-ai`

---