---
layout: default
title: "Horizon Summary: 2026-09-16 (ZH)"
date: 2026-09-16
lang: zh
---

> 从 35 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [泄露的 PAT 使攻击者 25 分钟内接管 Baseten 生产 GitHub](#item-tech-news-1) ⭐️ 8.0/10
2. [Groovy 沙箱绕过技术分析：以 Apache Syncope 漏洞链为例](#item-tech-news-2) ⭐️ 8.0/10
3. [Prior Labs 发布 TabPFN-3.5，新一代表格基础模型 SOTA](#item-tech-news-3) ⭐️ 8.0/10
4. [谷歌向全体工程师开放 Anthropic 的 Claude](#item-tech-news-4) ⭐️ 8.0/10
5. [联发科发布首款台积电 2 纳米制程手机芯片天玑 9600 Pro](#item-tech-news-5) ⭐️ 8.0/10
6. [“Project Lily”内幕：人工阅读 ChatGPT 聊天记录](#item-tech-news-6) ⭐️ 8.0/10
7. [Typesafe.ai 发布 System One 模型与 Jev 快速类型化推理系统](#item-tech-news-7) ⭐️ 7.0/10
8. [会听鸟鸣并绘制 19 世纪风格插画的电子墨水画框](#item-tech-news-8) ⭐️ 7.0/10
9. [互联网档案馆更新 Wayback Machine 访问防护](#item-tech-news-9) ⭐️ 7.0/10
10. [Gemini 3.8 Live 及 Extended Thinking 发布，强化实时语音与推理](#item-tech-news-10) ⭐️ 7.0/10
11. [美国首次正式确认已部署太空武器](#item-tech-news-11) ⭐️ 7.0/10
12. [数据中心暂停令对美国建设的影响远小于预期](#item-tech-news-12) ⭐️ 7.0/10
13. [44M 参数三元 LLM 仅 19.8MB，CPU 推理约 1900 token/秒](#item-tech-news-13) ⭐️ 7.0/10
14. [工信部发改委印发“十五五”电子信息制造业规划，聚焦先进制程与国产芯片](#item-tech-news-14) ⭐️ 7.0/10
15. [桑德斯提案拟禁超级智能 AI 并设刑责](#item-tech-news-15) ⭐️ 7.0/10
16. [字节 ADrive 与腾讯网盘竞逐，AI 智能网盘战争升温](#item-tech-news-16) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [泄露的 PAT 使攻击者 25 分钟内接管 Baseten 生产 GitHub](https://www.strix.ai/blog/baseten-harbor-github-pat-takeover) ⭐️ 8.0/10

安全研究员通过一条 25 分钟的攻击路径，从一个公开的 Harbor 镜像仓库入手，最终获得了 Baseten 生产 GitHub 组织的管理员权限。攻击者从一个 Baseten 镜像仓库的 Docker 构建历史中提取到一个有效的 GitHub 个人访问令牌（PAT），该令牌属于 basetenbot，对 Baseten 的主产品仓库、驱动集群的 GitOps 仓库和 Homebrew tap 拥有管理员和推送权限，并能读写包括客户专属仓库在内的其他私有仓库。研究员于 7 月 13 日 23:10 报告了该令牌和仓库权限问题，Baseten 在 7 月 14 日将 Harbor 项目设为私有并轮换了令牌，随后确认此事件为严重问题。这一事件凸显了 AI 基础设施供应链中构建历史泄露凭据的实际风险。

hackernews · bearsyankees · 9月15日 18:11 · [社区讨论](https://news.ycombinator.com/item?id=49716476)

**「背景：GitHub 令牌与容器镜像供应链风险」** GitHub 个人访问令牌（PAT）是用于对 GitHub API 和仓库执行操作的长期凭据，一旦泄露可能使攻击者获得对代码库的读写乃至管理权限。容器镜像的构建历史会永久保存构建命令与环境变量，若在构建过程中把令牌写入镜像层，攻击者可通过拉取公开镜像并检查其历史记录来提取这些秘密；Strix 正是在对拉取的镜像层运行 TruffleHog 并检查镜像配置时，从 history\[\].created\_by 字段中发现了令牌。这类风险并非假设性威胁：2026 年 5 月 Grafana 也曾因 GitHub 令牌泄露导致代码库被下载并遭勒索，说明此类事故在真实世界中有明确的破坏性先例。

**「影响」** 对于发布容器镜像并依赖 GitHub 组织管理代码和基础设施的公司而言，此事件表明 Docker 构建历史中的令牌泄露可能直接导致生产系统的管理员接管，组织需审计镜像构建过程中的凭据暴露风险。

**「社区讨论」** 社区评论中，有人认为这是对 Strix 安全产品极好的营销，但承认对 Baseten 不利，并打算尝试该产品；另一些人则质疑这种做法是否合法，以及安全工具公司是否应以真实客户为营销素材，认为即使没有窃取意图，未经授权访问系统也可能越界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.strix.ai/blog/baseten-harbor-github-pat-takeover">We wanted to use Baseten for inference. We ended up with admin access to their GitHub - Strix</a></li>
<li><a href="https://thehackernews.com/2026/05/grafana-github-token-breach-led-to.html">Grafana GitHub Token Breach Led to Codebase Download and Extortion Attempt</a></li>

</ul>
</details>

**标签**: `#security`, `#github`, `#container-security`, `#AI-infrastructure`, `#penetration-testing`

---

<a id="item-tech-news-2"></a>
### [Groovy 沙箱绕过技术分析：以 Apache Syncope 漏洞链为例](https://xz.aliyun.com/news/92835) ⭐️ 8.0/10

本文以 Apache Syncope 的一个真实漏洞链为例，整理了 Groovy 黑名单沙箱的三类绕过方式：解释器逃逸、运行时间接调用、反射与黑名单盲区。文章从沙箱的实现原理出发，逐一说明每种绕过方式的切入点、绕过原因以及在真实目标上的利用效果。该分析对安全研究人员与开发人员具有实用价值，有助于理解 Groovy 沙箱的边界缺陷并针对性地进行加固。由于原文未披露漏洞编号、受影响版本与演示数据等细节，本次整理仅涵盖其方法与结论。

rss · 先知社区 · 9月15日 08:00

**「背景」** Apache Syncope 是一个开源的 Java 身份管理（IdM）系统，允许管理员通过 Groovy 脚本实现自定义逻辑，而 Groovy 是运行在 JVM 上的动态语言。为隔离不可信代码，Syncope 引入的沙箱通常采用黑名单方式拦截 Runtime.exec、ProcessBuilder 及不受限制的文件 I/O 等危险 API。2025 年 10 月披露的 CVE-2025-57738（由 Mike Cole 发现）显示恶意脚本可绕过该 Groovy 沙箱执行任意代码；官方于 3.0.14 与 4.0.2 版本中修补，但后续披露的受影响版本范围又扩展至 3.0.16、4.0.6 与 4.1.1，暗示黑名单沙箱仍存在绕过盲区。

**「影响」** 对依赖 Groovy 黑名单沙箱的 Apache Syncope 部署而言，这三类绕过方式可被利用实现远程代码执行，相关运维方应尽快收紧脚本执行环境，并补充白名单机制与调用链审计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberpress.org/apache-syncope-groovy-rce-vulnerability/">Apache Syncope Groovy RCE Vulnerability Allows Attackers Inject Malicious Code</a></li>
<li><a href="https://cybersecuritynews.com/apache-syncope-groovy-rce-vulnerability/">Apache Syncope Groovy RCE Vulnerability Let Attackers Inject Malicious Code</a></li>
<li><a href="https://vulners.com/search/vendors/apache/products/syncope">Syncope Security Vulnerabilities and Issues — Syncope CVE List | Vulners.com</a></li>

</ul>
</details>

**标签**: `#security`, `#Groovy`, `#sandbox-bypass`, `#Apache Syncope`, `#RCE`

---

<a id="item-tech-news-3"></a>
### [Prior Labs 发布 TabPFN-3.5，新一代表格基础模型 SOTA](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 8.0/10

Prior Labs 今日发布最新表格基础模型 TabPFN-3.5，该模型在 TabArena 与 BeyondArena 两个基准测试中均位列榜首，并宣称可在多达 100 万行、2 万特征的数据上达到 SOTA 水平。本次发布包含多个变体：TabPFN-3.5-Fast（alpha 版，速度比基础模型快 6 倍）、TabPFN-3.5-Thinking（通过 API 提供，以更多计算换取更高精度）以及 TabPFN-3.5-Plus。在 BeyondArena 上，TabPFN-3.5 在文本丰富、高基数与高维数据类别中领先，较此前最强基线高出 250 Elo 分，较此前的总榜领先者高出 150 Elo 分。TabPFN-3.5-Thinking 在 BeyondArena 上较基础模型高 20 Elo 分，在 TabArena 上高 44 Elo 分。

reddit · r/MachineLearning · /u/tuanacelik · 9月15日 16:18

**「背景」** TabPFN 是 Prior Labs 推出的面向表格数据的基础模型（tabular foundation model），其核心特点是借助上下文学习（in-context learning）直接对新的数据集进行预测，而无需像传统机器学习流程那样针对每个数据集单独训练模型。该系列已有多个迭代版本（如 TabPFN-2.5），可通过 PriorLabs 账户登录并接受许可条款后使用；本次发布的 TabPFN-3.5 是该系列的最新迭代，同时推出 Fast、Thinking、Plus 等变体。

**「影响」** 对于从事表格数据建模的开发者与研究者，TabPFN-3.5 的发布意味着可在速度（Fast）与精度（Thinking）之间按需选择的更高基准已可通过 Prior Labs 获取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://priorlabs.ai/tabpfn">TabPFN | Prior Labs</a></li>
<li><a href="https://priorlabs.ai/tabpfn-2">TabPFN | Prior Labs</a></li>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/TabPFN: ⚡ TabPFN: Foundation Model for ...</a></li>

</ul>
</details>

**标签**: `#tabular models`, `#foundation models`, `#machine learning`, `#SOTA`, `#TabPFN`

---

<a id="item-tech-news-4"></a>
### [谷歌向全体工程师开放 Anthropic 的 Claude](https://www.businessinsider.com/google-finally-lets-all-engineers-use-anthropics-claude-2026-9) ⭐️ 8.0/10

谷歌已向全公司工程师开放 Anthropic 旗下最强的编程模型 Claude（Opus 5）用于内部开发，但仅限于其内部开发平台 Antigravity。此前谷歌通常禁止大多数员工使用 Claude Code、OpenAI 的 Codex 等外部编程工具，要求他们改用自家 Gemini。谷歌发言人表示，Gemini 仍是内部开发的主要模型，Claude 按每位员工配额提供、作为补充。此举被视为对 AI 编码领域竞争压力的回应；谷歌是 Anthropic 的投资者，今年早些时候宣布计划向该公司投入最多 400 亿美元。

telegram · zaihuapd · 9月15日 05:31

**「背景」** 多年来，谷歌优先推广自家 AI 模型 Gemini，并长期禁止或限制大多数员工使用 Claude Code、OpenAI Codex 等外部编程工具，要求内部开发一律基于 Gemini。Antigravity 是谷歌内部版本的开发平台，此次政策调整正是通过该平台向全员开放 Anthropic 的 Opus 5 模型，并按每位员工的配额提供。谷歌同时是 Anthropic 的投资者，曾宣布计划向其投入最多 400 亿美元，因此这一转变被普遍视为对 AI 编码领域竞争压力的回应。

**「影响」** 谷歌向全体工程师开放内部 Antigravity 平台上的 Claude Opus 5 作为 Gemini 的补充，标志着这家长期限制外部编码工具的公司承认 Claude 在 AI 编码领域的优势；鉴于 Claude 已占美国企业 AI 市场 43.8%份额、且企业客户贡献了 Claude Code 一半以上收入，谷歌的内部采用可能成为其他大型企业引入 Claude 的示范，进一步巩固 Anthropic 的企业市场地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digg.com/tech/04cff254-0da4-4396-8105-4c12e0f47c90">Google grants broader internal access to Anthropic &#x27;s Claude amid...</a></li>
<li><a href="https://kingy.ai/news/google-engineers-anthropic-claude-ai-coding/">Google Opens the Door to Claude for All Engineers —and... - Kingy AI</a></li>
<li><a href="https://dnyuz.com/2026/09/14/google-finally-lets-all-engineers-use-anthropics-claude/">Google finally lets all engineers use Anthropic ’s Claude – DNYUZ</a></li>
<li><a href="https://www.kucoin.com/blog/anthropic-vs-openai-ramp-data-shows-claude-leading-us-enterprise-ai-market-share-at-43-8">Anthropic vs OpenAI: Ramp Data Shows Claude Leading US Enterprise AI Market Share at 43.8%| KuCoin</a></li>

</ul>
</details>

**标签**: `#Google`, `#Anthropic`, `#Claude`, `#AI coding`, `#enterprise AI`

---

<a id="item-tech-news-5"></a>
### [联发科发布首款台积电 2 纳米制程手机芯片天玑 9600 Pro](https://www.reuters.com/business/media-telecom/mediatek-launches-new-mobile-chip-using-tsmcs-most-advanced-technology-2026-09-15/) ⭐️ 8.0/10

联发科于 9 月 15 日发布旗舰手机芯片天玑 9600 Pro，采用台积电 2 纳米制程，成为该公司首款采用该制程的手机处理器；同日还发布采用 3 纳米制程的天玑 9600M。据联发科称，搭载这两款芯片的首批手机将很快上市。天玑 9600 Pro 配备专用 AI 处理器，在用户输入提示词、启动模型生成前的处理性能较上一代提升 51%。这是联发科首次进入 2 纳米制程节点，标志着其在先进半导体制造领域的布局取得关键进展。

telegram · zaihuapd · 9月15日 08:57

**「背景与来龙去脉」** 台积电的 2 纳米制程是目前最先进的半导体工艺节点，相比 3 纳米能在同等功耗下带来更高性能或更优能效，量产难度也更大。联发科于 2026 年 9 月 15 日发布天玑 9600 Pro，成为业内率先宣布跨入 2 纳米门槛的厂商；该芯片采用 2+3+3“全大核”CPU 架构，基于 Arm 核心，并支持 LPDDR6 内存与 UFS 5.0 存储。同场发布的还有采用 3 纳米制程的天玑 9600M。

**「影响」** 天玑 9600 Pro 使联发科首次跨入 2 纳米制程门槛，有助于提升其旗舰芯片在端侧 AI 算力上的竞争力，并将率先推动台积电 2 纳米产能进入手机处理器市场，可能改变高端移动芯片的竞争格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.semiconductor-digest.com/mediatek-launches-dimensity-9600-pro-on-tsmc-2nm-process/">MediaTek Launches Dimensity 9600 Pro on TSMC 2nm Process</a></li>
<li><a href="https://www.gizmochina.com/2026/09/15/mediatek-announces-dimensity-9600-pro-built-on-2nm-process-and-arms-c2-cores/">MediaTek announces Dimensity 9600 Pro built on 2nm process ...</a></li>
<li><a href="https://9to5google.com/2026/09/15/mediatek-dimensity-9600-pro-chip/">MediaTek Dimensity 9600 Pro goes official with 2nm process ...</a></li>

</ul>
</details>

**标签**: `#MediaTek`, `#Dimensity 9600 Pro`, `#2nm process`, `#AI hardware`, `#mobile chips`

---

<a id="item-tech-news-6"></a>
### [“Project Lily”内幕：人工阅读 ChatGPT 聊天记录](https://www.404media.co/inside-project-lily-the-humans-reading-your-chatgpt-chats/) ⭐️ 8.0/10

据 404 Media 报道，OpenAI 正在执行一项名为“Project Lily”的内部计划，雇用数百名合同工阅读大量真实用户的 ChatGPT 提示词及完整对话，以便为模型回复评分并提出修改意见。OpenAI 表示会在将数据交给审核员前尽量删除个人信息，但也承认敏感细节仍可能被看到。报道指出，这些对话可能包含敏感个人信息，引发对用户隐私和数据处理的担忧。此外，Anthropic 也确认使用人工审核来改进其模型。这一披露凸显了 AI 公司在模型质量改进过程中对用户数据的人工审查实践，以及其隐私保护措施的局限性。

telegram · zaihuapd · 9月15日 11:56

**「背景」** OpenAI 等大型 AI 公司通常依赖人工审核来改进模型性能，例如给模型回复评分或标注不安全内容。然而，这类审核一般被认为是在匿名化或处理后的数据上进行，用户不太清楚自己的真实对话可能被人工阅读。此次 404 Media 的报道揭露了 OpenAI 内部代号为 &\#x27;Project Lily&\#x27; 的项目，其雇用的数百名合同工会直接读取真实 ChatGPT 用户的提示词和完整对话，并可能接触敏感个人信息，同时 Anthropic 也承认采用类似的人工审核做法。

**「影响」** 对于依赖 ChatGPT 处理敏感或私人信息的用户，这一披露意味着其对话内容可能被人工审核员查看，尽管 OpenAI 声称会尝试匿名化，但无法完全保证隐私。这可能导致用户对 AI 服务信任度下降，并促使监管机构和公众更严格审视 AI 公司的数据实践。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.404media.co/inside-project-lily-the-humans-reading-your-chatgpt-chats/">Inside &#x27;Project Lily&#x27;: The Humans Reading Your ChatGPT Chats</a></li>

</ul>
</details>

**标签**: `#ai`, `#privacy`, `#openai`, `#chatgpt`, `#data-handling`

---

<a id="item-tech-news-7"></a>
### [Typesafe.ai 发布 System One 模型与 Jev 快速类型化推理系统](https://typesafe.ai/blog/introducing-system-one-models-and-jev) ⭐️ 7.0/10

Typesafe.ai 发布了新的 System One 模型及其配套系统 Jev，这是一种面向结构化任务（如分类、评分）的快速类型化推理方案。与通用生成式模型不同，Jev 接收任意文本输入（可包含复杂 JSON），并快速回答是非、多选或评分问题。据社区引用的官方文档，其响应为毫秒级，价格约为每百万 token 0.042 美元。该发布以牺牲通用生成能力换取速度与低成本的思路，引发了开发者对其在 CI 自动化、可观测性和回归检测等实际场景中应用的讨论，但其相对生成式模型的优势尚未得到充分验证。

hackernews · albelfio · 9月15日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49717558)

**「背景」** System One 模型是一类为软件系统直接提供快速、结构化决策而设计的 AI 模型，它评估输入状态并返回带类型的答案和概率，而非生成自由文本。Jev 是 TypeSafe（一家位于旧金山的 AI 实验室）推出的首款 System One 旗舰模型，目前处于早期访问阶段。与传统大语言模型不同，Jev 放弃了通用文本生成能力，专注于毫秒级、低成本的类型化推理，但官方宣称的速度与成本优势目前仍主要由厂商自行验证。

**「影响」** 对于需要在 CI 回归、日志分级或可观测性等场景中快速完成结构化判断的开发者，Jev 可能提供比通用生成式大模型更便宜、更快速的替代方案；但其能力仅限于结构化输出，无法像图灵完备的生成模型那样覆盖任意代码生成任务，实际影响仍有待实践检验。

**「社区讨论」** 社区普遍认可这一发布的新颖性，并看好其在 CI 冗余检测、可观测性日志升级等场景的应用，但也有用户质疑与生成式模型的速度对比具误导性，因为后者可输出图灵完备代码而 Jev 仅产生结构化结果。另有用户询问其是否在象棋、魔方等任务上优于大模型，以及结合设计式契约（design-by-contract）模式的可能性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.typesafe.ai/concepts/system-one">System One - TypeSafe AI</a></li>
<li><a href="https://runtimewire.com/article/typesafe-jev-system-one-ai-model-early-access">TypeSafe opens Jev early access for fast, typed AI decisions</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#AI models`, `#fast inference`, `#structured output`, `#developer tools`

---

<a id="item-tech-news-8"></a>
### [会听鸟鸣并绘制 19 世纪风格插画的电子墨水画框](https://github.com/arnegiacomo/fugleramme) ⭐️ 7.0/10

挪威开发者 Arne Munthe-Kaas（GitHub 账号 arnegiacomo）发布了一款开源电子墨水画框项目 fugleramme：它通过 BirdNET 识别周围的鸟鸣，并把检测到的鸟渲染成 19 世纪风格的插画。BirdNET 是一个传统神经网络分类器而非大语言模型，项目将机器学习、电子墨水硬件与生成式艺术融为一体。该项目以源码形式发布在 GitHub 上，并在 Hacker News 上获得了社区的高度关注和大量好评。此前的相关项目如 birdnet-go 也在推动鸟类识别类开源工具的流行，本作品被视为这一趋势的代表之一。

hackernews · arnemunthekaas · 9月15日 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49711544)

**「背景」** 该项目是一个基于树莓派的电子墨水屏相框，通过音频实现实时鸟类检测，AI 完全在本地运行，并将检测到的鸟以手工剪裁的 1800 年代风格插画形式呈现。麦克风将音频馈送给 BirdNET-Go，后者运行 BirdNET 分类器并负责所有检测配置。BirdNET 是一个传统的鸟类鸣声分类神经网络，而非大语言模型。

**「影响」** 对电子墨水屏与鸟类识别领域的爱好者和制作者而言，该项目提供了一个可直接复用的开源范例，展示了如何把 BirdNET 与低功耗显示硬件进行创意结合，并在 Hacker News 上激励了一批同类开发者投身于&\#x27;小巧而奇妙&\#x27;的构建实践。

**「社区讨论」** 社区评论普遍称赞该项目&\#x27;神奇&\#x27;，是近期 Hacker News 上最有启发性的作品之一；有评论澄清 BirdNET 是传统神经网络而非 LLM，并提到其与 birdnet-go 等项目共同带动了一波鸟类相关开源项目，还有人用&\#x27;鸽子携带数据报协议&\#x27;的玩笑呼应这一趋势，另有同为挪威人的评论者称其为&\#x27;纯粹的艺术&\#x27;。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/arnegiacomo/fugleramme">GitHub - arnegiacomo/fugleramme: E-ink bird frame for ...</a></li>
<li><a href="https://arnegiacomo.dev/fugleramme/">Fugleramme - arnegiacomo.dev</a></li>
<li><a href="https://github.com/arnegiacomo/fugleramme/tree/main/docs">fugleramme/docs at main · arnegiacomo/fugleramme · GitHub</a></li>

</ul>
</details>

**标签**: `#bird detection`, `#e-ink`, `#machine learning`, `#hardware`, `#creative coding`

---

<a id="item-tech-news-9"></a>
### [互联网档案馆更新 Wayback Machine 访问防护](https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/) ⭐️ 7.0/10

互联网档案馆（Internet Archive）发布更新称，其 Wayback Machine 服务正遭受高容量自动化爬虫流量的冲击，这些爬虫试图通过访问存档副本绕过对原始网站的封锁，导致服务出现中断。档案馆已部署防护措施以维持服务运行，并指出这种行为不仅给这一重要的非营利互联网基础设施带来负载，还导致部分网站已选择退出存档。此次事件反映出数字保存服务面临的滥用挑战，对依赖该服务的开发者、研究人员及更广泛的网络生态产生直接影响。

hackernews · ChrisArchitect · 9月15日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=49716176)

**「背景」** Wayback Machine 是互联网档案馆（Internet Archive）运营的数字档案服务，该组织是总部位于美国旧金山的一家非营利机构，服务自 2001 年向公众开放，允许用户回溯查看网站过去的样子。近期，这一服务遭受高规模自动化爬虫流量的冲击，这些爬虫试图通过访问存档副本绕开对原始网站访问的限制，迫使互联网档案馆实施保护措施，以确保服务保持可用。

**「影响」** Wayback Machine 的访问中断和部分网站退出存档，将直接影响依赖该服务进行历史数据检索的研究人员、开发者和普通用户。

**「社区讨论」** 评论中，用户对互联网档案馆表示支持与赞赏，认可其维护开放访问的努力；也有人报告了具体的技术问题（如部分电脑持续收到 429 错误而手机可正常访问），并提出了改进建议（记录错误时的系统、浏览器和 IP 信息）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wayback_Machine">Wayback Machine - Wikipedia</a></li>
<li><a href="https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/">An Update on Wayback Machine Access | Internet Archive Blogs</a></li>

</ul>
</details>

**标签**: `#internet archive`, `#web scraping`, `#service reliability`, `#digital preservation`, `#infrastructure`

---

<a id="item-tech-news-10"></a>
### [Gemini 3.8 Live 及 Extended Thinking 发布，强化实时语音与推理](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/) ⭐️ 7.0/10

Google 发布了 Gemini 3.8 Live 和 3.8 Live Extended Thinking，以增强实时语音交互与推理能力。新版本在语音质量、延迟和口音处理上均有改进，并首次支持工作区（Workspace）账号使用，解决了此前账号被搁置的问题。早期社区反馈正面，称其在南非荷兰语等小众语言的实时对话中表现出色，甚至优于 ChatGPT 的语音模式。不过这是一次渐进式更新，公告本身未提供深层技术细节。

hackernews · leumon · 9月15日 17:38 · [社区讨论](https://news.ycombinator.com/item?id=49715947)

**「背景」** Gemini 是 Google 开发的多模态 AI 模型系列，近期发布节奏很快：在 3.7 Flash 推出约三周后发布 3.8 Flash，约两周后又推出 3.8 Live。官方将 Gemini 3.8 Live 和 3.8 Live Extended Thinking 定位为“最先进的实时对话模型”，专为自然对话构建，其中 Extended Thinking 面向高复杂度任务、侧重于增强推理能力。两模型于同一篇博客公告中公布，代表 Google 在实时语音交互路线上将产品线拆分为通用对话与深度推理两个方向。

**「影响」** 对工作区用户而言，此版本意味着可以直接使用 Gemini Live 进行低延迟、高口音适应性的实时对话，此前这类账号往往被排除在最新发布之外。实际使用中，它能服务于语言练习等具体场景，为界面用户带来立即可用的体验提升。

**「社区讨论」** 社区普遍认为这是一次扎实的发布，语音自然、延迟低且能应对浓重口音，但也有用户指出 Gemini 3.8 尚未向 Google AI Plus 用户开放，同时有人询问 Google 何时能超越 Fable 和 Astra，并期待 Gemini 4 的发布时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Gemini 3 . 8 Live &amp; Gemini 3 . 8 Live Extended Thinking</a></li>
<li><a href="https://www.orcarouter.ai/blog/gemini-3-8-live-release">Gemini 3 . 8 Live : Google Splits Its Voice Line in Two</a></li>

</ul>
</details>

**标签**: `#gemini`, `#google-ai`, `#conversational-ai`, `#live-chat`, `#model-release`

---

<a id="item-tech-news-11"></a>
### [美国首次正式确认已部署太空武器](https://www.bbc.com/news/articles/ck790xg41ygro) ⭐️ 7.0/10

美国首次正式确认已在太空部署武器，这是其官方层面首次公开承认此类能力。分析认为，这一确认是重大的地缘政治与军事动向，直接影响卫星基础设施的安全、太空碎片的碰撞风险以及基于太空的技术运行。此表态引发外界对太空军事化趋势的担忧，并使轨道安全与治理议题变得更加紧迫。目前公开信息尚未披露所部署武器的具体类型、数量与作战用途。

hackernews · harporoeder · 9月15日 03:47 · [社区讨论](https://news.ycombinator.com/item?id=49707473)

**「背景」** 1967 年的《外层空间条约》仅禁止在轨部署大规模杀伤性武器（核武器、化学武器和生物武器），而激光、动能撞击器等常规武器在法理上并不被禁止。本次美国首次正式承认在地球轨道部署了太空武器，其对外宣称的目的是防御性保护美国军事力量，但未披露具体武器类型。这标志着美国首次公开承认具备进攻性太空作战能力，也使得关于太空军事化及轨道碎片（如凯斯勒效应）风险的讨论具备了现实依据。

**「影响」** 最直接的影响是，这一官方确认可能促使其他航天国家与私营卫星运营者重新评估轨道资产面临的风险，并推动太空碎片防控与轨道治理议题的加速讨论，但其具体军事后果仍有待进一步公开信息验证。

**「社区讨论」** 多位评论者主张太空应像南极一样保持中立，并援引凯斯勒效应警告碎片连锁碰撞可能长期阻断近地轨道使用；另有评论者注意到中方“敦促美国停止扩军”的表态，并回顾了美军定向能武器与航天飞机等历史项目。评论中还提及美苏曾险些达成废除核武器协议，但因美方坚持发展太空武器而告吹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.yahoo.com/news/politics/articles/us-deployed-space-weapon-air-015206073.html">US confirms for first time it has deployed space weapons - Yahoo</a></li>
<li><a href="https://www.reddit.com/r/news/comments/1wguhwn/us_confirms_for_first_time_it_has_deployed_space/">US confirms for first time it has deployed space weapons - Reddit</a></li>
<li><a href="https://www.youtube.com/watch?v=sW2DvaJwzgo">US confirms weapons in space - YouTube</a></li>

</ul>
</details>

**标签**: `#space weapons`, `#militarization of space`, `#satellites`, `#directed energy`, `#space policy`

---

<a id="item-tech-news-12"></a>
### [数据中心暂停令对美国建设的影响远小于预期](https://newsletter.semianalysis.com/p/everyone-says-datacenter-moratoriums) ⭐️ 7.0/10

SemiAnalysis 分析师 Maya Barkin 撰文，反驳“数据中心暂停令正在扼杀美国建设”这一普遍看法。文章引用具体容量数据指出，尽管有 20GW 的规划容量位于受限的地方边界之内，但真正实际搁浅的容量仅约 1,525MW；若计入纽约，全美受影响容量合计约 2.3GW。作者认为这些数字远低于外界担忧的规模，暂停令对 AI 基础设施与算力建设进度造成的拖累被严重高估。该文作为行业分析机构 SemiAnalysis 的数据驱动观点，为美国能源政策、算力建设与数据中心扩张的争论提供了反方论据。

rss · Semianalysis · 9月15日 20:54

**「背景：美国数据中心暂停令之争」** 近年来，美国各地对大型科技公司数据中心扩建的反对声浪不断升级，已形成全国性的抵制浪潮。在此背景下，多个州和地方政府在短时间内相继出台数据中心暂停令或限制性政策，引发了关于这些措施是否正阻碍美国数据中心建设的广泛讨论。SemiAnalysis 的这篇文章正是针对这一主流叙事提出反驳，并提供具体容量数据作为支持。

**「影响」** 该数据表明，被暂停令实际拖延的数据中心容量（全美含纽约约 2.3GW）远低于外界反复引用的 20GW“受限”规模，因此美国 AI 算力与数据中心建设的延期风险可能明显小于市场普遍预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/everyone-says-datacenter-moratoriums">Everyone Says Datacenter Moratoriums Are Killing the US Buildout .</a></li>
<li><a href="https://www.theguardian.com/us-news/ng-interactive/2026/aug/30/data-center-politics-democrats-republicans">The datacenter backlash is bringing the entire political... | The Guardian</a></li>
<li><a href="https://www.linkedin.com/posts/ai-now-institute_data-center-moratoriums-are-gaining-momentum-activity-7455705309920219136-bJLP">Data center moratoriums are gaining momentum at the local, state ...</a></li>

</ul>
</details>

**标签**: `#datacenter infrastructure`, `#AI infrastructure`, `#energy policy`, `#US technology policy`, `#compute buildout`

---

<a id="item-tech-news-13"></a>
### [44M 参数三元 LLM 仅 19.8MB，CPU 推理约 1900 token/秒](https://www.reddit.com/r/MachineLearning/comments/1wgzpli/i_trained_a_44m_parameter_quantized_llm_from/) ⭐️ 7.0/10

Reddit 用户 Final-Data-1410 发布了 SHADOW-50M，这是一个从零使用 45B token 训练、实际参数为 44M 的三元（ternary）LLM，完整模型仅 19.8MB，在笔记本电脑 CPU 上以约 1,900 token/秒运行，占用约 41MB RAM，并完全离线工作。模型采用 \{-1,0,+1\} 三值权重，73,880 词的词表由固定 512 位指纹而非训练嵌入表示，携带 159KB 编译内核；同一内核编译为 WebAssembly 后可在浏览器中达到约 500 token/秒。当模型判定需要计算时，固定电路会在 \[calc\] 标记处接管并直接填入正确数字，覆盖算术、百分比、日期、星期、单位、计数、排序、比较和小型程序机等任务。其持久记忆机制将注意力状态以每 token 288 字节的 1 位数据写入磁盘，索引每 token 22 字节，检索约需微秒级，100M token 时归档为 28.8GB 加 2.2GB 索引，借助内存映射进程仅用约 28MB RAM，且经强化后重复问题的 top-1 准确率从 0.571 提升到 0.743 而无需训练。作者公开了与 Supra-50M-Reasoning（51.8M 参数、bf16 Llama 风格）的对比：Supra 在 ARC-Easy（0.435 对 0.307）、PIQA（0.600 对 0.570）和 WikiText-2 困惑度（165 对 186）上全面胜出，但 SHADOW 在算术和事实检索等定向任务中表现更好；项目以 MIT 许可发布，附带 GitHub 代码、HuggingFace 权重与浏览器演示链接。

reddit · r/MachineLearning · /u/Final-Data-1410 · 9月15日 12:59

**「背景」** 三元量化将权重压缩到 \{-1,0,+1\} 三种取值，能用极少量存储和计算承载模型，适合边缘设备推理，但其容量通常远逊于传统稠密模型。该作者三周前曾发布 SHADOW-250M（60MB，CPU 约 400 token/秒），能检索磁盘归档但推理与计算能力有限，本次发布的 50M 版本正是为了实验如何在更小体积下改善这两个短板。

**「影响」** 该实验为边缘推理提供了一条可行路径：通过将计算交给固定电路、把持久记忆外置到磁盘与索引，用户可在 20MB 级模型上获得可用的算术与检索能力，社区成员已据此提交了 CUDA 引擎和内置 SHADOW 的 Peppa Pig 智能玩具（约 35 美元、无云无网）等应用，表明这类方案具备实际落地的潜力。

**标签**: `#LLM`, `#quantization`, `#efficient-inference`, `#ternary-weights`, `#edge-computing`

---

<a id="item-tech-news-14"></a>
### [工信部发改委印发“十五五”电子信息制造业规划，聚焦先进制程与国产芯片](https://www.secrss.com/articles/93961) ⭐️ 7.0/10

工业和信息化部与国家发展改革委联合印发《电子信息制造业发展“十五五”规划》，部署 17 项重点任务，明确提出要提高先进制程能力，突破高端手机核心芯片和 PC 高性能芯片，并加强开源鸿蒙等国产操作系统的搭载推广。规划设定到 2030 年规模以上企业营业收入突破 30 万亿元、产业研发投入强度达到 3.5%的目标，同时推进 RISC-V、人工智能芯片和终端、北斗等领域发展。该规划属于高层级产业政策指引，尚未披露具体制程节点、芯片性能指标或实施时间表等细化要求。

telegram · zaihuapd · 9月15日 03:10

**「背景」** 「十五五」是中国国民经济和社会发展的第十五个五年规划期，覆盖 2026 至 2030 年。《电子信息制造业发展“十五五”规划》属于该体系的行业专项规划，由工信部与国家发展改革委联合印发，通常以营业收入、研发投入强度等量化指标为引导，并部署产业重点任务。近年来，受外部出口管制等因素影响，中国持续推动半导体先进制程、核心芯片与国产操作系统的自主研发及生态建设，本规划正是这一政策主轴在 2026 至 2030 年间的延续与加码。

**「影响」** 该规划为 2030 年设定明确的量化目标（规模以上企业营收突破 30 万亿元、研发投入强度达 3.5%），意味着国内晶圆厂、芯片设计企业及鸿蒙生态参与者将据此调整未来数年的研发投资和产能布局，优先攻克先进制程、高端手机和 PC 芯片。对外部供应商而言，随着中国在 RISC-V 等领域加速推进技术自主，其在中国高端芯片和操作系统市场的份额将持续承压。由于这是纲领性文件而非具体产品发布，实际落地程度仍取决于后续配套政策和执行力度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.facebook.com/groups/595424764221375/posts/2350509045379596/">China&#x27;s hardware ecosystem is revolutionizing global innovation</a></li>
<li><a href="https://www.facebook.com/groups/1412540885733722/posts/4988053764849065/">How far will China&#x27;s push for technological independence go?</a></li>

</ul>
</details>

**标签**: `#policy`, `#semiconductors`, `#HarmonyOS`, `#RISC-V`, `#China tech`

---

<a id="item-tech-news-15"></a>
### [桑德斯提案拟禁超级智能 AI 并设刑责](https://www.techspot.com/news/113831-new-bernie-sanders-bill-would-ban-superintelligent-ai.html) ⭐️ 7.0/10

美国参议员伯尼·桑德斯与众议员卡萨尔联合提出《禁止人工超级智能法案》，拟永久禁止开发和部署超级智能 AI，并在联邦监管机构出台安全规则前暂停先进 AI 开发。违规个人将面临最高 20 年监禁，企业则可能遭受“公司死刑”式的处罚。法案还提出设立内阁级机构，监视前沿 AI 系统在各阶段的危险能力，并监督这些能力的清除。此外，法案推动达成国际协议，以便在全球范围内阻止超级智能的出现。目前该法案仅为提案，尚未进入立法生效阶段，但其刑事追责设计对 AI 研究机构、工程师和相关企业具有直接的合规影响。

telegram · zaihuapd · 9月15日 04:26

**「背景」** 所谓超级智能 AI，通常指在几乎所有认知任务上远超人类水平、尚无实际部署的前瞻性技术概念。佛蒙特州参议员桑德斯长期以来是反对不受监管 AI 和超级智能竞赛的代表人物，此前已多次就 AI 治理提出立法倡议。该法案是美国联邦层面 AI 监管辩论的一部分，目前各方在如何平衡技术创新与安全风险上仍存在广泛分歧。

**「影响」** 该法案若最终通过，将直接约束美国前沿 AI 实验室与研究人员：在联邦监管机构制定安全规则之前暂停先进 AI 开发，违规个人最高面临 20 年监禁，涉事企业可能被吊销经营资格（“公司死刑”），并需配合新设的内阁级机构监控和清除前沿系统的危险能力。不过，该法案目前仅为提案，须经国会立法程序方能生效，因此对现有研发节奏的实际影响仍取决于后续审议结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bitcoinfoundation.org/news/ai/sanders-pushes-permanent-us-superintelligent-ai-ban-with-20-year-prison-terms/">Sanders Pushes Permanent US Superintelligent AI Ban With...</a></li>
<li><a href="https://futurism.com/artificial-intelligence/bernie-sanders-banning-superintelligent-ai-imprisoning-developers-20-years">Bernie Sanders Proposes Banning Superintelligent AI and...</a></li>
<li><a href="https://www.techspot.com/news/113831-new-bernie-sanders-bill-would-ban-superintelligent-ai.html">New Bernie Sanders bill would ban superintelligent AI ... | TechSpot</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#regulation`, `#legislation`, `#superintelligent AI`, `#AI safety`

---

<a id="item-tech-news-16"></a>
### [字节 ADrive 与腾讯网盘竞逐，AI 智能网盘战争升温](https://www.36kr.com/p/3984022571964039) ⭐️ 7.0/10

字节跳动宣布将于本月发布独立企业级智能网盘 ADrive，目前已开放试用申请，产品定位为面向 AI 智能体与人类协同办公的工具，支持统一存储、团队协作、自然语言检索及智能文件处理。与此同时，腾讯云已于 2026 年 6 月启动全新

telegram · zaihuapd · 9月15日 06:47

**「背景」** 传统网盘市场长期以容量、下载速度等基础功能为主要竞争点，被称为“容量竞赛”。随着大模型与智能体技术成熟，网盘厂商开始将 AI 能力融入文件管理，转向智能检索、自动分类、团队协同与数据资产备份等场景。腾讯网盘与字节跳动的 ADrive 接连落地，标志着网盘赛道正从单纯的存储工具转向 AI 智能协同与数据赋能的竞争阶段。

**「影响」** 字节跳动与企业级产品 ADrive 以及腾讯面向个人和企业用户的“腾讯网盘”相继入局，将直接加速国内云盘市场从“工具型”向“智能化平台”的转型，而该市场 2024 年规模已达 50.18 亿元、同比增速达 27.78%；在当前向量数据库成本下降与 RAG 架构成熟的背景下，AI 能力已成为新的竞争焦点，缺乏相关技术底座改造能力的现有云盘厂商将面临被边缘化的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8wRFrA3gu4J">字 节 将发布独立 智 能 网 盘 “ ADrive ”， 腾 讯 网 盘 先已布局， 网 盘 AI 大战打响</a></li>
<li><a href="https://www.360why.com/industry/260711000010721.html">2026年个人云盘行业研究：50.18亿元市场规模与27.78%增速分析 - 热点...</a></li>
<li><a href="https://blog.csdn.net/byoass/article/details/161488401">企业云盘AI能力横评：2026年五大产品深度对比-CSDN博客</a></li>

</ul>
</details>

**标签**: `#cloud storage`, `#AI`, `#ByteDance`, `#Tencent`, `#collaboration`

---