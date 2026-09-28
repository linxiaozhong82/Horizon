# Horizon 每日速递 - 2026-09-28

> 从 34 条内容中筛选出 7 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：Google Search、llm、LLM、AI Overviews、model-release。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[一篇追问“Google 何时变得如此怪异”的文章引发 AI 搜索大讨论](https://sancho.bearblog.dev/google-weird/)**
2. **[Fireworks AI 发布首个自研研究模型 Ember-1](https://fireworks.ai/blog/ember-1)**
3. **[Sebastian Raschka：应投资于对开源权重模型的后训练](https://sebastianraschka.com/blog/2026/focusing-on-llm-post-training.html)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [Simon Willison 的 2026 年 LLM 主题演讲梳理全年 AI 进展](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. 算力芯片与服务器

- **关联热点**: [Simon Willison 的 2026 年 LLM 主题演讲梳理全年 AI 进展](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：一篇追问“Google 何时变得如此怪异”的文章引发 AI 搜索大讨论

**关联新闻**: [一篇追问“Google 何时变得如此怪异”的文章引发 AI 搜索大讨论](https://sancho.bearblog.dev/google-weird/)

**切入角度**: 一篇题为《Google 何时变得如此怪异？》的短文质疑如今使用 Google 搜索的体验越来越奇怪，登上了 Hacker News 首页，获得 752 分和 402 条评论。讨论很快聚焦于 AI Overviews、模型幻觉式回答，以及用户到底是否想要一个对话式助手而不是一串链接。 Google 搜索仍是数十亿人进入互联网的默认入口，因此它呈现答案的方式直接决定了用户看到什么信息、哪些网站能获得流量。这场争论折射出整个行业正在发生的转变：AI 生成的摘要正在取代传统的蓝色链接，引发对准确性、来源归属以及开放网络生态健康的担忧。 Google 的 AI Overviews 功能于 2024 年 5 月在美国上线，到 2024 年 10 月已推广至全球，Google 称其用户已超过十亿。该功能因不准确和幻觉问题屡遭批评，用户无法选择关闭，而 2025 年 6 月的一项研究发现，它引用最多的来源是 Quora 和 Reddit，而非权威的参考资料网站。

**可延展方向**: AI Overviews 是置于 Google 搜索结果最顶部的 AI 生成答案块，由 Google DeepMind 的 Gemini 系列大语言模型生成，目的是提供一份带有延伸链接的快速信息摘要。在这个语境下，“幻觉”指的是大语言模型生成的内容把虚假或误导性信息当作事实陈述出来，比如一个语气笃定却错误的答案，或一条凭空捏造的引用。由于这类系统是通过模式补全来生成听起来合理的文本，而不是检索经过验证的事实，因此在用户最信任它的日常问答场景中，反而可能最不可靠。

---

### 选题 2：Fireworks AI 发布首个自研研究模型 Ember-1

**关联新闻**: [Fireworks AI 发布首个自研研究模型 Ember-1](https://fireworks.ai/blog/ember-1)

**切入角度**: Fireworks AI 发布了 Ember-1，这是由其新成立的 Fireworks Research 团队打造的首个自研研究模型。Ember-1 是在 Kimi K3 基础上进行后训练得到的衍生模型，目标是在保持 K3 水平质量的同时将推理 token 减少约 40%，其中一个编码任务场景显示推理 token 减少了 71.3%，而质量评分保持不变。 这标志着这家原本被视为中立开源权重模型托管方的推理服务商发生了战略转向，开始推出自家模型。这引发了关于服务商信任和商业模式一致性的疑问：依赖 Fireworks 来部署他人开源模型的客户可能担心存在利益冲突；同时更廉价的推理也改变了它与 Kimi K3 等竞争对手在价格与质量上的对比格局。 Ember-1 并非全新的前沿基础模型，而是对 Kimi K3 进行后训练、使其跳过不必要的推理同时保留关键思考过程的产物；Fireworks 通过外部基准测试、真实客户 A/B 测试以及自家的编码和智能体工作负载对其进行了验证。该模型于 2026 年 9 月 23 日发布，并被视为 Fireworks Research 新模型系列的开端。

**可延展方向**: Fireworks AI 是一家美国 AI 基础设施公司，由前 Meta 工程师于 2022 年创立，专注于快速、低成本的推理服务，主要托管 Llama、DeepSeek、Qwen、Mixtral 等开源模型。Kimi K3 是一款强大的前沿开源权重模型，而"推理 token"指的是推理模型在给出答案前生成的中间思考步骤。减少这些 token 可以降低成本和延迟，同时不一定会损害答案质量。

---

### 选题 3：Sebastian Raschka：应投资于对开源权重模型的后训练

**关联新闻**: [Sebastian Raschka：应投资于对开源权重模型的后训练](https://sebastianraschka.com/blog/2026/focusing-on-llm-post-training.html)

**切入角度**: Sebastian Raschka 发表博文，主张与其从零开始构建新模型，不如投资于对现有开源权重 LLM 进行后训练，认为这是更高效的路径。他以 Fireworks 的专用推理模型 Ember-1 为例，说明何为更节省 token 的推理。 对大多数团队而言，对现有开源权重模型做后训练远比预训练一个前沿模型便宜，因此这一观点指出了有限算力与工程预算最该花在哪里。这也反映了更广泛的行业趋势：衡量推理质量不再只看基准分数，还要看模型为此消耗了多少 token。 Ember-1 基于 Kimi K3 构建，据称在保持相当质量的同时生成更短的推理链，token 用量减少约 40%。推理链更短意味着推理成本和延迟更低，而这往往是已部署推理模型的主要成本来源。

**可延展方向**: 后训练（post-training）指大语言模型在完成初始大规模预训练之后所经历的训练阶段，通常包括监督微调（指令微调）、RLHF 与 DPO 等基于偏好的对齐方法，以及近年来兴起的以推理能力为目标的强化学习。开源权重模型是指训练后的参数被公开发布、可供他人微调或改造的模型，而不只是通过 API 访问。节省 token 的推理是一个活跃的研究方向，目标是避免推理模型生成过长的思维链——即使最终答案正确，过长的推理过程也会推高成本。

---

1. [Simon Willison 的 2026 年 LLM 主题演讲梳理全年 AI 进展](#item-1) ⭐️ 8.0/10
2. [一篇追问“Google 何时变得如此怪异”的文章引发 AI 搜索大讨论](#item-2) ⭐️ 7.0/10
3. [Fireworks AI 发布首个自研研究模型 Ember-1](#item-3) ⭐️ 7.0/10
4. [Sebastian Raschka：应投资于对开源权重模型的后训练](#item-4) ⭐️ 7.0/10
5. [Naive.ai 开源 309B MoE 模型 Naive-N0.5-Flash，原生支持 1M 上下文](#item-5) ⭐️ 7.0/10
6. [177B MoE 模型从 SSD 流式加载，在 16GB RTX 5060 Ti 上跑到 9-10 tok/s](#item-6) ⭐️ 7.0/10
7. [17 岁开发者优化 CUDA 内核，双 Tesla P100 跑出 60tps](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Simon Willison 的 2026 年 LLM 主题演讲梳理全年 AI 进展](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/) ⭐️ 8.0/10

2026 年 9 月 25 日，Simon Willison 在圣何塞举行的 WeAreDevelopers World Congress North America 上发表了闭幕主题演讲，并于 9 月 27 日发布了带注释的幻灯片、讲稿以及 YouTube 视频。这场演讲按时间顺序梳理了 2026 年迄今为止 LLM 领域发生的所有大事，起点是他所称的 2025 年 11 月转折点——Claude Opus 4.5 和 GPT-5.1 的发布。 Willison 是大型语言模型领域读者最多的独立分析师之一，因此这种按时间顺序整理的年终综述，对开发者判断哪些进展是真正的转折点、哪些只是常规迭代升级，具有重要的参考价值。他提出的核心观点——编码智能体已从“经常出错”跨越到“可靠到可以日常使用”——是关于 AI 辅助软件开发实际成熟度的一个重要判断。 Willison 认为，2025 年 11 月发布的 Claude Opus 4.5 和 GPT-5.1 单看只是模型的渐进式改进，但与各自的编码智能体框架结合后，它们跨过了一条无形的可靠性门槛；Claude Code 自 2025 年 2 月起就已存在，Codex 则稍晚一些。他仍在使用那个刻意搞笑的“生成一只骑自行车的鹈鹕的 SVG”基准测试，并指出截至 2025 年 11 月，Claude 依然画不出像样的自行车，GPT-5.1 的车架也“相当糟糕”；他还强调这一年尚未结束，因此这份回顾本身仍不完整。

rss · Simon Willison · 9月27日 23:54

**背景**: Simon Willison 是 Django Web 框架和 Datasette 数据工具的创造者，他的博客已成为对新语言模型进行实测分析时被广泛引用的来源。在此语境下，“编码智能体”或“框架（harness）”指的是 Claude Code 和 OpenAI 的 Codex 这类工具，它们能让模型自主读取文件、执行命令并修改代码，而不只是在聊天窗口里回答问题。“画一只骑自行车的鹈鹕”的 SVG 提示词是 Willison 长期使用的一种非正式基准，因为它能在一个快速、可肉眼验证的任务中同时考察模型的绘图能力、空间推理能力和指令遵循能力。

**标签**: `#LLMs`, `#AI`, `#Simon Willison`, `#keynote`, `#trends`

---

<a id="item-2"></a>
## [一篇追问“Google 何时变得如此怪异”的文章引发 AI 搜索大讨论](https://sancho.bearblog.dev/google-weird/) ⭐️ 7.0/10

一篇题为《Google 何时变得如此怪异？》的短文质疑如今使用 Google 搜索的体验越来越奇怪，登上了 Hacker News 首页，获得 752 分和 402 条评论。讨论很快聚焦于 AI Overviews、模型幻觉式回答，以及用户到底是否想要一个对话式助手而不是一串链接。 Google 搜索仍是数十亿人进入互联网的默认入口，因此它呈现答案的方式直接决定了用户看到什么信息、哪些网站能获得流量。这场争论折射出整个行业正在发生的转变：AI 生成的摘要正在取代传统的蓝色链接，引发对准确性、来源归属以及开放网络生态健康的担忧。 Google 的 AI Overviews 功能于 2024 年 5 月在美国上线，到 2024 年 10 月已推广至全球，Google 称其用户已超过十亿。该功能因不准确和幻觉问题屡遭批评，用户无法选择关闭，而 2025 年 6 月的一项研究发现，它引用最多的来源是 Quora 和 Reddit，而非权威的参考资料网站。

hackernews · sancho-panza · 9月27日 20:12 · [社区讨论](https://news.ycombinator.com/item?id=49870367)

**背景**: AI Overviews 是置于 Google 搜索结果最顶部的 AI 生成答案块，由 Google DeepMind 的 Gemini 系列大语言模型生成，目的是提供一份带有延伸链接的快速信息摘要。在这个语境下，“幻觉”指的是大语言模型生成的内容把虚假或误导性信息当作事实陈述出来，比如一个语气笃定却错误的答案，或一条凭空捏造的引用。由于这类系统是通过模式补全来生成听起来合理的文本，而不是检索经过验证的事实，因此在用户最信任它的日常问答场景中，反而可能最不可靠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews</a></li>
<li><a href="https://en.wikipedia.org/wiki/LLM_hallucination">LLM hallucination</a></li>
<li><a href="https://blog.google/products-and-platforms/products/search/ai-mode-search/">Expanding AI Overviews and introducing AI Mode</a></li>

</ul>
</details>

**社区讨论**: 评论区观点明显分裂：一派认为普通用户一直就想要“电脑里有个小人”可以对话，AI Overviews 是巨大的体验提升，也是 Google 的一次产品胜利；另一派则觉得这一趋势令人不安。有用户举出具体的幻觉案例——询问哈利法克斯流浪者队是否还有机会进入 CPL 季后赛，却被告知该队已锁定季后赛席位——还有评论者把这一功能形容为对孤独感和拟社交依赖的变现，并呼吁人们去问身边真实的朋友。

**标签**: `#Google Search`, `#AI Overviews`, `#LLM Hallucination`, `#Search Quality`, `#Hacker News`

---

<a id="item-3"></a>
## [Fireworks AI 发布首个自研研究模型 Ember-1](https://fireworks.ai/blog/ember-1) ⭐️ 7.0/10

Fireworks AI 发布了 Ember-1，这是由其新成立的 Fireworks Research 团队打造的首个自研研究模型。Ember-1 是在 Kimi K3 基础上进行后训练得到的衍生模型，目标是在保持 K3 水平质量的同时将推理 token 减少约 40%，其中一个编码任务场景显示推理 token 减少了 71.3%，而质量评分保持不变。 这标志着这家原本被视为中立开源权重模型托管方的推理服务商发生了战略转向，开始推出自家模型。这引发了关于服务商信任和商业模式一致性的疑问：依赖 Fireworks 来部署他人开源模型的客户可能担心存在利益冲突；同时更廉价的推理也改变了它与 Kimi K3 等竞争对手在价格与质量上的对比格局。 Ember-1 并非全新的前沿基础模型，而是对 Kimi K3 进行后训练、使其跳过不必要的推理同时保留关键思考过程的产物；Fireworks 通过外部基准测试、真实客户 A/B 测试以及自家的编码和智能体工作负载对其进行了验证。该模型于 2026 年 9 月 23 日发布，并被视为 Fireworks Research 新模型系列的开端。

hackernews · gmays · 9月27日 17:31 · [社区讨论](https://news.ycombinator.com/item?id=49868830)

**背景**: Fireworks AI 是一家美国 AI 基础设施公司，由前 Meta 工程师于 2022 年创立，专注于快速、低成本的推理服务，主要托管 Llama、DeepSeek、Qwen、Mixtral 等开源模型。Kimi K3 是一款强大的前沿开源权重模型，而"推理 token"指的是推理模型在给出答案前生成的中间思考步骤。减少这些 token 可以降低成本和延迟，同时不一定会损害答案质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fireworks.ai/blog/ember-1">Introducing Ember-1 - fireworks.ai</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fireworks_AI">Fireworks AI</a></li>
<li><a href="https://www.explainx.ai/blog/fireworks-ember-1-kimi-k3-reasoning-tokens-2026">Ember-1: 71% Fewer Reasoning Tokens at K3 Price (2026 ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对开放模型的进展速度持乐观态度，有人表示这是在 CPU 上成功微调小型 Qwen 0.6B 模型用于英文转 Bash 翻译后迎来的模型训练黄金时代。担忧主要集中在服务商信任问题上：多位用户指出，他们选择 Fireworks 正是因为它中立地托管 DeepSeek 等开源模型，如今它推出自家竞品令人不安。还有人讨论定价问题，认为 Kimi K3 相对 Sol 等更便宜的方案性价比已下降，并争论开放模型是否会像 Linux 和 Wikipedia 那样持续超越专有模型。

**标签**: `#llm`, `#model-release`, `#fireworks-ai`, `#open-models`, `#inference-providers`

---

<a id="item-4"></a>
## [Sebastian Raschka：应投资于对开源权重模型的后训练](https://sebastianraschka.com/blog/2026/focusing-on-llm-post-training.html) ⭐️ 7.0/10

Sebastian Raschka 发表博文，主张与其从零开始构建新模型，不如投资于对现有开源权重 LLM 进行后训练，认为这是更高效的路径。他以 Fireworks 的专用推理模型 Ember-1 为例，说明何为更节省 token 的推理。 对大多数团队而言，对现有开源权重模型做后训练远比预训练一个前沿模型便宜，因此这一观点指出了有限算力与工程预算最该花在哪里。这也反映了更广泛的行业趋势：衡量推理质量不再只看基准分数，还要看模型为此消耗了多少 token。 Ember-1 基于 Kimi K3 构建，据称在保持相当质量的同时生成更短的推理链，token 用量减少约 40%。推理链更短意味着推理成本和延迟更低，而这往往是已部署推理模型的主要成本来源。

rss · Sebastian Raschka · 9月27日 22:12

**背景**: 后训练（post-training）指大语言模型在完成初始大规模预训练之后所经历的训练阶段，通常包括监督微调（指令微调）、RLHF 与 DPO 等基于偏好的对齐方法，以及近年来兴起的以推理能力为目标的强化学习。开源权重模型是指训练后的参数被公开发布、可供他人微调或改造的模型，而不只是通过 API 访问。节省 token 的推理是一个活跃的研究方向，目标是避免推理模型生成过长的思维链——即使最终答案正确，过长的推理过程也会推高成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fireworks.ai/blog/ember-1">Introducing Ember-1</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-training_of_large_language_models">Post-training of large language models</a></li>
<li><a href="https://arxiv.org/pdf/2503.16419">Stop Overthinking: A Survey on Efficient Reasoning for Large...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#post-training`, `#fine-tuning`, `#reasoning`, `#open-weight-models`

---

<a id="item-5"></a>
## [Naive.ai 开源 309B MoE 模型 Naive-N0.5-Flash，原生支持 1M 上下文](https://www.reddit.com/r/LocalLLaMA/comments/1wrs58t/naiven05flash_309ba155b/) ⭐️ 7.0/10

Naive.ai 发布了 Naive-N0.5-Flash，这是一个 309B 参数的开源 MoE（混合专家）模型，每个 token 大约激活 15.5B 参数，原生支持 1M token 上下文窗口，主要面向编程与 AI 研发场景。该模型采用 SWA/DSA 混合注意力架构，也就是说它并非依赖传统的全注意力机制来实现长上下文。 这为开源模型阵营再添一个前沿规模的 MoE，目前 300B 级别稀疏模型搭配百万 token 上下文正逐渐成为竞争标配；而其“无全注意力”的设计则反映出整个行业正在向更低成本的长上下文推理演进。如果权重确实完全开放，它将为 LocalLLaMA 社区提供一个体量庞大、偏重代码能力、且推理算力需求远低于同等总参数稠密模型的选项。 根据对该模型卡片的报道，其训练使用了 3.25T token、原生 1M token 上下文，并以小米开源的 MiMo-V2.5 为基座：先进行 50B token 的 indexer 预热，再做 3T token 的稀疏注意力训练，最后进行 200B token 的学习率衰减。值得注意的是，最初的发布贴本身极为简略，没有给出基准测试、许可证条款或硬件需求，因此大部分具体规格来自二手报道而非官方发布内容。

reddit · r/LocalLLaMA · /u/nullmove · 9月27日 18:48

**背景**: 混合专家（MoE）模型会把前馈层拆分成许多独立的“专家”子网络，每个 token 只激活其中一小部分专家，因此模型可以在拥有极大总参数量的同时，每个 token 的计算量却小得多——“总参数 309B、激活 15.5B”正是这一区别的体现。上下文窗口指的是模型一次能关注多少 token，1M token 的窗口大致足以一次性吞下相当规模的代码仓库，这正是它对编程智能体重要的原因。标准的全注意力计算量随序列长度呈平方级增长，因此像 SWA（滑动窗口注意力，只关注邻近 token）配合 DSA 这类稀疏注意力变体的混合设计，可以显著降低长上下文推理的开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/naiveai-open-weights-309b-naive-n05-flash-with-no-full-attention">NaiveAI Open-Weights 309B Naive-N0.5-Flash With No Full Attention</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://cameronrwolfe.substack.com/p/moe-llms">Mixture-of-Experts (MoE) LLMs - by Cameron R. Wolfe, Ph.D.</a></li>

</ul>
</details>

**标签**: `#LLM`, `#MoE`, `#long-context`, `#coding`, `#LocalLLaMA`

---

<a id="item-6"></a>
## [177B MoE 模型从 SSD 流式加载，在 16GB RTX 5060 Ti 上跑到 9-10 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1wrxap8/qwen38flashnext_177b_nvfp4119gib_ssd_streaming_at/) ⭐️ 7.0/10

一位开发者发布了一个概念验证性质的推理引擎（Inferred Thoughts），在单张 16GB RTX 5060 Ti、32GB DDR5 内存和一块 Gen5 NVMe SSD 上，运行量化为 NVFP4 GGUF（119 GiB）的 176.9B 参数 MoE 模型 Qwen3.8-Flash-Next，基准轮解码速度为 9.06 tok/s，最佳轮达到 10.4 tok/s。该引擎将大部分权重留在 SSD 上，仅在路由器选中专家时才把对应专家读入内存，而同一台机器上 llama.cpp 的平均解码速度仅为 4.9 tok/s。 它表明，消费级单卡机器可以通过把 NVMe SSD 当作第三级内存，运行远超其显存与内存总容量的前沿规模 MoE 模型。这对一直尝试在普通硬件上跑越来越大开源模型的本地推理社区很有意义，同时也暗示通过改进流式加载，v2 有望进一步提升到约 14-15 tok/s。 在 119 GiB 的模型中，约 20 GiB 驻留内存（4.4 GiB 稠密权重加 8.8 GiB 最热专家放在显存，6.0 GiB 次热专家放在锁页内存，0.6 GiB 词元嵌入表），其余 99 GiB 留在 SSD 上，其中包括 48.5 GiB 的路由专家和一个 50.7 GiB 的哈希 n-gram 表（每个词元读取 16 行）。每个词元激活 480 个专家（48 层各 10 个），其中约 377 个已在显存或内存中，约 103 个从 SSD 读取，每词元约读 270 MiB，专家命中率约 75%；已知限制包括仅支持 Blackwell sm_120、仅限 Windows 11/WSL2、仅支持贪婪解码，长时间运行时 SSD 温度可达 70°C（只读为主，因此写入磨损很小）。

reddit · r/LocalLLaMA · /u/TypicalPudding6190 · 9月27日 22:13

**背景**: 混合专家（MoE）模型包含许多独立的专家子网络，但每个词元只经过其中一小部分，因此未被使用的权重原则上可以存放在更慢、更便宜的存储上并按需读取。NVFP4 是 NVIDIA 为 Blackwell 代际张量核心设计的 4 位浮点量化格式，能让大模型大幅压缩而精度损失很小；GGUF 则是由 llama.cpp 推广的二进制模型文件格式，便于高效加载和量化存储。SSD 流式加载是一种新兴技术（如 oLLM 等项目采用），它把高速 NVMe 存储当作显存/内存的扩展，使大于机器内存的模型也能在本地运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>
<li><a href="https://www.blog.brightcoding.dev/2026/04/07/ollm-run-80b-models-on-8gb-vram">oLLM: Run 80B Models on 8GB VRAM - BrightCoding</a></li>
<li><a href="https://huggingface.co/docs/hub/gguf">GGUF · Hugging Face</a></li>

</ul>
</details>

**标签**: `#local-llm-inference`, `#mixture-of-experts`, `#ssd-offloading`, `#quantization`, `#consumer-gpu`

---

<a id="item-7"></a>
## [17 岁开发者优化 CUDA 内核，双 Tesla P100 跑出 60tps](https://www.reddit.com/r/LocalLLaMA/comments/1wrv2l3/2x_tesla_p100s_q6_k_quant_qwen_38_27b_60tps_v30/) ⭐️ 7.0/10

一位 17 岁开发者（Reddit 用户 /u/Kmic68）发布了一个针对 Tesla P100 做内核优化的 llama.cpp 分支，使 q6_k 量化下的 Qwen 3.8 27B 推理在零上下文时从约 7–15 tps 提升到 50–60 tps，在 260k 上下文时从 2–4 tps 提升到 30–35 tps。该工作还把零上下文 prefill 从约 220 tps 提升到约 350 tps，260k 上下文下提升到约 110 tps，并通过混合 FP16/FP32 运算修复了 FP16 舍入误差。 这说明像基于 Pascal 架构的 Tesla P100 这样已有十年、价格极低的二手数据中心 GPU，通过有针对性的内核优化后，仍能胜任大模型的本地推理，为爱好者提供了不到 200 美元就能以交互速度运行 27B 级模型的方案。这也反映出 LocalLLaMA 社区越来越把量化和手工调优内核，而非购买新硬件，视为压榨老卡性能的主要手段。 这些提升对启动参数很敏感：作者推荐使用 `-c 262144 -b 32768 -ub 1024 -np 1`，并指出若不加 `-b 32768`，在满上下文深度下 MTP 接受率会跌到接近零。他的数据是在显卡功耗被限制在 175W/250W、79°C 轻微热降频、PCIe Gen3 x16 插槽的条件下测得的，因此他估计若散热更好，prefill 与 decode 吞吐还能再提高 5–10%；相关改动已于 9 月 22 日合入，并支持 Qwen 3.8 flash 架构。

reddit · r/LocalLLaMA · /u/Kmic68 · 9月27日 20:42

**背景**: Tesla P100 是 NVIDIA 于 2016 年推出的 Pascal 架构数据中心加速卡，配备 16GB HBM2 显存，且没有张量核心，因此如今在二手市场上只卖约 80 美元，且现代推理软件对它的支持很差。LLM 推理分为两个不同阶段——prefill（一次性处理整个提示词）和 decode（逐个生成 token），两者的瓶颈各不相同，这也是该项目分别给出两组数据的原因。q6_k 是 llama.cpp 的一种量化格式，每个权重约 6.6 比特并采用分块缩放，介于更小的 4 比特量化与近乎无损的 8 比特量化之间，是折中的选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sitepoint.com/q4-vs-q6-vs-q8-quantization-local-llms/">Q4 vs Q6 vs Q8: The Quantization Decision Framework for Local LLMs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nvidia_Tesla">Nvidia Tesla - Wikipedia</a></li>
<li><a href="https://www.parasail.io/blog/prefill-vs-decode-llm-inference">Prefill vs . decode in LLM inference — Parasail</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#CUDA kernels`, `#GPU optimization`, `#quantization`, `#LocalLLaMA`

---

