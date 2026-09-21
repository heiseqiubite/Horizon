---
layout: default
title: "Horizon Summary: 2026-09-21 (ZH)"
date: 2026-09-21
lang: zh
---

> 从 32 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [Qwen Image 2.1：7B 开源模型，文字渲染与透明背景获好评](#item-tech-news-1) ⭐️ 8.0/10
2. [为何去污报告无法修复基准污染](#item-tech-news-2) ⭐️ 8.0/10
3. [美军因 AI 编造情报险些拦截中国船只](#item-tech-news-3) ⭐️ 8.0/10
4. [LG 电视被曝关机时录音，智能电视普遍追踪用户](#item-tech-news-4) ⭐️ 8.0/10
5. [长鑫科技第五代内存平台量产，24GB LPDDR5X 进驻国产旗舰手机](#item-tech-news-5) ⭐️ 8.0/10
6. [三星计划将 HBM4 产量翻倍以缓解 AI 内存瓶颈](#item-tech-news-6) ⭐️ 7.0/10
7. [ChatGPT 被曝使用广告追踪技术监听用户跨站行为](#item-tech-news-7) ⭐️ 7.0/10
8. [Vendure 跨渠道 IDOR 漏洞源码复盘](#item-tech-news-8) ⭐️ 7.0/10
9. [中国移动与高通完成 U6G 频段 6G 原型对接测试](#item-tech-news-9) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen Image 2.1：7B 开源模型，文字渲染与透明背景获好评](https://qwen.ai/blog?id=qwen-image-2.1) ⭐️ 8.0/10

通义千问发布 Qwen Image 2.1，这是仅 7B 参数的开源权重图像生成模型，显著小于前代 Qwen-Image（20B）。该模型原生支持透明背景，并以出色的文字渲染能力著称，被认为是当前开源权重市场中文本表现最佳的模型。尽管许可证更为严格（不同于前代许多 Qwen 模型的 Apache 许可），社区仍高度关注，并认为其技术价值突出。

hackernews · jmillikin · 9月20日 13:09 · [社区讨论](https://news.ycombinator.com/item?id=49775499)

**「背景」** Qwen 系列是阿里巴巴开发的开源大语言模型家族，此前发布的 Qwen-Image 1 拥有约 200 亿参数，属于体量较大的图像生成模型。Qwen Image 2.1 是该系列的最新图像模型，参数规模缩减至约 70 亿，同时原生支持生成透明背景图像（无需后处理抠图），并可通过 Diffusers 框架或 ComfyUI 等工具在本地部署使用。与 Qwen 以往多采用 Apache 等宽松许可的模型不同，此版本采用了明显更严格的许可证，这一点引发了社区的广泛关注和讨论。

**「影响」** 对需要在本地环境生成含清晰文字和透明背景图像的开发者与设计师而言，Qwen Image 2.1 提供了显著优于现有开源模型的质量，但严格许可证限制了其在商业和衍生场景中的使用。

**「社区讨论」** 社区评论肯定了模型体积小（7B）、原生透明背景以及优秀的文字渲染能力，尤其与 gpt-image-2 对比表现亮眼；同时也指出该模型的许可证比前代更严格，成为主要担忧点。部分用户还提到本地图像生成的整体水平已领先本地代码生成，实用性很高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen-Image-2.1">Qwen / Qwen - Image - 2 . 1 · Hugging Face</a></li>
<li><a href="https://github.com/QwenLM/Qwen-Image-2.1">GitHub - QwenLM/ Qwen - Image - 2 . 1 : Qwen &#x27;s most powerful...</a></li>

</ul>
</details>

**标签**: `#image generation`, `#open-source AI`, `#machine learning`, `#text-to-image`, `#Qwen`

---

<a id="item-tech-news-2"></a>
### [为何去污报告无法修复基准污染](https://www.reddit.com/r/MachineLearning/comments/1wlimaj/why_decontamination_reports_cant_fix_benchmark/) ⭐️ 8.0/10

今年 2 月，OpenAI 停止报告 SWE-bench Verified 并建议其他实验室也停止使用该基准，因为其测试的所有前沿模型都能重现部分任务的人类参考修复或问题陈述的逐字细节；六个月内性能仅提升 6 分，剩余分数中有多少真实能力已难以判断。作者指出，惯例的去污报告（声称训练数据中未发现基准内容）因三个结构性原因无法奏效：实验室自查无人能复核、语料库因版权诉讼风险不能公开、匹配机制漏掉改写、论坛教程、GitHub 解决方案及从基准生成的合成数据。为此他提出翻转评估权责的方案：评估方掌控测试，提交方不获标签、评估过程离线运行、评估方从指定提交自行构建代码并复现分数、测试数据尽量在提交冻结后生成，且结果必须可复现才计入。作者承认该方案未证明基准本身质量、隐藏测试集无法被反复提交挤压、出资方未泄露标签及第三方无法无数据重跑，并公开征求质疑，同时已用表格模型和私有测试集构建了小型实现。

reddit · r/MachineLearning · /u/NoahPersaud · 9月20日 14:31

**「背景」** 基准污染指大型语言模型的训练数据中混入测试样本，使模型在评估时通过记忆而非真实能力得分。去污报告是实验室声称其训练语料中未检索到测试内容的常规做法，SWE-bench Verified 则是用于评估模型实际软件工程修复能力的常用基准。

**「影响」** 依赖 SWE-bench Verified 等公共基准衡量模型能力的团队，在 OpenAI 退役该基准及去污报告局限被公开后，需要重新审视已有榜单分数的可信度，并向由评估方把控、可复现的评估协议迁移；不过作者提出的方案目前仅以小型实现呈现，尚未经大规模第三方验证。

**标签**: `#benchmark contamination`, `#AI evaluation`, `#machine learning`, `#SWE-bench`, `#LLM evaluation`

---

<a id="item-tech-news-3"></a>
### [美军因 AI 编造情报险些拦截中国船只](https://www.cnn.com/2026/09/18/politics/us-military-ai-false-intelligence-china-ship) ⭐️ 8.0/10

今年春天，美军针对一艘中国船只的武装拦截行动在军机升空后才被叫停，而驱动这次行动的核心情报由 AI 聊天机器人凭空编造。美国特种作战司令部一名情报分析员用 AI 聊天机器人将公开来源情报与机密信号情报融合分析，机器人错误识别了船上的货物清单；该分析员随后又用 AI 把错误结论包装成格式规范的正式情报报告，分发给各指挥层级。据四名知情人士透露，美军随即启动拦截该船的计划，其中两人称武装人员已准备登船、军机已经起飞，直到行动前夕官员深挖报告来源才发现整份报告由 AI 生成、货物信息有误。该事件凸显 AI 幻觉与自动化偏差在军事决策中可能直接触发真实武装行动的严重风险。

telegram · zaihuapd · 9月20日 03:07

**「背景」** 生成式 AI 聊天机器人在军事和情报领域正被用于融合多源信息、生成分析报告，其输出内容可能包含与事实不符的“幻觉”信息。当分析员缺乏独立核查机制、将 AI 生成的结论直接作为正式情报分发时，错误输入即可进入高风险指挥决策链，而人工核对环节的“橡皮图章式”放行会进一步放大这一风险。

**「影响」** 该事件显示 AI 编造的情报已具备触发真实军事冲突的现实可能，证明未经验证的 AI 输出一旦进入指挥链条即可导致武装行动的启动，防务部门将不得不对 AI 生成情报报告引入严格的来源追溯与人工独立核查流程。由于本次拦截仅在行动前夕靠人力追溯才被制止，当前 AI 辅助情报工作流中缺乏可证明有效性的验证机制的风险依然存在。

**标签**: `#ai-safety`, `#ai-hallucinations`, `#military-ai`, `#human-in-the-loop`, `#generative-ai`

---

<a id="item-tech-news-4"></a>
### [LG 电视被曝关机时录音，智能电视普遍追踪用户](https://www.theverge.com/tech/997682/every-tv-company-is-spying) ⭐️ 8.0/10

Gamers Nexus 发布了一段时长超过两小时的调查视频，声称 LG 智能电视在看似关机的情况下仍会录制并存储音频、追踪观看内容，甚至可能被远程入侵而沦为监控设备。报道还指出，几乎所有智能电视厂商都会通过自动内容识别（ACR）技术追踪用户的观看数据并与合作方共享，相关授权通常隐藏在冗长的用户协议中。LG 的回应未能平息用户的愤怒情绪。调查进一步显示，在被 root 之后，电视麦克风在语音指令结束后仍会继续录音 10 至 15 秒。专家呼吁出台联邦隐私法，要求获得用户明确同意并限制数据收集范围。

telegram · zaihuapd · 9月20日 04:22

**「背景」** Gamers Nexus 是一个以深度硬件测试和拆解闻名的技术媒体，此次调查通过 root 电视文件系统并进行网络抓包，发现 LG 智能电视在屏幕看似关闭时仍会通过麦克风录音，并在联网后上传数据，同时还会扫描家庭网络以识别附近的设备。自动内容识别（ACR）是行业普遍采用的技术，几乎所有智能电视都会通过它追踪观看内容并共享给广告合作方，通常隐藏在冗长的用户协议中，而 LG 的回应力图淡化问题，但未能平息用户的担忧。

**「影响」** 对 LG 智能电视用户而言，其音频和观看数据可能在看似关机时仍被采集，并存在被远程入侵成为监控设备的现实风险；这一披露也将整个行业普遍存在的 ACR 追踪行为置于监管焦点，或加速联邦隐私立法的推进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html">LG smart TVs caught logging audio with screen off and snooping on...</a></li>
<li><a href="https://www.breezyscroll.com/technology-news/lg-smart-tvs-record-audio-scan-home-network/">LG Smart TVs Caught Scanning Home Networks and Recording ...</a></li>
<li><a href="https://astig.ph/lg-smart-tv-privacy-records-audio-investigation-2026/">Is your LG smart TV listening to you? Investigation says it records ...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#smart-tv`, `#data-collection`, `#firmware`

---

<a id="item-tech-news-5"></a>
### [长鑫科技第五代内存平台量产，24GB LPDDR5X 进驻国产旗舰手机](https://m.thepaper.cn/newsDetail_forward_34108116) ⭐️ 8.0/10

长鑫科技于 9 月 20 日在 2026 世界制造业大会上宣布其第五代技术平台正式量产，基于该平台打造的 24GB LPDDR5X 产品已进入量产，并全面进入国产主流旗舰手机。该平台将内存阵列有源区半间距缩至 11.95 纳米，存储器电容深宽比达 45:1，核心动能区高度降至 6762 纳米。在同等条件下，每张晶圆的产出较上一代平台提升 50%以上。这一进展体现了中国存储芯片在先进制程和 3D 结构工艺上的推进，对 DRAM 市场格局和国产供应链具有重要意义。不过该消息目前仅来自官方发布，尚缺乏独立的第三方验证数据。

telegram · zaihuapd · 9月20日 05:19

**「背景」** 长鑫科技（长鑫存储）是中国规模最大、技术最先进的 DRAM 研发与制造一体化企业，自 2016 年成立以来专注于存储芯片自主发展，目前全球市占率已升至第四位，仅次于三星、SK 海力士与美光。它采用“BWL（埋入式字线）加堆叠电容”的架构，这也是全球三大 DRAM 厂商当前的主流技术路线，为其近年来的快速迭代奠定了基础。

**「影响」** 第五代 DRAM 平台量产让国产内存首次实质性切入长期由三星、SK 海力士、美光把持的高端智能手机内存市场，并为长鑫科技已获上市委会议通过的科创板 IPO 提供了可直接转化的量产产品支撑。不过，现阶段该平台是在无 EUV 条件下通过 DUV 多重曝光达到 1c 节点量级，每比特成本仍高于国际三巨头，HBM 等高端领域尚未突破，因此长鑫短期内更多扮演通用存储补位者的角色，而非全系列竞争者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-cn/%E9%95%BF%E9%91%AB%E5%AD%98%E5%82%A8">长鑫存储 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.21jingji.com/article/20260625/herald/2ae96cf459babea7b4794efa8e88e91f.html">长鑫科技深度报告：从零起步，10年追赶，剑指全球第三！ - 21经济网</a></li>
<li><a href="https://www.zhihu.com/question/2042900633947038528">中国第一大 DRAM 厂商长鑫科技科创板IPO获上市委会议通过，会对国产芯片市场有怎样的影响？ - 知乎</a></li>
<li><a href="https://www.huxiu.com/article/4892686.html">长鑫存储宣布第五代DRAM技术平台G5量产，工艺达1c节点级别</a></li>
<li><a href="https://www.sina.cn/weibo/detail/5345372936340318.html">国产内存终于啃下高端市场，这条产业链谁最受益？|长鑫存储|dram_新浪新闻</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#LPDDR5X`, `#semiconductor-manufacturing`, `#ChangXin`, `#memory`

---

<a id="item-tech-news-6"></a>
### [三星计划将 HBM4 产量翻倍以缓解 AI 内存瓶颈](https://en.sedaily.com/finance/2026/09/20/samsung-to-double-hbm4-output-next-year-sources-say) ⭐️ 7.0/10

据业内人士透露，三星电子计划明年将其 HBM4 和 HBM4E DRAM 的产量提高一倍以上，此举有望缓解 AI 加速器所需高带宽内存的供应紧张问题。该扩产计划直接回应了当前 HBM 供应成为 AI 硬件制造关键瓶颈的现状。HBM4 是新一代高带宽内存标准，旨在提供更高的数据传输速率和能效，而 HBM4E 则被认为是其增强版本。这一举措可能对全球 AI 芯片供应链产生重要影响，尤其是在中国 AI 芯片生产受限于 HBM 产能的背景下。然而，报道并未提供具体的产能数字或时间表，仅表明三星意图大幅提升相关产品出货量。

hackernews · giuliomagnifico · 9月20日 17:38 · [社区讨论](https://news.ycombinator.com/item?id=49778029)

**「背景」** HBM（高带宽内存）通过垂直堆叠 DRAM 晶粒来提供远超传统内存的带宽，是 AI 加速器最关键的上游瓶颈之一。三星电子于 2026 年 2 月率先量产了业界首款商用 HBM4，并预计在 2026 年下半年开始提供 HBM4E 样品，2027 年启动定制 HBM 样品出货；此前 TrendForce 曾报道三星计划在 2026 年将 HBM 产能提升 50%。据行业消息，三星明年计划将 HBM4 和 HBM4E 的产量提高一倍以上，这将使玻璃载板需求增至原来的 2.5 倍。

**「影响」** 三星计划于 2026 年将 HBM4 及 HBM4E DRAM 产出扩大一倍以上，此举将直接缓解 AI 加速器供应链中存储部件的紧缺状况，并有望抑制因 AI 需求远超供应而持续攀升的 HBM 合约与现货价格。不过，该产能翻倍计划源自媒体报道而非三星官方公告，实际扩产幅度与时间表仍存在不确定性。

**「社区讨论」** 有评论指出，中国 AI 加速器生产的真正瓶颈在于 HBM 产能而非处理器或光刻设备，例如华为升腾的产量受限于长鑫存储（CXMT）的 HBM 能力。另有用户对先进封装中的晶圆减薄工艺表示兴趣，还有人对扩产可能推高消费级 DRAM 价格表示担忧，并有人表达了对 HBM 技术发展的消极情绪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.sedaily.com/finance/2026/09/20/samsung-to-double-hbm4-output-next-year-sources-say">Samsung to Double HBM4 Output Next Year, Sources Say - Seoul Economic Daily</a></li>
<li><a href="https://news.samsung.com/global/samsung-ships-industry-first-commercial-hbm4-with-ultimate-performance-for-ai-computing">Samsung Ships Industry-First Commercial HBM4 With Ultimate Performance for AI Computing – Samsung Global Newsroom</a></li>
<li><a href="https://www.trendforce.com/news/2025/12/30/news-samsung-reportedly-plans-50-hbm-capacity-surge-in-2026-spotlight-on-hbm4/">[News] Samsung Reportedly Plans 50% HBM Capacity Surge in 2026, Spotlight on HBM4</a></li>
<li><a href="https://intuitionlabs.ai/articles/hbm-dram-ai-memory-demand">HBM, DRAM &amp; AI Demand: Memory Supply and Price Trends</a></li>
<li><a href="https://supplyics.com/insights/market-intelligence/2026-hbm-dram-memory-supply-chain-analysis/">2026 HBM and DRAM Supply Chain Analysis: Navigating AI-Driven ...</a></li>
<li><a href="https://enkiai.com/data-center/hbm-supply-crisis-2026-the-bottleneck-redefining-ai/">HBM Supply Crisis 2026: The Bottleneck Redefining AI - ENKI</a></li>

</ul>
</details>

**标签**: `#HBM`, `#Memory`, `#AI Hardware`, `#Semiconductor Manufacturing`, `#Supply Chain`

---

<a id="item-tech-news-7"></a>
### [ChatGPT 被曝使用广告追踪技术监听用户跨站行为](https://www.buchodi.com/chatgpt-now-knows-what-you-do-on-other-websites-via-ad-collector/) ⭐️ 7.0/10

据博客文章报道，ChatGPT 正在使用广告行业常用的追踪技术（ad collector）来收集用户在其他网站上的活动数据，这在 AI 聊天产品中尚属首次，引发新的隐私担忧。该机制本身并非新技术，但其应用场景从传统广告平台扩展到 AI 对话助手，改变了用户对隐私的预期，尤其对订阅付费用户而言更显突兀。社区指出，Firefox、Brave 和 Safari 浏览器具备相应防护机制，而 Chrome 和 Edge 则未提供同等保护。目前该报道的来源是一篇 AI 生成的博客，其原始性和准确性受到质疑，但话题本身涉及 ChatGPT 的数据收集实践，对关注隐私的 AI 用户具有重要参考价值。

hackernews · lmbbuchodi · 9月20日 15:18 · [社区讨论](https://news.ycombinator.com/item?id=49776729)

**「背景」** 广告技术（adtech）追踪机制通常通过第三方追踪脚本或 Cookie 在用户访问不同网站时收集其浏览行为，用于广告定向投放，这是互联网行业长期存在的标准做法。OpenAI 已宣布开始测试在 ChatGPT 中展示广告，以支持免费访问并为公司创造收入来源，同时承诺提供清晰的广告标识和隐私保护。正是这一广告业务的引入，使得原本常见的标准广告追踪技术被应用于 AI 聊天产品这一新场景，进而引发了关于对话场景下隐私预期的讨论。

**「影响」** 使用 Chrome 或 Edge 浏览器的 ChatGPT 付费订阅用户可能面临跨站活动数据被收集的风险，其隐私期望与传统广告跟踪场景不同，但现有浏览器防护并不覆盖这些主流浏览器。

**「社区讨论」** 评论者普遍对 AI 聊天产品中应用标准广告技术感到不适，认为付费订阅服务不应依赖广告追踪模式；同时有用户质疑该博客为 AI 生成，缺乏原创性，并引用浏览器文档指出 Firefox、Brave 和 Safari 提供了防护而 Chrome 和 Edge 未提供。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/testing-ads-in-chatgpt/">Testing ads in ChatGPT | OpenAI</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#privacy`, `#ad tracking`, `#AI`, `#data collection`

---

<a id="item-tech-news-8"></a>
### [Vendure 跨渠道 IDOR 漏洞源码复盘](https://xz.aliyun.com/news/92859) ⭐️ 7.0/10

先知社区发布了对 Vendure 中编号为 GHSA-7qvr-c5vf-xxfh 的跨渠道 IDOR 漏洞的源码级复盘。该开源电商平台中，订单子实体（Payment、Refund、Fulfillment、OrderHistoryEntry）不携带渠道归属，唯一的渠道边界是父订单，因此渠道隔离只是逐调用点约定的机制而非系统性保证。受影响版本的多条 Admin mutation 仅按 ID 全局加载子实体，从不回查父订单的渠道归属，导致跨渠道越权访问。其中退款路径最为典型，其渠道检查寄生在“订单行存在”这一业务事实上，绕过了对父订单渠道的校验。该问题对依赖 Vendure 实现租户隔离的开发者和安全实践者具有直接参考价值。

rss · 先知社区 · 9月20日 02:51

**「背景」** Vendure 是一个开源的电商平台，其核心设计是使用 Channel（渠道）来隔离不同租户或商家之间的数据与操作权限。此次安全公告 GHSA-7qvr-c5vf-xxfh（未关联 CVE）在官方 GitHub Releases 中被确认为一种跨渠道的写 IDOR，即受渠道限制的管理员可以通过枚举资源 ID 来修改其他渠道的资产和库存位置。该文章则将这一漏洞具体定位为跨渠道的支付/退款 IDOR，意味着攻击者能够借此跨越租户边界操作资金流转。

**「影响」** 受影响的 Vendure 管理后台 API 存在跨渠道 IDOR 风险，攻击者可通过 Admin mutation 按 ID 读取或操作其他租户订单的支付、退款、履约与订单历史等子实体数据。Vendure 官方已为旧版本发布补丁，并建议用户尽快升级到最新 v3.6.x 或更高版本以关闭该漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vendurehq/vendure/releases">Releases · vendurehq/ vendure · GitHub</a></li>
<li><a href="https://xz.aliyun.com/news/92859">当授权边界住在父订单里： Vendure GHSA - 7 qvr - c 5 vf - xxfh ...</a></li>
<li><a href="https://github.com/vendurehq/vendure/releases">Releases · vendurehq/vendure - GitHub</a></li>

</ul>
</details>

**标签**: `#security`, `#vendure`, `#IDOR`, `#e-commerce`, `#authorization`

---

<a id="item-tech-news-9"></a>
### [中国移动与高通完成 U6G 频段 6G 原型对接测试](https://www.ithome.com/1/004/708.htm) ⭐️ 7.0/10

9 月 20 日，中国移动与高通在中国移动协同创新基地完成了全球首个符合 3GPP 最新定义的 U6G 频段 6G 原型基站与终端原型对接测试，覆盖下行 400 MHz、上行 200 MHz 超大信道带宽及 128 通道超大规模 MIMO。本次验证将基站与终端原型纳入同一条端到端链路，初步验证了未来 6G 网络、终端与业务协同演进的可行性。该测试标志着 6G 在 3GPP 定义框架下首次实现原型级别的跨厂商互操作验证，但仍是早期原型阶段，距 6G 正式商用部署尚需数年。

telegram · zaihuapd · 9月20日 05:49

**「背景」** 6G 是继 5G 之后的第六代移动通信技术，国际标准组织 3GPP 负责制定其规范；U6G 频段（6425–7125 MHz）属于 6G 候选频谱范围。本次测试基于中国移动协同创新基地的 6G 开放众创试验装置，属于 6G 关键技术从研究迈入系统化验证阶段的早期原型测试。中国移动与高通于 2025 年 9 月 20 日完成的此次对接测试采用 128 通道大规模 MIMO 基站（下行 400MHz、上行 200MHz，子载波间隔 30kHz），旨在验证 6G 端到端链路的可行性。

**「影响」** 该对接测试完成了 6G 原型基站与终端在同一端到端链路中的首次互通验证，为 U6G 频段作为从 5G-A 向 6G 平滑演进的核心预商用频段提供了首个原型级实证，巩固了中国移动与高通在 6G 预商用技术验证中的领先地位。不过，这仍属早期原型验证，U6G 的最终频谱分配和商用部署尚需等待后续 3GPP 标准工作的确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://worldattention.com/stories/china-mobile-and-qualcomm-6g-prototype-interoperability-test-in-u6g-band-656032e69f">China Mobile and Qualcomm complete world’s first 6G ...</a></li>
<li><a href="https://www.chinanews.com.cn/cj/2026/09-20/10699878.shtml">中国移动与高通完成U6G频段6G原型基站与终端原型对接测试</a></li>
<li><a href="https://www.gate.com/news/detail/china-mobile-qualcomm-complete-first-u6g-6g-prototype-test-with-400mhz-24411259">China Mobile, Qualcomm Complete First U6G 6G Prototype Test ...</a></li>
<li><a href="https://www.btl.com.tw/en/news/536">MWC2026 – In-depth Analysis of U6G, Wi-Fi 8 and 6G RF ...</a></li>
<li><a href="https://worldattention.com/stories/china-mobile-and-qualcomm-6g-prototype-interoperability-test-in-u6g-band-656032e69f">China Mobile and Qualcomm complete world’s first 6G prototype ...</a></li>
<li><a href="https://www.newbtl.com/men/industryshow.php?id=738">MWC2026 – In-depth Analysis of U6G, Wi-Fi 8 and 6G RF ...</a></li>

</ul>
</details>

**标签**: `#6G`, `#China Mobile`, `#Qualcomm`, `#telecommunications`, `#MIMO`

---