---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 36 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [Gemini 3.7 Flash 发布，多模态推理新突破](#item-tech-news-1) ⭐️ 9.0/10
2. [Firefox 成为唯一支持 uBlock Origin 的主流浏览器](#item-tech-news-2) ⭐️ 8.0/10
3. [GLM-5.3 展示编码与零日漏洞挖掘能力](#item-tech-news-3) ⭐️ 8.0/10
4. [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](#item-tech-news-4) ⭐️ 8.0/10
5. [苹果联手阿里自研中国 AI 大模型，或成首个获批外企](#item-tech-news-5) ⭐️ 8.0/10
6. [Qwen 3.8 27B FP8 开源模型发布：本地推理能力突出](#item-tech-news-6) ⭐️ 7.0/10
7. [Claude Opus 5 使用体验退化：开发者抱怨表达迂回、过度坦白](#item-tech-news-7) ⭐️ 7.0/10
8. [RustDesk 实现 Wayland 真正无人值守远程访问](#item-tech-news-8) ⭐️ 7.0/10
9. [不要分类，要幻觉！用 LLM 生成候选标签再映射](#item-tech-news-9) ⭐️ 7.0/10
10. [oncothresh：临床阈值下的肿瘤学 AI 模型评估](#item-tech-news-10) ⭐️ 7.0/10
11. [torch-preflight: 一款用于 PyTorch 代码的静态检查工具](#item-tech-news-11) ⭐️ 7.0/10
12. [苹果提交外部购买抽成方案，费率最高 15%](#item-tech-news-12) ⭐️ 7.0/10
13. [谷歌被令简化第三方应用商店安装](#item-tech-news-13) ⭐️ 7.0/10
14. [PostgreSQL 修复高危 to\_char 漏洞](#item-tech-news-14) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Gemini 3.7 Flash 发布，多模态推理新突破](https://zeli.app/zh/digest/2026-08-13) ⭐️ 9.0/10

Google 正式推出 Gemini 3.7 Flash，这是 Gemini 3 系列中最新、性能最强的原生多模态推理模型。该模型原生支持文本、图像、视频、音频和 PDF 等多种输入格式，输入 token 上限高达 104 万，输出上限为 6.5 万。它全面支持代码执行、文件搜索、函数调用以及基于 Google Maps 的地理 grounding，并引入了可调节强度的 Thinking 模式（低、中、高三档，但不支持 minimal 模式）。虽然暂不支持音频生成、图像生成及 Live API，但其强大的上下文处理能力和工具调用能力使其成为构建复杂智能体的理想选择。

rss · Zeli · 8月13日 23:59

**「背景」** 多模态模型能够同时理解和处理文本、图像、音频等多种数据形式，而推理能力则让模型在给出答案前进行链式思考或调用工具，大幅提升复杂任务的可靠性。Google 的 Gemini 系列是其对标 OpenAI 等前沿模型的多模态产品线，近期持续迭代，旨在通过更大的上下文窗口和更丰富的工具集成来增强智能体应用。

**「影响」** 对于需要处理海量上下文、整合多种工具并执行复杂推理的开发者，Gemini 3.7 Flash 提供了更强大的构建基块，但音频和图像生成能力的缺失可能限制其在某些创意应用中的直接使用。

**标签**: `#AI`, `#machine learning`, `#open source`, `#tech industry`, `#software engineering`

---

<a id="item-tech-news-2"></a>
### [Firefox 成为唯一支持 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

随着 Chrome 转向 Manifest V3，Firefox 成为最后一个完整支持 uBlock Origin 扩展的主流浏览器。uBlock Origin 依赖的 webRequest 拦截 API 在 Manifest V3 中被限制，改用受限的 declarativeNetRequest，导致其功能在 Chrome 和 Edge 上大幅缩减。Firefox 不仅保留了对旧 API 的支持，还会对每次更新进行人工审核，防止恶意代码注入。这一变化凸显了浏览器扩展自由度与隐私保护之间的技术分歧，也促使部分开发者如 Sitetruth 和 Ad Limiter 的维护者放弃 Chrome 平台。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**「背景」** uBlock Origin 是一款开源广告拦截扩展，支持大量过滤规则，其强大功能依赖于浏览器扩展的 Manifest V2 API 提供的网络请求拦截能力。Google Chrome 自 2024 年起逐步转向 Manifest V3，该版本限制了声明式网络请求规则，导致 uBlock Origin 只能以功能受限的 uBlock Origin Lite 版本运行。目前，Firefox 仍维持对 Manifest V2 的全面支持，因此成为唯一能完整运行 uBlock Origin 的主流浏览器。

**「影响」** 依赖完整广告拦截功能的用户现只能选择 Firefox 作为主要浏览器；Chrome 和 Edge 用户需改用功能受限的 uBlock Origin Lite，但部分用户反馈仍无明显广告。

**「社区讨论」** 社区普遍认为 Firefox 是自由拦截广告的最后堡垒，部分用户赞赏其代码审查机制；但也有评论指出 uBlock Origin Lite 在 Edge 上已能有效屏蔽广告，对 Manifest V2 支持的依赖存疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://factually.co/fact-checks/technology/manifest-v3-ad-blockers-ublock-origin-brave-firefox-2026-16ed91">How Manifest V 3 Changed Ad Blockers: uBlock Origin , Br...</a></li>

</ul>
</details>

**标签**: `#browsers`, `#firefox`, `#ad-blocking`, `#manifest-v3`, `#privacy`

---

<a id="item-tech-news-3"></a>
### [GLM-5.3 展示编码与零日漏洞挖掘能力](https://z.ai/blog/glm-5.3) ⭐️ 8.0/10

GLM-5.3 是智谱 AI 在 GLM-5.2 基础上通过后训练增强的模型，在编码和网络安全领域展现出新兴能力，能够自主发现零日漏洞并执行红队攻击任务。该模型在 Claude Code 等环境中成功完成了包含 WordPress 插件远程代码执行和 Linux 6.8 内核漏洞利用的实战，获得用户高度评价。智谱同步推出漏洞披露计划（cvd.z.ai），大规模扫描开源软件并已发现多个高危 CVE 漏洞，涵盖多个流行项目。尽管模型仍略逊于 Sol 和 Fable 等前沿成果，但其在漏洞利用链基准测试上的表现已较为接近，显示出实用化潜力。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**「背景」** GLM-5.3 是智谱（Z.ai）发布的大型语言模型，基于与 GLM-5.2 相同的 743B 参数基础模型，所有能力提升均来自大规模后训练。该模型以开放权重形式发布，重点关注编程、智能体任务，并在网络安全领域展现出超越训练预期的涌现能力。

**「影响」** 该模型显著降低了自动化漏洞发现与利用的门槛，可能加速攻防双方的技术演进，但其大规模扫描并快速披露漏洞的做法也引发了关于伦理与披露节奏的讨论。

**「社区讨论」** 社区讨论热烈，用户分享了在红队任务中成功使用 GLM-5.3 的经验，并指出其能力接近 Sol 和 Fable 等顶尖模型，但经济性仍不足以替代 OpenAI。同时，社区对模型大规模扫描开源软件并披露漏洞的做法表示关注，认为此类扫描成本正在快速下降，可能导致漏洞发现速度超出修复能力，类似 Anthropic 的 Project Glasswing 也在推进类似方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/glm-5-3-launch-cyber-defense-benchmarks-august-2026">GLM-5.3 Launch: Benchmarks, Pricing &amp; Access (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://x.com/Zai_org/status/2088132965922476159">Introducing GLM-5.3: Built to Code. Ready for Cyber ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#coding`, `#GLM`, `#vulnerability-discovery`

---

<a id="item-tech-news-4"></a>
### [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note preview，这是 dots3 系列首个开放权重模型。该模型总参数 280B，采用 MoE 架构每次仅激活 16B 参数，支持 512K 上下文，可处理文字、图像、视频和音频等多模态输入。模型引入了 TEMPO 强化学习方法，通过自批判和测试时价值估计训练长程智能体。权重已在 Hugging Face 开源，并同步发布了 VibeSearchBench 和 VibeLifeBench 两个真实场景智能体基准。

telegram · zaihuapd · 8月14日 08:27

**「背景」** Mixture of Experts（MoE）架构通过每次仅激活部分专家网络来降低推理成本，使大模型能在保持海量总参数的同时控制计算量。dots3-note 的 512K 上下文长度远超大多数开源模型，能够处理超长文档和多模态内容。TEMPO 是一种新的强化学习方法，利用自批判和测试时价值估计来训练智能体执行长序列任务。

**「影响」** AI 研究者和工程师能够基于该开源模型探索高效推理与长上下文智能体，且 TEMPO 方法和新基准可能推动强化学习在真实场景中的应用。

**标签**: `#AI`, `#open-source`, `#MoE`, `#multi-modal`, `#reinforcement learning`

---

<a id="item-tech-news-5"></a>
### [苹果联手阿里自研中国 AI 大模型，或成首个获批外企](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

苹果已专门为中国市场训练一款自研大语言模型，并获得阿里巴巴的支持，一改此前依赖第三方模型的策略。该模型已在上月完成中国网信办生成式 AI 服务备案，预计未来数月随 iOS 更新上线，Apple Intelligence 亦将借此落地。若最终获批，苹果将成为首个获北京许可、在华提供自有 AI 模型的外国公司，这标志着外企在中国 AI 监管下的重要突破。

telegram · zaihuapd · 8月14日 14:47

**「背景」** 苹果此前在中国市场依赖第三方 AI 模型提供服务，但为满足中国对生成式 AI 的监管要求并更好地掌控用户体验，现已转向自研大语言模型。该模型在阿里巴巴的支持下训练，并已于上月在中国网信办完成生成式 AI 服务备案，为 Apple Intelligence 在华落地扫清了关键合规障碍。

**「潜在影响」** 苹果已在中国网信办完成生成式 AI 服务备案，若后续落地，将成为首个获准在华提供自有 AI 模型的外国公司，为其将 Apple Intelligence 引入中国 iPhone 市场扫清关键合规障碍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/980160/apple-intelligence-china-custom-ai-model-alibaba">Apple trained its own AI model for China with help from Alibaba | The Verge</a></li>
<li><a href="https://enterpriseai.economictimes.indiatimes.com/amp/news/industry/apple-takes-alibabas-support-for-training-china-specific-ai-model-report/133232437">Apple takes Alibaba’s support for training China-specific AI model: Report, ETEnterpriseai</a></li>
<li><a href="https://enterpriseai.economictimes.indiatimes.com/amp/news/industry/apple-takes-alibabas-support-for-training-china-specific-ai-model-report/133232437">Apple takes Alibaba’s support for training China-specific AI model: Report, ETEnterpriseai</a></li>
<li><a href="https://www.latestly.com/technology/apple-taps-alibaba-for-china-ai-model-boosts-apple-intelligence-7559965.html/amp">Apple Develops Custom AI Model for China With Alibaba Support Ahead of Apple Intelligence Launch | 📲 LatestLY</a></li>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/980160/apple-intelligence-china-custom-ai-model-alibaba">Apple trained its own AI model for China with help from Alibaba | The Verge</a></li>

</ul>
</details>

**标签**: `#Apple`, `#China`, `#AI regulation`, `#large language models`, `#Alibaba`

---

<a id="item-tech-news-6"></a>
### [Qwen 3.8 27B FP8 开源模型发布：本地推理能力突出](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 7.0/10

Qwen 3.8 27B FP8 是通义千问系列最新开源模型，采用 FP8 量化，可在本地硬件上运行。该模型在推理能力上表现突出，成为继 Gemma 4 之后第二个通过特定私有基准测试的本地模型，但推理过程消耗了 5 倍于 Gemma 4 的 tokens，且 VRAM 使用效率较低。社区反馈显示，模型在思维链中采用了简化的笔记式表达（如省略‘to’‘we’等词），疑似影响多令牌预测（MTP）性能。同时，Jinja 模板配置存在问题，需手动修复才能正确控制推理行为。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**「背景」** Qwen 3.8 是阿里巴巴通义实验室发布的 Qwen 系列模型的新版本，其中 27B 参数量的密集模型是本次更新的重点之一。FP8 表示该模型采用 8 位浮点量化，可在消费级硬件上实现本地推理，同时保持较高的性能。该模型基于混合注意力骨干架构，与同系列的 MoE 旗舰模型共享技术基础，专注于提升推理能力与本地部署效率。

**「影响」** 对于需要本地运行且重视推理准确性的任务，Qwen 3.8 27B FP8 提供了优于多数现有本地模型的推理表现，但伴随更高的计算开销和 VRAM 占用，可能限制实际部署。

**「社区讨论」** 社区认可其推理能力提升，但担忧高 token 消耗和 VRAM 效率，并指出 Jinja 模板配置错误需手动修复；此外，有用户赞赏其绘画能力，但思维链风格的改变可能影响性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B-FP8">Qwen / Qwen 3 . 8 - 27 B - FP 8 · Hugging Face</a></li>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.8-27B">Qwen / Qwen 3 . 8 - 27 B | vLLM Recipes</a></li>

</ul>
</details>

**标签**: `#qwen`, `#llm`, `#open-source`, `#model-release`, `#reasoning`

---

<a id="item-tech-news-7"></a>
### [Claude Opus 5 使用体验退化：开发者抱怨表达迂回、过度坦白](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

近日，大量开发者反馈 Claude Opus 5 的写作风格明显退化，表现为句子绕弯、用词抽象、突然抛出结论，甚至频繁“坦白”错误、过度沟通，导致使用体验极为疲惫。部分用户已被迫退回 Opus 4.8 或转向 OpenAI 的 Sol 模型，认为后者更易协作。讨论帖分析认为，Opus 5 的后训练可能已从面向人类转为面向 AI 代理之间的通信，使得人类交流的细微之处被视为干扰。该帖在 Hacker News 上获得 723 分和 659 条评论，反映出这一问题在开发者群体中引起了广泛共鸣。

hackernews · numeri · 8月14日 10:12 · [社区讨论](https://news.ycombinator.com/item?id=49296740)

**「背景」** Claude Opus 5 是 Anthropic 于 2026 年 7 月 24 日推出的旗舰大语言模型，定价为每百万 tokens 输入 5 美元、输出 25 美元，与此前的 Opus 4.8 持平。该模型面向复杂推理、编码和长时间智能体工作，在 CursorBench 3.2 等基准测试中性能接近 Anthropic 最强的 Fable 5，但任务成本仅为其一半左右。

**「影响」** 对于依赖 Claude Opus 5 进行日常开发的用户，这一变化直接导致生产力下降和精神疲劳，迫使部分人迁移至旧版本或竞品模型。

**「社区讨论」** 多数评论与作者共鸣，指出 Opus 5 的迂回表达和“坦白”式沟通令人疲惫，有人推测这是模型优化目标转向代理间通信的结果；也有用户分享了诸如“反空洞地板蒙蔽了空洞案例之门”等极端案例，并强调无严格指令时模型会偏离方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/anthropic/claude-opus-5">Claude Opus 5 - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://luwai.fr/en/resources/claude-opus-5-cout-agents-ia-pme-2026-07-26">Claude Opus 5 : Anthropic &#x27;s Most Capable AI Model in 2026</a></li>
<li><a href="https://ccleaks.com/news/claude-opus-5-launch-july-2026">Claude Opus 5 Anthropic launch on July 24 at $5/$25 | ccleaks News</a></li>

</ul>
</details>

**标签**: `#AI`, `#developer-tools`, `#large-language-models`, `#user-experience`, `#Claude`

---

<a id="item-tech-news-8"></a>
### [RustDesk 实现 Wayland 真正无人值守远程访问](https://rustdesk.com/blog/unattended-remote-access-wayland/) ⭐️ 7.0/10

RustDesk 现在为 Wayland 会话提供了真正的无人值守远程访问功能，解决了此前 Linux 用户在此类环境下无法进行预登录远程控制的主要痛点。该更新使得 RustDesk 服务能够在 Wayland 显示服务器上以系统服务方式运行，无需用户事先登录桌面，便可直接连接远程会话。这一改进对依赖 RustDesk 进行远程维护、服务器管理或远程工作的开发者与系统管理员尤为重要，因为 Wayland 已在主流 Linux 发行版中逐渐取代 X11。

hackernews · rustdesk · 8月14日 16:12 · [社区讨论](https://news.ycombinator.com/item?id=49300759)

**「背景」** RustDesk 是一款开源远程桌面工具。Wayland 是 Linux 桌面环境逐步取代 X11 的现代显示协议，其安全设计导致远程桌面 API 需要用户在本地会话中明确授权，因此长期难以实现无人值守的远程访问。RustDesk 通过直接与内核层交互（如利用 PipeWire 和屏幕捕获门户），绕过了这一限制，实现了在登录界面（GDM）和冷重启后无需用户干预的远程连接。

**「影响」** 对于使用 Wayland 的 Linux 用户，尤其是需要维护无头服务器或远程工作站的开发者和系统管理员，现在可以依赖 RustDesk 实现无需物理干预的完全远程管理。

**「社区讨论」** 社区普遍认为该更新及时解决了长期存在的痛点，许多用户表示欢迎。然而，有评论指出 RustDesk 在自托管时仍缺乏加密连接支持，这引发了安全方面的担忧；另有用户就其与 VNC 及 Remmina 等工具的差异和性能表现进行提问，反映出对远程桌面方案选择的持续讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustdesk.com/blog/unattended-remote-access-wayland/">Unattended Remote Access on Wayland with RustDesk — RustDesk</a></li>
<li><a href="https://sourcefeed.dev/a/to-crack-wayland-rustdesk-went-straight-to-the-kernel">To Crack Wayland , RustDesk Went Straight to the... — SourceFeed</a></li>

</ul>
</details>

**标签**: `#remote-desktop`, `#wayland`, `#rustdesk`, `#open-source`, `#software-engineering`

---

<a id="item-tech-news-9"></a>
### [不要分类，要幻觉！用 LLM 生成候选标签再映射](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 7.0/10

Simon Willison 介绍了一种处理大型标签集的实用技巧：当标签过多（如他博客的 1856 个标签）无法完全放入 LLM 上下文时，让模型直接“幻觉”出全新的候选标签，然后利用向量嵌入将生成的标签映射到现有标签集中距离最近的标签。该方法源自 Doug Turnbull，通过提示词示例（如家居分类层级）引导模型输出符合分类体系形状的标签，再通过嵌入相似度完成匹配，从而避免直接要求模型从庞大标签列表中做选择。

rss · Simon Willison · 8月14日 21:54

**「背景」** 传统上，使用 LLM 对内容进行分类需要将全部候选标签提供给模型，但当标签数量超出上下文窗口限制时便无法直接使用。Doug Turnbull 提出的方案是先让模型自由生成新标签，再借助向量嵌入在这些生成标签与已有的真实标签之间建立语义映射，从而绕开了上下文长度的瓶颈。

**「影响」** 拥有大量标签的开发者可以借此技术，在不缩减标签集的前提下，利用 LLM 实现自动标签匹配，并通过向量嵌入保证映射的准确性。

**标签**: `#LLMs`, `#tagging`, `#vector-embeddings`, `#classification`, `#software-engineering`

---

<a id="item-tech-news-10"></a>
### [oncothresh：临床阈值下的肿瘤学 AI 模型评估](https://www.reddit.com/r/MachineLearning/comments/1vod2c8/opensource_python_library_nocode_web_dashboard/) ⭐️ 7.0/10

开源 Python 库 oncothresh 及其配套的无代码网页仪表盘，专为在固定临床决策阈值上评估肿瘤学 AI 模型而设计，提供了灵敏度、特异度、阳性预测值、阴性预测值、bootstrap 置信区间、阈值敏感度曲线、边界校准和决策曲线净收益等指标。该工具弥补了现有基准（如 PathBench）只关注全局指标而忽略阈值特异性评估的空白，其库本身依赖轻量（numpy/scipy/scikit-learn/pydantic），仪表盘则通过 Docker Compose 本地运行，无需云端依赖。目前项目处于 v0.1 阶段，作者欢迎社区反馈。

reddit · r/MachineLearning · /u/adom2989 · 8月14日 17:06

**「背景」** 许多肿瘤学 AI 模型输出连续值，但在临床决策中需根据固定阈值（如肿瘤细胞密度、Ki-67、PD-L1 评分）将结果二值化为“是/否”，以决定是否进行活检或治疗。传统评估指标如 AUC、ICC、MAE 衡量的是整体一致性，无法反映模型在具体工作点上（即决策阈值处）的可靠性。oncothresh 正是针对这一缺口，提供阈值特异性的评估与不确定性量化。

**「影响」** 该工具使肿瘤学 AI 模型的开发者和研究人员能直接评估模型在临床决策阈值上的表现和不确定性，提升了模型在实际诊疗流程中评估的精准性，弥补了现有通用基准的不足。

**标签**: `#machine-learning`, `#open-source`, `#healthcare`, `#python`, `#model-evaluation`

---

<a id="item-tech-news-11"></a>
### [torch-preflight: 一款用于 PyTorch 代码的静态检查工具](https://www.reddit.com/r/MachineLearning/comments/1vo8vv0/a_linter_for_pytorch_torchpreflight_p/) ⭐️ 7.0/10

作者发布了 torch-preflight，一个针对 PyTorch 训练代码的静态检查工具（linter），无需导入或执行代码即可检测常见错误。它能发现诸如在循环中追加损失（losses.append\(loss\)）导致计算图累积、循环内缺少 zero\_grad\(\)、梯度累积时未除以累积步数、以及在 DDP 中未使用 DistributedSampler 等 13 条规则所覆盖的 GPU 资源浪费问题。该工具还提供 VRAM 估算功能，只需指定训练脚本和目标 GPU，就能在启动实例前预判运行是否适配，并给出节省显存的修改建议及对应的 GiB 数。目前项目仍在早期阶段，已通过 pip 发布，作者在四个模型和一块 T4 上的测试显示内存估算误差在 4% 以内，并希望社区反馈以降低误报。

reddit · r/MachineLearning · /u/LeJanbandhu · 8月14日 14:30

**「背景」** 在 PyTorch 训练中，一些看似无害的代码习惯（如将损失张量直接追加到列表）会保留整个自动求导图，导致显存耗尽；梯度累积时若忘记按累积步数缩放损失，则等效于增大学习率，影响训练正确性。静态检查工具（linter）可以在不执行代码的情况下通过模式匹配或抽象解释发现这类问题，从而节省 GPU 小时和成本。

**「影响」** 对于 PyTorch 开发者，尤其是经常在云 GPU 上运行训练任务的用户，torch-preflight 有望在提交任务前发现易被忽略的内存泄漏和逻辑错误，直接减少因程序崩溃或错误训练而浪费的 GPU 费用。

**标签**: `#PyTorch`, `#linter`, `#debugging`, `#VRAM estimation`, `#deep learning`

---

<a id="item-tech-news-12"></a>
### [苹果提交外部购买抽成方案，费率最高 15%](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

苹果向美国法院提交了针对 App Store 外部购买的新佣金方案，标准应用抽成 15%，视频、新闻等合作项目及订阅续费 10%，小型企业计划应用 5%。该方案是苹果与 Epic Games 法律纠纷的延续，此前美国最高法院驳回了苹果暂停费率审理的请求。Epic 将有机会回应，苹果计划在 9 月 14 日前向最高法院提交书面意见。

telegram · zaihuapd · 8月14日 02:33

**「背景」** 苹果与 Epic Games 的长期诉讼中，美国法院要求苹果允许开发者引导用户使用 App Store 以外的支付方式，同时裁定苹果可对这些外部购买收取佣金，以补偿其知识产权和平台服务。为此，苹果向法院提交了具体的佣金费率提案，作为确定合理收费的法律程序的一部分。\[tool-1-1\]

**「影响」** 苹果提出的外部购买抽成方案将直接影响美国 App Store 开发者选择外部购买的经济考量，其中标准应用抽成 15%，小型企业计划 5%。然而，该方案尚需法院审理，Epic 的反对可能影响最终费率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/">Apple proposes commissions of up to 15 % for off - App Store ...</a></li>

</ul>
</details>

**标签**: `#apple`, `#app-store`, `#commissions`, `#epic-games`, `#technology-industry`

---

<a id="item-tech-news-13"></a>
### [谷歌被令简化第三方应用商店安装](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 7.0/10

美国地区法官 James Donato 下令谷歌在一周内取消 Play 商店中安装第三方安卓应用商店的多余警告弹窗和步骤，使安装流程与普通应用一致。法院认定这些多步操作是蓄意制造的“反竞争摩擦”，旨在吓退用户。该指令源自 Epic 诉谷歌反垄断案，陪审团此前已裁定谷歌在安卓应用分发市场构成非法垄断。

telegram · zaihuapd · 8月14日 09:55

**「案件背景」** 该命令源于 Epic Games 诉谷歌反垄断案，此前陪审团裁定谷歌在安卓应用分发上构成非法垄断。法官 James Donato 认定谷歌在 Play Store 中为第三方应用商店安装设置的额外警告和步骤是“反竞争摩擦”，旨在吓退用户并阻碍竞争。第九巡回上诉法院此前已就谷歌 Play Store 的垄断行为作出相关裁决。

**「影响」** Android 用户在安装第三方应用商店时将不再面对多余警告步骤，安装流程与普通应用无异，可能促进应用商店竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/08/google-ordered-to-make-it-easier-to-download-alternative-android-app-stores/">Judge gives Google one week to fix &quot;anticompetitive&quot; app store download in Google Play - Ars Technica</a></li>
<li><a href="https://www.mobilemarketingreads.com/judge-orders-google-to-remove-barriers-to-rival-app-store-installs-on-google-play/">Judge orders Google to remove barriers to rival app store installs on Google Play</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Android`, `#app stores`, `#Google`, `#legal`

---

<a id="item-tech-news-14"></a>
### [PostgreSQL 修复高危 to\_char 漏洞](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 7.0/10

PostgreSQL 项目披露高危漏洞 CVE-2026-14669，CVSS 评分 8.8。该漏洞源于 to\_char\(timestamptz\) 函数在处理超长 POSIX 时区缩写时存在堆缓冲区溢出，使已获得低权限数据库账户的攻击者能够以 PostgreSQL 服务进程的操作系统权限执行任意代码。受影响版本为 PostgreSQL 18.5、17.11、16.15、15.19 及 14.24 之前的所有版本，但 18.5 因回归问题未正式发布，因此 18 系列用户需直接升级至 18.6，其他版本用户分别升级至 17.11、16.15、15.19 或 14.24。本次小版本更新无需转储数据库或运行 pg\_upgrade，更新程序文件并重启服务即可完成修复。

telegram · zaihuapd · 8月14日 14:35

**「背景」** to\_char 是 PostgreSQL 中将时间戳格式化为字符串的函数，其内部会根据时区设置将 timestamptz 转换成对应时区的时间表示。如果用户能够设置一个超长的 POSIX 时区缩写，该缩写在被处理时可能导致固定大小的堆缓冲区溢出，从而破坏内存。

**「影响」** 拥有低权限数据库账户的攻击者可通过构造恶意时区值，利用此堆溢出漏洞以 PostgreSQL 服务进程权限执行任意代码，进而完全控制数据库服务器。

**标签**: `#security`, `#PostgreSQL`, `#vulnerability`, `#database`, `#CVE`

---