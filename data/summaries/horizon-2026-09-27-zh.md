# Horizon 每日速递 - 2026-09-27

> 从 27 条内容中筛选出 6 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：AI agents、diagrams、LLMs、Excalidraw、developer-tools。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Drawgent：在实时 Excalidraw 画布上作图的 AI 编程代理](https://tangled.org/yanndegat.tngl.sh/drawgent)**
2. **[Reladraw：让你自己决定元素位置的新型图表语言](https://github.com/reladraw/reladraw)**
3. **[程序员热议：在大模型时代如何继续享受编程](https://discourse.haskell.org/t/how-to-keep-enjoying-programming-in-a-world-of-llms/14705)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [DeepSeek 的 DSec 在 160 台 EPYC 节点上同时运行 38 万个沙箱](https://arxiv.org/abs/2609.22978)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [DeepSeek 的 DSec 在 160 台 EPYC 节点上同时运行 38 万个沙箱](https://arxiv.org/abs/2609.22978)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [DeepSeek 的 DSec 在 160 台 EPYC 节点上同时运行 38 万个沙箱](https://arxiv.org/abs/2609.22978)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Drawgent：在实时 Excalidraw 画布上作图的 AI 编程代理

**关联新闻**: [Drawgent：在实时 Excalidraw 画布上作图的 AI 编程代理](https://tangled.org/yanndegat.tngl.sh/drawgent)

**切入角度**: Drawgent 是一款新的开发工具，它以协作者身份加入 Excalidraw 房间，表现为一个带有自己光标的“Agent”参与者，其编辑动作会实时反映在共享画布上。人类用户仍可照常在 excalidraw.com 上工作，代理的改动会同步出现在同一房间中，房间内的通信流量通过房间密钥进行端到端加密。 它把 AI 编程代理从纯文本聊天和终端输出推进到空间化、可视化的协作场景，这对于以图表承载讨论的架构评审和头脑风暴尤为重要。同时它也处在快速扩张的 MCP 工具体系之中，让模型能对外部应用执行操作，而不仅仅是描述操作。 该代理操作的是实时共享画布，而非生成静态图片，因此双方的编辑是协作式的，并能通过代理光标即时可见。由于 Excalidraw 将图表存储为带坐标和边界框的结构化元素数据，代理必须处理布局几何信息而非自由文本——这也是多位评论者指出的主要摩擦点。

**可延展方向**: Excalidraw 是一款开源虚拟白板，可在浏览器中直接绘制手绘风格的图表、流程图和草图，并支持实时协作房间。MCP（Model Context Protocol，模型上下文协议）是一个把 AI 应用连接到外部系统的开放标准，让代理可以调用工具、读取第三方应用的数据。Drawgent 把两者结合起来：代理不再只是输出一段图表描述，而是以参与者身份接入白板会话本身。

---

### 选题 2：Reladraw：让你自己决定元素位置的新型图表语言

**关联新闻**: [Reladraw：让你自己决定元素位置的新型图表语言](https://github.com/reladraw/reladraw)

**切入角度**: Reladraw 是一种全新的文本式图表语言，已在 GitHub 发布并通过 Show HN 帖子亮相；它允许用户声明实体、分组和箭头，同时显式指定它们的相对位置，而不是完全依赖自动布局。项目提供了无需安装的在线 Playground、简单的 npm install 安装方式，以及可直接接入 Claude 或其他编码智能体的 Agent Skill。 现有的图表 DSL（如 Mermaid、Graphviz、D2）往往要在“声明式语法方便但排版不可控”和“Draw.io 等手动编辑器强大却费时、且不利于智能体操作”之间二选一。Reladraw 恰好瞄准这一空白，而在 AI 编码智能体日益成为图表主要使用者的当下，一种紧凑、确定性、便于智能体操控的语言，有望大幅降低开发者心智模型与智能体产出之间的可视化对齐成本。 其位置控制采用相对方式表达（例如 "from: left to: right"），而非绝对坐标，这使源码保持紧凑，但也限制了布局精确到像素的程度。项目有意收窄范围，只聚焦方框、分组和箭头，而非成熟绘图工具的庞杂功能；早期用户反馈还暴露出一些粗糙之处，例如自定义边未能智能地渲染为弧形箭头。

**可延展方向**: 图表即代码（diagram-as-code）工具大致分为两派：一派是 Mermaid、Graphviz、D2 这类自动布局语言，用户只声明节点与连线，几何位置由引擎决定；另一派是 Draw.io 这类图形编辑器，所有元素都靠手工摆放。自动布局工具书写快、便于版本比对，但在大型流程图等场景下常生成难看甚至难以阅读的结果；手工编辑器精确但费时，且难以被脚本或 AI 智能体驱动。Reladraw 试图兼顾两者，既保留声明式文本格式，又让作者能操控相对位置；它还提供了一个 Agent Skill——一种打包好的能力，让 Claude 等智能体可以完成生成图表之类的特定任务。

---

### 选题 3：程序员热议：在大模型时代如何继续享受编程

**关联新闻**: [程序员热议：在大模型时代如何继续享受编程](https://discourse.haskell.org/t/how-to-keep-enjoying-programming-in-a-world-of-llms/14705)

**切入角度**: 一个 Hacker News 讨论帖（153 分、208 条评论）同时在 Haskell Discourse 论坛上出现，程序员们围绕在大语言模型（LLM）越来越替代人写代码的背景下，是否还能以及如何继续享受编程这门手艺展开辩论。参与者分享了各自关于技能退化、"技能表达" 丧失，以及把 AI 当作协作者而非替代者从而重拾乐趣的亲身经历。 这场讨论折射出越来越多开发者的身份危机——他们的手艺感、专业能力认同和职业满足感都与亲手写代码紧密相连；这可能影响团队、教育机构和工具厂商如何看待 AI 辅助开发。它说明 LLM 的价值不仅是生产力问题，还关乎整个行业的动力、学习与长期技能培养。 有评论者指出，把任何任务交给 LLM 往往会导致对应的人类技能退化，因此一些人刻意不向 AI 求助，以保护自己解决问题的能力。也有人报告了相反的效果，称 LLM 降低了摩擦，让他们能在几小时内从零上手不熟悉的语言和技术栈；整场讨论没有数据支撑，只有个人经验与类比。

**可延展方向**: GitHub Copilot、ChatGPT、Claude 等基于 LLM 的编程助手能够根据自然语言提示生成可运行的代码，过去几年里已在专业软件开发中被广泛采用。Hacker News 是知名的技术论坛，开发者经常在此讨论行业趋势，这条帖子也被转到了 Haskell 社区的 Discourse 论坛。这场辩论与制造业和自动化领域的老问题相呼应：当工具承担了手艺的一部分工作，从业者可能既失去技能，也失去它带来的满足感。

---

1. [DeepSeek 的 DSec 在 160 台 EPYC 节点上同时运行 38 万个沙箱](#item-1) ⭐️ 7.0/10
2. [Reladraw：让你自己决定元素位置的新型图表语言](#item-2) ⭐️ 7.0/10
3. [Drawgent：在实时 Excalidraw 画布上作图的 AI 编程代理](#item-3) ⭐️ 7.0/10
4. [十五年后回望：Apple Cards 应用的起源故事](#item-4) ⭐️ 7.0/10
5. [程序员热议：在大模型时代如何继续享受编程](#item-5) ⭐️ 7.0/10
6. [Conversations 开发者与 Google Play 分道扬镳，XMPP 应用转为免费](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek 的 DSec 在 160 台 EPYC 节点上同时运行 38 万个沙箱](https://arxiv.org/abs/2609.22978) ⭐️ 7.0/10

DeepSeek 在 arXiv 上发布了 DSec（DeepSeek Elastic Compute）论文，描述了一套沙箱基础设施，可在 160 台基于 EPYC 的服务器节点上同时运行约 38 万个沙箱。从 DeepSeek-V4.1 开始，DeepSeek 将 rollout 执行迁移到 DSec 上，并拆分为两部分：承载脚手架（如 DeepSeek Harness）及其工具的 agent 沙箱，以及提供与脚手架无关的控制层的 worker 容器。 智能体强化学习需要大量并行且带状态的运行环境，而如何高效地提供这些环境，是规模化训练强智能体的主要瓶颈之一。DSec 表明，通过与强化学习训练循环协同设计沙箱层，可以把这样规模的沙箱集群压缩到相对较小的硬件上，这可能降低其他实验室构建智能体模型的基础设施门槛。 该系统与强化学习框架协同设计：它把带状态的 rollout 执行与可被抢占的 GPU 训练解耦，并将沙箱生命周期与训练过程相协调，从而在回收闲置资源的同时保留 rollout 状态。论文的作者名单异常庞大——共有 131 位署名作者，据报道还有 31 位贡献者甚至未在页面上列出。

hackernews · shenli3514 · 9月26日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=49859112)

**背景**: 智能体的强化学习通过让模型在环境中反复行动（例如带工具调用的代码解释器）并根据结果学习来实现；为保证安全与可复现，每个这样的环境通常被隔离在一个轻量级沙箱或 microVM 中。由于训练需要大量并行 rollout，同时 GPU 资源又必须被动态释放和重新分配，因此沙箱集群既要规模巨大，又要具备弹性。DSec 正是 DeepSeek 针对这一调度问题给出的方案，以系统论文而非模型发布的形式对外公开。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://arxiv.org/html/2609.22978v1">DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://technode.com/2026/09/23/deepseek-dsec-agent-training-sandbox-infrastructure/">DeepSeek details DSec sandbox infrastructure for agent training · TechNode</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者最震惊的是其规模——有人称在 160 台 EPYC 节点上跑 38 万个并发沙箱“简直疯狂”——并由此联想到智能体集群（agent swarm）的潜在影响：一位读者询问这是否是一种“agent 运行底座”，另一位则怀疑这种能力是否意味着可指挥由 38 万个智能体组成的集群攻击任意目标。讨论中反复出现的另一个话题与技术本身关系不大，而是论文庞大的作者名单，有评论者认为这可能是一种人才保护策略，避免竞争对手识别出具体研究人员并挖角。

**标签**: `#DeepSeek`, `#distributed-systems`, `#infrastructure`, `#sandboxes`, `#elastic-compute`

---

<a id="item-2"></a>
## [Reladraw：让你自己决定元素位置的新型图表语言](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw 是一种全新的文本式图表语言，已在 GitHub 发布并通过 Show HN 帖子亮相；它允许用户声明实体、分组和箭头，同时显式指定它们的相对位置，而不是完全依赖自动布局。项目提供了无需安装的在线 Playground、简单的 npm install 安装方式，以及可直接接入 Claude 或其他编码智能体的 Agent Skill。 现有的图表 DSL（如 Mermaid、Graphviz、D2）往往要在“声明式语法方便但排版不可控”和“Draw.io 等手动编辑器强大却费时、且不利于智能体操作”之间二选一。Reladraw 恰好瞄准这一空白，而在 AI 编码智能体日益成为图表主要使用者的当下，一种紧凑、确定性、便于智能体操控的语言，有望大幅降低开发者心智模型与智能体产出之间的可视化对齐成本。 其位置控制采用相对方式表达（例如 "from: left to: right"），而非绝对坐标，这使源码保持紧凑，但也限制了布局精确到像素的程度。项目有意收窄范围，只聚焦方框、分组和箭头，而非成熟绘图工具的庞杂功能；早期用户反馈还暴露出一些粗糙之处，例如自定义边未能智能地渲染为弧形箭头。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**背景**: 图表即代码（diagram-as-code）工具大致分为两派：一派是 Mermaid、Graphviz、D2 这类自动布局语言，用户只声明节点与连线，几何位置由引擎决定；另一派是 Draw.io 这类图形编辑器，所有元素都靠手工摆放。自动布局工具书写快、便于版本比对，但在大型流程图等场景下常生成难看甚至难以阅读的结果；手工编辑器精确但费时，且难以被脚本或 AI 智能体驱动。Reladraw 试图兼顾两者，既保留声明式文本格式，又让作者能操控相对位置；它还提供了一个 Agent Skill——一种打包好的能力，让 Claude 等智能体可以完成生成图表之类的特定任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49858513">Show HN: Reladraw – A diagram language where you decide where ...</a></li>
<li><a href="https://github.com/reladraw/reladraw">reladraw/reladraw - GitHub</a></li>
<li><a href="https://claude.com/blog/skills">Introducing Agent Skills | Claude by Anthropic</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上认可该工具切中了痛点，有人称它“在 AI 编码时代非常必要”，可用于让心智模型与智能体对齐；也有人指出 Mermaid 在时序图和甘特图上表现不错，但在位置至关重要的流程图上很差。最有价值的反馈是建议将“拓扑结构”（箭头、分组）与“布局关注点”解耦，并把 Reladraw 用作 C4 图表的布局层；另有人追问智能体自身能否生成足够复杂的图表，还有用户报告了一个 bug：带有显式左右端点的自定义边未能渲染成弧形箭头。

**标签**: `#diagrams`, `#developer-tools`, `#DSL`, `#visualization`, `#AI-agents`

---

<a id="item-3"></a>
## [Drawgent：在实时 Excalidraw 画布上作图的 AI 编程代理](https://tangled.org/yanndegat.tngl.sh/drawgent) ⭐️ 7.0/10

Drawgent 是一款新的开发工具，它以协作者身份加入 Excalidraw 房间，表现为一个带有自己光标的“Agent”参与者，其编辑动作会实时反映在共享画布上。人类用户仍可照常在 excalidraw.com 上工作，代理的改动会同步出现在同一房间中，房间内的通信流量通过房间密钥进行端到端加密。 它把 AI 编程代理从纯文本聊天和终端输出推进到空间化、可视化的协作场景，这对于以图表承载讨论的架构评审和头脑风暴尤为重要。同时它也处在快速扩张的 MCP 工具体系之中，让模型能对外部应用执行操作，而不仅仅是描述操作。 该代理操作的是实时共享画布，而非生成静态图片，因此双方的编辑是协作式的，并能通过代理光标即时可见。由于 Excalidraw 将图表存储为带坐标和边界框的结构化元素数据，代理必须处理布局几何信息而非自由文本——这也是多位评论者指出的主要摩擦点。

hackernews · parasitid · 9月26日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=49857729)

**背景**: Excalidraw 是一款开源虚拟白板，可在浏览器中直接绘制手绘风格的图表、流程图和草图，并支持实时协作房间。MCP（Model Context Protocol，模型上下文协议）是一个把 AI 应用连接到外部系统的开放标准，让代理可以调用工具、读取第三方应用的数据。Drawgent 把两者结合起来：代理不再只是输出一段图表描述，而是以参与者身份接入白板会话本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tangled.org/yanndegat.tngl.sh/drawgent">yanndegat.tngl.sh/drawgent at main · Tangled</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://excalidraw.com/">Excalidraw Whiteboard</a></li>

</ul>
</details>

**社区讨论**: 评论者总体感兴趣但态度务实：有人指出 Excalidraw 官方已经提供了开源的第一方 MCP 端点和服务器；另一位表示在大量尝试后认为基于 Excalidraw 的方案仍不够理想，最终选择 Mermaid 作为对代理最友好的媒介，并为此写了一个 Obsidian 插件。也有人认为画图真正的价值来自它逼出的思考过程，还有人认为相比让模型去估算边界框和像素坐标的 JSON 式画布抽象，HTML 被严重低估了；另有一位开发者把自己的 whiteboard-agents 类似项目开源出来供对比。

**标签**: `#AI agents`, `#Excalidraw`, `#diagramming`, `#developer tools`, `#MCP`

---

<a id="item-4"></a>
## [十五年后回望：Apple Cards 应用的起源故事](https://lexontech.org/fifteen-years-later-the-apple-cards-origin-story) ⭐️ 7.0/10

一篇在苹果 2011 年 Cards 应用发布约十五年后发表的回顾文章，深入讲述了这款产品是如何被打造出来的，包括其凸版印刷式打印流程、与美国邮政（USPS）合作开发的、可在紫外光下显现的隐形条码以实现全程物流追踪，以及那些自认被“Sherlocked”的竞争创业公司随后的失败。 它记录了一个罕见案例：苹果迫使一支小团队进入小众的实体印刷业务，还让美国邮政改变了其扫描流程，这生动展现了早期 iPhone 时代苹果对合作伙伴和第三方开发者所拥有的巨大影响力。 该应用提供横跨六个类别、约 21 款模板设计，可将 iPhone 拍摄的照片与实体卡片结合，并采用“轻触压印”（kiss impression）的凸版印刷方式而非深压凹；追踪条码被喷涂在信封上，仅在特定紫外光下可见，从而使信封表面保持干净无痕。

hackernews · ksec · 9月26日 09:13 · [社区讨论](https://news.ycombinator.com/item?id=49854693)

**背景**: Cards 是苹果随 iOS 5 于 2011 年一同推出的应用，用户可在 iPhone 上设计实体贺卡，随后由苹果代为印刷并寄出。尽管名称相似，它与后来推出的 Apple Card 信用卡毫无关系。实体邮件的追踪通常依赖印在信封上的可见条码，而凸版印刷传统上采用轻压的“轻触压印”，把油墨铺在纸面上而不会深压入纸。在苹果社区的行话中，某个产品被“Sherlocked”（被 Sherlock 掉）意味着苹果把第三方应用的功能吸收进了自家操作系统或第一方应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apple.fandom.com/wiki/Cards">Cards | Apple Wiki | Fandom</a></li>
<li><a href="https://www.usps.com/">Welcome | USPS</a></li>

</ul>
</details>

**社区讨论**: 评论区的亲身经历为文章增色不少：Sincerely 联合创始人 solfox 回忆称，当年 Cards 主题演讲播出时他感到自己“被 Sherlocked 了”，因为其团队的 Postagram 和 Sincerely Ink 早已实现从 iPhone 照片寄出印刷卡片；也有人指出创始人主导式产品开发不那么光鲜的一面（许多人为注定无法落地的点子熬夜苦干），有人对 USPS 隐形条码的细节表示赞赏，还有人称赞 Cards 是一种把随手拍的照片寄给不上网的年长亲属的、毫无摩擦的完美方式。

**标签**: `#Apple`, `#product-history`, `#printing`, `#entrepreneurship`, `#HN-discussion`

---

<a id="item-5"></a>
## [程序员热议：在大模型时代如何继续享受编程](https://discourse.haskell.org/t/how-to-keep-enjoying-programming-in-a-world-of-llms/14705) ⭐️ 7.0/10

一个 Hacker News 讨论帖（153 分、208 条评论）同时在 Haskell Discourse 论坛上出现，程序员们围绕在大语言模型（LLM）越来越替代人写代码的背景下，是否还能以及如何继续享受编程这门手艺展开辩论。参与者分享了各自关于技能退化、"技能表达" 丧失，以及把 AI 当作协作者而非替代者从而重拾乐趣的亲身经历。 这场讨论折射出越来越多开发者的身份危机——他们的手艺感、专业能力认同和职业满足感都与亲手写代码紧密相连；这可能影响团队、教育机构和工具厂商如何看待 AI 辅助开发。它说明 LLM 的价值不仅是生产力问题，还关乎整个行业的动力、学习与长期技能培养。 有评论者指出，把任何任务交给 LLM 往往会导致对应的人类技能退化，因此一些人刻意不向 AI 求助，以保护自己解决问题的能力。也有人报告了相反的效果，称 LLM 降低了摩擦，让他们能在几小时内从零上手不熟悉的语言和技术栈；整场讨论没有数据支撑，只有个人经验与类比。

hackernews · signa11 · 9月26日 09:41 · [社区讨论](https://news.ycombinator.com/item?id=49854875)

**背景**: GitHub Copilot、ChatGPT、Claude 等基于 LLM 的编程助手能够根据自然语言提示生成可运行的代码，过去几年里已在专业软件开发中被广泛采用。Hacker News 是知名的技术论坛，开发者经常在此讨论行业趋势，这条帖子也被转到了 Haskell 社区的 Discourse 论坛。这场辩论与制造业和自动化领域的老问题相呼应：当工具承担了手艺的一部分工作，从业者可能既失去技能，也失去它带来的满足感。

**社区讨论**: 整体情绪是复杂而自省的，而非敌意：有评论者把这一转变比作仍喜欢用手工工具鼓捣汽车的爱好者，另一位则用 "流水线厨师被微波炉取代" 的比喻来形容技能表达的丧失。一些开发者表示会刻意抵制 LLM 的帮助以避免技能退化，另一些人则说 LLM 通过降低摩擦、代劳枯燥的 "破事" 让编程更有乐趣，还有人指出自己在 LLM 出现之前早就讨厌这份工作了。

**标签**: `#LLMs`, `#developer-experience`, `#AI-assisted-coding`, `#programming-culture`, `#software-craft`

---

<a id="item-6"></a>
## [Conversations 开发者与 Google Play 分道扬镳，XMPP 应用转为免费](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 7.0/10

Android 平台 XMPP 客户端 Conversations 的开发者 Daniel Gultsch 发布文章，说明了该应用为何改为免费，以及为何要撤离 Google Play 商店。这一声明在社区论坛引发广泛讨论，标志着知名开源 Android 应用与 Google 应用分发平台之间的一次公开决裂。 这为长期以来针对 Google Play 抽成、审查流程不透明以及开发者支持薄弱的批评增添了一个有分量的开发者声音，也表明部分开源维护者正转向直接分发或替代渠道。该讨论还触及更广泛的应用商店“守门人”问题，以及 Google 对 Android 用户安装软件方式日益收紧的控制。 Conversations 是一款面向 Android 6.0 及以上版本的开源 Jabber/XMPP 客户端，此前在 Google Play 上为付费应用，如今改为免费并在该渠道之外提供。其核心不满并不在于 Google 的抽成本身，而在于开发者为此换来的糟糕支持以及缓慢、不透明的审核流程。

hackernews · ezst · 9月26日 10:55 · [社区讨论](https://news.ycombinator.com/item?id=49855315)

**背景**: Conversations 是一款基于 XMPP（可扩展消息与在线状态协议）的即时通讯客户端。XMPP 是一种开放的联邦式标准，最初名为 Jabber，任何人都可以自建服务器，不同服务器上的用户之间可以互通，运作方式很像电子邮件。与 WhatsApp 等中心化服务不同，XMPP 不绑定任何单一厂商的基础设施，因此该客户端可以脱离专有商店独立分发。Google Play 是 Google 官方的 Android 应用商店，开发者通常需支付 15% 至 30% 的抽成，并通过账号与商业资质验证；而在现代 Android 版本中，从商店之外安装的应用会触发安全警告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conversations_(software)">Conversations (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/XMPP">XMPP - Wikipedia</a></li>
<li><a href="https://conversations.im/">Conversations : the very last word in instant messaging</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为，真正的问题在于 Google 糟糕而缺乏人情味的开发者支持，而非抽成本身；有人指出，如果审核和反馈足够快速有用，开发者会乐意缴纳这笔费用，而 Google 之所以能如此行事，靠的正是垄断地位。不少人分享了自己的遭遇：一位开发者称因 Google 的电话验证环节假定开发者都是个人或小团队，导致其产品一年都无法上架；还有人认为 Play 已从对爱好者友好的空间变成官僚化的“真正的商业平台”，并逐步打压侧载。此外，评论中也普遍表达了对 Conversations 及其开发者的赞赏。

**标签**: `#Google Play`, `#app stores`, `#open source`, `#Android`, `#monopoly`

---

