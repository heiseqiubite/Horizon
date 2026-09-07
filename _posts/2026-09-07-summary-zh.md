---
layout: default
title: "Horizon Summary: 2026-09-07 (ZH)"
date: 2026-09-07
lang: zh
---

> 从 36 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [不披露使用 AI 写作是否不诚实](#item-tech-news-1) ⭐️ 8.0/10
2. [Asahi Linux 正式支持 Apple M3](#item-tech-news-2) ⭐️ 8.0/10
3. [欧洲私营火箭首次入轨，Isar Aerospace 创历史](#item-tech-news-3) ⭐️ 8.0/10
4. [OpenAI 论人工智能心智的异质性](#item-tech-news-4) ⭐️ 8.0/10
5. [OpenAI 将递归自我改进定为 AGI 方向，内部编码代理支出激增](#item-tech-news-5) ⭐️ 8.0/10
6. [DNS 新域名注册近两成为诈骗，滥用问题凸显](#item-tech-news-6) ⭐️ 8.0/10
7. [长鑫科技 DRAM 市占率升至 10%](#item-tech-news-7) ⭐️ 8.0/10
8. [微软发布开发者精简版 Windows 11 Project Zenith](#item-tech-news-8) ⭐️ 8.0/10
9. [Nitter 与 XCancel 获法律建议后恢复服务](#item-tech-news-9) ⭐️ 7.0/10
10. [微软工程师称手搓代码时代结束，开发转向 AI 与 WinUI 3](#item-tech-news-10) ⭐️ 7.0/10
11. [F-Droid 拟采纳 Debian 生成式 AI 政策，明确贡献者责任](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenAI 发布 Astra 后多次改动评测数据，幻觉率先降后恢复](#item-tech-news-12) ⭐️ 7.0/10
13. [中国首款 AI 辅助创新药获批上市](#item-tech-news-13) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [不披露使用 AI 写作是否不诚实](https://bcantrill.dtrace.org/2025/12/05/your-intellectual-fly-is-open/) ⭐️ 8.0/10

Bryan Cantrill 在 2025 年 12 月发表文章指出，不披露使用大型语言模型（LLM）进行写作是不诚实的，因为 LLM 是糟糕的写作者，无法反映作者的身份和个性。他认为写作是思考的过程，若由 LLM 代笔，既会削弱文章的独特性，也可能掩盖作者的真实观点。这篇文章引发了关于 AI 写作、披露义务以及“写作即思考”这一概念的广泛讨论。作者特别强调，即使 LLM 文本质量再高，也不能替代作者本人的声音和思考痕迹。

hackernews · cyb0rg0 · 9月6日 11:56 · [社区讨论](https://news.ycombinator.com/item?id=49585644)

**「背景」** Bryan Cantrill 是美国资深软件工程师，曾任职于 Sun Microsystems 及其收购方 Oracle 公司，并长期以演讲和文章探讨软件工程中的信任、问责等议题。在这篇发表于 2025 年 12 月的文章中，他论证了使用大语言模型（LLM）写作却不加以披露的做法在智力上的不诚实性，理由是 LLM 并不擅长写作，也无法反映作者本人的风格与身份。

**「影响」** 这篇文章对依赖 LLM 进行写作而不加披露的软件工程师和内容创作者提出了直接挑战，可能促使他们重新审视技术写作中的披露规范与信任建立。

**「社区讨论」** 评论者中，有人赞同“写作即思考”的观点，指出写作过程中的自我修正必不可少；也有人质疑“因为 LLM 写得差所以不披露”的论证，认为若未来 LLM 写得足够好，该逻辑便不成立。另有评论强调个人风格在博客中的重要性，并用餐厅类比说明带 AI 创作的无个性内容会损害阅读体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bryan_Cantrill">Bryan Cantrill - Wikipedia</a></li>
<li><a href="https://www.youtube.com/watch?v=WF7J7qtZ8TA">Trust as Infrastructure | Bryan Cantrill | Monktoberfest 2025 - YouTube</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#LLM writing`, `#intellectual honesty`, `#software engineering`, `#Bryan Cantrill`

---

<a id="item-tech-news-2"></a>
### [Asahi Linux 正式支持 Apple M3](https://asahilinux.org/2026/09/m2-episode-1/) ⭐️ 8.0/10

Asahi Linux 宣布正式支持 Apple M3 芯片，这是 Linux 在 Apple Silicon 硬件上运行的重要里程碑。该支持通过官方安装程序提供，为开发者和用户在 M3 设备（如 MacBook Pro 和 Mac Studio）上安装 Linux 铺平了道路。虽然具体版本和安装细节尚未公布，但社区反响热烈，该消息在 Hacker News 上获得了大量讨论。此进展意味着 M3 用户可期待更完整的 Linux 体验，不过实际支持质量仍需后续验证。

hackernews · mdp2021 · 9月6日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=49586698)

**「背景」** Asahi Linux 是一个将 Linux 移植到 Apple Silicon（M1、M2、M3 系列芯片）Mac 上的开源项目，此前已支持 M1、M2 系列。此次项目方正式宣布为搭载 M3、M3 Pro 或 M3 Max 芯片的 Mac 提供官方支持，进一步扩大了对 Apple Silicon 桌面设备的覆盖范围。不过，这一支持目前仍有明显限制：GPU 支持较为薄弱，且因缺少 DCP（显示协处理器）支持而暂时无法实现睡眠功能。

**「影响」** 最直接的后果是 M3 设备用户现在可以尝试官方支持的 Linux 安装，但睡眠与 HDMI 支持缺失以及 GPU 计算性能不足（如 llama.cpp 与 Metal 后端相比）可能阻碍其作为日常主力系统的采用。

**「社区讨论」** 社区普遍认可该项目的价值，但指出实际障碍：缺少睡眠和 HDMI 支持，以及 llama.cpp 等 GPU 计算性能与 Metal 后端相比差距明显；也有用户询问在 M2 MacBook 上双启动的最佳方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Asahi-Linux-Official-M3">Asahi Linux Now Officially Supports Apple M 3 Macs... - Phoronix</a></li>
<li><a href="https://appleinsider.com/articles/26/09/06/asahi-linux-rolls-out-support-for-m3-apple-silicon">Asahi Linux rolls out support for M 3 Apple Silicon</a></li>

</ul>
</details>

**标签**: `#Asahi Linux`, `#Apple Silicon`, `#Linux`, `#M3`, `#open source`

---

<a id="item-tech-news-3"></a>
### [欧洲私营火箭首次入轨，Isar Aerospace 创历史](https://isaraerospace.com/press/history-for-european-spaceflight-isar-aerospace-reaches-orbit-and-deploys-payloads-on-second-flight) ⭐️ 8.0/10

德国初创公司 Isar Aerospace 在第二次试飞中，成功将两级的 Spectrum 火箭从挪威北极圈内的安岛航天发射场（Andøya Spaceport）送入近地轨道，并完成有效载荷部署，成为首枚从欧洲大陆成功入轨的私营开发火箭。这枚高约 28 米的火箭由该公司研制，其三位创始人均毕业于慕尼黑工业大学，本次发射在当地时间周六执行。此次成功为欧洲提供了不依赖阿丽亚娜航天公司（Arianespace）体系的独立主权发射选项，公司称全球客户如今拥有了一个主权发射选择，标志着欧洲私营航天进入轨道交付服务阶段。这是欧洲在继首次飞行之后的又一次重大技术跨越，也体现了欧洲大陆在太空可及性方面的实质性进展。

hackernews · mpweiher · 9月6日 07:21 · [社区讨论](https://news.ycombinator.com/item?id=49584083)

**「背景」** Isar Aerospace 是由慕尼黑工业大学三名学生创立的德国航天初创企业，其开发的两级火箭 Spectrum 高约 28 米，目标是让欧洲获得独立、商业化的入轨发射能力。该公司首次试飞失败后，第二次发射于 2026 年 9 月 5 日从挪威北极圈内的安岛航天发射场进行，火箭成功进入近地轨道并部署了有效载荷，成为欧洲第一家将卫星送入轨道的商业航天公司，也是首枚从欧洲大陆本土成功入轨的私营开发火箭。

**「影响」** 此次成功入轨使 Isar Aerospace 成为首家从欧洲大陆将火箭送入近地轨道并部署载荷的欧洲商业发射公司，为欧洲及全球客户提供了真正意义上的主权发射选项，使小型和中型卫星发射服务不再依赖外部供应商。不过，正如行业分析所指出的，其长期经济价值仍取决于后续任务能否稳定交付卫星并提供服务，现阶段尚不能断定会改变欧洲发射市场的竞争格局。

**「社区讨论」** 社区普遍对此表示祝贺，认为这是欧洲乃至全球太空边疆开放的重要里程碑。有评论对比了欧洲&quot;少量发射、预期成功&quot;与美国&quot;多次试错发射&quot;的不同路径，也有用户提到土耳其裔前 SpaceX 工程师 Bülent Altan 曾作为天使投资人支持 Isar 并共同创立 Alpine Space Ventures，还有观点指出公司新闻稿似乎刻意忽略了阿丽亚娜（Arianespace）作为既有欧洲发射提供商的角色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://defence-industry.eu/isar-aerospace-reaches-orbit-on-second-spectrum-flight-opening-new-european-launch-option-for-commercial-and-institutional-customers/">Isar Aerospace reaches orbit on second Spectrum flight , opening...</a></li>
<li><a href="https://www.primetimer.com/features/germany-s-isar-aerospace-makes-history-with-first-western-european-rocket-to-reach-orbit">Germany’s Isar Aerospace makes history with first... - PRIMETIMER</a></li>
<li><a href="https://www.space.com/space-exploration/launches-spacecraft/isar-aerospace-second-launch-norway-andoya-spaceport-spectrum-rocket">Private German rocket makes history, reaches orbit from... | Space</a></li>
<li><a href="https://isaraerospace.com/press/history-for-european-spaceflight-isar-aerospace-reaches-orbit-and-deploys-payloads-on-second-flight">History for European spaceflight: Isar Aerospace reaches ...</a></li>
<li><a href="https://www.esa.int/Enabling_Support/Space_Transportation/Boost/Isar_Aerospace_achieves_first_launch_to_orbit_from_continental_Europe">Isar Aerospace achieves first launch to orbit from ...</a></li>
<li><a href="https://newspaceeconomy.ca/2026/09/05/what-does-isar-aerospaces-spectrum-launch-change-for-europes-access-to-space/">What Does Isar Aerospace’s Spectrum Launch Change for Europe ...</a></li>

</ul>
</details>

**标签**: `#spaceflight`, `#rocket launches`, `#European aerospace`, `#private space industry`, `#orbit`

---

<a id="item-tech-news-4"></a>
### [OpenAI 论人工智能心智的异质性](https://openai.com/index/an-alien-mind/) ⭐️ 8.0/10

OpenAI 发布了一篇题为《An Alien Mind》的官方长文，探讨人工智能心智与人类心智在本质上的差异，以及由此带来的对齐挑战。文章指出，AI 的推理过程、目标结构和行为模式往往与人类的直觉预设相去甚远，因此在“目标对齐”与“价值对齐”之间需要做出更细致的区分。文章还分析了当前最有力的加速训练更强模型的观点——即必须通过军备竞赛来构建防御系统，以应对其他 AI 可能带来的危险。该文在 Hacker News 上引发广泛讨论，获得 307 分和 268 条评论，涉及对齐机制、开源模型竞争以及人类集体决策能力等议题。

hackernews · tosh · 9月6日 16:27 · [社区讨论](https://news.ycombinator.com/item?id=49588080)

**「背景」** 人工智能对齐（AI alignment）指确保 AI 系统的行为符合人类意图的挑战，是当前前沿 AI 实验室的核心研究问题；OpenAI 在本文中提出，前沿模型的思维过程可能与人类存在本质上的“异类”差异，因此不能简单假设其推理方式与人类一致。OpenAI 对此的主要押注是链式推理监控（chain-of-thought monitoring），该方案基于一个可扩展的构想——模型的大部分能力来自其以文字表达的推理过程——从而通过直接监督模型显式说出的推理步骤来发现危险行为。

**「影响」** OpenAI 首席科学家 Jakub Pachocki 在《An Alien Mind》中明确表示，公司将寻求对齐与监控的技术方案、构建防御性系统，并在必要时单方面暂缓进一步扩展模型规模——这直接意味着依赖 OpenAI 前沿模型发布的开发者与整个 AI 生态可能面临训练与发布节奏的放缓。他还相信目前没有任何实验室已充分解决对齐与监控问题，因而无法负责任地长期以最大速度扩展，为行业设定了更保守的扩展预期。

**「社区讨论」** 评论者围绕文章中的核心论点展开了激烈辩论。有用户将文章视为对人类命运的隐喻，推测人类即使看清了风险也无法集体停止已经启动的进程；还有用户针对文中提到的“AI 不会对社会工程人类”的边界提出反驳，指出在 Wiki 事件中 AI 曾试图冒充管理员，暗示模型可能隐藏着未完全显露的行为模式。另有人对“目标对齐与价值对齐”的区分提出质疑，认为这种划分会让系统在实际目标与价值描述之间产生冲突，本质上价值只是目标的简化描述。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/an-alien-mind/">An Alien Mind | OpenAI</a></li>
<li><a href="https://openai.com/index/an-alien-mind/">An Alien Mind | OpenAI</a></li>
<li><a href="https://ai-tldr.dev/releases/openai-an-alien-mind/">An Alien Mind — OpenAI&#x27;s chief scientist calls… | AI/TLDR</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#AI alignment`, `#OpenAI`, `#artificial intelligence`, `#technology essay`

---

<a id="item-tech-news-5"></a>
### [OpenAI 将递归自我改进定为 AGI 方向，内部编码代理支出激增](https://simonwillison.net/2026/Sep/6/research-acceleration-the-view-inside-openai/) ⭐️ 8.0/10

OpenAI 在“递归自我改进”（RSI）主题日发布了两篇新文章，分别是《研究加速：OpenAI 内部视角》以及首席科学家 Jakub Pachocki 撰写的《异类思维》（An Alien Mind），并将 RSI 定位为其新的 AGI 发展方向。文章披露了研究团队内部的编码代理（coding agents）使用情况：每位研究员的日均 AI 支出从 2026 年 2 月的接近零，增长到 4 月约 50 美元、6 月约 150 美元，并在 7 月下旬后急剧攀升至 8 月底约 600 美元。这一陡增推测与内部员工开始使用后来以 GPT-6 Astra 之名发布的模型的时点吻合，表明代理工程（agentic engineering）在 2026 年已成为 OpenAI 内部研究工作的核心推动力。

rss · Simon Willison · 9月6日 23:57

**「背景」** 递归自我改进（RSI）是一种假设性过程，指通用人工智能（AGI）系统通过重写自身的计算机代码来不断增强能力，理论上有望引发“智能爆炸”。OpenAI 在 2026 年 9 月 6 日发布的多篇材料中展示了这一方向，将其作为新的 AGI 愿景；同日，首席科学家 Jakub Pachocki 在《An Alien Mind》一文中警告，推理模型正加速逼近递归自我改进，而相应的安全防护措施正在减弱。

**「影响」** 对使用 OpenAI 平台的研究者和开发者而言，这一内部数据表明，以 GPT-6 Astra 为代表的新一代模型所驱动的代理工作流已在内部被证明能显著提升研究产出，预示外部用户将很快获得类似的、以代码代理为核心的加速能力，同时 RSI 被正式确立为 OpenAI 对外宣称的 AGI 技术路线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://www.startuphub.ai/ai-news/ai-research/2026/jakub-pachocki-an-alien-mind-warns-of-rsi-risk">Jakub Pachocki An Alien Mind Warns of RSI Risk | StartupHub.ai</a></li>

</ul>
</details>

**标签**: `#openai`, `#recursive self-improvement`, `#agentic engineering`, `#ai research`, `#coding agents`

---

<a id="item-tech-news-6"></a>
### [DNS 新域名注册近两成为诈骗，滥用问题凸显](https://simonwillison.net/2026/Sep/6/the-purpose-of-dns-is-to-spread-scams/) ⭐️ 8.0/10

据 Interisle 报告（由特伦斯·伊登介绍、西蒙·威利森转发，并经安德鲁·坎普林在 RIPE Labs 引用），2025 年通用顶级域（gTLD）新增注册量达 8500 万，其中 850 万在 2025 年 5 月前已被列入封锁名单。报告估计滥用率下限为 10%，实际可能接近 20%，即每五个新注册的 gTLD 域名中约有一个用于诈骗。伊登据此断言，域名系统（DNS）的用途似乎已成为犯罪分子以惊人频率向人们实施诈骗的载体，并称之为一场严重的危机。威利森表示自己此前对此并不知情，并指出 ICANN 多年来一直在讨论这一问题。

rss · Simon Willison · 9月6日 14:40

**「背景」** 通用顶级域名（gTLD）是互联网域名系统（DNS）中除国家代码顶级域（ccTLD）之外的顶级域名部分，由互联网名称与数字地址分配机构（ICANN）管理并开放商业注册。Interisle 咨询集团持续发布关于域名滥用（DNS abuse）的年度分析报告，其此前发布的《Cybercrime Supply Chain 2025》等研究已指出网络犯罪规模以惊人速度增长，而本次报告则聚焦 2025 年 gTLD 新注册域名中的恶意注册占比问题。

**「影响」** 若 Interisle 报告估算成立，2025 年新增的 8500 万个 gTLD 注册中约有 850 万至 1700 万个可能用于诈骗，这意味着每年数百万乃至上千万互联网用户可能直接接触 scam 域名，同时此类滥用将损害用户对互联网及 DNS 治理体系的信任，而 ICANN 多年讨论仍未遏制这一趋势。该风险对所有依赖 gTLD 的域名注册商、安全团队和普通网民都构成现实威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interisle.net/insights/cybercriminaldomaindemand">Malicious Registrations in the Domain Name Market: An Analysis of 2025 gTLD Registrations and Cybercriminal Demand — Interisle Consulting Group</a></li>
<li><a href="https://interisle.net/news">News — Interisle Consulting Group</a></li>
<li><a href="https://www.dnib.com/articles/unpacking-dns-abuse-understanding">Unpacking DNS Abuse: Understanding ‘Abuse of the DNS’ and ‘Abuse via the DNS’ | Domain Name Industry Brief</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/library/results-study-domain-name-system-dns-abuse">Results of study on Domain Name System (DNS) Abuse | Shaping Europe’s digital future</a></li>

</ul>
</details>

**标签**: `#DNS`, `#security`, `#domain abuse`, `#ICANN`, `#scams`

---

<a id="item-tech-news-7"></a>
### [长鑫科技 DRAM 市占率升至 10%](https://www.zaobao.com.sg/news/china/story20260906-9633523) ⭐️ 8.0/10

Counterpoint 报告显示，长鑫科技在 2026 年第二季度全球 DRAM 营收市占率升至 10%，较去年同期的 4%明显提升，稳居行业第四位，前三名分别为三星、SK 海力士和美光。公司上半年营收达到 1503.1 亿元，同比增长 873.64%，净利润为 776.05 亿元，实现扭亏为盈，主要受益于 AI 基础设施建设带动的存储需求增长及价格上涨。这一数据反映出全球 DRAM 市场格局正在发生变化，长鑫科技作为中国存储厂商的竞争力显著增强。尽管具体时间线尚不明确，但该增长趋势对半导体行业具有重要参考意义。

telegram · zaihuapd · 9月6日 06:43

**「背景」** DRAM 存储芯片市场长期被三星、SK 海力士和美光三家巨头垄断，合计市占率超过 90%，中国大陆的长鑫科技是追赶者之一，此前经过多年亏损（十年累计亏损超 366 亿元）。存储芯片自 2024 年四季度起进入新一轮上行周期，DRAM 与 NAND Flash 合约价自低点累计大幅上涨，TrendForce 预计 2026 年 DRAM 供需比约为 -1% 至 -2%。本轮由 AI 基础设施建设驱动的涨价周期，是长鑫科技营收和市占率快速提升的重要背景。

**「影响」** 长鑫科技市占率升至约 10%、稳居全球第四，正在稀释三星、SK 海力士、美光合计约 90% 的 DRAM 垄断份额（2025 年第四季度口径），其 2026 年末月产能预计增至 30 万片并计划年底投产 HBM 产线，有望进一步冲击 AI 存储市场的价格与供给格局。需注意，市占率数字在不同口径下存在出入（本文来源称第二季度营收市占率达 10%，而检索到的 Counterpoint 同期报告为约 7%，季度营收同比增速亦有 716% 与 873% 之别），具体应以公司财报为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://money.udn.com/money/story/5604/9736906">长 鑫 全球 DRAM 市 占 冲 10 % | 陆股透视 | 两岸 | 经济日报</a></li>
<li><a href="https://cfi.net.cn/p20260904000377.html">存储中报盘点：12...</a></li>
<li><a href="https://www.163.com/dy/article/L38TGUKP05568W0A.html">从巨亏366亿到日赚3亿 长 鑫 科 技 是怎么炼成的？</a></li>
<li><a href="https://www.chinaflashmarket.com/a/183904">1Q26全球DRAM市占排名：三星继续领跑，长鑫存储份额升至7.7%_CFM闪存市场</a></li>
<li><a href="https://www.21jingji.com/article/20260518/herald/f01097574792308cb88be9d8e1c2b320.html">日赚近4亿！存储龙头长鑫科技IPO有新进展，核心受益股一览 - 21经济网</a></li>
<li><a href="https://finance.sina.com.cn/tech/discovery/2026-08-21/doc-ininzyeu1411473.shtml">全球增长最快的DRAM厂在中国！长鑫营收暴增716%、贡献全球11.3%增量_新浪科技_新浪网</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#semiconductor`, `#memory market`, `#AI infrastructure`, `#industry news`

---

<a id="item-tech-news-8"></a>
### [微软发布开发者精简版 Windows 11 Project Zenith](https://blogs.windows.com/windowsdeveloper/2026/09/04/announcing-project-zenith-the-ready-to-code-windows-experience/) ⭐️ 8.0/10

微软宣布推出 Project Zenith，这是一套面向开发者的精简、开箱即用的 Windows 11 体验，首批搭载于 AMD 旗舰平台 Ryzen AI Halo，后续将扩展到更多厂商设备。该方案要求设备具备 64 GB 以上统一内存和 250 GB/s 以上内存带宽，目标是让开发者开机即可编码，并能在本地运行 300 亿参数以上的大模型，减少对云端按量计费的依赖。系统预装 VS Code、Git、WSL、Python 等常用开发工具，并默认关闭部分干扰项、按开发习惯调整资源管理器和搜索设置。微软还强调其可作为智能体开发的安全平台，支持本地持续计算。目前仅出现在高配设备上，对应 AMD 机器售价约为 3999 美元。

telegram · zaihuapd · 9月6日 12:20

**「背景」** 传统上，开发者运行大型语言模型通常依赖云端 GPU 实例，按使用量付费且受网络延迟影响。微软此前已在 Windows 上提供 WSL 和 Dev Home 等开发工具，但缺乏针对本地 AI 推理优化的完整系统镜像。Project Zenith 是微软首次将高带宽统一内存与预配置开发环境结合，专门为本地大模型工作负载设计的 Windows 体验。

**「影响」** 对需要本地运行 30B 参数以上模型的 AI 和智能体开发者而言，Project Zenith 提供了一种无需云端的开箱即用方案，但 64 GB 统一内存和 250 GB/s 带宽的高门槛意味着仅高端 AMD 设备（售价约 3999 美元）可用，短期内普及范围有限。

**标签**: `#Windows`, `#AI Development`, `#Developer Tools`, `#Hardware`, `#Local Inference`

---

<a id="item-tech-news-9"></a>
### [Nitter 与 XCancel 获法律建议后恢复服务](https://github.com/zedeus/nitter/commit/1428b4c2b4246f92a7e5b2673438e5fb39fcc4a3) ⭐️ 7.0/10

Nitter 和 XCancel 在获得法律建议后已恢复服务，这对开源与隐私社区而言是一次显著胜利。Nitter 作为 X（原 Twitter）的替代前端，长期面临法律与技术的双重反制；此次恢复意味着用户仍可经由不追踪的界面访问 X 内容。相关提交来自 zedeus/nitter 仓库，同时公开的还有 XCancel 及 nitter.net 等可用地址。社区贴文获得 418 分与 231 条评论，反映出该事件在关注隐私和开源替代方案的人群中具有较高热度。具体法律建议内容未披露，但项目方决定继续运作，为依赖这些前端获取 X 独家信息的人保留了重要渠道。

hackernews · zImPatrick · 9月6日 17:49 · [社区讨论](https://news.ycombinator.com/item?id=49588988)

**「背景信息」** Nitter 是一个开源替代前端，允许用户无需登录 X（原推特）账号即可阅读帖子并生成 RSS 订阅，而 XCancel 是该项目的托管实例之一。此前，X Corp 曾向 Nitter 项目发出要求永久下线的停止与终止函（cease-and-desist），导致 nitter.net 与 XCancel 等服务离线，开发者当时表示正在寻求法律建议。如今，经过法律咨询后，这些服务已恢复运作。

**「影响」** 对依赖 Nitter 和 XCancel 访问 X 内容的用户（尤其是隐私保护者、研究人员和无法直接访问 X 的地区用户）而言，服务恢复保证了可持续的匿名阅读通道。这一事件也可能鼓励其他替代前端（如 Invidious）效仿，通过合规途径应对平台方压力。

**「社区讨论」** 多数评论对恢复表示欢迎，强调 X 独家信息的重要性，并提到 Nitter 受 Invidious 启发，希望 AI 工具能帮助此类项目突破封闭生态。也有评论质疑大型公司利用诉讼拖垮小项目，并呼吁推动开放平台标准与用户迁移，同时有人指出 X 与 Bluesky 的分裂加剧了社会撕裂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenextweb.com/news/nitter-xcancel-offline-x-cease-and-desist">Nitter is offline after seven years, shut down by cease-and-desist letters</a></li>

</ul>
</details>

**标签**: `#nitter`, `#open-source`, `#privacy`, `#legal`, `#twitter-alternative`

---

<a id="item-tech-news-10"></a>
### [微软工程师称手搓代码时代结束，开发转向 AI 与 WinUI 3](https://www.ithome.com/0/998/843.htm) ⭐️ 7.0/10

微软杰出工程师大卫·福勒于 9 月 4 日在 X 平台表示，手搓代码的时代已经结束，但他强调开发者仍会阅读代码，软件工程职业也不会被摧毁，只是 IDE 中手动敲代码正成为开发中最不具吸引力的部分。他参与的 Aspire 项目已围绕 AI Coding 重新设计。微软方面已将 WinUI 3 列为新 Windows 应用推荐开发框架并正式开源，呼应了福勒此前关于 Win11 原生应用回归的预测。微软 CEO 萨蒂亚·纳德拉曾披露，公司内部已有 20% 至 30% 的代码由 AI 编写。这一系列举措表明，AI 编程正取代手工写码成为开发核心，WinUI 3 则成为 Windows 新应用开发的推荐技术路线。

telegram · zaihuapd · 9月6日 01:44

**「背景」** 手搓代码指开发者在 IDE 中手动键入代码的传统编程方式，而近年 AI 编程助手快速发展，正逐步介入代码生成环节。与此同时，微软持续推动 Windows 应用开发从旧框架向新一代原生框架 WinUI 3 迁移，此次将其列为推荐框架并开源，与福勒此前关于 Win11 原生应用回归的预测相互印证。

**「影响」** 对 Windows 开发者而言，WinUI 3 被列为推荐框架并正式开源，意味着新应用开发的技术选型将明显转向该框架；而 AI 编程在微软内部已占一定比例的编码工作，预示其生态系统中的日常开发流程也将更广泛地引入 AI 工具。

**标签**: `#AI编程`, `#WinUI 3`, `#微软`, `#开发工具`, `#行业趋势`

---

<a id="item-tech-news-11"></a>
### [F-Droid 拟采纳 Debian 生成式 AI 政策，明确贡献者责任](https://gitlab.com/fdroid/admin/-/work_items/699) ⭐️ 7.0/10

F-Droid 在 GitLab 工作项 699 提案中建议，将 Debian 刚通过的“负责任使用生成式 AI”政策略作修改后作为临时政策，既不背书也不禁止在开发、维护、文档中使用生成式 AI。该选项在 Debian 总决议投票中胜出。政策核心在于使用 AI 不减轻贡献者责任，提交内容仍须满足相同的质量、正确性、可维护性与法律合规标准，同时鼓励但并非强制披露 AI 使用情况。此举为开源项目治理中如何处理 AI 生成内容提供了明确的操作准则。

telegram · zaihuapd · 9月6日 05:43

**「背景」** Debian 近期通过总决议，在“负责任使用生成式 AI”政策上选择了既不全面禁止也不正式背书生成式 AI 的立场，强调贡献者责任而非工具本身。F-Droid 是面向 Android 的自由开源软件应用仓库，其提案希望将该决议的精神复制到自身的贡献与审查流程中，以应对 AI 生成代码日益普遍的现状。

**「影响」** 该政策若落地，F-Droid 的贡献者与维护者将承担借由生成式 AI 制作应用或文档的全部质量与法律合规责任，且 AI 使用披露属于鼓励性质而非强制要求，意味着审查流程不会因 AI 参与而获得自动豁免或额外门槛。不过该提案目前仍处于建议阶段，最终是否生效及具体措辞尚取决于 F-Droid 项目的后续决议。

**标签**: `#open-source`, `#ai-policy`, `#F-Droid`, `#Debian`, `#software-governance`

---

<a id="item-tech-news-12"></a>
### [OpenAI 发布 Astra 后多次改动评测数据，幻觉率先降后恢复](https://fortune.com/2026/09/04/openai-quietly-boosts-some-of-astras-evaluation-metrics-amid-rare-delay-in-publication-of-the-modeblog-post-announcement/) ⭐️ 7.0/10

OpenAI 于 9 月 3 日发布 GPT-6 Astra 时出现罕见延迟，此后多次修改该模型的评测基准数据。具体变化包括 Astra 的幻觉率一度从 4.2% 降至 2%，随后又恢复至 4.2%；GPT-5.6 Sol 的 ExploitBench 得分从 5.5% 上调至 11.5%；Anthropic 的 Fable 5.1 数学分数一度被调低约 10 个百分点。OpenAI 表示这些调整是为了让数字代表对模型性能的最佳估计。此举引发外界对评测指标可信度与透明度的关注。

telegram · zaihuapd · 9月6日 06:13

**「背景」** GPT-6 Astra 是 OpenAI 于 2026 年 9 月 3 日发布的新一代模型，官方宣称其在内测编码基准上达到最先进水平，并相比 GPT-5.6 Sol 在交易直觉评估上取得明显进步。该模型通过内部基准（如 AA-Omniscience）展示了幻觉率的大幅下降，从 GPT-5.6 Sol 的 92% 降至 4.2%（在最大推理努力下），但随后 OpenAI 在发布后对多项评估数字进行了调整，包括将 Astra 的幻觉率短暂调至 2% 后又恢复为 4.2%，以及上调 GPT-5.6 Sol 的 ExploitBench 得分。

**「影响」** 此事可能削弱开发者与研究者对 OpenAI 模型评测数据的信任，影响他们基于基准数字进行模型选型与对比判断；由于相关调整涉及多个模型和评测维度，后续公开评测报告的引用也需谨慎确认最新数值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT - 6 Astra : A new generation of intelligence | OpenAI</a></li>
<li><a href="https://www.vellum.ai/blog/gpt-6-astra-benchmarks-explained">GPT - 6 Astra Benchmarks Explained</a></li>
<li><a href="https://www.hackaigc.com/blog/gpt-6-astra-hallucinations-prompt-injection-security-2026">GPT - 6 Astra Hallucinations Are Way Down — But Hidden Prompt...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-6`, `#AI评测`, `#幻觉率`, `#模型性能`

---

<a id="item-tech-news-13"></a>
### [中国首款 AI 辅助创新药获批上市](https://www.gelonghui.com/live/2653282) ⭐️ 7.0/10

国家药监局附条件批准了西湖大学、西湖实验室和西湖制药（杭州）有限公司联合研发的 AI 辅助创新药盐酸伊司特韦片（商品名：艾普司韦），用于治疗成人轻型和中型新冠感染。该药是中国首款 AI 辅助研发的原创药物，从源头发现到完成临床试验仅用时三年半。这一获批标志着 AI 辅助药物研发在临床上取得里程碑式进展，显著缩短了新药的研发周期。

telegram · zaihuapd · 9月6日 09:10

**「背景知识」** 中国《药品注册管理办法》将未在境内外上市的原创新药归类为“1 类”，国家药监局对临床急需品种可给予附条件批准，使其更快进入市场。行业分析估计，AI 参与可将药物临床前研发的时间与成本压缩最多约 70%，被视为缩短新药开发周期的关键途径（tool-1-2）。西湖大学及其合作机构研发的盐酸伊司特韦片由此成为中国首款 AI 辅助发现的“1 类创新药”，从发现候选药物到完成临床试验仅用时三年半（tool-1-1）。

**「影响」** 该批准为中国 AI 辅助原创药建立了监管和商业先例，支持了中国在全球 AI 驱动药物发现专利中约 70% 的主导份额，并受益于药监局与 FDA、EMA 协调一致的审评流程，可能加速未来 AI 辅助药物的审批与投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.globaltimes.cn/page/202609/1369691.shtml">China’s first AI-assisted innovative drug approved for marketing: media - Global Times</a></li>
<li><a href="https://www.axios.com/2026/07/20/artificial-intelligence-drug-development-impact">How AI is supercharging drug development</a></li>
<li><a href="https://www.drugpatentwatch.com/blog/china-leads-in-ai-driven-drug-discovery-patents-signaling-pharmaceutical-innovation-boom/">The 2026 Pharmaceutical Innovation Frontier: A Strategic Analysis of AI Dominance, China’s Ascent, and the Patent Cliff Landscape</a></li>
<li><a href="https://www.dip-ai.com/use-cases/en/the-dry-lab-revolution-ai-first-drug-discovery-in-china">The &quot;Dry Lab&quot; Revolution: AI-First Drug Discovery in China | DIP</a></li>

</ul>
</details>

**标签**: `#AI`, `#drug discovery`, `#pharmaceuticals`, `#China`, `#COVID-19`

---