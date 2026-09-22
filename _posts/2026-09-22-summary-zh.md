---
layout: default
title: "Horizon Summary: 2026-09-22 (ZH)"
date: 2026-09-22
lang: zh
---

> 从 40 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [M6 Mac mini 实测：多核追平 Intel 旗舰，GPU 翻倍](#item-tech-news-1) ⭐️ 9.0/10
2. [小米开源 MiMo-V2.6：原生全模态 MoE，Pro 激活 42B 参数](#item-tech-news-2) ⭐️ 8.0/10
3. [Sun 错在哪里：回顾与教训](#item-tech-news-3) ⭐️ 8.0/10
4. [Cloudflare 正式推出 Python Workers](#item-tech-news-4) ⭐️ 8.0/10
5. [Jev 问世：TypeSafe AI 推出输出结构化概率的“决策模型”](#item-tech-news-5) ⭐️ 8.0/10
6. [不想读你未写的内容](#item-tech-news-6) ⭐️ 7.0/10
7. [Transformer 架构交互式可视化指南上线](#item-tech-news-7) ⭐️ 7.0/10
8. [xAI 发布 Grok 4.7：增量更新引发性能与竞争力争议](#item-tech-news-8) ⭐️ 7.0/10
9. [MoE 模型推理硬件映射解析](#item-tech-news-9) ⭐️ 7.0/10
10. [亚马逊 Bedrock 接入 Kimi K3，分成合作落地](#item-tech-news-10) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [M6 Mac mini 实测：多核追平 Intel 旗舰，GPU 翻倍](https://www.bilibili.com/video/BV1JQhz6fE1x) ⭐️ 9.0/10

据极客湾 Geekerwan 的实测数据，Apple 新款 M6 Mac mini 采用 2+4+6 核 CPU 配置，基于台积电 N2 工艺，超大核频率达 4.8 GHz。其多核性能已与 Intel Panther Lake X9 388H 旗舰处理器持平，单核性能较 M4 提升超过 50%。GPU 升级至 12 核，光追和游戏表现大幅增强，游戏性能接近 M4 的两倍。功耗方面，CPU 满载约 25W，双烤整机约 65W。该数据来自极客湾的早期测试，尚未获得 Apple 官方规格确认。

telegram · zaihuapd · 9月21日 16:32

**「背景」** 苹果跳过了 M5 世代，直接于 2026 年 8 月发布搭载 M6 芯片的新款 Mac mini，起售价约 29,900 新台币，比前代 M4 型号高约 3,000 新台币。这是首款采用台积电 2 纳米（N2）工艺的 Apple Silicon 芯片，CPU、GPU 和 NPU 均全面升级。Geekerwan 等评测机构已取得实机并展开测试，其公布的跑分数据成为评估该芯片性能的关键参考。

**「影响评估」** 对于等待下一代 Mac mini 的用户和开发者而言，M6 在能效比和 GPU 性能上的显著提升意味着更高负载的本地 AI 推理、游戏和图形工作流有望在紧凑机身内获得近两倍的性能，且功耗维持在 65W 级别；不过，该数据来自非官方渠道，最终性能取决于 Apple 正式发布时的调校与散热设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.kocpc.com.tw/archives/25652">M6 Mac mini Performance Tested: More Cores, How Much Faster ...</a></li>
<li><a href="https://www.macrumors.com/2026/09/15/apple-m6-chip-benchmark/">M6 Chip Benchmark Surfaces Ahead of New Mac Mini Launch Next Week</a></li>
<li><a href="https://appleinsider.com/articles/26/09/15/first-m6-benchmarks-reveal-how-much-raw-power-the-mac-mini-has">M6 benchmarks reveal how far Apple&#x27;s boosted the Mac mini</a></li>

</ul>
</details>

**标签**: `#apple-silicon`, `#computer-hardware`, `#processor-benchmarks`, `#tsmc-n2`, `#mac-mini`

---

<a id="item-tech-news-2"></a>
### [小米开源 MiMo-V2.6：原生全模态 MoE，Pro 激活 42B 参数](https://mimo.xiaomi.com/mimo-v2-6) ⭐️ 8.0/10

小米 MiMo 团队于 9 月 22 日发布并开源了原生全模态 MoE 模型系列 MiMo-V2.6，包含旗舰版 Pro 和兼顾效率、成本的 Flash 两个版本，覆盖编程、电脑操作、3D 场景与视听内容创作等智能体任务。其中 Flash 为 309B 总参数/15B 激活参数，Pro 为 1.02T 总参数/42B 激活参数，面向高吞吐的 Pro-UltraSpeed 在同等质量下输出速度最高可提升 20 倍。团队负责人罗福莉称，这可能是开源模型团队迄今按算力计规模最大的单次强化学习训练之一，其训练采用 MixRL 联合中等难度、可验证的代码与智能体任务，并用 MOPD 合并游戏、3D 和主观评测等难验证或超长任务的能力。团队还同步开源了由 MiMo 训练轨迹蒸馏的 Qwen 模型、7000 个多样化环境和完整强化学习框架，网页体验、API 与 Hugging Face 入口均已开放。

hackernews · volf\_ · 9月21日 20:12 · [社区讨论](https://news.ycombinator.com/item?id=49792730)

**「背景」** 小米 MiMo 是小米 LLM-Core 团队推出的开源大模型系列，MiMo-V2.6 是其最新版本，包含旗舰版 Pro（总参数 1.02T、激活参数 42B）与兼顾效率的 Flash（总参数 309B、激活参数 15B）两个型号，均采用混合专家（MoE）架构，即每次推理只激活部分参数以平衡效果与成本。该系列为原生全模态模型，覆盖编程、电脑操作、3D 场景与视听内容创作等智能体任务，训练采用 MixRL 联合强化学习方法，并通过 MOPD 能力合并技术整合多来源能力。小米团队负责人罗福莉此前曾参与 DeepSeek R1 的研发，此次开源还附带实时训练仪表盘、技术报告、7000 个多样化环境与完整强化学习框架，强调训练过程的透明性，此前已有 MiMo-V2-Flash 等技术报告作为系列铺垫。

**「影响」** 对开源 AI 社区而言，本次开源将完整强化学习框架、7000 个多样化环境和蒸馏 Qwen 模型一并公开，使小型团队能够复制大规模 RL 训练管线，而 Pro-UltraSpeed 最高 20 倍的输出提速则为高吞吐推理场景提供实际部署收益。

**「社区讨论」** 社区评论普遍赞赏小米在训练透明度上的努力，一位用户称实时训练仪表盘是非常好的学习与教学工具，技术报告也异常详尽；另一用户则对中国模型的性价比印象深刻，stymaar 补充确认了两款模型的参数规模。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Xiaomi_MiMo">Xiaomi MiMo - Wikipedia</a></li>
<li><a href="https://mimo.mi.com/docs/en-US/updates/model">Xiaomi MiMo-V2.6 Series: 3 New Models Officially Released</a></li>
<li><a href="https://runtimewire.com/article/xiaomi-open-sources-mimo-v2-6-rl-cost-3-47m">Xiaomi open-sources MiMo-V2.6 and the RL machinery behind it</a></li>

</ul>
</details>

**标签**: `#open-source`, `#LLM`, `#Mixture-of-Experts`, `#Xiaomi`, `#AI research`

---

<a id="item-tech-news-3"></a>
### [Sun 错在哪里：回顾与教训](https://bcantrill.dtrace.org/2026/09/20/what-sun-got-wrong/) ⭐️ 8.0/10

Bryan Cantrill 的这篇文章回顾了 Sun Microsystems 的失败，剖析了导致其衰落的战略、技术与文化因素。文章在社区中引发了关于销售文化、决策失误和技术选择的热烈讨论。Cantrill 的分析为理解工程驱动型公司如何在商业执行上失败提供了重要洞察。

hackernews · chmaynard · 9月21日 14:03 · [社区讨论](https://news.ycombinator.com/item?id=49787436)

**「背景」** Sun Microsystems 是一家从 1982 年存续至 2010 年的美国科技公司，开发和销售计算机、硬件、软件及信息技术服务，并以 Java 和 Solaris 等关键技术闻名。它在工作站的崛起与后来衰落的过程中，曾深刻影响整个计算行业。了解这段兴衰历史，有助于理解 Bryan Cantrill 这篇回顾文章所剖析的 Sun 在战略和技术决策上的失误。

**「社区讨论」** 评论者普遍认为 Sun 过于注重工程而忽视商业运营，并列举了具体失误，如 2002 年取消 Solaris on x86、未能与 Google 达成合作，以及繁琐的销售流程。部分用户分享了使用 Sun 硬件的美好回忆，还有用户将 Sun 的兴衰与当前高估值科技股进行类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sun_Microsystems">Sun Microsystems - Wikipedia</a></li>
<li><a href="https://www.cgaa.org/article/sun-microsystems">Sun Microsystems: Rise, Fall, and Legacy of a Tech Icon - CGAA</a></li>

</ul>
</details>

**标签**: `#Sun Microsystems`, `#technology history`, `#systems engineering`, `#business strategy`, `#Solaris`

---

<a id="item-tech-news-4"></a>
### [Cloudflare 正式推出 Python Workers](https://blog.cloudflare.com/python-workers-ga/) ⭐️ 8.0/10

Cloudflare 宣布其服务器端 Workers 平台对 Python 的支持现已正式全面可用\(GA\),结束了长达两年的预览期,Python 由此成为 Cloudflare Developer Platform 上的第一等、完全受支持的语言。该实现的核心是将 Python 编译为 WebAssembly 并通过 Pyodide 运行,Cloudflare 还贡献了上游代码,使 HTTP 客户端能够在 WebAssembly 环境中直接经由 JavaScript 的 fetch API 路由请求,同时通过 PEP 783 标准化的 PyEmscripten 支持 PyPI 包。这一进展使 Python 开发者能够直接在 Cloudflare 边缘网络上运行代码,标志着无服务器边缘计算领域的重要里程碑。

hackernews · torutofu · 9月21日 13:38 · [社区讨论](https://news.ycombinator.com/item?id=49787142)

**「背景信息」** Cloudflare Workers 是运行在 Cloudflare 边缘网络上的服务器端无服务器计算平台，此前主要以 JavaScript/TypeScript 为支撑。两年前，Cloudflare 推出 Python Workers 预览版，让开发者能在 Workers 运行时中运行 Python 应用，并借助 Pyodide/WebAssembly 以及 urllib3 等 HTTP 客户端的上游贡献，使 Python 包生态得以在 WebAssembly 环境中工作。如今 Python Workers 正式发布（GA），使 Python 成为该平台上与 TypeScript 同级的一等支持语言。

**「影响」** 对 Python 开发者而言,现在可以直接在 Cloudflare 边缘网络运行 Python 代码并使用 PyPI 生态的包,大幅降低了无服务器边缘计算的入门门槛;同时这一标准化工作\(PEP 783\)也为 WebAssembly 环境下的 Python 包兼容性确立了参照,可能推动整个边缘计算生态的演进。

**「社区讨论」** urllib3 维护者指出,为 Requests 带来 Pyodide/JSPI 支持的大型贡献是由外部贡献者获得资助完成的,并未流向维护者团队,暗示贡献与资助的分配存在不均衡;竞争对手 Wasmer 的 syrusakbary 认可 Cloudflare 在包支持方面的显著进步\(PEP 783\),但认为部分核心架构问题仍未解决;另有评论将此举与 2008 年 Google App Engine 的 Python 2.5 支持相类比,调侃技术发展似乎回到了原点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/python-workers-ga/">Python Workers are now generally available | Cloudflare Blog</a></li>
<li><a href="https://www.technobezz.com/news/cloudflare-python-workers-general-availability">Cloudflare Makes Python Workers Generally Available</a></li>
<li><a href="https://developers.cloudflare.com/workers/languages/python/">Write Cloudflare Workers in Python · Cloudflare Workers docs</a></li>

</ul>
</details>

**标签**: `#Python`, `#Cloudflare Workers`, `#Serverless`, `#Edge Computing`, `#WebAssembly`

---

<a id="item-tech-news-5"></a>
### [Jev 问世：TypeSafe AI 推出输出结构化概率的“决策模型”](https://simonwillison.net/2026/Sep/21/jev/) ⭐️ 8.0/10

人工智能公司 TypeSafe AI 发布了 Jev，这是其称之为“System One 模型”（也被称为“决策模型”）新品类中的首个产品。与传统 LLM 不同，Jev 仍接受文本输入，但不再生成文本，而是返回浮点数形式的分类结果、是非判断、评分及置信度，官方将其描述为“非结构化状态进、类型化概率决策出”。Jev 只按输入计费，每百万 token 仅 0.042 美元，输出完全免费，价格甚至低于 OpenAI 的 GPT-5 Nano（0.05 美元/百万 token）；API 支持是非（Noul，源自伯努利分布）、选项选择和区间评分三类问题，且多问题可并行评估，速度很快。作者认为这类模型适合垃圾邮件检测、标签建议、优先级排序及搜索重排等分类任务，但也指出其相比 LLM 更回归黑箱，偏差问题更难排查，因此评测与结构化实验尤为重要。发布不到一周，社区已涌现 jevchat、jev-leftpad、jev-2048 等创意项目，以及基于 Qwen 3.5 的开源权重复刻 Kev。

rss · Simon Willison · 9月21日 23:09

**「背景」** 传统大语言模型按输入和输出 token 计费，且输出单价通常远高于输入，其优势在于生成自由文本，但结果仍属难以保证可靠性的黑箱。Jev 所属的“决策模型”类别则改变了这一交互范式：不再输出文本，而是直接以浮点数形式给出离散决策与置信度，从而可能大幅改变结构化决策任务的用法、成本与速度。

**「影响」** 对从事分类、排序与重排等结构化决策任务的开发者和团队，Jev 带来了显著更低的成本（输入每百万 token 0.042 美元、输出免费）与更高的速度，使大规模评测实验变得极为经济；不过其不可解释的浮点数输出可能隐藏偏差，若用于求职者排名等敏感场景风险明显，需配合严格评测。

**标签**: `#LLM architecture`, `#AI models`, `#decision models`, `#TypeSafe AI`, `#machine learning`

---

<a id="item-tech-news-6"></a>
### [不想读你未写的内容](https://blog.colinbreck.com/i-dont-want-to-read-what-you-didnt-write/) ⭐️ 7.0/10

这篇博客文章认为，AI 生成的文本无法传递作者的真实意图，因为写作本质上是将信息从一个人的大脑转移到另一个人的大脑，而大语言模型只能根据作者提供的少量语义信息进行猜测，无法填补缺失的那部分。作者批评了一种常见做法：人们用 AI 构建新事物后，又用 AI 逆向总结成设计文档，结果读起来“不仅困难，而且令人痛苦”。虽然这是一篇观点性文章，但它触及了技术写作中的实际摩擦，在实践者中引起广泛共鸣，尤其是关于 AI 对评审和文档质量的负面影响。文章没有提供实证数据，但明确表达了对 AI 写作在技术沟通中失去人情味和真实性的担忧。

hackernews · mooreds · 9月21日 22:30 · [社区讨论](https://news.ycombinator.com/item?id=49794330)

**「背景：AI 辅助写作与读者信任」** 随着大语言模型（LLM）的普及，越来越多工程师开始用 AI 生成或润色技术文档、设计文档和代码评审说明。然而，基于 Cynthia Dunlop 发布的开发者调查报告，约 78% 的读者一旦认为文章由 AI 辅助或代笔，就会停止阅读；克里斯滕森（Colin Breck）这篇博文的出发点正是对这种“AI 气味”文本的抗拒，认为它无法传递作者真实的意图和上下文。

**「影响」** 对于依赖代码评审和技术文档的工程师而言，AI 生成的冗长描述和“后补”设计文档会显著增加阅读负担，甚至导致变更被拒绝，因为评审者无法确认哪些内容真正出自作者意图。

**「社区讨论」** 评论者大多认同文章的核心观点：有人用比特信息论解释 LLM 无法填补缺失的语义信息；有人抱怨 AI 生成的 PR 描述过于冗长，反而令人反感；还有人表示更愿意读未经修饰的原始思路，而不是经过 AI“消化”的文本。也有评论指出文章的开头第一句恰恰就是作者所批评的那种 AI 腔调，形成一种有趣的自我指涉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.colinbreck.com/i-dont-want-to-read-what-you-didnt-write/">I Don ’ t Want to Read What You Didn ’ t Write</a></li>

</ul>
</details>

**标签**: `#AI writing`, `#technical communication`, `#software engineering`, `#LLM`, `#content quality`

---

<a id="item-tech-news-7"></a>
### [Transformer 架构交互式可视化指南上线](https://poloclub.github.io/transformer-explainer/) ⭐️ 7.0/10

佐治亚理工学院 Poloclub 数据可视化实验室推出了交互式可视化工具 Transformer Explainer，旨在以可视化的方式逐层剖析 Transformer 架构的内部工作原理，为 AI/ML 工程师和学生提供一条直观的学习路径。该工具通过可交互的界面展示注意力矩阵、注意力头等核心组件的运算过程，帮助读者理解现代大语言模型底层的注意力机制与动态权重构建方式。社区评论显示它获得了积极反响，被认为制作精良、具有真实的教学价值；有读者指出，其将注意力矩阵与 Value 向量相乘的过程类比为在推理时动态构造一个小型稠密网络层的观察尤为精辟，这类观点在以往解释中较少被强调。该资源目前托管于 poloclub.github.io/transformer-explainer/，但从内容形态看属于教学性工具而非时效性新闻，官方未披露具体的发布版本与日期信息。

hackernews · aray07 · 9月21日 19:43 · [社区讨论](https://news.ycombinator.com/item?id=49792342)

**「背景」** Transformer 是一种深度学习架构，最初由 2017 年的论文《Attention Is All You Need》提出，如今已成为 GPT、ChatGPT、Claude、Gemini 等大多数现代 AI 系统的基础。它依靠自注意力机制（attention mechanism）并行处理序列数据，取代了早期的循环神经网络，而注意力头在训练和推理过程中动态构建权重。这个交互式可视化工具正是面向希望直观理解 Transformer 内部工作原理的 AI/ML 工程师和学生。

**「影响」** 对于希望理解 Transformer 机制的 AI/ML 学习者而言，该工具提供了一条低门槛的交互式探索路径，可与《The Illustrated Transformer》等经典图文教程形成互补，帮助初学者突破注意力头与参数计算等抽象概念的理解障碍。

**「社区讨论」** 评论区整体反馈正面，有读者称赞工具&quot;做得很好&quot;，并在推理时动态构建网络层这一点上产生了共鸣；但也有读者指出工具在解释温度参数时使用&quot;safety&quot;一词并不准确，因为温度为 0 的文本会产生一种人工化的&quot;缺乏惊喜&quot;特征。另有读者推荐初学者搭配阅读《The Illustrated Transformer》，并提到&quot;transformer&quot;一词与电力工程中的变压器在术语上容易混淆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generative_pre-trained_transformer">Generative pre-trained transformer - Wikipedia</a></li>
<li><a href="https://dev.to/mangeshmandlik/transformer-basics-the-architecture-behind-chatgpt-claude-and-gemini-1ljg">Transformer Basics: The Architecture Behind... - DEV Community</a></li>

</ul>
</details>

**标签**: `#transformers`, `#deep learning`, `#visualization`, `#educational tool`, `#NLP`

---

<a id="item-tech-news-8"></a>
### [xAI 发布 Grok 4.7：增量更新引发性能与竞争力争议](https://x.ai/news/grok-4-7) ⭐️ 7.0/10

xAI 于近期发布大语言模型 Grok 4.7，这是对 Grok 4.6 的增量更新。据社区信息，其权重（参数）规模比 4.6 增加约 40%，但 API 定价保持不变，仍为输入每百万 token 2 美元、输出 6 美元。该版本比原定发布日期推迟了近两周，并选在传闻中 Anthropic Opus 5.5 发布的前一天推出。社区初步测试显示，Grok 4.7 的推理速度明显变慢、使用成本更高，而在编码和智能体工作流中的表现是否真正超越 4.6 或达到 Sol/Opus 的智能水平尚不明确。有评论推测 xAI 可能通过让模型消耗更多推理 token 来推高基准分数，也有观点认为这是团队在更大规模训练上的渐进铺垫，期待 Grok 5 带来更显著提升。整体来看，这被视为一次竞争压力下的战术性模型迭代，而非技术突破。

hackernews · meetpateltech · 9月21日 15:50 · [社区讨论](https://news.ycombinator.com/item?id=49788838)

**「背景」** Grok 是 xAI 推出的前沿大语言模型系列，此前版本如 Grok 4.6 已用于编程、智能体工作流等场景。Grok 4.7 是该系列的增量更新，官方介绍称它相比 4.6 采用了新的、更大的基础模型，并通过更长的强化学习训练，在难度更高、且偏重耗时数小时的长任务样本上进行了优化。该模型于 2026 年 9 月 21 日发布，可通过 Cursor、Grok Build 和 xAI API 使用，API 标准定价与 4.6 相同（每百万输入 token 2 美元、每百万输出 token 6 美元）。

**「影响」** 对使用 xAI API 的开发者而言，Grok 4.7 在价格不变的情况下推理更慢、参数量增长约 40%，意味着实际计算成本和等待时间上升，需要结合自身编码与智能体工作流的质量需求重新评估是否切换。当前证据尚不足以确认其在真实任务上显著优于 Grok 4.6，且未来表现可能受到即将发布的 Opus 5.5 的竞争挤压。

**「社区讨论」** 社区反应分化明显：有开发者指出 4.7 参数增加 40% 但价格未变、发布延期近两周，怀疑 xAI 对自身结果也不满意，并预计 Opus 5.5 将大幅超越其基准；也有开发者反馈 4.6 已难满足其编码与智能体工作流需求，4.7 速度更慢、成本更高，是否越过“智能下限”仍不确定。部分评论者则乐观看待发布节奏加快，认为团队在更大规模训练上逐步积累经验，Grok 5 有望带来明显跃升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/news/grok-4-7">Introducing Grok 4.7 | SpaceXAI</a></li>
<li><a href="https://kingy.ai/blog/grok-4-7-release-features-pricing-access/">Grok 4.7 Is Out: Features, Pricing &amp; How to Try It - kingy.ai</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#large language models`, `#xAI`, `#Grok`, `#machine learning`

---

<a id="item-tech-news-9"></a>
### [MoE 模型推理硬件映射解析](https://newsletter.semianalysis.com/p/computation-and-data-movement-for) ⭐️ 7.0/10

SemiAnalysis 的 Tanj Bennett 发布了一份技术分析，聚焦于将混合专家（MoE）模型映射到推理硬件上的方法。内容涵盖模型结构、数据流以及高效服务部署，旨在为工程人员优化 AI 推理系统提供参考。分析强调了结构设计对数据移动和计算效率的影响，并指出在推理场景下合理组织专家模块和路由机制的重要性。由于原始内容概要有限，具体技术细节与性能数据未能完整呈现，但该分析针对当前大规模模型部署的实用性需求。

rss · Semianalysis · 9月21日 18:14

**「背景：混合专家模型与推理硬件」** 混合专家（Mixture of Experts，MoE）架构已广泛应用于前沿大语言模型，它不仅增加了参数量，更改变了推理服务的结构与经济性：每个词元（token）只会激活部分专家子网络，因此哪些张量处于活动状态、哪些数据必须保持邻近都会随请求动态变化。这种按词元动态路由的机制，使得推理时的数据移动开销成为在神经网络处理器（NPU）等硬件上部署与高效服务的关键瓶颈。理解 MoE 的结构和流程，是评估相关硬件映射与调度方案的基础。

**「影响」** 对于从事 AI 推理系统开发和硬件选型的工程师，该分析提供了将 MoE 模型高效映射到硬件的思考框架，有助于优化服务部署中的计算与数据移动策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/computation-and-data-movement-for">Computation and Data Movement for Inference</a></li>

</ul>
</details>

**标签**: `#Mixture of Experts`, `#inference`, `#hardware`, `#model serving`, `#AI systems`

---

<a id="item-tech-news-10"></a>
### [亚马逊 Bedrock 接入 Kimi K3，分成合作落地](https://36kr.com/newsflashes/3992769217428488) ⭐️ 7.0/10

亚马逊云科技旗下大模型服务平台 Amazon Bedrock 宣布接入开源大模型 Kimi K3，全球企业开发者现可通过 Bedrock 直接调用该模型，此前传闻的 Kimi 与海外云厂商收入分成合作由此正式落地。按照这一分成模式，云厂商将 Kimi 模型上架到自身平台，并基于模型调用量与月之暗面进行分成。这是中国大模型公司首次以收入分成模式向全球三大云厂商输出模型能力，标志着国产大模型出海与商业化路径出现新的里程碑。

telegram · zaihuapd · 9月21日 06:44

**「合作背景」** 月之暗面（Moonshot AI）的 Kimi K3 是一款开源权重大模型，开发方称其为首个达到 2.8 万亿参数的开源模型，主打编程与知识工作场景，并于 2026 年 9 月 18 日上线 Amazon Bedrock。在此之前的 2026 年 8 月，路透社报道月之暗面正与微软、亚马逊和谷歌等美国云厂商谈判收入分成协议，由这些云厂商托管其 Kimi K3 模型并基于调用量分成。这一背景解释了本次亚马逊 Bedrock 集成的意义，它使此前传闻的分成合作正式落地。

**「实际影响」** 全球企业开发者现可通过 Amazon Bedrock 直接调用 Kimi K3，模型同时已上线阿里云百炼平台，AWS 称其为编码和知识工作提供了新的强大选项；这一事件标志着月之暗面与海外云厂商基于调用量的收入分成模式正式落地，为中国大模型公司首次以分成方式向全球云厂商输出模型能力确立了可复制的商业路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/moonshot-ais-kimi-k3-arrives-on-amazon-bedrock-with-1m-token-context/">Moonshot AI ’s Kimi K 3 Arrives on Amazon Bedrock With 1M-Token...</a></li>
<li><a href="https://www.jpost.com/business-and-innovation/tech-and-start-ups/article-906633">Moonshot AI in talks with Microsoft, Google, Amazon over Kimi ...</a></li>
<li><a href="https://equalocean.com/news/2026082722142-moonshot-ai-talks-microsoft-amazon-google-kimi-k3-revenue-sharing">Moonshot AI in Talks With Microsoft, Amazon and Google on Kimi ...</a></li>
<li><a href="https://finance.biggo.com/news/c56898f3-c444-4706-b83f-e1d4b4276366">Kimi K3 Lands on AWS Bedrock as Moonshot AI&#x27;s Overseas ...</a></li>
<li><a href="https://www.scmp.com/tech/tech-trends/article/3368274/moonshots-kimi-k3-lands-amazon-key-test-chinese-open-source-ai-revenue">Moonshot’s Kimi K3 lands on Amazon in key test for Chinese ...</a></li>
<li><a href="https://www.kucoin.com/news/flash/kimi-k3-integrated-on-aws-bedrock-and-alibaba-cloud-revenue-sharing-agreements-confirmed">Kimi K3 Integrated on AWS Bedrock and Alibaba Cloud, Revenue ...</a></li>

</ul>
</details>

**标签**: `#Kimi K3`, `#AWS Bedrock`, `#大模型`, `#云厂商合作`, `#收入分成`

---