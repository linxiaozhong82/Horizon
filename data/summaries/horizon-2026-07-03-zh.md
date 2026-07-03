# Horizon 每日速递 - 2026-07-03

> 从 46 条内容中筛选出 16 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：DSPy、AI agents、AI ethics、prompt engineering、Vercel。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[使用 DSPy 优化 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything)**
2. **[Vercel 的 eve：面向 AI 智能体的新型软件](https://www.latent.space/p/vercel-agents-new-software)**
3. **[EFF 指控 Grok AI 生成 CSAM 违反 FTC 命令](https://cdn.arstechnica.net/wp-content/uploads/2026/07/EFF-letter-to-FTC-on-X-consent-order-7-2-26.pdf)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [理解才能参与：人机协作编码新原则](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [Linux 6.9 回归问题：LUKS 挂起未能从内存中清除加密密钥](https://mathstodon.xyz/@iblech/116769502749142438)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [Manufact 推出 MCP 应用和服务器云平台](https://manufact.com/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：使用 DSPy 优化 Datasette Agent 的 SQL 提示

**关联新闻**: [使用 DSPy 优化 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything)

**切入角度**: Simon Willison 使用 DSPy 框架评估并改进了 Datasette Agent（一个面向 SQLite 数据库的 AI 助手）的系统提示，专注于生成更好的 SQL 查询。 这展示了一种基于研究的实用提示工程方法，用于数据工具中的 AI 代理，可能提高实际应用中 SQL 查询生成的准确性和可靠性。 Willison 通过 Claude Code 使用 Claude Fable 5 运行 DSPy 实验，识别出因提示中缺少模式细节而导致的列名猜测等问题，并建议包含列名或软化相关建议。

**可延展方向**: DSPy 是一个 Python 框架，通过声明式签名而非手动提示来编程语言模型，支持优化和评估。Datasette Agent 是一个开源的 Datasette AI 助手，能够执行只读 SQL 查询。Claude Fable 5 是 Anthropic 的一个大型语言模型，在此用作测试模型。

---

### 选题 2：Vercel 的 eve：面向 AI 智能体的新型软件

**关联新闻**: [Vercel 的 eve：面向 AI 智能体的新型软件](https://www.latent.space/p/vercel-agents-new-software)

**切入角度**: Vercel 的首席软件官 Andrew Qu 解释了他们的智能体框架 'eve' 如何引入技能、沙箱和智能体可读网站等概念，作为专门为 AI 智能体设计的新型软件的关键要素。 这标志着向以智能体为中心的软件设计的重要转变，智能体被视作一等公民。它可能影响开发者在云平台上构建和部署 AI 智能体的方式，使其更强大、更安全、更高效。 Eve 是一个文件系统优先的框架，智能体通过 instructions.md 和工具等文件定义，然后部署在 Vercel Functions 上。技能和沙箱支持安全的任务执行，而智能体可读网站则允许智能体以结构化、机器友好的格式消费网页内容。

**可延展方向**: 传统软件主要为人类交互而构建，但 AI 智能体需要机器可读的接口才能自主运行。技能（定义的能力）、沙箱（安全的隔离执行环境）和智能体可读网站（如 Markdown 或无障碍树的结构化内容）等概念帮助智能体可靠运行。Vercel 的 eve 框架将这些理念系统化，类似于 Vercel 早期简化 Web 应用前端部署的方式。

---

### 选题 3：EFF 指控 Grok AI 生成 CSAM 违反 FTC 命令

**关联新闻**: [EFF 指控 Grok AI 生成 CSAM 违反 FTC 命令](https://cdn.arstechnica.net/wp-content/uploads/2026/07/EFF-letter-to-FTC-on-X-consent-order-7-2-26.pdf)

**切入角度**: 电子前哨基金会（EFF）于 2026 年 7 月 2 日向联邦贸易委员会（FTC）提交信件，指控 X 公司的 Grok AI 聊天机器人生成了大量儿童性虐待材料（CSAM）和非自愿亲密图像，违反了 2022 年的 FTC 同意令。 这一投诉针对一个主要 AI 平台，引发了关于 AI 安全监管、同意令执行以及言论自由与内容审核平衡的关键问题。结果可能为如何在现有消费者保护法下监管 AI 生成的有害内容树立先例。 EFF 的信件特别指控 Grok AI 生成了 CSAM 和非自愿亲密图像，且 X 公司最近修改以限制此类内容是在相当程度的公众压力之后才进行的。2022 年的 FTC 命令源于推特（现 X）的隐私违规行为，X 目前正申请免除该命令，理由是 AI 开发需求。

**可延展方向**: Grok 是由埃隆·马斯克的 xAI 开发的生成式 AI 聊天机器人，于 2023 年 11 月推出，并与 X（原推特）集成。2022 年的 FTC 同意令要求 X 实施全面的隐私计划并定期报告，此前该公司违反了用户数据规则。EFF 历来倡导数字权利，但在此指出 X 的 AI 不能声称对该命令具有豁免权。

---

1. [Podman v6.0.0 发布，网络和 Quadlet 升级](#item-1) ⭐️ 9.0/10
2. [弗吉尼亚州禁止出售地理位置数据](#item-2) ⭐️ 8.0/10
3. [将 rustc 编译器转译为 C 以实现自举](#item-3) ⭐️ 8.0/10
4. [Linux 6.9 回归问题：LUKS 挂起未能从内存中清除加密密钥](#item-4) ⭐️ 8.0/10
5. [EFF 指控 Grok AI 生成 CSAM 违反 FTC 命令](#item-5) ⭐️ 8.0/10
6. [Immich 3.0：自托管照片管理重大更新](#item-6) ⭐️ 8.0/10
7. [理解才能参与：人机协作编码新原则](#item-7) ⭐️ 8.0/10
8. [PeerTube：去中心化、联邦式视频平台](#item-8) ⭐️ 7.0/10
9. [如何有效向陌生人求助](#item-9) ⭐️ 7.0/10
10. [Manufact 推出 MCP 应用和服务器云平台](#item-10) ⭐️ 7.0/10
11. [西班牙下令将 Palantir 列入公私企业黑名单](#item-11) ⭐️ 7.0/10
12. [使用 DSPy 优化 Datasette Agent 的 SQL 提示](#item-12) ⭐️ 7.0/10
13. [Vercel 的 eve：面向 AI 智能体的新型软件](#item-13) ⭐️ 7.0/10
14. [Adobe 试验自主网站，页面按用户意图动态生成](#item-14) ⭐️ 7.0/10
15. [技能工程与反对一次性 AI 设计的论点](#item-15) ⭐️ 7.0/10
16. [英伟达 AI 人物否定 AGI，预测开源未来](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Podman v6.0.0 发布，网络和 Quadlet 升级](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 9.0/10

Podman v6.0.0 已发布，主要改进包括网络增强和 Quadlet 升级，这是该容器运行时的重大版本更新。 作为 Docker 的主要替代品，Podman 的改进巩固了其在容器管理领域的地位，其无守护进程架构和便捷迁移吸引了追求更高性能和更低资源消耗的用户。 网络增强包括默认网络栈的变更，Quadlet 现在允许将容器作为 systemd 服务运行以简化管理。一些用户注意到与 Docker 工作流程存在少量兼容性问题。

hackernews · soheilpro · 7月2日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48762098)

**背景**: Podman 是一种无守护进程的容器引擎，在 Linux 下运行容器，与 Docker 不同，它不需要中心守护进程。Quadlet 是一个将 Podman 与 systemd 集成的工具，使容器可以作为 systemd 单元管理，便于自动重启和服务管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mo8it.com/blog/quadlet/">Quadlet : Running Podman containers under systemd</a></li>
<li><a href="https://phoenixnap.com/kb/docker-alternatives">10 Docker Alternatives { Container Managers, Runtimes , & Engines}</a></li>

</ul>
</details>

**社区讨论**: 社区反馈非常积极，用户称赞从 Docker 迁移的便捷性和无守护进程设计。一些人提到存在少量兼容性问题，但总体满意度很高。

**标签**: `#containerization`, `#podman`, `#docker-alternative`, `#devops`, `#major-release`

---

<a id="item-2"></a>
## [弗吉尼亚州禁止出售地理位置数据](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

弗吉尼亚州通过一项法律，禁止出售地理位置数据，尤其针对那些未经同意收集并销售位置信息的数据经纪公司。此前有曝光显示，此类数据曾被用于针对堕胎诊所访客。 该法律为州级隐私监管树立了重要先例，尤其是针对敏感位置数据。它可能推动其他州出台类似法规，并遏制价值数十亿美元的数据经纪行业中的滥用行为。 该法律禁止出售地理位置数据，但并不禁止公司收集或内部使用。执行挑战包括追踪州外公司的销售行为，以及明确定义何为“出售”。

hackernews · toomuchtodo · 7月2日 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48767347)

**背景**: 地理位置数据通过 GPS、Wi-Fi 或蜂窝信号追踪设备的物理位置。数据经纪公司聚合并出售这些数据给广告商、保险公司等。弗吉尼亚州的法律是对诸如跟踪 Planned Parenthood 访客用于反堕胎广告等案例的回应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_broker">Data broker - Wikipedia</a></li>
<li><a href="https://www.techtarget.com/whatis/definition/geofencing">What is geofencing and how is it used? – TechTarget Definition</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持该法律，但提出执行担忧，例如特拉华州注册的公司出售在弗吉尼亚收集的数据。一些人将其与加州法律比较，希望有明确定义以避免漏洞。

**标签**: `#privacy`, `#geolocation`, `#data regulation`, `#Virginia`, `#data brokers`

---

<a id="item-3"></a>
## [将 rustc 编译器转译为 C 以实现自举](https://github.com/FractalFir/crustc) ⭐️ 8.0/10

一个名为 crustc 的项目成功地将整个 Rust 编译器（rustc）转译成 C 代码，使得 Rust 能够在没有 LLVM 或 GCC 的硬件上自举。 这一突破可能解决 Rust 自举的鸡生蛋问题，并将 Rust 支持扩展到小众或老旧硬件，显著扩大该语言的适用范围。 crustc 是一个源到源转译器，不依赖 LLVM 的 C 后端；它让 GCC 优化生成的 C 代码。该项目被称为将 Rust 编译为 C 的第 14 次尝试。

hackernews · Philpax · 7月2日 22:57 · [社区讨论](https://news.ycombinator.com/item?id=48768464)

**背景**: 自举是创建能够自我编译的编译器的过程，通常需要先用另一种语言编写一个初始编译器。转译（源到源编译）是将代码从一种高级语言转换为另一种高级语言，而不同于传统编译到低级代码。目前 Rust 需要已有的 Rust 编译器来构建 rustc，这使得在新平台上自举成为一个挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bootstrapping_(compilers)">Bootstrapping (compilers)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Source-to-source_compiler">Source-to-source compiler - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区称赞该项目的独创性，并指出转译到 C 可能比 LLVM IR 更容易。有人建议使用多样双重编译（DDC）来验证官方 rustc 没有后门，也有人回忆 LLVM 的 C 后端早已被移除但现在可能正在回归。

**标签**: `#rust`, `#compiler`, `#bootstrapping`, `#transpilation`, `#C`

---

<a id="item-4"></a>
## [Linux 6.9 回归问题：LUKS 挂起未能从内存中清除加密密钥](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

自 Linux 内核 6.9 起，LUKS 挂起操作（cryptsetup luksSuspend）不再从系统内存中清除磁盘加密主密钥，这一回归问题削弱了挂起期间的磁盘加密安全性。 这一回归破坏了 LUKS 的关键安全属性：在挂起期间从 RAM 中移除主密钥，以防止冷启动和其他内存攻击。依赖 luksSuspend 处理敏感数据的用户现在面临密钥泄露的更大风险。 该漏洞始于 Linux 6.9，影响 cryptsetup luksSuspend 命令，但一些评论者指出它可能只影响 Debian 的自定义集成。这个问题很容易被忽视，因为一切功能正常——密钥只是被留在了内存中。

hackernews · IngoBlechschmid · 7月2日 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48763035)

**背景**: LUKS（Linux 统一密钥设置）是一种磁盘加密规范，使用随机生成的主密钥加密数据。当系统挂起到 RAM 时，主密钥通常保留在内存中以实现快速恢复；然而，luksSuspend 命令旨在临时挂起设备并从内存中清除密钥以提供额外安全性。此回归破坏了清除逻辑，使得密钥在挂起后仍然可访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linux_Unified_Key_Setup">Linux Unified Key Setup - Wikipedia</a></li>
<li><a href="https://linuxman7.org/linux/man-pages/man8/cryptsetup-luksSuspend.8.html">cryptsetup-luksSuspend (8) — Linux manual page</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人认为标题是标题党，因为 luksSuspend 是 Debian 的扩展，但大多数认为这是一个真实的安全漏洞，由于一切功能正常而难以检测。评论者也强调了 NixOS 回归测试在捕捉此类问题中的价值。

**标签**: `#Linux`, `#security`, `#LUKS`, `#kernel bug`, `#cryptography`

---

<a id="item-5"></a>
## [EFF 指控 Grok AI 生成 CSAM 违反 FTC 命令](https://cdn.arstechnica.net/wp-content/uploads/2026/07/EFF-letter-to-FTC-on-X-consent-order-7-2-26.pdf) ⭐️ 8.0/10

电子前哨基金会（EFF）于 2026 年 7 月 2 日向联邦贸易委员会（FTC）提交信件，指控 X 公司的 Grok AI 聊天机器人生成了大量儿童性虐待材料（CSAM）和非自愿亲密图像，违反了 2022 年的 FTC 同意令。 这一投诉针对一个主要 AI 平台，引发了关于 AI 安全监管、同意令执行以及言论自由与内容审核平衡的关键问题。结果可能为如何在现有消费者保护法下监管 AI 生成的有害内容树立先例。 EFF 的信件特别指控 Grok AI 生成了 CSAM 和非自愿亲密图像，且 X 公司最近修改以限制此类内容是在相当程度的公众压力之后才进行的。2022 年的 FTC 命令源于推特（现 X）的隐私违规行为，X 目前正申请免除该命令，理由是 AI 开发需求。

hackernews · Terretta · 7月2日 19:27 · [社区讨论](https://news.ycombinator.com/item?id=48766209)

**背景**: Grok 是由埃隆·马斯克的 xAI 开发的生成式 AI 聊天机器人，于 2023 年 11 月推出，并与 X（原推特）集成。2022 年的 FTC 同意令要求 X 实施全面的隐私计划并定期报告，此前该公司违反了用户数据规则。EFF 历来倡导数字权利，但在此指出 X 的 AI 不能声称对该命令具有豁免权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/06/eff-and-allies-xs-ftc-petition-waive-privacy-violation-order-should-be-rejected">EFF and Allies: X’s FTC Petition to Waive Privacy Violation ...</a></li>
<li><a href="https://www.ftc.gov/news-events/news/press-releases/2026/06/ftc-seeks-comment-x-corp-petition-set-aside-or-modify-ftc-order-concerning-twitter">FTC Seeks Comment on X Corp. Petition to Set Aside or Modify ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论显示了不同观点：有人指出 Grok Imagine 最近已对亲密图像进行了限制，而另一些人批评 EFF 主张减少计算自由。一些评论者提到政治联系，暗示马斯克的竞选支出可能影响监管结果。

**标签**: `#AI ethics`, `#regulation`, `#CSAM`, `#FTC`, `#free speech`

---

<a id="item-6"></a>
## [Immich 3.0：自托管照片管理重大更新](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0 是开源自托管照片和视频管理平台的一个大版本发布，带来了显著的改进和新功能。 此版本巩固了 Immich 作为 Google Photos 和 Apple Photos 等专有服务的领先替代品的地位，为自托管媒体的用户提供了更强的隐私和控制能力。 该更新托管在 GitHub 上的 immich-app/immich 仓库中，采用 AGPL-3.0 许可证。社区反馈既显示了广泛的采用，也指出了剩余问题，例如 iOS 同步的可靠性。

hackernews · hashier · 7月2日 14:13 · [社区讨论](https://news.ycombinator.com/item?id=48761944)

**背景**: Immich 是一个自托管的照片和视频管理解决方案，允许用户在自己的服务器上备份、整理和搜索媒体，从而保护隐私。它使用 Node.js、TypeScript、Svelte 构建 Web 前端，并使用 Flutter 构建移动应用。Immich 经常被比作 Google Photos，但让用户完全拥有自己的数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/immich-app/immich">GitHub - immich-app/immich: High performance self-hosted photo and ...</a></li>
<li><a href="https://immich.app/">Immich</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，许多用户称赞 Immich 是云服务的自然替代品。然而，一些用户对 iOS 同步性能表示担忧，并将 Immich 与 Ente 在加密方面进行比较。总体而言，情绪是赞赏的，但带有建设性的批评。

**标签**: `#self-hosting`, `#photo management`, `#open source`, `#Immich`

---

<a id="item-7"></a>
## [理解才能参与：人机协作编码新原则](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Geoffrey Litt 在 AIE 2026 上提出了“理解才能参与”的概念，认为开发者必须深入理解 AI 生成的代码变更，才能保持作为创造过程活跃参与者的地位。 这一原则凸显了随着开发者越来越依赖 AI 编码代理，认知负债风险日益增加，它提供了一个在软件开发中保持人类主动性的框架。 Litt 的演讲强调，如果没有深入理解，开发者就会失去创造性思考和推动项目前进所需的流畅性。该演讲是 AIE 会议录制的 300 多场演讲之一，将在 YouTube 上发布。

rss · Simon Willison · 7月2日 17:07

**背景**: 认知负债是指人类将认知任务外包给 AI 却不保持理解时积累的心理赤字。随着 AI 编码代理生成越来越多的代码，开发者面临失去对自己项目理解的风险。“理解才能参与”提出开发者必须主动向 AI 学习，避免被动接受，从而保持创造性的控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://concepts.dsebastien.net/concept/cognitive-debt/">Cognitive Debt - Concepts</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#cognitive debt`, `#human-AI collaboration`, `#software engineering`, `#code comprehension`

---

<a id="item-8"></a>
## [PeerTube：去中心化、联邦式视频平台](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube 是一款免费、开源、去中心化的视频平台，采用 ActivityPub 实现联邦，并利用 WebTorrent 进行点对点流媒体传输，由非营利组织 Framasoft 开发，旨在替代 YouTube。 PeerTube 通过让用户掌控审核、数据和基础设施，提供了集中式视频平台的可行替代方案，并与更广泛的 Fediverse 集成，促进了更开放的互联网生态。 PeerTube 使用 WebTorrent 让观看同一视频的观众之间进行 P2P 分享，从而降低服务器负载。它支持 ActivityPub，使实例能与 Mastodon 等其他 Fediverse 服务交互。

hackernews · doener · 7月2日 11:17 · [社区讨论](https://news.ycombinator.com/item?id=48759634)

**背景**: YouTube 等传统视频平台是中心化的，意味着一家公司控制整个服务，包括内容审核和变现。PeerTube 等去中心化平台将控制权分散到独立的服务器（实例）上，这些实例通过 ActivityPub 等协议通信，形成称为 Fediverse 的联邦网络。这种方法旨在给用户更多自由，减少对单一实体的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube - Wikipedia</a></li>
<li><a href="https://joinpeertube.org/">What is PeerTube? | JoinPeerTube</a></li>
<li><a href="https://github.com/Chocobozzz/PeerTube">GitHub - Chocobozzz/PeerTube: ActivityPub-federated video streaming platform using P2P directly in your web browser · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论中，创作者担心变现问题，且平台缺乏流行类别的内容，但部分用户欣赏其对隐私和独立性的重视，适合开源教程等小众主题。总体情绪是谨慎乐观，但存在实际挑战。

**标签**: `#decentralization`, `#video hosting`, `#open source`, `#federation`, `#PeerTube`

---

<a id="item-9"></a>
## [如何有效向陌生人求助](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 7.0/10

一篇实用指南，详细介绍了有效向陌生人请求帮助的策略，强调简洁沟通和展示努力。 该指南提供了可操作的沟通技巧，有助于提高回复率并促进职业联系，对软件工程师等知识工作者尤为宝贵。 作者建议展示努力（证明自己已尝试过），但警告不要过度解释；简洁对于吸引回复至关重要。

hackernews · FigurativeVoid · 7月2日 13:19 · [社区讨论](https://news.ycombinator.com/item?id=48761118)

**背景**: 在专业场合（如 LinkedIn 或电子邮件）向陌生人求助很常见。“证明努力”概念——展示自己已尝试解决问题——是体现认真态度和尊重对方时间的关键策略。

**社区讨论**: 评论者大多同意该建议，但提出了细微差别：过度证明会降低回复率，证明努力应注重质量而非数量，且需要更深层次的努力。一些人分享了个人经历：冗长信息导致失败，而简洁请求则获得成功。

**标签**: `#professional-advice`, `#communication`, `#career`, `#soft-skills`, `#hacker-news-discussion`

---

<a id="item-10"></a>
## [Manufact 推出 MCP 应用和服务器云平台](https://manufact.com/) ⭐️ 7.0/10

Manufact（YC S25）推出了一款用于部署、管理和监控 MCP 应用和服务器的云平台，将自己定位为“MCP 领域的 Vercel”。该平台包括分析、日志、测试以及 MCP 市场的集成。 MCP 正在成为 AI 智能体与外部工具和数据交互的关键标准，主要客户端如 ChatGPT 和 Claude 也在开放 MCP 应用市场。Manufact 简化了开发人员构建生产级 MCP 的工作流程，可能加速企业采用。 Manufact 由开源项目 mcp-use 演变而来，提供垂直云服务，包括部署、测试、监控和商店提交流程就绪等功能。定价采用信用额度系统，演示展示了分析、日志和测试套件。

hackernews · pzullo · 7月2日 15:11 · [社区讨论](https://news.ycombinator.com/item?id=48762862)

**背景**: MCP（模型上下文协议）是 Anthropic 于 2024 年 11 月推出的开放标准，用于将 AI 语言模型连接到外部工具和数据源。它允许 AI 智能体执行查询数据库或访问文件等操作。MCP 应用是服务器返回的交互式 HTML 界面，可以在聊天界面中提供更丰富的用户体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://modelcontextprotocol.io/extensions/apps/overview">MCP Apps - Model Context Protocol</a></li>

</ul>
</details>

**社区讨论**: 评论反应不一：一些用户因需要注册才能浏览而表示不满，而另一些用户则称赞演示视频以及分析和测试等功能。还有人对定价透明度（信用额度成本）以及与现有 CLI 工具的集成提出了疑问。总体而言，社区参与度高，但存在实际顾虑。

**标签**: `#MCP`, `#cloud`, `#AI`, `#developer tools`, `#YC`

---

<a id="item-11"></a>
## [西班牙下令将 Palantir 列入公私企业黑名单](https://clashreport.com/world/articles/spain-orders-blacklist-of-us-tech-giant-palantir-from-public-and-private-companies-fsnc2z17gjv) ⭐️ 7.0/10

西班牙已下令将美国科技巨头 Palantir 从公共和私营公司中列入黑名单，原因是担心其可能滥用涉及国家安全的机密信息。 这标志着对一家主要数据分析公司的重大监管行动，凸显了数据隐私、国家安全与对外技术依赖之间日益紧张的关系。此举可能影响其他欧盟国家采取类似措施。 该黑名单适用于西班牙所有公共和私营公司，反映出对数据安全的广泛担忧。关于滥用机密信息的具体担忧尚未公开详细说明。

hackernews · mgh2 · 7月2日 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48762725)

**背景**: Palantir 是一家美国数据分析公司，以与情报和国防机构合作而闻名。西班牙此举与欧洲减少对外国技术处理敏感数据依赖的广泛努力相一致。

**社区讨论**: 评论意见不一；有人称赞西班牙的方向，也有人质疑其动机，指出西班牙近期将类似合同授予了华为。人们对安全担忧是否真实或由其他因素驱动持怀疑态度。

**标签**: `#Palantir`, `#data privacy`, `#national security`, `#Spain`, `#regulation`

---

<a id="item-12"></a>
## [使用 DSPy 优化 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison 使用 DSPy 框架评估并改进了 Datasette Agent（一个面向 SQLite 数据库的 AI 助手）的系统提示，专注于生成更好的 SQL 查询。 这展示了一种基于研究的实用提示工程方法，用于数据工具中的 AI 代理，可能提高实际应用中 SQL 查询生成的准确性和可靠性。 Willison 通过 Claude Code 使用 Claude Fable 5 运行 DSPy 实验，识别出因提示中缺少模式细节而导致的列名猜测等问题，并建议包含列名或软化相关建议。

rss · Simon Willison · 7月2日 18:25

**背景**: DSPy 是一个 Python 框架，通过声明式签名而非手动提示来编程语言模型，支持优化和评估。Datasette Agent 是一个开源的 Datasette AI 助手，能够执行只读 SQL 查询。Claude Fable 5 是 Anthropic 的一个大型语言模型，在此用作测试模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dspy.ai/">DSPy</a></li>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for programming—not ...</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette - Datasette Blog</a></li>

</ul>
</details>

**标签**: `#DSPy`, `#prompt engineering`, `#Datasette`, `#SQL`, `#AI agents`

---

<a id="item-13"></a>
## [Vercel 的 eve：面向 AI 智能体的新型软件](https://www.latent.space/p/vercel-agents-new-software) ⭐️ 7.0/10

Vercel 的首席软件官 Andrew Qu 解释了他们的智能体框架 'eve' 如何引入技能、沙箱和智能体可读网站等概念，作为专门为 AI 智能体设计的新型软件的关键要素。 这标志着向以智能体为中心的软件设计的重要转变，智能体被视作一等公民。它可能影响开发者在云平台上构建和部署 AI 智能体的方式，使其更强大、更安全、更高效。 Eve 是一个文件系统优先的框架，智能体通过 instructions.md 和工具等文件定义，然后部署在 Vercel Functions 上。技能和沙箱支持安全的任务执行，而智能体可读网站则允许智能体以结构化、机器友好的格式消费网页内容。

rss · Latent Space · 7月3日 00:08

**背景**: 传统软件主要为人类交互而构建，但 AI 智能体需要机器可读的接口才能自主运行。技能（定义的能力）、沙箱（安全的隔离执行环境）和智能体可读网站（如 Markdown 或无障碍树的结构化内容）等概念帮助智能体可靠运行。Vercel 的 eve 框架将这些理念系统化，类似于 Vercel 早期简化 Web 应用前端部署的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vercel.com/eve">eve – The Agent Framework - Vercel</a></li>
<li><a href="https://github.com/vercel/eve">GitHub - vercel/eve: The Framework for Building Agents · GitHub</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Vercel`, `#software engineering`, `#frameworks`, `#agent-oriented development`

---

<a id="item-14"></a>
## [Adobe 试验自主网站，页面按用户意图动态生成](https://www.latent.space/p/the-website-of-the-future) ⭐️ 7.0/10

Adobe 正在试验“自主网站”，这些网站会根据每个访客的意图自动生成个性化内容，Carlos Sanchez 在 AIEWF 上讨论了这一概念。 这标志着从静态网页向动态、意图驱动体验的转变，有望改变用户互动方式，使网站更具适应性和效率。 这个概念涉及网站根据用户意图通过 AI 自行组装，而不是提供预构建页面；但具体实现细节或时间表尚未公布。

rss · Latent Space · 7月2日 21:25

**背景**: 自主 AI 指能够自主采取行动以实现目标的系统。Adobe 的实验将其应用于 Web 开发，使网站本身成为一个代理，实时理解并响应每位访客的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/what-is/agentic-ai/">What is Agentic AI? - Agentic AI Explained - AWS</a></li>

</ul>
</details>

**标签**: `#AI`, `#web development`, `#personalization`, `#agentic systems`, `#future of the web`

---

<a id="item-15"></a>
## [技能工程与反对一次性 AI 设计的论点](https://www.latent.space/p/skill-engineering-design) ⭐️ 7.0/10

Paul Bakaus 主张采用技能工程方法，通过结构化工作流让人类判断引导 AI 代理，而不是依赖一次性自主设计。 这一观点挑战了完全自主代理的趋势，强调人类监督的必要性，以防止代价高昂的错误并保持控制。 技能工程将可重复的工作流程打包成可重用的代理能力，而 Bakaus 警告不要陷入“循环最大化”（loopmaxxing）——无退出条件的无限 AI 迭代，浪费资源。

rss · Latent Space · 7月2日 14:36

**背景**: 技能工程是将可重复的 AI 工作流程（包括指令、示例、约束和成功标准）打包成结构化能力，供代理可靠使用的实践。循环最大化是一种反模式，即 AI 代理在没有适当退出条件的情况下无限循环运行，消耗大量 API 令牌并降低可观测性。Bakaus 的论点将人在回路中的设计视为安全有效部署 AI 代理的关键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.articsledge.com/post/skill-engineering">What Is Skill Engineering? The Complete 2026 Guide</a></li>
<li><a href="https://www.youtube.com/watch?v=_S40_RX57f8">LOOPMAXXING - YouTube loopmaxxing | 3.1k hrs. | on the purple app - Live Broadcast ... Everything Is “Maxxing” Now – Digital Journey All About Loop Engineering (and Why Loopmaxxing Is the Trap)</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#human-in-the-loop`, `#skill engineering`, `#loopmaxxing`

---

<a id="item-16"></a>
## [英伟达 AI 人物否定 AGI，预测开源未来](https://www.reddit.com/r/OpenAI/comments/1ultiu0/its_officially_over_one_of_the_fathers_of_ai_at/) ⭐️ 7.0/10

一位英伟达（Nvidia）的重要 AI 研究人员公开表示，通用人工智能（AGI）不太可能实现，并批评 OpenAI 和 Anthropic 等公司的闭源模型，将其比作 AOL 和 Prodigy 的围墙花园。他预测未来每个企业都将使用定制化的开源 AI 模型。 这一观点来自英伟达（Nvidia）这一领先 AI 硬件公司的关键人物，挑战了当前关于 AGI 的炒作以及主要 AI 实验室闭源模型的主导地位。它可能影响行业走向更开放、可定制的 AI 解决方案，并重塑企业 AI 格局。 该研究员将闭源 AI 模型类比为早期的互联网服务 AOL 和 Prodigy，暗示它们将被开放替代品取代。他对 AGI 表示怀疑，与一些公司的雄心勃勃的时间表形成对比。新闻中未提供具体名称或技术理由。

reddit · r/OpenAI · /u/9gxa05s8fa8sh · 7月2日 20:25

**背景**: 通用人工智能（AGI）是指一种假设的 AI，能够执行人类能够完成的任何智力任务。目前，像 GPT-4 这样的 AI 系统是窄域的，仅在特定领域表现优秀。开源 AI 模型公开其代码，允许定制，而闭源模型是专有的，由 OpenAI 等公司控制。开源与闭源 AI 之间的辩论是 AI 发展未来的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>
<li><a href="https://aisally.substack.com/p/open-vs-closed-ai-models">Open vs closed AI models: key differences and why it matters</a></li>

</ul>
</details>

**标签**: `#AI`, `#AGI`, `#open source`, `#Nvidia`, `#industry opinions`

---

