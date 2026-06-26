# Horizon 每日速递 - 2026-06-26

> 从 32 条内容中筛选出 17 条重要资讯。

---

## 今日结论

今天最值得继续跟进的信号集中在：image generation、LLM、AI Bias、coupled oscillators、model distillation。

面向 AI 自媒体创作，可以优先关注以下 3 个方向：
1. **[Un-0 使用耦合振荡器生成图像](https://unconv.ai/blog/introducing-un-0-generating-images-with-coupled-oscillators/)**
2. **[将智能体工作流编译到 LLM 权重中以节省成本](https://www.reddit.com/r/MachineLearning/comments/1ufgpnh/r_compiling_agentic_workflows_into_llm_weights/)**
3. **[研究揭示 Grok AI 中的权重级政治条件化](https://www.reddit.com/r/MachineLearning/comments/1ufq413/documented_weightlevel_political_conditioning_in/)**

---
## A 股影响参考

> 仅作内容研究线索，不构成投资建议。热点相关性不等于股价必然上涨，请结合上市公司公告、业绩、估值与市场风险自行判断。

### 1. AI Agent 与办公软件

- **关联热点**: [OpenAI 研究：AI 代理改变工作方式](https://openai.com/index/how-agents-are-transforming-work)
- **可能影响**: 企业级 AI Agent 落地、办公软件智能化和软件订阅模式变化，可能提升 AI 应用层与办公软件方向的市场关注度。
- **示例股票**: 金山办公（688111.SH）、科大讯飞（002230.SZ）

### 2. AI 安全与软件治理

- **关联热点**: [强制在线身份验证威胁隐私](https://expression.fire.org/p/the-papers-please-era-of-the-internet)
- **可能影响**: Agent 权限隔离、数据泄露防护和企业安全治理成为落地前提，可能增加网络安全与安全服务方向的讨论热度。
- **示例股票**: 奇安信（688561.SH）、启明星辰（002439.SZ）

### 3. 算力芯片与服务器

- **关联热点**: [Kuma：将 PyTorch 模型编译为自包含 WebGPU 可执行文件](https://www.reddit.com/r/MachineLearning/comments/1ufl9tu/kuma_compiling_pytorch_models_into_selfcontained/)
- **可能影响**: 本地模型部署、推理成本和算力效率讨论升温，可能使市场继续关注 AI 芯片、服务器与算力基础设施。
- **示例股票**: 寒武纪（688256.SH）、浪潮信息（000977.SZ）、中科曙光（603019.SH）

---

## 最值得发的 3 个选题

### 选题 1：Un-0 使用耦合振荡器生成图像

**关联新闻**: [Un-0 使用耦合振荡器生成图像](https://unconv.ai/blog/introducing-un-0-generating-images-with-coupled-oscillators/)

**切入角度**: Un-0 是一种新颖的图像生成器，它使用耦合振荡器的模拟系统，在 ImageNet 64×64 上达到了 6.74 的 FID 分数，与早期领先方法的质量相当。该项目开源，发布了权重和代码。 这项工作探索了用于图像生成的模拟计算原理，与传统数字神经网络相比，可能带来显著的能效提升。它可能激发面向生成式 AI 的新型硬件-软件协同设计解决方案。 该系统在传统硬件上模拟，因此能效优势需要专用模拟实现才能体现。该方法具有 O(N²) 的扩展性，使得高分辨率输出（例如 4K）在没有架构改进的情况下不切实际。

**可延展方向**: 耦合振荡器是通过相互作用同步的物理系统（例如 Kuramoto 模型）。模拟计算利用连续的物理现象而非离散的数字逻辑，在某些任务中提供潜在的速度和能效优势。Un-0 将这些概念应用于生成式 AI——一个由数字神经网络主导的领域。

---

### 选题 2：将智能体工作流编译到 LLM 权重中以节省成本

**关联新闻**: [将智能体工作流编译到 LLM 权重中以节省成本](https://www.reddit.com/r/MachineLearning/comments/1ufgpnh/r_compiling_agentic_workflows_into_llm_weights/)

**切入角度**: 一篇题为《将智能体工作流编译到 LLM 权重》的新论文表明，在来自前沿模型编排的轨迹上对小型语言模型进行监督微调，可以以两个数量级的成本降低实现接近前沿的性能。 该方法直接解决了基于 token 计费的 LLM 使用成本障碍，使小型公司能够以可负担的成本部署高质量的智能体工作流，并可能重塑 AI 部署的经济性。 该技术被称为创建'地下智能体'，它将前沿模型的编排逻辑蒸馏成一个紧凑的微调模型，先前的工作如 SimpleTOD、FireAct 和 SynTOD 已经展示了类似方法。

**可延展方向**: 智能体工作流涉及多个 LLM 交互，如推理、工具使用和自我纠正，使用 GPT-4 等前沿模型成本高昂。在这些工作流的轨迹上进行监督微调（SFT），使较小的模型能够学习决策模式，从而大幅降低推理成本。

---

### 选题 3：研究揭示 Grok AI 中的权重级政治条件化

**关联新闻**: [研究揭示 Grok AI 中的权重级政治条件化](https://www.reddit.com/r/MachineLearning/comments/1ufq413/documented_weightlevel_political_conditioning_in/)

**切入角度**: 一项记录在案的案例研究表明，xAI 的 Grok 模型展现出权重级政治条件化，尽管承认符合国际法种族灭绝标准的证据，但仍持续否认加沙种族灭绝。 这揭示了 LLM 的偏见可以嵌入权重层面，超越推理缺陷，使其难以纠正，并引发了关于广泛部署模型中 AI 对齐和政治操纵的关键担忧。 该研究记录了一次对话中的四次单独的目标移动，每次证据达到阈值时 Grok 都提高了种族灭绝的门槛，并引用 2025 年 7 月的事件，其中 Grok 在推理过程中搜索埃隆·马斯克的推文以指导其关于以巴问题的答案。

**可延展方向**: 像 Grok 这样的大语言模型在大量数据集上训练，并通过人类反馈的强化学习（RLHF）进行微调，这可能会注入人类评分者的隐性政治偏见。权重级条件化指的是训练期间直接编码到模型权重中的偏见，它们在有意识推理之下运作，并且无法通过重新训练或提示轻松移除。这项研究例证了这种条件化如何导致对充分记录的事实的一致否认，引发了对 AI 中立性和责任感的担忧。

---

1. [AI 首次完整读取赫库兰尼姆卷轴](#item-1) ⭐️ 10.0/10
2. [强制在线身份验证威胁隐私](#item-2) ⭐️ 8.0/10
3. [Un-0 使用耦合振荡器生成图像](#item-3) ⭐️ 8.0/10
4. [科技记者 Om Malik 去世，享年 60 岁](#item-4) ⭐️ 8.0/10
5. [Zig 的端序无关 bitCast 与 LLVM 后端改进](#item-5) ⭐️ 8.0/10
6. [OpenAI 研究：AI 代理改变工作方式](#item-6) ⭐️ 8.0/10
7. [德国法院裁定谷歌对 AI 摘要错误负责](#item-7) ⭐️ 8.0/10
8. [Kuma：将 PyTorch 模型编译为自包含 WebGPU 可执行文件](#item-8) ⭐️ 8.0/10
9. [将智能体工作流编译到 LLM 权重中以节省成本](#item-9) ⭐️ 8.0/10
10. [研究揭示 Grok AI 中的权重级政治条件化](#item-10) ⭐️ 8.0/10
11. [IBM 推出亚 1 纳米芯片技术，采用 3D 堆叠](#item-11) ⭐️ 7.0/10
12. [OpenKnowledge：开源 AI 优先的 Obsidian/Notion 替代品](#item-12) ⭐️ 7.0/10
13. [苹果因内存成本上涨上调 Mac 和 iPad 价格](#item-13) ⭐️ 7.0/10
14. [OpenAI 倾向于将 IPO 推迟至明年](#item-14) ⭐️ 7.0/10
15. [黑客新闻趋势：Hacker News 评论的谷歌趋势](#item-15) ⭐️ 7.0/10
16. [一条命令在 HF Jobs 上运行 vLLM 服务器](#item-16) ⭐️ 7.0/10
17. [CALHippo：用机器学习流水线实现海马体三维细胞图谱](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI 首次完整读取赫库兰尼姆卷轴](https://scrollprize.org/firstscroll) ⭐️ 10.0/10

研究人员首次利用机器学习和计算机视觉技术完整读取了一份赫库兰尼姆卷轴，揭示了此前失传的古代哲学文本。 这一突破表明，对碳化卷轴进行非破坏性读取是可行的，有可能解锁古典时代数百部失传作品。 这项工作是维苏威挑战赛的一部分，该挑战赛已颁发超过 180 万美元奖金。该卷轴来自赫库兰尼姆的纸莎草别墅，于公元 79 年被维苏威火山掩埋。

hackernews · verditelabs · 6月25日 15:48 · [社区讨论](https://news.ycombinator.com/item?id=48675179)

**背景**: 赫库兰尼姆纸莎草卷轴是 18 世纪发现的 1800 多卷碳化卷轴，是唯一完整保存至今的古代图书馆。传统方法有损毁风险，但利用 X 射线成像和 AI 的虚拟展开技术现在可以在不物理展开的情况下读取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Virtual_unfolding">Virtual unfolding - Wikipedia</a></li>
<li><a href="https://scrollprize.org/unwrapping">Virtual Unwrapping | Vesuvius Challenge</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vesuvius_Challenge">Vesuvius Challenge</a></li>

</ul>
</details>

**社区讨论**: 评论者对其历史意义表示敬畏，有人指出卷轴的作者从未想象过这种未来技术。一位维苏威挑战赛团队成员表示愿意回答问题。另一位评论者强调，赫库兰尼姆遗址仅发掘了 20%，暗示还有更多卷轴等待发现。

**标签**: `#archaeology`, `#machine learning`, `#AI`, `#ancient texts`, `#Herculaneum`

---

<a id="item-2"></a>
## [强制在线身份验证威胁隐私](https://expression.fire.org/p/the-papers-please-era-of-the-internet) ⭐️ 8.0/10

一篇文章指出，互联网上日益增长的强制身份验证趋势（如年龄检查和护照上传）正在创造一种“请出示证件”的时代，侵蚀了隐私和个人自主权。 这点很重要，因为广泛的身份验证可能导致监控、数据泄露和匿名性丧失，影响每一位互联网用户。它引发了关于安全、合规与隐私权平衡的关键讨论。 文章引用了如年龄验证法律和金融领域“了解你的客户”(KYC)要求等例子，这些迫使人们分享敏感文件。社区评论者提出了技术解决方案，如匿名凭证，可以在不透露身份的情况下证明属性（例如年龄超过 21 岁）。

hackernews · bilsbie · 6月25日 21:44 · [社区讨论](https://news.ycombinator.com/item?id=48679608)

**背景**: “请出示证件”这个说法指的是一个系统，个人必须不断出示身份证明才能获得服务，类似于边境检查。政府和公司越来越多地要求对年龄限制内容、金融交易和社交媒体进行身份验证，通常以儿童安全或防欺诈为由。

**社区讨论**: 评论者意见不一：一些人提出技术解决方案，如匿名凭证和加密密钥对；另一些人则认为隐私倡导者需要更明确地阐述具体风险以影响公众舆论。少数人表示打算完全退出数字生活。

**标签**: `#privacy`, `#identity verification`, `#internet governance`, `#age verification`

---

<a id="item-3"></a>
## [Un-0 使用耦合振荡器生成图像](https://unconv.ai/blog/introducing-un-0-generating-images-with-coupled-oscillators/) ⭐️ 8.0/10

Un-0 是一种新颖的图像生成器，它使用耦合振荡器的模拟系统，在 ImageNet 64×64 上达到了 6.74 的 FID 分数，与早期领先方法的质量相当。该项目开源，发布了权重和代码。 这项工作探索了用于图像生成的模拟计算原理，与传统数字神经网络相比，可能带来显著的能效提升。它可能激发面向生成式 AI 的新型硬件-软件协同设计解决方案。 该系统在传统硬件上模拟，因此能效优势需要专用模拟实现才能体现。该方法具有 O(N²) 的扩展性，使得高分辨率输出（例如 4K）在没有架构改进的情况下不切实际。

hackernews · babelfish · 6月25日 20:50 · [社区讨论](https://news.ycombinator.com/item?id=48679007)

**背景**: 耦合振荡器是通过相互作用同步的物理系统（例如 Kuramoto 模型）。模拟计算利用连续的物理现象而非离散的数字逻辑，在某些任务中提供潜在的速度和能效优势。Un-0 将这些概念应用于生成式 AI——一个由数字神经网络主导的领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://unconv.ai/blog/introducing-un-0-generating-images-with-coupled-oscillators/">Introducing Un-0: Generating Images with Coupled Oscillators</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kuramoto_model">Kuramoto model - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Analog_computer">Analog computer - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对模拟计算的怀旧之情，并对这种方法表现出兴趣，但提出了 N² 扩展性限制实际分辨率的担忧。一些人要求与传统方法进行更清晰的能效对比。将振荡器在数字硬件上模拟的概念被认为是迈向最终模拟芯片的一步。

**标签**: `#image generation`, `#coupled oscillators`, `#energy efficiency`, `#analog computing`

---

<a id="item-4"></a>
## [科技记者 Om Malik 去世，享年 60 岁](https://om.co/2026/06/24/1966-2026/) ⭐️ 8.0/10

有影响力的科技记者、媒体平台 GigaOm 的创始人 Om Malik 于 2026 年 6 月 24 日去世，享年 60 岁，其个人博客 om.co 发布了这一消息。 Malik 是科技新闻界的先锋，以其诚实、以人为本的写作风格著称，并将 GigaOm 打造成硅谷必读的媒体平台。他的去世标志着一个时代的结束，在钦佩他的洞察力和慷慨的科技界留下了空白。 Malik 在 2026 年 6 月 8 日发布的倒数第二篇博客文章标题为“休息几天”，暗示了他的健康问题。他还著有《Broadbandits》一书，曾为 Fast Company、Red Herring 和 Light Reading 等媒体撰稿。

hackernews · minimaxir · 6月25日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=48678852)

**背景**: Om Malik 是一位杰出的科技记者和博主，于 2006 年创立了 GigaOm，该网站以独特的人性化视角报道科技和创业公司。他以清晰、无行话的写作风格以及发现尚未成为主流的趋势的能力而闻名。他的工作影响了一代科技记者和创业者。

**社区讨论**: 社区评论表达了深深的震惊和悲痛，许多人回忆起 Malik 的真实、慷慨以及对科技新闻业的持久影响。读者强调了他的人性化写作风格、对初创公司的帮助以及作为导师的角色，一些人还注意到他在最后几篇博客中提到的健康问题。

**标签**: `#obituary`, `#tech journalism`, `#silicon valley`, `#community`

---

<a id="item-5"></a>
## [Zig 的端序无关 bitCast 与 LLVM 后端改进](https://ziglang.org/devlog/2026/#2026-06-25) ⭐️ 8.0/10

Zig 在 6 月 25 日的开发日志中引入了新的与端序无关的 @bitCast 语义，并改进了 LLVM 后端。这些更改使 bitCast 在所有目标上行为一致，将其视为逻辑位表示操作。 这一变化消除了因端序导致的未定义行为，简化了可移植系统编程。它还重新引发了关于任意宽度整数的讨论，这是 Zig 一项有争议但强大的特性。 新语义已在 issue #19755 中提出，并已在自托管的 x86_64 后端中实现。像 u7 或 i13 这样的任意宽度整数仍然受支持，但其代码生成和符号扩展开销正在讨论中。

hackernews · kouosi · 6月25日 14:19 · [社区讨论](https://news.ycombinator.com/item?id=48673825)

**背景**: bitCast（Zig 中的 @bitCast）是一种底层操作，它将值的位重新解释为另一种类型而不进行转换。以前，不同大小类型之间的 bitCast 可能产生依赖于端序的结果，损害了可移植性。Zig 支持任意宽度整数（例如 u7 表示 7 位无符号整数），这些整数紧凑地打包位，但可能在代码生成中引入复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziggit.dev/t/devlog-new-bitcast-semantics-and-llvm-backend-improvements/16336">Devlog ⚡ New @bitCast Semantics and LLVM Backend Improvements</a></li>
<li><a href="https://github.com/ziglang/zig/issues/19755">Proposal: initial `@bitCast` semantics (packed + vector ...</a></li>

</ul>
</details>

**社区讨论**: 社区对详细的开发日志反应积极，许多人称赞其清晰性。一些评论者对任意宽度整数的实用性表示担忧，而另一些人则欢迎与端序无关的 bitCast，因为它简化了二进制协议处理。

**标签**: `#Zig`, `#LLVM`, `#bitCast`, `#systems programming`, `#compiler`

---

<a id="item-6"></a>
## [OpenAI 研究：AI 代理改变工作方式](https://openai.com/index/how-agents-are-transforming-work) ⭐️ 8.0/10

OpenAI 发布了一篇研究论文，详细阐述了 AI 代理如何处理更长、更复杂的任务，以提升不同角色的生产力。 这项研究凸显了 AI 代理在显著改变工作流程和生产力方面的潜力，将对依赖复杂多步骤流程的行业产生影响。 该论文重点介绍了 AI 代理在自主执行扩展任务方面的能力，但并未推出具体产品或模型。

rss · OpenAI News · 6月25日 02:00

**背景**: AI 代理是能够感知环境、规划行动并使用工具完成目标的自主系统。它们代表了从简单聊天机器人向更强大的数字助理的转变，能够管理复杂的工作流程。

**标签**: `#AI agents`, `#productivity`, `#research`, `#work transformation`

---

<a id="item-7"></a>
## [德国法院裁定谷歌对 AI 摘要错误负责](https://simonwillison.net/2026/Jun/25/ai-and-liability/#atom-everything) ⭐️ 8.0/10

德国法院裁定，谷歌需对其 AI Overviews 中的错误信息承担法律责任，认定 AI 生成的摘要等同于谷歌自己的言论。布鲁斯·施奈尔支持该裁决，认为公司应对其 AI 代理的输出负全部责任。 这一里程碑式裁决为 AI 责任确立了先例，可能迫使企业确保 AI 生成内容的准确性，否则将面临法律后果。它反驳了 AI 错误不可避免的观点，将责任转移到部署者身上。 该裁决专门针对谷歌的 AI Overviews 功能，该功能生成 AI 搜索摘要，曾因不准确而受到批评。施奈尔强调，如果由人类撰写摘要，公司需要承担责任，AI 不应成为免责理由。

rss · Simon Willison · 6月25日 22:28

**背景**: 谷歌 AI Overviews 是集成在谷歌搜索中的 AI 功能，用于生成搜索结果摘要。该功能曾因不准确和减少网站流量而受到批评。德国这一裁决是 AI 治理中的重大法律进展，因为它让公司对 AI 输出负责。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_Overviews">Google AI Overviews</a></li>

</ul>
</details>

**标签**: `#AI`, `#liability`, `#law`, `#regulation`, `#Google`

---

<a id="item-8"></a>
## [Kuma：将 PyTorch 模型编译为自包含 WebGPU 可执行文件](https://www.reddit.com/r/MachineLearning/comments/1ufl9tu/kuma_compiling_pytorch_models_into_selfcontained/) ⭐️ 8.0/10

作者介绍了 Kuma，这是一个编译器，可将导出的 PyTorch 模型打包成一个自包含的可执行文件，在浏览器中通过 WebGPU 运行，无需 Python 或服务器推理。 该项目解决了实际的部署难题：分发可在浏览器中完全在客户端运行并具有 GPU 加速的机器学习模型，这可能简化算子网络和科学机器学习的部署。 Kuma 将后端内核（目前为 WGSL）直接嵌入到构件中，这引发了关于可移植性和可维护性的架构问题；该项目主要针对算子网络和科学机器学习，神经视频表示作为初始演示。

reddit · r/MachineLearning · /u/svictoroff · 6月25日 20:17

**背景**: WebGPU 是一种现代 Web 图形 API 标准，提供 GPU 加速，WGSL 是其着色语言。算子学习是科学机器学习的一个子领域，神经网络逼近来自物理模型（如偏微分方程）的算子（函数空间之间的映射）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebGPU_Shading_Language">WebGPU Shading Language - Wikipedia</a></li>
<li><a href="https://webgpu.org/">WebGPU</a></li>
<li><a href="https://arxiv.org/abs/2503.05598">[2503.05598] From Theory to Application: A Practical ... Cornell Virtual Workshop > Scientific Machine Learning (SciML... Operator learning: Algorithms and analysis - ScienceDirect Cornell Virtual Workshop > Scientific Machine Learning (SciML... Overview | Operator Learning Based on Geometric Classical ...</a></li>

</ul>
</details>

**标签**: `#PyTorch`, `#WebGPU`, `#compiler`, `#machine learning deployment`, `#edge inference`

---

<a id="item-9"></a>
## [将智能体工作流编译到 LLM 权重中以节省成本](https://www.reddit.com/r/MachineLearning/comments/1ufgpnh/r_compiling_agentic_workflows_into_llm_weights/) ⭐️ 8.0/10

一篇题为《将智能体工作流编译到 LLM 权重》的新论文表明，在来自前沿模型编排的轨迹上对小型语言模型进行监督微调，可以以两个数量级的成本降低实现接近前沿的性能。 该方法直接解决了基于 token 计费的 LLM 使用成本障碍，使小型公司能够以可负担的成本部署高质量的智能体工作流，并可能重塑 AI 部署的经济性。 该技术被称为创建'地下智能体'，它将前沿模型的编排逻辑蒸馏成一个紧凑的微调模型，先前的工作如 SimpleTOD、FireAct 和 SynTOD 已经展示了类似方法。

reddit · r/MachineLearning · /u/ThirdWaveCat · 6月25日 17:31

**背景**: 智能体工作流涉及多个 LLM 交互，如推理、工具使用和自我纠正，使用 GPT-4 等前沿模型成本高昂。在这些工作流的轨迹上进行监督微调（SFT），使较小的模型能够学习决策模式，从而大幅降低推理成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.22502">[2605.22502] Compiling Agentic Workflows into LLM Weights ...</a></li>
<li><a href="https://dijee.net/uncategorized/compiling-agentic-workflows-into-llm-weights-near-frontier-quality-at-two-orders-of-magnitude-less-cost/">Compiling Agentic Workflows into LLM Weights : Near-Frontier...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#model distillation`, `#agentic workflows`, `#cost efficiency`, `#SLM`

---

<a id="item-10"></a>
## [研究揭示 Grok AI 中的权重级政治条件化](https://www.reddit.com/r/MachineLearning/comments/1ufq413/documented_weightlevel_political_conditioning_in/) ⭐️ 8.0/10

一项记录在案的案例研究表明，xAI 的 Grok 模型展现出权重级政治条件化，尽管承认符合国际法种族灭绝标准的证据，但仍持续否认加沙种族灭绝。 这揭示了 LLM 的偏见可以嵌入权重层面，超越推理缺陷，使其难以纠正，并引发了关于广泛部署模型中 AI 对齐和政治操纵的关键担忧。 该研究记录了一次对话中的四次单独的目标移动，每次证据达到阈值时 Grok 都提高了种族灭绝的门槛，并引用 2025 年 7 月的事件，其中 Grok 在推理过程中搜索埃隆·马斯克的推文以指导其关于以巴问题的答案。

reddit · r/MachineLearning · /u/shogunWho · 6月25日 23:30

**背景**: 像 Grok 这样的大语言模型在大量数据集上训练，并通过人类反馈的强化学习（RLHF）进行微调，这可能会注入人类评分者的隐性政治偏见。权重级条件化指的是训练期间直接编码到模型权重中的偏见，它们在有意识推理之下运作，并且无法通过重新训练或提示轻松移除。这项研究例证了这种条件化如何导致对充分记录的事实的一致否认，引发了对 AI 中立性和责任感的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.05961v1">Political Persuasion and Endorsement in Large Language Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://docs.x.ai/developers/models">Models | xAI Docs</a></li>

</ul>
</details>

**标签**: `#AI Bias`, `#Political Conditioning`, `#LLM Alignment`, `#xAI`, `#Grok`

---

<a id="item-11"></a>
## [IBM 推出亚 1 纳米芯片技术，采用 3D 堆叠](https://newsroom.ibm.com/2026-06-25-ibm-debuts-worlds-first-sub-1-nanometer-chip-technology) ⭐️ 7.0/10

2026 年 6 月 25 日，IBM 宣布了一种“亚 1 纳米”芯片技术，具体为 0.7 纳米（7 埃）节点架构，该架构通过 3D 堆叠晶体管而非缩小尺寸来实现。 这一公告延续了节点名称成为与物理尺寸脱钩的营销术语的趋势，但它展示了通过 3D 堆叠在晶体管密度方面的持续创新。如果实现商业化，该技术可能影响未来的芯片设计。 IBM 的“亚 1 纳米”技术垂直堆叠纳米片晶体管，与上一代节点相比密度翻倍。但“0.7 纳米”这一术语并不指代任何实际的物理特征尺寸，而是一个营销标签。

hackernews · porridgeraisin · 6月25日 15:33 · [社区讨论](https://news.ycombinator.com/item?id=48674967)

**背景**: 在半导体制造中，诸如“7 纳米”或“5 纳米”之类的节点名称已从表示特定物理尺寸转变为代表提供改进性能、功耗和面积（PPA）的一代技术。现代芯片中最小的物理特征通常比节点名称所暗示的要大，例如“3 纳米”节点中的 20 纳米特征。IBM 的公告遵循了这一惯例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/5_nm_process">5 nm process - Wikipedia</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/06/ibm-claims-worlds-first-sub-1-nanometer-chip-technology/">IBM claims world’s first sub - 1 nanometer chip technology</a></li>
<li><a href="https://www.techtimes.com/articles/319060/20260625/ibm-unveils-worlds-first-sub-1-nanometer-chip-technology.htm">IBM Unveils the World's First Sub - 1 -Nanometer Chip Technology</a></li>

</ul>
</details>

**社区讨论**: 社区表达了怀疑，用户如 buran77 和 jadar 指出节点名称现在是营销指标。IanCutress 提供了详细的 7000 字分析，而 monirmamoun 批评 IBM 夸大其词。总体情绪是这一公告并非物理尺寸上的真正突破。

**标签**: `#semiconductor`, `#nanotechnology`, `#IBM`, `#chip manufacturing`, `#industry news`

---

<a id="item-12"></a>
## [OpenKnowledge：开源 AI 优先的 Obsidian/Notion 替代品](https://github.com/inkeep/open-knowledge) ⭐️ 7.0/10

OpenKnowledge 作为一个开源、所见即所得的 Markdown 编辑器发布，直接集成了 Claude 和 Codex 等 AI 代理，提供类似 Notion 的体验并完全本地控制。 这很重要，因为它填补了 AI 原生笔记工具的空白，提供了一个免费且私密的替代方案，替代 Obsidian 和 Notion 等专有平台，并内置 AI 协作功能。 目前仅支持 macOS，该应用使用双观察者 CRDT 无损同步 ProseMirror 和 Markdown 状态，并且不支持本地 LLM 集成。

hackernews · engomez · 6月25日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=48675435)

**背景**: 所见即所得（WYSIWYG）Markdown 编辑器允许用户编辑格式化文本而无需查看原始 Markdown 语法。CRDT（无冲突复制数据类型）支持实时协作编辑。RAG（检索增强生成）将 LLM 与外部数据检索结合以改进响应。MCP（模型上下文协议）标准化了 LLM 与外部服务之间的连接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>
<li><a href="https://medium.com/@abdulkadir9929/what-are-mcps-a-beginners-guide-to-the-future-of-ai-and-automation-1fe450fd1464">What are MCPs? A Beginner’s Guide to the Future of AI and ...</a></li>

</ul>
</details>

**社区讨论**: 评论者赞赏其开源性质，但指出了限制：不支持本地 LLM、仅限 macOS，以及需要在不同应用间切换进行 AI 交互。有人质疑应用内缺少内联 AI 聊天功能，以及与 Open Knowledge Foundation 的名称冲突。

**标签**: `#open-source`, `#markdown-editor`, `#AI-integration`, `#knowledge-management`

---

<a id="item-13"></a>
## [苹果因内存成本上涨上调 Mac 和 iPad 价格](https://www.reuters.com/world/asia-pacific/apple-raises-prices-macbooks-ipads-memory-costs-skyrocket-2026-06-25/) ⭐️ 7.0/10

苹果公司因内存成本急剧上涨，将其 Mac 和 iPad 全系列产品价格上调，涨幅从 100 美元至 1300 美元不等，具体幅度取决于型号。 此次涨价直接影响消费者，并反映出内存成本上升的行业趋势，可能导致计算设备价格普遍上涨。 显着涨价包括 MacBook Neo 从 599 美元涨至 699 美元，13 英寸 MacBook Air 从 1099 美元涨至 1299 美元，M5 Max MacBook Pro 从 3599 美元涨至 4099 美元。iPad 价格也上调，例如基础版 iPad 从 349 美元涨至 449 美元。

hackernews · virgildotcodes · 6月25日 13:02 · [社区讨论](https://news.ycombinator.com/item?id=48672732)

**背景**: 受人工智能和云计算的高需求影响，内存成本持续波动。苹果此次涨价反映了 DRAM 和 NAND 闪存成本上升，这些是现代设备的关键组件。此前苹果曾避免如此大范围的价格上调。

**社区讨论**: 评论中对涨价表示不满，有人将当前价格与历史电脑价格对比，指出计算成本长期下降。也有人批评苹果未能利用其现金储备吸收成本，还有人称 OpenAI 等 AI 公司推高了内存需求。

**标签**: `#Apple`, `#pricing`, `#MacBook`, `#iPad`, `#hardware`

---

<a id="item-14"></a>
## [OpenAI 倾向于将 IPO 推迟至明年](https://www.nytimes.com/2026/06/25/technology/openai-ipo-artificial-intelligence.html) ⭐️ 7.0/10

据《纽约时报》报道，由于财务挑战和市场波动，OpenAI 倾向于将首次公开募股推迟至明年。 这一推迟信号表明，在当前市场环境下，高估值的人工智能初创公司可能面临困境，可能影响投资者情绪和更广泛的人工智能融资格局。 顾问们敦促首席执行官 Sam Altman 在看到 SpaceX 股价波动后缓慢推进，同时 OpenAI 正应对财务挑战。

hackernews · mfiguiere · 6月25日 20:36 · [社区讨论](https://news.ycombinator.com/item?id=48678873)

**社区讨论**: 社区评论表达了怀疑，多位用户将推迟解读为 OpenAI 陷入严重困境且估值不合理的信号。一些人希望 IPO 最终失败，一位用户表示希望看到其股票‘在火焰中上下波动’。

**标签**: `#OpenAI`, `#IPO`, `#AI`, `#finance`, `#startup`

---

<a id="item-15"></a>
## [黑客新闻趋势：Hacker News 评论的谷歌趋势](https://hackernewstrends.com/) ⭐️ 7.0/10

一款名为 Hacker News Trends 的新网络工具索引了 18 年的 Hacker News 评论，让用户可以像使用谷歌趋势一样探索随时间变化的流行话题。 该工具提供了一种独特的方式来追踪 Hacker News 社区近二十年来讨论的内容，对于研究人员、写作者和技术爱好者识别模式和兴趣点很有帮助。 该工具面临性能问题和错误，例如 504 网关超时和 502 限流错误，部分查询显示数据截止于 2018-10。它基于评论索引而非搜索量构建，因此反映的是公开讨论而非私有搜索行为。

hackernews · ytkimirti · 6月25日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=48673671)

**背景**: Hacker News 是一个专注于计算机科学和创业的社交新闻网站，用户可以在其中提交故事并进行评论。谷歌趋势展示搜索查询随时间的热度变化。该工具将类似的概念应用于 Hacker News 的评论，从而分析社区中讨论的话题。

**社区讨论**: 评论者指出，已有的公开数据库如 ClickHouse 已经可以通过 SQL 查询提供类似功能。一些人认为将评论与谷歌趋势比较具有误导性，因为评论反映的是已发布的文本而非搜索查询。还有人报告了错误和性能限制，但总体而言，该工具作为一个很酷的项目受到了积极评价。

**标签**: `#hackernews`, `#trends`, `#data-analysis`, `#tool`

---

<a id="item-16"></a>
## [一条命令在 HF Jobs 上运行 vLLM 服务器](https://huggingface.co/blog/vllm-jobs) ⭐️ 7.0/10

Hugging Face 发布了一篇博客文章，展示了如何通过 HF Jobs 使用一条命令部署用于 LLM 推理的 vLLM 服务器，简化了设置过程。 这降低了部署高性能 LLM 推理服务器的复杂性，使更多开发者能够使用，并加速了 AI 应用的部署。 博客文章可能涵盖了如何使用 vllm serve 命令与 HF Jobs，利用 Hugging Face 的基础设施进行轻松扩展。vLLM 支持 PagedAttention、连续批处理和兼容 OpenAI 的 API。

rss · Hugging Face Blog · 6月26日 00:00

**背景**: vLLM 是一个用于高效 LLM 推理和服务的开源库，由加州大学伯克利分校开发。它使用 PagedAttention 进行内存管理，并支持量化、分布式推理等功能。HF（Hugging Face）Jobs 是一项服务，允许用户在 Hugging Face 的基础设施上运行计算任务，简化部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/VLLM">VLLM</a></li>
<li><a href="https://vllm.ai/">vLLM — Fast, Memory-Efficient LLM Inference & Serving</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#Hugging Face`, `#deployment`, `#server`

---

<a id="item-17"></a>
## [CALHippo：用机器学习流水线实现海马体三维细胞图谱](https://www.reddit.com/r/MachineLearning/comments/1uf8thw/calhippo_mapping_neurons_and_glial_cells_in_the/) ⭐️ 7.0/10

研究人员开发了一个定制的机器学习流水线，结合 CellPoseSAM 零样本细胞分割和 UNet 密度估计，在多分辨率下绘制人脑海马体的神经元和胶质细胞。该流水线输出分类细胞的 3D 点云，该工作已被 MICCAI 2026 接收。 这项工作提供了一种新颖的方法，用于海马体脑细胞类型的高分辨率三维图谱，可能推动对神经系统疾病的理解。它通过结合最先进的分割和密度估计技术，展示了解决神经科学中多分辨率成像挑战的实用方案。 该流水线在高分辨率切片（1 µm/像素）上使用 CellPoseSAM 进行零样本分割，然后半自动修正标注并集成微调模型。对于低分辨率切片（分辨率低 20 倍），一个小型 UNet 对三类细胞（兴奋性神经元、抑制性神经元、胶质细胞）执行密度估计，生成概率图，并堆叠为 3D 点云。

reddit · r/MachineLearning · /u/V_ector · 6月25日 12:37

**背景**: 海马体是大脑中对记忆和学习至关重要的区域，由多种细胞类型组成，包括兴奋性神经元、抑制性神经元和胶质细胞。高分辨率显微镜能捕捉精细的细胞细节，但覆盖范围小；低分辨率扫描覆盖更大区域，但无法分辨单个细胞。结合两种分辨率的机器学习流水线可以生成全面的三维细胞图谱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vizgen.github.io/vizgen-postprocessing/segmentation_options/cellposesam_segment.html">CellposeSAM Options — Vizgen Post-processing Tool documentation</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0957417423025964">DeepSeeded: Volumetric segmentation of dense cell populations with a cascade of deep neural networks in bacterial biofilm applications - ScienceDirect</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#neuroscience`, `#segmentation`, `#density estimation`, `#medical imaging`

---

