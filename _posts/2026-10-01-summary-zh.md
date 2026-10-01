---
layout: default
title: "Horizon Summary: 2026-10-01 (ZH)"
date: 2026-10-01
lang: zh
---

> 从 34 条内容中筛选出 11 条重要资讯。

---

**科技新闻**
1. [谷歌发布主打编程调试的旗舰模型 Gemini 4 Argon](#item-tech-news-1) ⭐️ 9.0/10
2. [分词技术综述：覆盖算法、多语言与替代方案](#item-tech-news-2) ⭐️ 8.0/10
3. [CO₂Jump：免训练采样器自纠正图文联合生成](#item-tech-news-3) ⭐️ 8.0/10
4. [DeepSeek 开源华为升腾基础组件，推进升腾 950 超节点方案](#item-tech-news-4) ⭐️ 8.0/10
5. [哔哩哔哩开源 Index-Translate 多语言翻译模型](#item-tech-news-5) ⭐️ 8.0/10
6. [Reddit 停用 RSS 与公开 API](#item-tech-news-6) ⭐️ 8.0/10
7. [特朗普与六大科技巨头签署 AI 安全协议](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare 进军公共证书颁发机构](#item-tech-news-8) ⭐️ 7.0/10
9. [微软外包员工审查 Copilot 图片提示，引发隐私与劳权担忧](#item-tech-news-9) ⭐️ 7.0/10
10. [Kimi K3 进入 OpenAI 企业结算，创中国模型先例](#item-tech-news-10) ⭐️ 7.0/10
11. [OpenAI 瓦解模型蒸馏攻击并归因月之暗面相关人员](#item-tech-news-11) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [谷歌发布主打编程调试的旗舰模型 Gemini 4 Argon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/) ⭐️ 9.0/10

谷歌宣布推出 Gemini 4 Argon，这是其最新的旗舰 AI 模型，重点强化了智能体式编程与调试能力，例如据称能自主完成代码调试以及迁移 C/C++ 代码库至 Rust 等任务。谷歌表示将继续收集早期测试者的反馈并迭代护栏措施，之后才会尽快向开发者、企业和消费者开放 Argon。目前该模型的完整可用版本尚未广泛发布，官方也未给出具体的开放时间表。相关分析指出，Argon 标志着谷歌在 AI 模型竞争中的又一个重要节点。

hackernews · bradleyg223 · 9月30日 20:04 · [社区讨论](https://news.ycombinator.com/item?id=49913571)

**「背景」** Gemini 4 Argon 是谷歌于 2026 年 9 月 30 日发布的新一代旗舰前沿模型，官方将其定位为面向复杂软件工程、专业法律与金融工作以及网络防御的“前沿智能新时代”。该模型拥有业界领先的 100 万 token 上下文长度，旨在支持深度、多步骤的长期任务推理。此次发布延续了谷歌今年在 Gemini 系列上密集迭代的节奏（此前已有 Gemini 3.8 等版本），成为各大实验室在 AI 模型能力上持续交替领先的最新一例。

**「影响」** Google 已率先向特定网络安全合作伙伴和早期测试者提供 Gemini 4 Argon，这批用户可立即利用其 100 万 token 的上下文窗口与先进的自主编码、调试能力处理复杂的长期专业任务；不过普通开发者、企业和消费者仍需等待 Google 完成护栏迭代后才能使用，该模型目前尚未全面公开发布。

**「社区讨论」** 有用户分享了 Gemini 3.8 Flash 的惊人经历：在 Strix Halo 上调试 ROCm 版 llama.cpp 时，模型自动挂接 GDB 到 GPU 驱动、逆向内核队列 ioctl 接口并编写 LD\_PRELOAD 的 C shim，令其啧啧称奇；另一些评论认为各前沿实验室持续互相超越，AI 能力正分散至更多厂商，这反驳了 Dario Amodei 关于赢家通吃（concentrating）的论断，并把“模型和提供商可替换”视为重要原则。此外，不少用户借 Argon 尚未正式发布一事调侃 Gemini“迟迟发不出模型”，也有开发者对谷歌用 Argon 将 C/C++ 迁移到 Rust 的做法表示感慨或嘲讽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon</a></li>
<li><a href="https://www.callmissed.com/blog/gemini-argon-google-announced-september-30-2026">Gemini 4 Argon : What Google Announced September... | CallMissed</a></li>
<li><a href="https://www.gptunnel.ru/en/blog/gemini-4-argon">Gemini 4 Argon : what Google &#x27;s new model changes · GPTunneL</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon</a></li>
<li><a href="https://www.cnbc.com/2026/09/30/google-gemini-4-argon-ai.html">Google rolls out Gemini 4 Argon , its most advanced model</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#machine learning`, `#model release`

---

<a id="item-tech-news-2"></a>
### [分词技术综述：覆盖算法、多语言与替代方案](https://www.reddit.com/r/MachineLearning/comments/1wuccjf/tokenization_a_survey_for_modern_nlp_r/) ⭐️ 8.0/10

32 位分词研究人员在过去约 8 个月中合作完成了这份关于现代 NLP 分词领域最全面的综述，涵盖算法、评估、多语言、编码、理论等各个方面。论文还讨论了分词器的潜在替代方案，如潜在（latent）或视觉（visual）分词，以及约束生成、token healing、分词器安全等相邻课题。该综述旨在填补分词这一影响所有 NLP 领域却长期缺乏系统研究的问题，为实践者和研究者提供权威参考。全文可于文章附带的 alphaxiv 链接中获取。

reddit · r/MachineLearning · /u/mcmcmcmcmcmcmcmcmc\_ · 9月30日 18:13

**「背景」** 分词（tokenization）是将文本切分为模型可处理的片段（token）的过程，直接影响语言模型的词汇表、训练效率和多语言表现。尽管它对模型性能和部署有深远影响，却长期缺乏系统性总结，本研究正是对此盲区的全面梳理。

**「影响」** 这份综述为 NLP 研究和工程实践提供了关于分词技术、评估方法和替代方案的集中知识，有助于研究者快速了解领域现状并识别未来研究方向，同时为依赖分词器的模型开发者提供实用的配置参考。

**标签**: `#tokenization`, `#NLP`, `#language models`, `#survey`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [CO₂Jump：免训练采样器自纠正图文联合生成](https://www.reddit.com/r/MachineLearning/comments/1wtyl5m/concurrent_image_understanding_and_generation/) ⭐️ 8.0/10

一篇提交至 NeurIPS 2026 的论文（由 Google、Google DeepMind 与石溪大学合作）提出名为 CO₂Jump 的免训练采样器，用于解决联合文本与图像生成中的图文不一致问题——例如模型能口述正确的迷宫解法却画出另一条路径。该方法利用文本置信度与跨模态注意力在去噪采样中指导图像更新，并允许将低置信度 token 重新掩码后再次生成，使早期决策能在生成过程中被修正，且每个去噪步骤仅需一次模型前向传播。作者在图像编辑、迷宫求解与数织（Nonograms）任务上进行了评估，并发布了 JEdit-1M、JMaze-200K 与 JNono-200K 三个数据集。在 8 至 512 个采样步数范围内，CO₂Jump 是受比较采样器中唯一在编辑质量与 grounding（图文对应关系）两方面均单调提升的方案；联合准确率要求文本答案与生成图像同时正确。

reddit · r/MachineLearning · /u/Upstairs\_Theme2785 · 9月30日 07:28

**「背景」** 联合文本–图像生成常采用去噪采样过程逐步生成输出，但如果文本与图像各自独立采样，二者很容易在语义上不一致，且先前步骤的错误难以在后续修正。CO₂Jump 在采样中以文本置信度和跨模态注意力为信号引导图像更新，并将低置信度 token 重新掩码以重新生成，从而实现无需额外训练的自纠正机制。

**「影响」** 对于从事多模态生成与编辑的研究者，CO₂Jump 提供了一种可与现有任务特定微调模型直接配合的免训练自纠正采样方案，每个去噪步骤仅需一次前向传播；其发布的三套数据集也为图文一致性的联合评测提供了新的基准。

**标签**: `#multimodal generation`, `#sampling methods`, `#image understanding`, `#NeurIPS`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [DeepSeek 开源华为升腾基础组件，推进升腾 950 超节点方案](https://mp.weixin.qq.com/s/X41mKH4Ds-VXUAnK6M8Eww) ⭐️ 8.0/10

DeepSeek 于 2026 年 9 月 30 日宣布开源面向华为升腾平台的基础组件，涵盖 TileLang 高级语言编译工具、计算库和分布式通信库，并包含 DeepGEMM Ascend、DeepEP Ascend、TileKernels、FlashMLA 和 DeepSelect 等项目。这些组件与其此前面向英伟达平台的组件相对应，旨在将 DeepSeek 的软件栈扩展至华为升腾硬件。DeepSeek 表示，相关组件在多项测试中性能接近硬件上限，并与华为共同推进基于升腾 950 的 128 卡超节点方案。目前官方公告中缺乏具体的性能测试数据、基准细节和验证信息，实际效果有待进一步确认。这一开源举措对 AI 基础设施的多厂商部署格局具有潜在影响，可能加速升腾生态在 AI 训练和推理中的采用。

telegram · zaihuapd · 9月30日 03:09

**「背景」** DeepSeek 此前为英伟达平台开发了 TileLang 编译工具、DeepGEMM 计算库和 DeepEP 通信库等基础组件，此次将这些组件移植到华为升腾平台。TileLang 是面向 AI 计算的高级语言编译工具，其升腾版本封装底层的升腾 C 指令，在提供高级编程接口的同时不牺牲硬件性能。这一举措正值中国加速构建可替代英伟达的软件栈、降低对英伟达依赖的背景下，华为也随之公布了双方共同定义的 128 卡 SuperPoD Flex 超节点设计。

**「影响」** DeepSeek 开源升腾基础组件为中国开发者提供了不依赖 NVIDIA CUDA 的国产 AI 软件栈，使其得以在华为升腾芯片上部署 AI 训练与推理负载，有助于降低对 NVIDIA 的依赖性，并在美国出口管制背景下支撑国产 AI 生态的自主发展；不过，此次公告未提供独立的性能验证数据，宣称的“接近硬件上限”性能仍有待实测确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dqindia.com/news/deepseek-expands-huawei-ascend-push-with-six-open-source-ai-tools-12594158">DeepSeek expands Huawei Ascend push with six open - source AI tools</a></li>
<li><a href="https://pandaily.com/deepseek-ascend-infra-oss-tilelang-deepgemm-deepep-superpod-flex">DeepSeek Open - Sources Ascend Versions of TileLang , DeepGEMM ...</a></li>
<li><a href="https://www.geopolitechs.org/p/deepseek-builds-for-huawei-ascend">DeepSeek Builds for Huawei Ascend - Geopolitechs</a></li>
<li><a href="https://www.profilenews.com/en/deepseek-and-huawei/">DeepSeek and Huawei Expand Nvidia Alternatives for AI Chips</a></li>
<li><a href="https://finance.yahoo.com/news/home-grown-heroes-huawei-deepseek-093000982.html">Home-grown heroes: how Huawei and DeepSeek are helping China...</a></li>
<li><a href="https://www.dqindia.com/news/deepseek-expands-huawei-ascend-push-with-six-open-source-ai-tools-12594158">DeepSeek expands Huawei Ascend push with six open-source AI tools</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#Huawei Ascend`, `#open source`, `#AI infrastructure`, `#TileLang`

---

<a id="item-tech-news-5"></a>
### [哔哩哔哩开源 Index-Translate 多语言翻译模型](https://www.ithome.com/1/008/914.htm) ⭐️ 8.0/10

哔哩哔哩（Bilibili）Index LLM 团队于 9 月 30 日开源 Index-Translate 多语言翻译模型家族，2B、9B 以及 35B-A3B（预览版）文本模型权重已在 Hugging Face 与 ModelScope 平台开放，共支持 150 种语言。该系列基于 Qwen3.5 构建，支持术语、格式和保留内容等翻译指令控制，并进一步扩展至语音翻译、音节可控翻译和长文档翻译等场景。此次开源为 NLP 工程师与研究者提供了可落地的高质量多语言翻译基座，覆盖从小参数部署到大规模推理的不同算力需求，也有助于降低行业在垂直领域翻译任务上的二次开发门槛。

telegram · zaihuapd · 9月30日 14:08

**「背景信息」** Index-Translate 是哔哩哔哩 Index LLM 团队于 2026 年 9 月 30 日开源的多语言机器翻译模型家族，提供 2B、9B 和 35B-A3B 三种规模的文本模型，支持 150 种语言，并包含术语控制、语音翻译、受控配音和长文档翻译等能力，权重已发布在 Hugging Face 与 ModelScope 上。该模型基于阿里巴巴研发的开源大语言模型 Qwen 3.5 构建，Qwen 系列自推出以来以开放权重和宽松许可吸引了大量团队在其基础上进行二次开发，Index-Translate 即沿用了这一基础架构和训练范式。近年来，Meta 的 NLLB、OPUS-MT 等开源多语言翻译模型不断涌现，而 Index-Translate 在此基础上进一步引入了受控配音、术语保留等面向实际生产场景的高级功能，这在同类开源模型中相对少见。

**「影响」** 对于 NLP 工程师和研究者，该开源免去了从零训练的成本，可立即在 Hugging Face 或 ModelScope 获取并部署基于 Qwen3.5、覆盖 150 种语言的多语言翻译模型（2B/9B/35B-A3B），并直接借助术语控制、格式与保留内容指令及长文档翻译能力落地本地化等生产场景；其中 35B-A3B 仍为 preview 版本，正式可用性有待后续验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/IndexTeam/Index-Translate-35B-A3B">IndexTeam/ Index - Translate -35B-A3B · Hugging Face</a></li>
<li><a href="https://www.openai-hub.com/news/2235/">B站开源 Index - Translate 翻译模型：覆盖150种语言 - OpenAI Hub</a></li>

</ul>
</details>

**标签**: `#Open Source`, `#Machine Translation`, `#Large Language Models`, `#Multilingual AI`, `#Bilibili`

---

<a id="item-tech-news-6"></a>
### [Reddit 停用 RSS 与公开 API](https://techcrunch.com/2026/09/30/reddit-is-killing-rss-feeds-ending-public-api-access-because-of-ai-bots/) ⭐️ 8.0/10

Reddit 宣布于 11 月 13 日停止 RSS 订阅支持，并将在 2027 年 3 月关闭公开 API，理由是防止 AI 机器人等大规模抓取和自动化滥用。公司建议版主改用 Discord Relay，并规定第三方应用和机器人开发者须在 2027 年 1 月 12 日前完成注册，否则将被移除 API 访问权限。此举影响依赖 Reddit 数据的开发者、研究人员及内容聚合工具，也反映平台对 AI 数据采集的收紧。

telegram · zaihuapd · 10月1日 00:27

**「背景」** RSS 是一种让用户订阅网站内容更新的轻量级格式，而 Reddit 的公开 API 则允许第三方应用、研究者和开发者以编程方式读取平台数据，并长期作为 AI 训练、内容聚合与自动化工具的重要数据来源。Reddit 以大规模抓取和自动化滥用（尤其是 AI 机器人）为由，宣布于 11 月 13 日停用 RSS 订阅支持，并计划于 2027 年 3 月彻底关闭公开 API 访问；另有报道指出，第三方应用与机器人开发者需在 2027 年 1 月 12 日前完成注册，否则将被移除 API 访问权限。

**「影响」** 对于依赖 Reddit 公开 API 或 RSS 的开发者、研究者和第三方应用而言，其数据获取和自动化流程将在上述日期前中断，未在 2027 年 1 月 12 日前注册的机器人将被移除访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://daily.dev/posts/reddit-is-killing-rss-feeds-and-ending-public-api-access-because-of-ai-bots-etgqokzhb">Reddit is killing RSS feeds and ending public API access...</a></li>
<li><a href="https://superintelligencenews.com/ai-fields/large-language-models/reddit-rss-feeds-ai-scraping-crackdown/">Reddit Ends RSS Feeds Amid AI Scraping Crackdown</a></li>
<li><a href="https://dailybeirut.com/en/technology-and-science/reddit-shut-down-rss-feeds-public-api-2027/">Reddit to End RSS Feeds and Public API by 2027 · Daily Beirut</a></li>

</ul>
</details>

**标签**: `#Reddit`, `#API`, `#RSS`, `#AI bots`, `#platform policy`

---

<a id="item-tech-news-7"></a>
### [特朗普与六大科技巨头签署 AI 安全协议](https://www.zaobao.com.sg/news/world/story20260930-9758185) ⭐️ 7.0/10

美国总统特朗普于当地时间 9 月 29 日与谷歌、Anthropic、Meta、OpenAI、xAI 和英伟达的掌门人共同签署一份一页纸的人工智能安全协议，并将文件发布在 Truth Social 上。特朗普称该文件具有“道义约束力”。协议要求企业建立四层控制机制，包括配合外部审计机构独立评估 AI 管控系统、设立董事会独立委员会监督，并在模型训练和部署期间围绕网络安全、生物和化学威胁监控 AI 能力与对齐情况，确保各项措施按预期运行。

telegram · zaihuapd · 9月30日 02:30

**「背景」** 人工智能安全治理一直是技术政策讨论的焦点，尤其是大模型能力快速提升后，外界对 AI 被滥用或失控风险的担忧加剧。此前业界和监管机构已提出多种自愿性安全承诺，但通常缺乏统一的监督与审计机制。这份协议试图通过外部审计、董事会监督和能力威胁监控等机制，为头部 AI 企业建立一套可验证的安全管理框架。

**「影响」** 该协议若落地，将直接影响参与企业的内部治理流程和外部审计安排，并为后续 AI 监管政策提供参考样本，但因其不具备法律约束力，实际执行效果仍取决于企业自愿配合程度。

**标签**: `#AI safety`, `#technology policy`, `#artificial intelligence`, `#industry agreement`, `#regulation`

---

<a id="item-tech-news-8"></a>
### [Cloudflare 进军公共证书颁发机构](https://blog.cloudflare.com/cloudflare-certificate-authority/) ⭐️ 7.0/10

Cloudflare 宣布计划成为公共证书颁发机构，已申请加入 Chrome、Apple、Microsoft 和 Mozilla 的根证书计划，并与 GlobalSign 签署协议收购后者一个受广泛信任的根证书。目前该公司尚未开始签发证书。新的 CA 将优先支持 ACME 协议实现证书的自动签发和续期，并计划于 2027 年第一季度签发生产级默克尔树证书（MTC），以服务后量子互联网时代的安全需求。这一举措标志着大型基础设施厂商进入公共 CA 市场，对 TLS/SSL 生态和 Web 安全工具链具有潜在深远影响。

telegram · zaihuapd · 9月30日 06:26

**「背景」** 公共证书颁发机构是受浏览器和操作系统根证书计划信任的实体，负责为网站签发 TLS/SSL 证书以建立加密连接。要成为受信任的 CA，必须通过 Apple、Google、Microsoft、Mozilla 等根商店运营者的严格审核，而 ACME 协议则是 Let&\#x27;s Encrypt 推广的自动化证书签发标准。Cloudflare 通过收购现有根证书有望缩短审核周期，但仍需满足各根计划的技术和合规要求。

**「影响」** 对于依赖自动化证书管理的网站运营者和开发者，未来可能获得来自 Cloudflare 的 ACME 签发和续期选项，并受益于其基础设施规模；但证书签发最早要到 2027 年才能实现，且能否成功融入各浏览器根计划仍有不确定性。

**标签**: `#certificate authority`, `#TLS/SSL`, `#post-quantum cryptography`, `#ACME`, `#web security`

---

<a id="item-tech-news-9"></a>
### [微软外包员工审查 Copilot 图片提示，引发隐私与劳权担忧](https://www.404media.co/humans-reading-copilot-prompts-images/) ⭐️ 7.0/10

据 404 Media 和 The Verge 报道，微软为优化 Copilot 的图片生成与编辑效果，雇佣了数百名外包合同工，对用户输入的提示词、请求以及随手上传的私人照片进行逐一人工审阅与评估，这意味着发送给 Copilot 的内容在云端并非绝对私密。这些底层审查员被迫承受大量冲击性内容的轰炸，包括低俗露骨的“偷拍（upskirt）”性暗示照片，以及可能涉嫌违法的动物祭祀影像，给员工带来严重的精神创伤与心理压榨。事件同时暴露了 AI 服务后台真人审查机制对用户隐私的威胁，以及对从事内容审核的外包劳工权益的侵害。

telegram · zaihuapd · 9月30日 07:13

**「背景」** 微软 Copilot 作为生成式 AI 助手，其图片生成与编辑功能依赖用户输入的提示词和上传的图片来优化模型表现。根据微软官方文档，Copilot 通过 Microsoft Graph 访问用户数据，并基于组织数据生成答复，这意味着用户的输入和内容会经过公司系统处理，而非完全本地化。为改进 AI 性能，微软有时会引入外包人员对用户提示和生成内容进行人工评估，特别是涉及图片生成功能时，这引发了关于用户隐私和员工福祉的讨论。

**「影响」** 据 404 Media 报道，使用 Microsoft Copilot 图片生成与编辑功能的用户需意识到，其输入的对话提示词与上传的私人照片可能被外包合同工逐一审阅，这意味着相关数据并不具备绝对私密性。同时，据报道，这些负责内容审核的外包员工被要求持续接触大量低俗、疑似偷拍（upskirt）及潜在违法的动物祭祀影像，承受严重的精神创伤与心理压力，这反映了 AI 服务数据安全与劳工权益方面的潜在风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy">Data, Privacy , and Security for Microsoft Copilot | Microsoft Learn</a></li>
<li><a href="https://copilot.com/">Microsoft Copilot | Вход</a></li>
<li><a href="https://www.youtube.com/watch?v=EYp8JWRoqic">Best Prompts for Microsoft Copilot in Excel - YouTube</a></li>
<li><a href="https://copilot.cloud.microsoft/">Copilot | ИИ-чат для работы</a></li>

</ul>
</details>

**标签**: `#privacy`, `#AI ethics`, `#Microsoft Copilot`, `#content moderation`, `#labor practices`

---

<a id="item-tech-news-10"></a>
### [Kimi K3 进入 OpenAI 企业结算，创中国模型先例](https://36kr.com/newsflashes/4005691489112198) ⭐️ 7.0/10

美国 AI 基础设施公司 Baseten 宣布，企业用户现可在 OpenAI 编程工具 Codex 中直接使用中国开源模型 Kimi K3，相关调用费用将计入企业已有的 OpenAI 采购承诺额度，无需新增供应商采购流程。这是中国开源模型首次进入 OpenAI 的企业付费结算体系，标志着跨生态集成取得实质性进展。Kimi K3 由此进入 OpenAI 企业客户的主流付费通道，简化了采购流程，但具体功能支持范围和性能限制尚未披露。该消息来自 36 氪新闻快讯，目前属于发布公告阶段，而非技术深度评测。

telegram · zaihuapd · 9月30日 11:23

**「背景」** Kimi K3 是月之暗面（Moonshot AI）发布的 2.8 万亿参数开源权重模型，拥有 100 万 token 的上下文窗口，在编码基准测试中击败了 Anthropic 的 Claude Fable 5 和 OpenAI 的 GPT-5.6 Sol，且价格约为对手的三分之一。OpenAI Codex 是 OpenAI 的编程工具，其企业通道允许大型企业客户将模型调用费用计入与 OpenAI 签署的采购承诺额度，从而省去新增供应商的采购与结算流程；此前该通道基本只覆盖 OpenAI 自身或生态内模型。此次经美国 AI 基础设施公司 Baseten 接入，Kimi K3 成为首个进入 OpenAI 企业付费结算体系的中国开源模型。

**「影响」** 对于已与 OpenAI 签订采购承诺的企业客户，Kimi K3 将可直接通过既有结算通道使用，显著降低引入新模型的采购与管理成本，尤其利于需要中国模型能力的跨国企业；但具体调用限制和结算费率尚未公开，实际采用规模仍有待观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://k3-kimi.com/">Kimi K 3 : 2.8T Open-Weight Model — Benchmarks, Pricing &amp; Guides</a></li>
<li><a href="https://news.tomorrow-today.co.za/p/china-s-kimi-k3-steals-the-coding-crown-openai-builds-a-keyboard-for-a-post-keyboard-world">China&#x27;s Kimi K 3 Steals the Coding Crown + OpenAI Builds...</a></li>

</ul>
</details>

**标签**: `#AI`, `#OpenAI`, `#Kimi K3`, `#enterprise`, `#open source`

---

<a id="item-tech-news-11"></a>
### [OpenAI 瓦解模型蒸馏攻击并归因月之暗面相关人员](https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/) ⭐️ 7.0/10

OpenAI 宣布已瓦解一起针对其模型的协调性模型蒸馏活动，攻击者通过操纵交互界面提取受保护的推理内容。该活动最早于 2026 年 7 月初出现，7 月 24 至 25 日达到高峰，涉及 4000 多名用户的约 1.6 万次请求；截至 7 月 28 日，OpenAI 已瓦解涉及 1.5 万余名用户的相关活动。OpenAI 将核心活动归因于与月之暗面（Kimi 开发商）有关联的人员，并已通过 Frontier Model Forum 等渠道与业界和政府共享信息。这一事件凸显了大模型厂商之间围绕推理内容保护与合规使用边界的新一轮冲突。

telegram · zaihuapd · 10月1日 01:18

**「背景」** 模型蒸馏是指利用一个已训练模型（如 OpenAI 的 GPT 系列）的输出或行为来训练另一个更小或专用模型的技术。OpenAI 在 2026 年 9 月 30 日称其识别并瓦解了一场“对抗性蒸馏”活动，即攻击者试图通过大量交互提取其模型受保护的推理过程。OpenAI 将核心活动归因于与月之暗面（Kimi 开发商）相关人员，并称该活动最早出现在 2026 年 7 月初，7 月 24 至 25 日为高峰，涉及 4000 多名用户的 1.6 万次请求，7 月 28 日前已瓦解 1.5 万余名用户的相关活动。蒸馏本身是行业常见做法，但当它涉及提取受保护推理内容或违反服务条款时，就会被视为攻击行为。

**「影响」** 这一归因将直接影响 OpenAI 与月之暗面之间的行业信任关系，并可能促使各家模型厂商加强对蒸馏活动的监测与追责；但由于相关指控尚未获得月之暗面的公开回应或独立证实，结论仍需保持审慎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://metallab.ai/en/2026/10/openai-disrupts-model-distillation-campaign">OpenAI says it disrupted Moonshot -linked distillati… — METAL</a></li>
<li><a href="https://www.brocker.org/openai-disrupts-model-distillation-campaign-moonshot-attribution">OpenAI disrupts model - distillation campaign , cites Moonshot AI</a></li>
<li><a href="https://cellcog.ai/blog/openai-moonshot-distillation/">OpenAI Distillation Campaign : What It Says About Moonshot</a></li>

</ul>
</details>

**标签**: `#openai`, `#ai-security`, `#model-distillation`, `#moonshot-ai`, `#kimi`

---