---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 38 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [滑动窗口注意力在长上下文推理上击败线性注意力](#item-tech-news-1) ⭐️ 8.0/10
2. [库克卸任苹果 CEO，特努斯接棒聚焦 AI 与折叠屏 iPhone](#item-tech-news-2) ⭐️ 8.0/10
3. [DeepSeek 发布 V4 系列首款多模态实验模型权重](#item-tech-news-3) ⭐️ 8.0/10
4. [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展，包括 uBlock Origin](#item-tech-news-4) ⭐️ 7.0/10
5. [ChatGPT Work 工具与技能参考：Playwright 浏览器自动化亮点](#item-tech-news-5) ⭐️ 7.0/10
6. [NAT 与互联网中心化的“原罪”之争](#item-tech-news-6) ⭐️ 7.0/10
7. [wrapture：将 wrapt 补丁扩展为测试与追踪工具](#item-tech-news-7) ⭐️ 7.0/10
8. [HN 文摘：OpenShot 4.0 本地 AI 调色与 Chrome 扩展变动](#item-tech-news-8) ⭐️ 7.0/10
9. [GNN 时序泄漏问题与 SynthFin-AML 基准的提出](#item-tech-news-9) ⭐️ 7.0/10
10. [Entropic Scree：评估脏数据信号强度的新诊断工具](#item-tech-news-10) ⭐️ 7.0/10
11. [Claude 遭窃密木马劫持账号，Anthropic 强制登出并删付款信息](#item-tech-news-11) ⭐️ 7.0/10
12. [OpenClaw 发布最大更新 2.0](#item-tech-news-12) ⭐️ 7.0/10
13. [MiniMax 与智谱上半年收入大幅增长但仍亏损](#item-tech-news-13) ⭐️ 7.0/10
14. [欧盟将 ChatGPT、Reddit、Roblox 列为超大型服务](#item-tech-news-14) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [滑动窗口注意力在长上下文推理上击败线性注意力](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

一篇新的 arXiv 预印本论文（编号 2608.28444，作者为 Alexia Jolicoeur-Martineau、Rhea Sanjay Sukthanker、Pashmina Cameron 和 Emy Gervais）声称，带 sink 的滑动窗口注意力（SWA）在长上下文推理基准测试中的表现优于线性注意力变体。论文报告称，在 Needle-in-a-Haystack 和 BABILong 两项任务上，SWA 的性能比线性注意力高出 2 到 10 倍。作者指出，这一研究方向此前未与更简单的基线进行适当比较，而他们的方案无需后训练、运行速度快且内存占用低。论文明确推荐“改用 SWA 而不是后训练线性模型”，并承认线性注意力可能需从头训练或大量后训练才能达到 SWA 的水平。该结果对当前耗费后训练算力来生产线性注意力模型的做法提出了直接挑战。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 8月31日 16:35

**「背景」** 标准 Transformer 的注意力机制具有二次方计算复杂度，导致长上下文处理成本高昂。为缓解这一问题，研究者提出了多种方案，包括线性注意力（将复杂度降低到线性）和滑动窗口注意力（仅关注局部窗口，同时利用 sink token 保持全局信息）。后者被认为更为简单，但此前在长上下文推理任务上缺乏系统对比。

**「影响」** 对正在投入大量算力进行后训练以生产线性注意力模型的研究团队和工程团队而言，该结果意味着可能需要重新评估技术路线，因为更简单的 SWA 基线在推理任务上可能更高效且效果更好。不过，该结论基于论文选取的基准测试，在其他任务或实际部署场景中的普适性仍需进一步验证。

**标签**: `#sliding-window attention`, `#linear attention`, `#long-context reasoning`, `#LLM efficiency`, `#arXiv preprint`

---

<a id="item-tech-news-2"></a>
### [库克卸任苹果 CEO，特努斯接棒聚焦 AI 与折叠屏 iPhone](https://www.bloomberg.com/news/articles/2026-08-30/apple-s-new-ceo-john-ternus-takes-reins-from-tim-cook-focusing-on-ai) ⭐️ 8.0/10

8 月 31 日是蒂姆·库克担任苹果 CEO 的最后一天，51 岁的硬件工程老将约翰·特努斯自 9 月 1 日起接任 CEO，库克将继续留任执行主席。库克在全员信中表示不会离开苹果，并称赞特努斯聪慧、优秀、能力出众。新 CEO 的头号任务是推动 AI 落地，补齐 Siri 升级延期等短板。苹果秋季发布会定于 9 月 9 日，首款折叠屏 iPhone 届时亮相，据称配备 12GB RAM 并深度植入 Siri AI，可结合屏幕、日历与相机理解现实场景。

telegram · zaihuapd · 8月31日 10:21

**「背景：特努斯其人」** 约翰·特努斯生于 1975 年，毕业于宾夕法尼亚大学机械工程专业，曾任苹果硬件工程高级副总裁，负责 iPhone、iPad、Mac、Apple Watch、AirPods 和 Apple Vision Pro 等产品的硬件开发。他自 2016 年起领导苹果硬件工程团队，此前在 Virtual Research Systems 担任机械工程师。2026 年 9 月 1 日，在苹果工作 25 年后，他正式接替蒂姆·库克出任 CEO。

**「影响」** 特努斯接任 CEO 后的首个公开考验将是 9 月 9 日发布的折叠屏 iPhone，市场将据此判断苹果能否重振长期停滞的 AI 布局；若进展缓慢，苹果与谷歌、OpenAI 等对手的 AI 差距将持续成为投资者关注的风险点。

**「社区讨论」** 未提供社区评论，故省略此块。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/John_Ternus">John Ternus - Wikipedia</a></li>
<li><a href="https://www.apple.com/leadership/john-ternus/">Apple Leadership - John Ternus - Apple</a></li>
<li><a href="https://www.britannica.com/money/John-Ternus">John Ternus | Incoming Apple CEO &amp; Hardware Engineering Executive | Britannica Money</a></li>
<li><a href="https://marketwise.com/investing/tim-cook-apple-ceo-steps-down-john-ternus-successor-investors-impact/">What Apple&#x27;s CEO Change to John Ternus Means for Investors - MarketWise</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262141791-apple-ternus-ceo-ai-siri-iphone-tim-jay-tradingkey">Apple Leadership Change Imminent: What Challenges Face New CEO Ternus, and Can He Lead Apple to Win the AI War?</a></li>

</ul>
</details>

**标签**: `#Apple`, `#CEO transition`, `#AI`, `#Siri`, `#iPhone`

---

<a id="item-tech-news-3"></a>
### [DeepSeek 发布 V4 系列首款多模态实验模型权重](https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp) ⭐️ 8.0/10

DeepSeek 发布了 V4 系列首款实验性多模态模型 DeepSeek-V4-Flash-Vision-Exp，其权重已公开在 Hugging Face 上。该模型在 V4-Flash 架构基础上加入视觉模块并继续训练，从而具备视觉理解能力。相比 V4-Flash-0731，其多模态 agent 能力显著提升，ApexBench 得分从 26.2 升至 36.5，而文本 agent 任务表现基本持平。模型目前处于实验性状态，适合 AI 开发者和研究者下载评测其视觉与多模态能力。

telegram · zaihuapd · 8月31日 11:41

**「背景信息」** DeepSeek 的 V4 系列此前以纯文本模型（如 V4-Flash-0731）发布，而 DeepSeek-V4-Flash-Vision-Exp 是该系列首次在 Flash 架构上加入视觉模块的实验性多模态版本，通过持续训练提升多模态 agent 能力。ApexBench 是用于评估多模态 agent 表现的基准，DeepSeek 在该模型中报告了 Pass@1 成绩，成绩从 26.2 提升至 36.5，同时文本 agent 任务表现基本持平。

**「影响」** 该模型权重已在 Hugging Face 公开发布，并同步上线 DeepSeek API 平台，开发者可在多模态 agent 场景中直接调用或微调，其 ApexBench 得分从 V4-Flash-0731 的 26.2 提升至 36.5，文本 agent 任务表现基本持平；由于属于实验性版本，生产环境使用仍需谨慎验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datalearner.com/en/benchmarks/apexbench">ApexBench: Multimodal Agent Benchmark and Model Scores | DataLearner ...</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek -ai/ DeepSeek - V 4 - Flash - Vision - Exp · Hugging Face</a></li>
<li><a href="https://api-docs.deepseek.com/updates/">DeepSeek API Docs</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#multimodal AI`, `#vision model`, `#Hugging Face`, `#benchmarks`

---

<a id="item-tech-news-4"></a>
### [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展，包括 uBlock Origin](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 7.0/10

谷歌终于从 Chrome 网上应用店移除了所有 Manifest V2 扩展，其中就包括广受欢迎的 uBlock Origin。这是长期以来备受期待的变更，影响了数百万用户和整个扩展生态系统，标志着浏览器安全、广告拦截和用户控制方面的重大里程碑。用户对此表示担忧，许多人已经开始迁移到 Firefox。这一举措意味着 Chrome 用户只能依赖功能受限的 Manifest V3 替代品，或者转向其他仍支持 MV2 的浏览器。

hackernews · twapi · 8月31日 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**「背景」** Chrome 扩展通过“清单”（Manifest）文件声明其所需权限与运行方式，Manifest V2 是沿用多年的旧规范，而 Google 自 2023 年起逐步以更强调安全、限制后台执行与远程代码的 Manifest V3 取代它。据 Chrome 开发者文档，Chrome 网上应用店已停止接受可见性设为“公开”或“未列出”的新 V2 扩展，并取消了将 V2 扩展从“私密”改为其他可见性的能力；Chrome 也已开始移除对旧 V2 扩展平台的支持，并在警告中提示用户点击“查找替代方案”以转用 V3 版本。由于众多浏览器基于 Chromium 框架，这些浏览器同样可能屏蔽 V2 扩展；uBlock Origin 因依赖 V2 中更宽松的拦截规则 API 而受冲击，其精简版 uBlock Origin Lite 则兼容 V3。

**「影响」** 依赖 uBlock Origin 等 MV2 扩展的 Chrome 用户将无法再从网上应用店安装这些工具，必须寻找如 uBlock Origin Lite 等功能较弱的替代品，或者改用仍支持 MV2 的 Firefox 等其他浏览器。

**「社区讨论」** 评论者普遍认为广告拦截已成为安全问题，尤其是针对不熟悉技术的用户，并批评谷歌、微软等公司未能有效过滤自身广告服务中的恶意广告。许多用户强烈建议切换到 Firefox，称 uBlock Origin 在 Firefox 上表现最佳，也有部分人回忆 Chrome 早期的优点，但如今更推荐他人避开 Chrome。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V 2 support timeline | Chrome for Developers</a></li>
<li><a href="https://www.computerworld.com/article/3481519/what-windows-users-need-to-know-about-chromes-browser-extension-shakeup.html">What Windows users need to know about Chrome &#x27;s browser...</a></li>
<li><a href="https://www.webtech360.com/detail/google-officially-removes-manifest-v2-extensions-in-chrome-73007515.html">Google Officially Removes Manifest V 2 Extensions in Chrome</a></li>

</ul>
</details>

**标签**: `#chrome`, `#manifest v2`, `#uBlock Origin`, `#ad blocking`, `#browser extensions`

---

<a id="item-tech-news-5"></a>
### [ChatGPT Work 工具与技能参考：Playwright 浏览器自动化亮点](https://codex-tool-reference.simonw.chatgpt.site/) ⭐️ 7.0/10

一个由社区维护的 ChatGPT Work 工具与技能参考站点在 Hacker News 上被分享（发布于 codex-tool-reference.simonw.chatgpt.site），系统整理了 ChatGPT Work 可用的 tools、skills 及用法说明。其中最受关注的是一个控制浏览器的技能（control-browser），它指导 ChatGPT Work 通过 Node.js REPL 启动 Playwright 实例，并执行 nodeRepl.write\(await browser.documentation\(\)\); 来获取下一步操作指令。这份文档为使用 ChatGPT Work 进行自动化任务的开发者提供了一手资料，属于实用参考指南而非重大产品发布或深度技术分析。社区讨论参与度中等，评论中包含来自知名 AI 开发者 Simon Willison 的见解。

hackernews · ijidak · 8月31日 14:07 · [社区讨论](https://news.ycombinator.com/item?id=49510000)

**「背景」** ChatGPT Work 是 OpenAI 面向团队推出的智能体式工作模式，由 GPT-5.6 驱动，可通过连接工具、自动化任务把目标转化为成品。与普通 Chat 不同，Work 拥有独立的多项能力（通过标签页切换访问），并支持按计划或由应用事件触发任务，还可与技能（skills）结合以完成更复杂的工作。本条目所引用的参考文档，正是社区汇总整理这些 Work 工具与技能的资源。

**「影响」** 对使用 ChatGPT Work 的开发者而言，这份参考将零散的工具与技能集中成可查用的目录，使其无需自行逆向文档即可直接采用已验证的 Playwright 浏览器自动化模式。

**「社区讨论」** simonw 认为最有趣的是 control-browser 技能，它通过脚本化 Node.js REPL 启动 Playwright 并借助动态 documentation\(\) 输出引导后续操作；darepublic 则提醒部分 work tools 会拖慢流程并消耗大量 tokens，satvikpendem 质疑它与 Codex 的差异，montroser 还提出普通尺寸屏幕下侧边栏无法独立滚动、难以浏览列表下半部分的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/30/understanding-chatgpt-work/">Understanding ChatGPT Work | Simon Willison’s Weblog</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>
<li><a href="https://learn.chatgpt.com/docs/automations?surface=app">Run tasks on a schedule or from supported app events in ChatGPT</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#AI Tools`, `#Browser Automation`, `#Playwright`, `#Reference Guide`

---

<a id="item-tech-news-6"></a>
### [NAT 与互联网中心化的“原罪”之争](https://dreamstation.systems/personal/ntppost.html) ⭐️ 7.0/10

一篇博客文章认为，网络地址转换（NAT）是互联网走向中心化的最早原因之一，因为它削弱了人们像过去一样开放地运行服务器的能力。Linux NAT 实现的工程师 Rusty Russell 在评论中回应，承认自己当年为避免端口预留、把更多连接挤进同一个 IP 地址所做的取舍，导致来自不同地址的入站流量无法路由，用户不再拥有公共端点。文章还指出，NAT 让“我的设备连接云、云再连接其他设备”的客户端-服务器思维变得理所当然，而这一切最初只是 IPv4 地址匮乏的产物。围绕这篇文章的讨论既肯定了这一技术判断，也对其是否堪称“原罪”提出质疑。

hackernews · robinpie · 8月31日 02:23 · [社区讨论](https://news.ycombinator.com/item?id=49504905)

**「背景」** NAT 是应对 IPv4 地址枯竭的技术手段，让大量设备共享一个公网 IP，同时将这些设备对入站连接隐藏起来。在 NAT 普及之前，运行服务器非常简单——运行一个程序、把地址告诉别人即可；而 NAT 打破了这种入站路由，并逐渐改变了人们对互联网架构的认知，使依赖中介和云端成为常态。

**「影响」** 最直接的后果是，普通用户自建服务器的能力被普遍削弱，“客户端—云端”模式成为默认形态，进而助长了互联网服务的集中化；不过正如社区讨论所指出的，这一影响的程度取决于 NAT 的部署方式，即普通 NAT 与电信级 NAT（CGNAT）之间的区别。

**「社区讨论」** 最具分量的发言来自 Linux NAT 的实现者 Rusty Russell，他承认自己的设计选择——避免端口预留、只要远端地址可以区分就尽量把一个 IP 塞进更多连接——使得来自不同地址的入站流量不可路由，用户不再拥有公共端点，并自嘲这是“穷人的防火墙”。也有评论者反驳称，将 NAT 称为“原罪”是夸大其词：普通 NAT 只要可控就没问题，真正限制用户自由的是 CGNAT，而 NAT 反而保护了大量运行未修补旧版 Windows 的不安全设备。

**标签**: `#networking`, `#NAT`, `#internet architecture`, `#centralization`, `#technology history`

---

<a id="item-tech-news-7"></a>
### [wrapture：将 wrapt 补丁扩展为测试与追踪工具](https://simonwillison.net/2026/Aug/31/introducing-wrapture/) ⭐️ 7.0/10

Graham Dumpleton（wrapt、mod\_wsgi 和 New Relic Python 代理的作者）发布了新的 Python 库 wrapture，将 wrapt 的 monkeypatching 理念扩展到同时适用于测试和追踪。该库可以包装任意函数或方法，既能覆盖其返回值，也能记录所有调用流程，从而成为 unittest.mock 的替代方案，并为现有项目提供追踪能力。wrapture 内置 OpenTelemetry 支持，并提供完全基于配置的 TOML 机制（如 capture、observe、sink 配置）来为项目添加追踪。项目目前仅有几周历史，是 Dumpleton 首个大规模、完全由 AI 助手编写代码和文档的项目，但他强调这是经过精心设计的工程，而非“vibe coding”。后续博文介绍了其单元测试模式，例如通过 binding 和 on\_call.returns 或 transforms\_result 来桩替换或修改方法返回值。

rss · Simon Willison · 8月31日 23:59

**「背景」** wrapt 是 Python 中常用的 monkeypatching 库，允许在不修改原始代码的情况下包装函数和对象，Graham Dumpleton 是其作者。Python 开发者通常使用 unittest.mock 来替换测试中的依赖，但传统的 mock 与追踪功能相互分离，而 wrapture 尝试将这两种需求统一到同一个包装机制中。

**「影响」** 对于需要同时进行测试和观测的 Python 开发者，wrapture 提供了一种统一的替代方案，可减少对 unittest.mock 的依赖，并利用 OpenTelemetry 为现有项目添加低干扰的追踪；但由于项目过于年轻，生产环境中采用仍需谨慎评估，且其代码和文档全部由 AI 生成，可能存在未被发现的缺陷。

**标签**: `#python`, `#testing`, `#tracing`, `#monkeypatching`, `#observability`

---

<a id="item-tech-news-8"></a>
### [HN 文摘：OpenShot 4.0 本地 AI 调色与 Chrome 扩展变动](https://zeli.app/zh/digest/2026-08-31) ⭐️ 7.0/10

Hacker News 文摘汇编了多项技术新闻，重点包括开源视频编辑器 OpenShot 4.0 发布、Google 完成 Manifest V2 扩展移除以及 Burning Man 上的免费电话亭。OpenShot 4.0 新增屏幕与摄像头录制、专业级 Color View（色轮、曲线、示波器）以及 Object Mask 功能，后者利用本地运行的机器学习模型实现无需联网或订阅的智能抠像，并带来十种新特效。Google 已将 Chrome Web Store 中所有 MV2 扩展移除，包括 uBlock Origin，已安装的扩展在 Chrome 138 及更早版本中仍可运行但无法更新，Brave 则在其后台托管了四款热门 MV2 扩展供用户启用。文摘还包含 Steam 12TB 数据泄露、Claude Code Auto Mode 安全漏洞等多项内容。

rss · Zeli · 8月31日 23:59

**「背景」** OpenShot 是一个开源视频编辑器，此前缺乏专业级调色和 AI 功能；Chrome 正在用 Manifest V3 取代旧的 MV2 扩展系统，旨在提升安全与性能，但限制了许多广告拦截扩展。Brave 等其他 Chromium 浏览器曾依赖 Chrome Web Store，因此也受此影响。

**「影响」** OpenShot 用户将免费获得本地离线 AI 抠像和专业调色能力，无需订阅或上传数据；Chrome 用户则可能失去 uBlock Origin，需改用 Brave 或接受广告拦截能力下降。

**标签**: `#OpenShot`, `#video editing`, `#local AI`, `#open source`, `#Hacker News`

---

<a id="item-tech-news-9"></a>
### [GNN 时序泄漏问题与 SynthFin-AML 基准的提出](https://www.reddit.com/r/MachineLearning/comments/1w3imxy/your_gnn_is_probably_just_an_overcomplicated_mlp/) ⭐️ 7.0/10

一则 Reddit 帖文指出，在动态图上训练图神经网络（GNN）时普遍存在时间泄漏问题：如果使用静态快照训练，模型会通过消息传递看到未来边（例如第 10 天的边被纳入第 2 天的损失计算），导致性能虚高。为强制因果边界，作者发布了合成基准数据集 SynthFin-AML v10.0（10 万个节点、120 万条边），并采用严格的 3 快照切分方案：训练图仅含≤第 7 天的边、验证图≤第 8 天、测试图≤第 10 天，以物理隔离时间窗口来约束 GNN 的感受野。该基准还修复了表格泄漏——欺诈与正常零售交易的金额共享同一对数正态分布（μ=8.517，σ=0.8），并对比了调优的 LightGBM 与归纳式 GraphSAGE。在严格时序切分下，LightGBM（11 个特征）的 PR-AUC 为 0.848，GraphSAGE 为 0.881，说明 GNN 仍有真实的、非泄漏所致的优势，但差距并不悬殊。该基准已以 Pull Request 形式提交至 PyTorch Geometric（PR \#10774），旨在为动态图评估建立更严格的标准。

reddit · r/MachineLearning · /u/Glabmayt2075 · 8月31日 16:21

**「背景」** 图神经网络通过消息传递聚合邻居信息，在动态金融交易网络中，若直接对静态快照做训练，2 跳聚合会把未来的边纳入当前时刻的嵌入计算，违反时间因果性。传统转导式随机切分在金融交易数据上失效，而许多合成数据又存在欺诈金额与正常交易可统计区分的分布泄漏，导致基线评估失真。SynthFin-AML 正是为消除这两类泄漏、建立可信的动态图评估标准而设计。

**「影响」** 对从事反洗钱或动态图建模的研究者而言，该基准揭示了一个普遍的方法论缺陷：此前许多 GNN 在动态图上的优越结果可能源于时序泄漏而非模型能力，SynthFin-AML 为此提供了一个可执行的更严格评估标准；但 GNN 与树模型的性能差距（PR-AUC 0.881 对 0.848）也表明其优势尚未达到质变。

**标签**: `#graph neural networks`, `#temporal leakage`, `#benchmark dataset`, `#dynamic graphs`, `#anti-money laundering`

---

<a id="item-tech-news-10"></a>
### [Entropic Scree：评估脏数据信号强度的新诊断工具](https://www.reddit.com/r/MachineLearning/comments/1w3br9c/how_to_assess_if_there_is_a_strong_signal_in_your/) ⭐️ 7.0/10

红迪网用户 Chocolate\_Milk\_Son 发布了名为 Entropic Scree 的新型表格数据诊断工具，用于评估高维、真实世界且未经整理（脏）数据中的信号强度。该工具可估计信号的互信息体积（帮助判断信号能否在数据的特异性噪声中幸存）、整体特异体积信噪比（SNR）、内在秩、可解耦的变量子网络，以及数据与标准 PCA 线性假设的契合程度（线性充分性）。与传统 PCA 变体依赖线性方差、秩序或欧氏距离不同，它评估的是变换后的互信息度量，对参数或距离假设的依赖更少，适用场景更广。该工具是 arXiv 论文《From Garbage to Gold》（arXiv:2603.12288）框架的实用诊断实现，其技术预印本（DOI 10.5281/zenodo.22028087）和 GitHub 仓库已公开，核心函数目前以 R 代码形式提供，Python 和 R 软件包即将发布。

reddit · r/MachineLearning · /u/Chocolate\_Milk\_Son · 8月31日 12:02

**「背景」** 互信息（Mutual Information）是一种非参数化的变量相关性度量，相比依赖线性方差、秩排序或欧氏距离的主成分分析（PCA）等传统降维方法，它能捕捉更复杂的非线性依赖关系。信噪比（SNR）衡量信号与噪声的体积比，而内在维度（或内在秩）则刻画数据在低维空间中有效表示所需的复杂度。了解这些概念有助于理解 Entropic Scree 诊断工具评估高维脏数据中信号强度的原理。

**「影响」** 对于需要处理高维、含噪表格数据的从业者，Entropic Scree 提供了一种比标准 PCA 假设更少的信号强度与内在秩诊断方法，且核心 R 函数现已可直接调用，Python 和 R 软件包也即将发布。

**标签**: `#data-analysis`, `#tabular-data`, `#dimensionality-reduction`, `#mutual-information`, `#diagnostics`

---

<a id="item-tech-news-11"></a>
### [Claude 遭窃密木马劫持账号，Anthropic 强制登出并删付款信息](https://www.searchenginejournal.com/anthropic-warns-hackers-are-stealing-claude-sessions-to-hijack-accounts/587566/) ⭐️ 7.0/10

Anthropic 发现黑客正利用常见窃密木马盗取用户的 Claude 登录会话，进而劫持账号并冒用消耗使用额度，已强制登出受影响账户并删除保存的付款方式。涉事木马包括 Windows 平台的 Vidar、LummaC2、StealC、RedLine、Acreed 以及 Mac 平台的 AMOS。攻击通过劫持登录会话绕过了双重验证（2FA），有用户因下载破解游戏感染木马而被盗号。Anthropic 建议用户停止使用非官方破解软件，感染后应退出所有设备登录、清除 Cookie，必要时重装系统。官方还删除了受影响账户中保存的付款方式，以防进一步资金损失。

telegram · zaihuapd · 8月31日 03:22

**「背景」** 窃密木马（infostealer）是一类专门窃取浏览器 Cookie、登录令牌、自动填充密码等敏感数据的恶意软件，常随破解软件或盗版资源捆绑传播。攻击者盗取 Claude 的登录会话令牌后，无需密码便能直接接管账号，因此即使开启双重验证也无法阻止此类会话劫持。这种攻击手法已成为云服务和 AI 平台账号被盗的主要途径之一。

**「影响」** 受影响的 Claude 用户需要重新验证身份并重新绑定付款方式，且若感染木马的设备未彻底清理，账号存在再次被劫持并造成使用额度与资金损失的风险。

**标签**: `#ai-security`, `#anthropic`, `#session-hijacking`, `#cybersecurity`, `#threat-intel`

---

<a id="item-tech-news-12"></a>
### [OpenClaw 发布最大更新 2.0](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 7.0/10

OpenClaw 于 8 月 30 日发布其史上最大更新 2.0，汇集逾 1.6 万个拉取请求，约占项目迄今全部拉取请求的一半，由 933 名贡献者（含 569 名首次参与者）共同完成，团队为此近七周未发布新版本。此次更新覆盖安装、消息、记忆、技能、模型、浏览器、插件与安全等全部环节，同时简化了安装流程，重建了浏览器端体验，并新增共享云端会话以支持多人协作。这一庞大贡献规模反映出该项目开源社区的极高活跃度和广泛参与度。

telegram · zaihuapd · 8月31日 04:38

**「背景」** OpenClaw 是一款开源的 AI 智能体平台，允许用户通过自然语言发出指令，由 AI 自动调度消息、记忆、技能、模型、浏览器与插件等模块完成任务。该项目的发布节奏通常较快，但本次 2.0 更新（对应版本 v2026.8.1）历经约七周的积累后才集中交付，汇集了 933 名贡献者提交的逾 1.6 万个拉取请求，约占项目迄今全部拉取请求的一半。此次发布同时重建了浏览器端控制界面，并引入 SQLite 会话存储与共享云端多人协作等新能力。

**「对用户与开发者的影响」** 对 OpenClaw 用户与开发者而言，2.0 一次合并了约占项目历史全部拉取请求一半的逾 1.6 万个变更，团队为此专门验证了全新安装与既有版本升级两条路径的可用性；与此同时，此次大规模扩张也令未经验证的第三方技能带来的安全风险更受研究者关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techgenyz.com/openclaw-2-0-update-better-browser-agent-options/">OpenClaw 2.0 is Out. Big Update, Easier Start, Better Browser, More Agent Options - Techgenyz</a></li>
<li><a href="https://www.explainx.ai/blog/openclaw-2-0-release-august-2026">OpenClaw 2.0 Release — 16K PRs, Rebuilt UI (2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://docs.openclaw.ai/releases/2026.8.1">v2026.8.1 (AKA OpenClaw 2.0) · OpenClaw</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://openclaw.ai/blog/openclaw-2-accidentally">OpenClaw 2.0, Accidentally - OpenClaw Blog</a></li>

</ul>
</details>

**标签**: `#OpenClaw`, `#Open Source`, `#Software Release`, `#Community Development`, `#AI Agent`

---

<a id="item-tech-news-13"></a>
### [MiniMax 与智谱上半年收入大幅增长但仍亏损](https://ir-upload.realxen.net/iis/0100/uploads/iis/2026/12300095-0.PDF) ⭐️ 7.0/10

MiniMax 与智谱分别公布截至 2026 年 6 月底的上半年业绩，两家公司收入均大幅增长但仍处于亏损状态。MiniMax 期内收入 1.17 亿元，同比增长 283.1%，亏损 3.58 亿元，同比收窄 11%。智谱 2026 年上半年实现营业收入 9.54 亿元，同比增长 399.7%，其中云端部署收入占比提升至 86.5%，开放平台及 API 业务收入同比增长超 27 倍。智谱归母净亏损 20.71 亿元，同比收窄 12.1%，经调整净亏损率同比收窄 3.5 倍，其 MaaS 平台用户数超 740 万、较年初增长 144%，付费日活用户增长 603%。需要说明的是，该数据源自 Telegram 转发的一份 PDF 文件，而非两家公司的官方公告，内容可信度存在一定不确定性。

telegram · zaihuapd · 8月31日 13:11

**「背景」** MiniMax（稀宇科技）是一家总部位于上海的人工智能公司，开发多模态模型及消费级应用（如 Talkie、星野和视频生成服务海螺 AI），其于 2026 年 1 月在香港联交所上市。智谱（Z.ai）由清华大学教授于 2019 年创立，背后有美团、腾讯和蚂蚁集团投资，并声称其技术可与 OpenAI 及 Anthropic 的旗舰产品匹敌。两家公司均于 2026 年完成在港 IPO，且发行都获得超额认购。

**「影响」** 对关注中国 AI 商业化的投资者与行业观察者而言，智谱 API 业务收入增长超 27 倍、付费日活用户增长 603% 等数据表明，MaaS 与云端部署正成为大模型厂商可验证的变现路径，但两家公司利润仍为负值，盈利拐点尚未到来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MiniMax_Group">MiniMax Group - Wikipedia</a></li>
<li><a href="https://restofworld.org/2026/zhipu-ai-minimax-ipo/">China’s MiniMax, Zhipu AI beat OpenAI to IPO - Rest of World</a></li>

</ul>
</details>

**标签**: `#AI Industry`, `#Financial Results`, `#MaaS`, `#MiniMax`, `#Zhipu`

---

<a id="item-tech-news-14"></a>
### [欧盟将 ChatGPT、Reddit、Roblox 列为超大型服务](https://www.euronews.com/next/2026/08/31/eu-places-chatgpt-reddit-and-roblox-under-strictest-digital-safety-rules) ⭐️ 7.0/10

欧盟委员会于 8 月 31 日依据《数字服务法》正式认定 ChatGPT 为超大型在线搜索引擎，并将 Reddit 和 Roblox 列为超大型在线平台，原因是这三项服务在欧盟的月均活跃用户均超过 4500 万人。被认定后，三者有四个月过渡期，期间需开展年度系统性风险评估、接受独立审计，并向监管机构及经审核的研究人员共享数据，重点覆盖非法内容、未成年人保护和用户身心健康等风险。这一认定意味着这三项服务将承担欧盟数字监管框架下最严格的合规义务，直接影响其运营方式与数据治理流程。

telegram · zaihuapd · 8月31日 14:39

**「背景信息」** 《数字服务法》是欧盟针对数字服务的一套全面监管规则，对超大型在线平台和搜索引擎施加额外义务，以降低系统性风险并增强透明度。欧盟委员会依据月活跃用户数（超过 4500 万人）来划定监管门槛，被认定为超大型服务的公司须遵守更严格的风险管理、审计和透明度要求。

**「影响」** 对 ChatGPT、Reddit 和 Roblox 而言，最直接的后果是必须在四个月过渡期内建立合规机制，包括委托独立审计和建立数据共享渠道，否则可能面临欧盟的罚款或其他执法措施。

**标签**: `#EU regulation`, `#Digital Services Act`, `#ChatGPT`, `#Reddit`, `#Roblox`

---