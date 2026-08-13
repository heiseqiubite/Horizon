---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 35 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [GPT-5.6 Sol Ultrafast 模式实现 7 倍推理加速](#item-tech-news-1) ⭐️ 8.0/10
2. [DRAM“意大利面条化”工具发布，硬件攻击面扩大](#item-tech-news-2) ⭐️ 8.0/10
3. [DeepSeek V4 Pro 0813 开放权重模型发布](#item-tech-news-3) ⭐️ 8.0/10
4. [worldproof 揭示像素指标无法排名世界模型](#item-tech-news-4) ⭐️ 8.0/10
5. [特朗普签署备忘录，允许私企海外网络攻击](#item-tech-news-5) ⭐️ 8.0/10
6. [DeepMind 手语转文字模型 SL2T 落地 Pixel 11](#item-tech-news-6) ⭐️ 8.0/10
7. [Gemini 3.7 Flash 发布](#item-tech-news-7) ⭐️ 7.0/10
8. [DeepSeek 发布 Harness 开发者预览版，实现可追溯 AI 代理框架](#item-tech-news-8) ⭐️ 7.0/10
9. [苹果拟为 Siri AI 按使用量付费购买新闻内容，预算或达九位数](#item-tech-news-9) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GPT-5.6 Sol Ultrafast 模式实现 7 倍推理加速](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 与 OpenAI 联合宣布，其 GPT-5.6 Sol 模型在 Ultrafast 模式下处理 HLE 推理基准测试时，仅用 11 小时 11 分钟完成全部 2500 道问题，相比 Claude Fable 5 的 78 小时 27 分钟，推理速度提升近 7 倍。这一加速使前沿 AI 推理任务能在单个工作日内完成，有望大幅缩短等待时间，提升复杂思考的迭代效率。然而，官方并未明确声明 Ultrafast 模式下的准确率与标准 GPT-5.6 Sol 完全一致，性能对等性尚待验证。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**「背景」** HLE（Human-Like Evaluation）是一套高难度推理基准测试，用于衡量模型在复杂认知任务上的表现。Cerebras 是一家专注于高性能 AI 芯片的公司，其晶圆级引擎硬件专门针对大模型推理加速，此次与 OpenAI 合作将 GPT-5.6 Sol 部署于该硬件上，以提升推理速度。

**「影响」** 前沿 AI 开发者与研究人员可借助该加速方案，在更短时间内获得复杂推理结果，加速实验迭代和原型验证；但若最终准确率存在折损，其实用价值将受到限制。

**「社区讨论」** 社区普遍认可推理加速对提升思考质量的重要性，尤其是通过迭代改进复杂推理。但多位评论者指出，官方未确认 Ultrafast 模式下的准确率与标准 GPT-5.6 Sol 完全对等，且未公布定价，引发了对性能折损和实际可及性的担忧。

**标签**: `#AI`, `#inference`, `#performance`, `#LLM`, `#hardware`

---

<a id="item-tech-news-2"></a>
### [DRAM“意大利面条化”工具发布，硬件攻击面扩大](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 8.0/10

著名安全研究员 Christopher Domas 公开了一款名为“skitter-creek-bath-salts”的工具，用于对 DRAM 进行“意大利面条化”（spaghettifying），即通过操纵 DRAM 控制器的内部状态，使内存访问行为变得混乱且难以预测。该工具利用现代 DRAM 控制器的复杂性，攻击者在获得 ring 0 权限后，可深入“负 ring”区域，完全控制内存子系统，从而绕过传统的安全边界。根据 README，该工具目前适用于 AMD Jaguar 架构（2013 年），但已提及 Zen 3 的寄存器基址不同，暗示可能扩展到较新处理器。此技术直接威胁依赖硬件信任根的平台，如游戏主机（Xbox、PlayStation），一旦取得 ring 0，后续攻击面将完全敞开。工具将配合即将举行的 Black Hat 演讲公开，进一步揭示 DRAM 控制器中的隐蔽攻击面。

hackernews · matt\_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**「背景」** 现代 DRAM 控制器通过地址加扰（bank swizzle）将物理地址非线性映射到内存芯片的实际行、列和存储体，以优化性能并增加逆向工程难度。在某些 AMD 处理器上，内存控制器中的地址转换寄存器可被操纵，从而改变这一映射，打破原本由硬件强制实施的内存隔离，使攻击者能够访问平台安全处理器（PSP）、系统管理模式（SMM）内存和 CPU 微码等隐藏区域。该技术已在 AMD Family 16h（Jaguar）架构上演示，该架构常见于 2013 年的游戏主机和低功耗设备。

**「影响」** 在基于 AMD Jaguar 处理器的系统（如 Xbox One、PlayStation 4）上，拥有 ring-0 权限的攻击者现在可以通过操纵内存控制器访问硬件管理的 DRAM 内部状态，从而打破了原本隔离 ring-0 与内存子系统的安全边界。目前尚不清楚该技术是否能扩展到 Zen 3 等更新的 AMD 平台或其他 CPU 供应商。

**「社区讨论」** 社区对 Domas 的演讲表示极大期待，认为其过往研究讲解深入浅出。讨论中，人们普遍担忧该技术可能动摇游戏主机的安全根基，同时对工具在 AMD Jaguar 之外 CPU 上的实际适用性存疑，目前仅有 Zen 3 寄存器地址差异的初步线索，尚不明确是否可发起有效攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/amd-hardware-vulnerability-exposed-by-dram-address-scrambling-research">AMD DRAM Scrambling Exploit Bypasses Security Fences | Linxi News</a></li>
<li><a href="https://lwn.net/Articles/1088778/">Domas: Bypassing memory protection with AMD&#x27;s memory ...</a></li>
<li><a href="https://zeli.app/en/story/49286341">Spaghettifying DRAM: Unlock Everything on the CPU | Zeli</a></li>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>

</ul>
</details>

**标签**: `#hardware security`, `#DRAM exploitation`, `#low-level programming`, `#reverse engineering`, `#memory protection`

---

<a id="item-tech-news-3"></a>
### [DeepSeek V4 Pro 0813 开放权重模型发布](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 8.0/10

DeepSeek 发布了最新的 DeepSeek V4 Pro 0813 模型，拥有 1.7 万亿参数，权重已在 Hugging Face 开放下载（893 GB）。该模型通过 API 提供，支持低、中、高三种推理强度，Simon Willison 的测试显示不同推理级别下生成的图像风格差异显著。基准测试信息目前仅从非官方渠道流传，官方未发布正式公告。模型设计面向高级推理、代码生成与长周期 Agent 工作流，上下文窗口达 100 万 token，API 价格为输入每百万 token 0.1537 美元、输出 0.8697 美元。

rss · Simon Willison · 8月12日 23:59

**「背景」** DeepSeek 此前已于四月和七月分别发布了 V4 Pro 和 V4 Flash 模型，并均开放了权重，因此本次 V4 Pro 0813 的开放权重延续了该公司一贯的开放策略，并非意外之举。

**「影响」** 研究人员和开发者可立即在本地部署或通过 OpenRouter 等 API 使用该模型，其可调节的推理强度为创意生成任务提供了新的控制手段，可能促进相关应用开发。

**标签**: `#DeepSeek`, `#open-weight model`, `#AI model release`, `#large language models`, `#Hugging Face`

---

<a id="item-tech-news-4"></a>
### [worldproof 揭示像素指标无法排名世界模型](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

worldproof 是一个开源诊断工具，用于分析世界模型根据起始帧和动作序列预测未来帧时在何处、为何失败。作者在验证过程中发现，传统像素指标（如 SSIM、PSNR）在真实机器人视频上无法有效区分模型性能：即使使用“复制最后一帧”的简单基线，其 SSIM 也可达 0.983，且误差不随预测步数增加而增加。进一步测量表明，在 DROID 数据集上，指标随步数先饱和、后单调下降、再饱和，只有约 8 至 24 步的区间内模型可被区分，该窗口取决于帧率与任务速度。该工具还提供动态区域掩码变体、基于分层自助法的置信区间聚合以及多种保真度与物理不变性指标，已以 Apache-2.0 协议开源。

reddit · r/MachineLearning · /u/georgia\_bucea · 8月13日 19:58

**「背景」** 世界模型旨在从观测和动作序列预测未来帧，常用于机器人学习与具身智能。评估这类模型常采用 SSIM、PSNR、LPIPS 等像素级指标，衡量预测帧与真实帧的相似度，但这些指标在静态背景占主导的机器人视频中容易被高估，且可能无法反映对动态变化的预测能力。

**「影响」** 对于使用真实机器人视频的世界模型研究者，评估时必须根据帧率和任务速度确定可用的评价步数窗口，否则传统的像素指标可能无法有效区分模型性能，导致错误排名。

**标签**: `#world models`, `#evaluation`, `#pixel metrics`, `#robot video`, `#open-source tool`

---

<a id="item-tech-news-5"></a>
### [特朗普签署备忘录，允许私企海外网络攻击](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 8.0/10

美国总统特朗普签署备忘录，允许私营企业在联邦政府直接控制和监督下，于海外开展监控和网络攻击，以打击针对美国人的外国网络化跨国犯罪组织。国土安全部将负责运行该项目，并与司法部协调监督；参与企业须维持至少 100 万美元的保证金或托管款，违约即被没收。该政策将私营部门纳入进攻性网络行动，标志着美国网络战策略的重大转变。

telegram · zaihuapd · 8月13日 05:10

**「背景：美国网络攻击政策的历史演变」** 以往，进攻性网络行动主要由美国网络司令部、国家安全局等政府机构执行，私营企业仅被允许进行被动防御，法律明令禁止其主动“回击”黑客。2026 年 8 月 12 日，特朗普总统签署备忘录，首次授权经审查的私营公司在政府监督下，针对外国网络犯罪组织开展网络监控与网络效应操作，打破了此前的政策界限。

**「政策影响」** 该举措将使美国在进攻性网络行动中更加依赖私营部门，使其模式接近于中国和俄罗斯长久以来利用私企黑客辅助国家安全任务的做法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberscoop.com/trump-memo-private-sector-offensive-hacking/">Trump turns to private sector in offensive hacking operations memo | CyberScoop</a></li>
<li><a href="https://www.techtimes.com/articles/324233/20260813/trump-deputizes-private-companies-offensive-cyber-strikes-against-foreign-criminals.htm">Trump Deputizes Private Companies for Offensive Cyber Strikes Against Foreign Criminals</a></li>
<li><a href="https://www.nytimes.com/2026/08/13/us/politics/trump-private-companies-hacking-cybercriminals.html">Trump Gives Green Light to U.S. Companies to Aim Hacks at ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#government-policy`, `#offensive-cyber`, `#private-sector`, `#surveillance`

---

<a id="item-tech-news-6"></a>
### [DeepMind 手语转文字模型 SL2T 落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

谷歌 DeepMind 发布了大规模多语言手语转文字模型 SL2T，首次将手语 AI 集成到消费产品中，目前已在 Pixel 11 的 Gboard 键盘和 Live Transcribe 实时字幕应用中上线，支持美国手语转英语。该模型使用超过 10 万小时、涵盖 50 多种手语的数据进行训练，在 FLEURS-ASL 基准上以零样本方式取得 70 BLEURT 分数，远高于此前的最佳纪录。为保护隐私，SL2T 仅处理手部和身体姿态关键点，不读取原始视频流。

telegram · zaihuapd · 8月13日 08:55

**「背景」** 手语识别与翻译通常需要分析原始视频，存在隐私风险和较高的计算开销，而基于姿态关键点的方法能有效缓解这些问题。FLEURS-ASL 是评估多语言手语转文本翻译质量的基准，BLEURT 是一种自动评价指标，分数越高表示译文与参考译文越接近。

**「影响」** Pixel 11 用户现在可以通过 Gboard 和 Live Transcribe 直接将美国手语转换为英语文字，为使用美国手语的听障群体提供了更便捷的实时沟通方式。后续计划扩展至更多设备和语言，虽然具体时间表尚未公布，但路径已明确。

**标签**: `#sign-language-recognition`, `#pose-estimation`, `#accessibility`, `#DeepMind`, `#machine-translation`

---

<a id="item-tech-news-7"></a>
### [Gemini 3.7 Flash 发布](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

谷歌发布了 Gemini 3.7 Flash 模型，这是其成本效益型 Flash 系列的一次小幅更新，主要增强了视觉理解能力。该模型在 Gemini API 上提供，采用限时优惠定价，至 2026 年 12 月 31 日前输入/输出 token 价格较低，之后将翻倍。社区测试显示，在图像转 HTML 等视觉任务上，Gemini 3.7 Flash 表现优于价格相近的同类模型，但仍不及 Opus 5。此次更新侧重于高容量、低成本的文本与视觉应用场景，其定价策略和快速迭代引发开发者关注。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**「背景」** Gemini Flash 系列是 Google 推出的低成本 AI 模型，此前 Gemini 3.6 Flash 于三周前刚刚发布。本次 Gemini 3.7 Flash 在发布时附带阶段性优惠定价，输入价格为每百万 tokens 0.75 美元，输出为 3.75 美元，该价格将于 2026 年 12 月 31 日后上调至标准费率。

**「影响」** 对于当前使用 Gemini Flash 模型的开发者，限时优惠可降低短期成本，但 2026 年底后的价格翻倍以及模型快速迭代可能导致长期规划的不确定性。

**「社区讨论」** 社区测试中，Gemini 3.7 Flash 在图像转代码任务上表现尚可但非顶尖，有用户认为 Opus 5 仍是最佳。开发者对限时优惠定价感到困惑，因为模型可能很快被新版本取代；部分用户指出其相对于更低成本竞品（如 Luna）的价值优势不明显。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://venturebeat.com/technology/googles-gemini-3-7-flash-targets-coding-and-agents-with-a-50-introductory-price-cut">Google’s Gemini 3.7 Flash targets coding and agents with a 50% introductory price cut | VentureBeat</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262103251-google-google-gemini-3-7-flash-models-coding-agent-benchmarks-introducing-tradingkey">Google Launches Gemini 3.7 Flash: Major Leap in Coding and Agent Capabilities, Three-Week Iteration Sets New Speed Record for Low-Cost Models</a></li>

</ul>
</details>

**标签**: `#AI`, `#machine-learning`, `#Google`, `#Gemini`, `#model-release`

---

<a id="item-tech-news-8"></a>
### [DeepSeek 发布 Harness 开发者预览版，实现可追溯 AI 代理框架](https://deepseek.com/harness/en/) ⭐️ 7.0/10

DeepSeek 发布了开源开发者预览版框架 Harness，用于构建具备可追溯和热重载插件系统的 AI 代理。该框架基于 Cordis v4 论文，将每个运行记录为仅追加的会话日志，涵盖系统提示、推理、工具调用和上下文注入，并支持从同一事件流中恢复、分叉和回放。其核心架构采用“一切皆插件”，允许插件在运行时动态加载与卸载，并自动回退副作用。目前以 MIT 许可证发布，但作者提醒此为早期版本，可能包含大量粗糙边缘和破坏性兼容变更。

hackernews · bjin · 8月13日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**「背景」** 该框架建立在 Cordis v4 论文之上，该论文描述了一种支持热重载和卸载时自动清理副作用（如连接、内存分配、注册处理程序等）的插件系统架构。Cordis 已在另一个名为 Koishi 的项目中使用了四年，而 Harness 将其扩展至 AI 代理领域，使得 UI 组件等也可动态启用/销毁。

**「影响」** 对于 AI 代理开发者，Harness 提供了美国模型通常不提供的完整会话可追溯性，有望加速开源代理工具的开发，尽管其早期预览状态意味着需要应对频繁的破坏性变更。

**「社区讨论」** 社区普遍认可其可追溯性为亮点，但对其完全基于插件的架构反应不一，部分开发者表示对插件模式感到疲劳；作者本人提醒该版本尚处早期预览，预期存在大量不兼容变更。

**标签**: `#AI agents`, `#developer tools`, `#open-source`, `#deepseek`, `#traceability`

---

<a id="item-tech-news-9"></a>
### [苹果拟为 Siri AI 按使用量付费购买新闻内容，预算或达九位数](https://9to5mac.com/2026/08/12/report-apple-seeks-publisher-deals-to-give-siri-ai-better-access-to-current-events/) ⭐️ 7.0/10

苹果正在与出版商洽谈多年内容授权协议，为预计于 2026 年晚些时候推出的 Siri AI 提供当前新闻与信息。区别于大型 AI 公司常见的预付固定授权费，苹果讨论了按内容使用量向合作方付费的方案，整体预算可能达到九位数。该模式若落地，或重塑 AI 助手与新闻出版业的商业关系，但苹果目前拒绝置评，且尚未宣布任何合作。

telegram · zaihuapd · 8月13日 04:40

**「背景」** Siri AI 是苹果计划推出的新一代语音助手，旨在通过更智能的信息检索与生成能力提供实时新闻等服务。当前 AI 公司通常以一次性预付款方式获取新闻内容授权，而按使用量付费的模式更贴近实际内容消耗，可能降低前期成本并更灵活地反映价值。

**「影响」** 该模式若成功实施，可能促使出版商与 AI 公司转向基于实际使用量的计费方式，从而改变内容授权的商业惯例，但其实际影响将取决于 Siri AI 的最终推出情况与市场采用程度。

**标签**: `#Apple`, `#Siri`, `#AI`, `#news licensing`, `#tech industry`

---