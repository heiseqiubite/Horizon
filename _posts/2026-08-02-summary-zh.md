---
layout: default
title: "Horizon Summary: 2026-08-02 (ZH)"
date: 2026-08-02
lang: zh
---

> 从 39 条内容中筛选出 15 条重要资讯。

---

1. [OpenAI Astra 模型破解十项长期数学难题](#item-1) ⭐️ 10.0/10
2. [DeepSeek 发布 V4-Flash-0731：304B 参数模型，性价比领先同类](#item-2) ⭐️ 9.0/10
3. [EA 550 亿美元卖身沙特财团，下周正式完成](#item-3) ⭐️ 9.0/10
4. [HN 精选摘要 2026-07-31 · 电梯为何总不来？算法背后的真相](#item-4) ⭐️ 8.0/10
5. [NetBSD 11.0 发布，引入 MICROVM 内核与 NPF 防火墙改进](#item-5) ⭐️ 7.0/10
6. [RipGrep 的 musl 二进制文件在超大规模搜索时发生段错误，引发系统级技术讨论](#item-6) ⭐️ 7.0/10
7. [加拿大悄然签署联合国网络犯罪公约，引发监控担忧](#item-7) ⭐️ 7.0/10
8. [Flint：面向 AI 时代的可视化语言](#item-8) ⭐️ 7.0/10
9. [可解释性研究探究 KataGo 神经网络内部的对称性](#item-9) ⭐️ 7.0/10
10. [视觉语言模型可以在基准测试中取得高分，同时悄然抹去有意义的术语并引入幻觉偏差 \[P\]](#item-10) ⭐️ 7.0/10
11. [Qwen 发布 Audio-3.0-ASR-Flash，医学术语识别率超 95%](#item-11) ⭐️ 7.0/10
12. [腾讯砍掉对标 GTA 的 3A 大作《Last Sentinel》](#item-12) ⭐️ 7.0/10
13. [中国在联合国峰会向全球南方推广开放权重 AI 模型](#item-13) ⭐️ 7.0/10
14. [微软确认今年推出 Copilot「超级应用」](#item-14) ⭐️ 7.0/10
15. [长鑫存储 LPDDR6 研发验证近尾声，速率达 12800 Mbps](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI Astra 模型破解十项长期数学难题](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 10.0/10

OpenAI 宣布其下一代主要模型 Astra 的内部版本在十个长期未解决的数学与理论计算机科学问题上取得突破，这些问题至少十年未见主要进展。涵盖高维球体堆积、非索菲克群存在性、Connes 刚性猜想反证、算术电路下界、量子并行重复、最近向量问题硬度及多色 Ramsey 数等领域，每个证明的 token 成本约为 2000 美元。 这代表着 AI 从单纯的计算工具转变为数学研究中的主要研究协作者，可能从根本上改变数学研究的开展方式。结果通过 Lean 定理证明器进行了形式化验证，为 AI 生成证明的正确性提供了严格的验证，赋予了这些发现显著的可信度。 证明可在 openai/ten-proofs GitHub 仓库中获取，包含 Lean 4 形式化代码，另有一篇描述性论文和一份由 LLM 生成的 PDF 重构了证明推理过程。OpenAI 坦承数学论证由 AI 生成，人类负责整理与形式化，但值得注意的是，没有披露有多少问题在花费 token 后未能得出解决方案。

telegram · zaihuapd · 8月1日 07:59

**背景**: Lean 是一种基于归纳构造演算的证明助手和函数式编程语言，自 2013 年起由微软开发，现由非营利组织 Lean Focused Research Organization 维护。它使数学家能够编写可被机器验证正确性的形式化证明，消除验证中的人为错误。Astra 所攻克的问题，如非索菲克群存在性和最近向量问题硬度，是群论和格密码学中长期未解决的深层问题。此前不久，Anthropic 的 Claude 模型也使用 Mythos Preview 发现了密码学弱点，表明前沿 AI 模型参与理论研究的更广泛趋势正在形成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sofic_group">Sofic group - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lattice_problem">Lattice problem - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 数学界在线上正经历被许多人称为集体&\#x27;深蓝时刻&\#x27;的冲击，Kirwin Hampshire 发表了题为《数学的暗夜》的文章，描述这些进展引发的深刻精神危机。博主 Simon Willison 赞赏了公开证明和推理痕迹的透明度，但指出缺少实际使用的提示词，并质疑有多少问题在尝试后未能成功。陶哲轩此前提出的&\#x27;大数学&\#x27;愿景——AI 承担技术性繁重工作的大规模人机协作——似乎正以超出预期的速度变为现实。

**标签**: `#AI`, `#Mathematics`, `#OpenAI`, `#Theorem Proving`, `#Lean`

---

<a id="item-2"></a>
## [DeepSeek 发布 V4-Flash-0731：304B 参数模型，性价比领先同类](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 9.0/10

DeepSeek 发布了 V4-Flash-0731 模型，拥有 3040 亿参数（在 Hugging Face 上占 167GB），具备显著增强的智能体能力，输入价格为每百万 token 0.14 美元，输出价格为每百万 token 0.27 美元。Artificial Analysis 将其排名置于 MiniMax M3（428B）之上，认为它可能是当前性价比最高的模型。 此次发布以约为竞争对手十分之一的成本提供了与大得多的模型相当甚至更优的智能水平，颠覆了 LLM 性价比前沿。智能分数相近或更低的模型成本高出十倍，只有价格显著更高的模型如 Grok 4.5、Claude Opus 5 和 GPT-5.6 Sol 才在智能基准上超过它。 该模型的默认推理级别表现不佳，正如骑自行车的鹈鹕绘图测试所示，但将 reasoning\_effort 切换为 high 后输出质量显著提升。该模型通过 OpenRouter 和 Hugging Face 以开放权重形式提供，可通过命令行工具 &\#x27;llm&\#x27; 配合 &\#x27;-o reasoning\_effort high&\#x27; 参数调用。

rss · Simon Willison · 7月31日 23:59

**背景**: DeepSeek 是一家中国 AI 实验室，以发布具有竞争力的开放权重模型著称，这些模型在性能和价格上均挑战西方前沿模型。Agentic AI（智能体 AI）是指能够自主追求目标、使用工具并在人类定义的约束内采取行动的 AI 系统。Artificial Analysis 是一个独立的基准测试平台，评估 LLM 的智能水平和成本，并在帕累托前沿图上展示哪些模型提供最佳的单位美元智能回报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open - Weights Model ? | AI 21</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#Large Language Models`, `#Agentic AI`, `#AI Economics`, `#Open Weights`

---

<a id="item-3"></a>
## [EA 550 亿美元卖身沙特财团，下周正式完成](https://www.gamersky.com/news/202607/2180618.shtml) ⭐️ 9.0/10

由沙特公共投资基金牵头的财团以 550 亿美元收购 EA 的交易预计将于 2026 年 8 月正式完成。这将成为史上第二大游戏收购案，并使 EA 转变为一家私人公司。

telegram · zaihuapd · 8月1日 09:10

**标签**: `#gaming-industry`, `#mergers-and-acquisitions`, `#saudi-arabia`, `#ea`, `#private-equity`

---

<a id="item-4"></a>
## [HN 精选摘要 2026-07-31 · 电梯为何总不来？算法背后的真相](https://zeli.app/zh/digest/2026-07-31) ⭐️ 8.0/10

本期 HN 精选摘要深入分析了电梯调度算法，揭示了目的层调度系统的反直觉发现；审视了主要大语言模型提供商在 AI 会话可移植性与供应商锁定方面的做法；并报道了 DeepSeek-V4-Flash 公测版的发布，该版本增强了 Agent 能力。

rss · Zeli · 7月31日 23:59

**标签**: `#algorithms`, `#AI/ML`, `#vendor-lock-in`, `#DeepSeek`, `#systems`

---

<a id="item-5"></a>
## [NetBSD 11.0 发布，引入 MICROVM 内核与 NPF 防火墙改进](https://blog.netbsd.org/tnf/entry/netbsd_11_0_released) ⭐️ 7.0/10

NetBSD 11.0 已正式发布，引入了专为 x86（i386 和 amd64）设计的 MICROVM 内核，利用 PVH 启动、VirtIO MMIO 及多项内核优化，可在 2020 年代级别的 CPU 上约 10 毫秒内完成启动。该版本还改进了 NPF 防火墙，新增二层过滤和基于用户/组的过滤功能，并带来大量硬件支持增强。 10 毫秒的启动时间使 NetBSD 成为微服务和云原生环境中快速 VM 启动的可行选择，而这一领域传统上由基于 Linux 的方案主导。NPF 防火墙的增强也使 NetBSD 的过滤能力更接近 PF 和 iptables 的功能水平，提升了其在网络基础设施场景中的竞争力。 MICROVM 内核通过 \`build.sh\` 配合 \`kernel=MICROVM\` 目标构建，同时支持 i386 和 amd64 架构。发布说明承认存在一些未解决的问题，维护者表示该版本修复的问题远多于引入的问题，体现了透明而审慎的发布理念。

hackernews · jaypatelani · 8月1日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49136736)

**背景**: NetBSD 是一款免费、安全且高度可移植的类 UNIX 操作系统，基于伯克利网络发布版 2（4.4BSD-Lite），以支持多种硬件平台的设计理念著称。NPF 是 NetBSD 的有状态包过滤防火墙，可与 Linux 的 iptables、FreeBSD 的 ipfw 和 OpenBSD 的 PF 相媲美。MICROVM 内核概念顺应了行业内为微服务工作负载优化轻量级虚拟机的更广泛趋势，类似于 Linux 阵营的 Firecracker 和 Cloud Hypervisor 等项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.netbsd.org/releases/formal-11/NetBSD-11.0.html">Announcing NetBSD 11.0 RC7 (July 21, 2026)</a></li>
<li><a href="https://www.phoronix.com/news/smolBSD">smolBSD Builds On The NetBSD-MicroVM Kernel For Booting To Service VMs In Milliseconds - Phoronix</a></li>
<li><a href="https://www.wikiwand.com/EN/NPF_%28firewall%29">NPF ( firewall ) - Wikiwand</a></li>

</ul>
</details>

**社区讨论**: 讨论参与者对 BSD 操作系统相对于 Linux 的现状和相关性表示好奇，疑问其使用量和开发活跃度是在增长还是萎缩。多位评论者强调了 MICROVM 内核 10 毫秒启动时间和 NPF 二层过滤等值得关注的特性，另有一位用户询问在 NetBSD 上通过 Wine 运行仅支持 Windows 的 SDR 软件的可行性。

**标签**: `#NetBSD`, `#Operating Systems`, `#BSD`, `#Open Source`, `#Kernel`

---

<a id="item-6"></a>
## [RipGrep 的 musl 二进制文件在超大规模搜索时发生段错误，引发系统级技术讨论](https://github.com/BurntSushi/ripgrep/issues/3494) ⭐️ 7.0/10

在 ripgrep 使用 musl 静态链接的二进制文件中，报告了一个在超大规模目录搜索时触发的段错误 Bug（GitHub issue \#3494）。该问题引发了关于 musl 的 mallocng 分配器在多线程竞争下性能的广泛技术讨论，甚至引起了 Linux 内核开发者的关注。 ripgrep 是开发者生态系统中最广泛使用的搜索工具之一，而基于 musl 的静态二进制文件因具有最佳可移植性而被普遍分发。该 Bug 暴露了 musl 默认分配器在高强度多线程负载下的深层局限性，不仅影响 ripgrep，还影响任何基于 musl 构建的性能敏感型应用。 根本原因涉及 musl 的 mallocng 分配器，该分配器在多线程内存分配竞争下表现不佳，导致通常受 I/O 限制的应用变为受 malloc 限制。一份针对该 Bug 的 AI 生成分析（托管于 github.com/dfoxfranke/ripgrep-3494-analysis）写得非常详尽，以至于一位内核开发者最初怀疑是人类撰写的，但后来在内核邮件列表补丁讨论中被评价为&quot;相当差&quot;。

hackernews · throwaway2037 · 8月1日 12:34 · [社区讨论](https://news.ycombinator.com/item?id=49133889)

**背景**: musl 是一个面向 Linux 的轻量级 C 标准库，常用于生成无运行时依赖、可在任何 Linux 发行版上运行的静态链接二进制文件。ripgrep 为 Linux 分发基于 musl 的静态二进制文件以最大化可移植性。musl 的默认分配器 mallocng 设计上注重正确性和简洁性，但在多线程分配竞争下相比 jemalloc 或 mimalloc 等替代方案存在已知弱点。在 HPC（高性能计算）集群上，对共享并行文件系统运行 ripgrep 等搜索工具会产生大量小 I/O 操作，从而压垮元数据服务器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Musl">musl - Wikipedia</a></li>
<li><a href="https://github.com/BurntSushi/ripgrep">BurntSushi / ripgrep: ripgrep recursively searches ... - GitHub Download ripgrep - Free Fast Search Tool for Windows, macOS ... ripgrep Cheatsheet - Linuxize Ripgrep – Search Smarter, Code Faster with Ripgrep’s Powerful ... ripgrep Command in Linux: Fast Recursive Search | Linuxize Ripgrep cheatsheet - Skerritt.blog</a></li>

</ul>
</details>

**社区讨论**: 讨论中出现了多种观点：Orphis 指出 musl 的 mallocng 分配器不适合 ripgrep 这类多线程性能关键型应用，并质疑为何没有替换为更高性能的分配器。dosman33 认为，在 HPC 集群文件系统上运行 ripgrep 从根本上是一种反模式，因为会产生过量的小 I/O，建议重新设计工作流程。AI 生成的分析引发了元讨论，内核开发者 ndesaulniers 观察到它最初难以与人类作品区分，但最终在内核补丁讨论中被标记为&quot;相当差&quot;。

**标签**: `#ripgrep`, `#musl`, `#memory-allocator`, `#systems-programming`, `#debugging`

---

<a id="item-7"></a>
## [加拿大悄然签署联合国网络犯罪公约，引发监控担忧](https://www.michaelgeist.ca/2026/07/a-surveillance-treaty-in-disguise-the-trouble-with-canadas-quiet-decision-to-sign-the-un-cybercrime-convention/) ⭐️ 7.0/10

加拿大已悄然签署了《联合国反网络犯罪公约》，隐私倡导者如 Michael Geist 认为该条约以国际网络犯罪合作为幌子扩大了政府监控权力。截至 2026 年 5 月，已有 76 个参与方签署该条约，包括加拿大、澳大利亚、欧盟以及多个威权政权。 该条约因 enabling 跨境监控和缺乏充分隐私保障的数据共享而受到数字权利组织的广泛批评，可能迫使各国协助外国政府获取用户数据。加拿大的签署表明其倾向于一个若被批准纳入国内法可能削弱现有隐私保护的框架。 签署条约与批准条约不同——签署仅表示意向，并不使该国受条约义务约束，因此加拿大仅签署的即时法律影响有限。该公约将在第 40 个国家批准后才会生效，其实际影响将取决于各国如何在国内层面加以实施。

hackernews · iamnothere · 8月1日 14:19 · [社区讨论](https://news.ycombinator.com/item?id=49134694)

**背景**: 《联合国反网络犯罪公约》经过多年谈判后于 2024 年 12 月由联合国大会通过，是首个专门针对网络犯罪的国际条约。尽管支持者将其视为打击跨国网络犯罪的工具，批评者认为其关于跨境数据访问、司法互助和实时监控的宽泛条款缺乏充分的人权保障。该条约同时获得了民主国家和威权政权的支持，引发了对其可能被滥用于政治监控的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unodc.org/unodc/en/cybercrime/convention/home.html">United Nations Convention against Cybercrime</a></li>
<li><a href="https://www.linkedin.com/pulse/united-nations-cybercrime-convention-defining-step-toward-a-wali-moyrf">The United Nations Cybercrime Convention : A Defining Step...</a></li>
<li><a href="https://www.napforum.org/policy-briefs/dangers-of-ambiguity-in-the-un-cybercrime-treaty">Dangers of Ambiguity in the UN Cybercrime Treaty - Marshall Green</a></li>

</ul>
</details>

**社区讨论**: 社区讨论集中在签署与批准条约之间的重要区别，用户指出加拿大仅签署的即时法律效力有限。多位评论者观察到包括威权政权在内的许多国家都已签署，且加拿大通常会签署联合国协议。评论者还赞扬了 Michael Geist 二十年来对加拿大隐私问题的深入调查和报道。

**标签**: `#privacy`, `#surveillance`, `#cybercrime`, `#policy`, `#international-law`

---

<a id="item-8"></a>
## [Flint：面向 AI 时代的可视化语言](https://microsoft.github.io/flint-chart/) ⭐️ 7.0/10

Flint 是微软开发的一种可视化语言，旨在通过提供一种可渲染至多种图表后端的中间规范，来简化 AI 生成的图表。

hackernews · vinhnx · 8月1日 02:45 · [社区讨论](https://news.ycombinator.com/item?id=49130604)

**标签**: `#data-visualization`, `#AI`, `#LLM-tools`, `#Microsoft`, `#charting`

---

<a id="item-9"></a>
## [可解释性研究探究 KataGo 神经网络内部的对称性](https://www.reddit.com/r/MachineLearning/comments/1vcrki2/how_symmetric_are_the_insides_of_a_go_network_r/) ⭐️ 7.0/10

KataGo 的维护者发布了一项可解释性研究，探讨超人类水平的围棋神经网络是否学习到与棋盘方向无关的内部表示，还是针对 8 种旋转/翻转方向分别记忆这些概念。研究发现，虽然 8 倍数据增强能自然带来一定的对称性不变性，但网络并未实现完美的对称，且分析过程中出现了一个意料之外的发现。 这项工作难得地揭示了超人类水平神经网络内部表示的机制性理解，直接回答了仅靠数据增强是否能诱导真正的对称性不变性，还是模型不可避免地为每个方向记忆冗余特征的问题。这些发现对更广泛的机器学习可解释性领域有重要意义，因为理解神经网络如何表示几何对称性对模型效率、泛化能力和架构设计都有深远影响。 KataGo 的架构在结构上并不强制对称性——唯一的对称诱导机制是随机 8 倍数据增强，即在每个训练批次中随机化棋盘的空间方向。该研究的分析和写作主要由 AI 辅助完成，但有 KataGo 维护者的详细人工指导和反馈，所有代码均通过链接的 GitHub 仓库公开提供。

reddit · r/MachineLearning · /u/icosaplex · 8月1日 16:18

**背景**: KataGo 是一个免费开源的围棋程序，与 DeepMind 的 AlphaGo Zero 类似，使用蒙特卡洛树搜索配合卷积神经网络进行局面评估和策略选择。围棋的规则在棋盘的 8 种旋转和翻转（即二面体群 D4）下完全对称，意味着一个局面无论方向如何，在战略上是完全相同的。数据增强是一种通过随机变换训练样本帮助模型泛化的技术，在本例中每个棋盘局面在训练时以随机选择的方向呈现，而非将对称性硬编码到网络架构中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://katagotraining.org/">KataGo Distributed Training</a></li>
<li><a href="https://en.everybodywiki.com/KataGo">KataGo - EverybodyWiki Bios &amp; Wiki</a></li>

</ul>
</details>

**标签**: `#Machine Learning Interpretability`, `#KataGo`, `#Neural Networks`, `#Computer Go`, `#Data Augmentation`

---

<a id="item-10"></a>
## [视觉语言模型可以在基准测试中取得高分，同时悄然抹去有意义的术语并引入幻觉偏差 \[P\]](https://www.reddit.com/r/MachineLearning/comments/1vcipzz/vlms_can_score_well_on_benchmarks_while_silently/) ⭐️ 7.0/10

本文表明，视觉语言模型在放射学报告生成中能取得高基准测试分数，但同时会悄然抹去具有临床意义的术语并引入带有偏见的内容，并提出了一种衡量该现象的框架。

reddit · r/MachineLearning · /u/ade17\_in · 8月1日 09:27

**标签**: `#VLM`, `#Medical AI`, `#Benchmark Evaluation`, `#Radiology Report Generation`, `#AI Safety`

---

<a id="item-11"></a>
## [Qwen 发布 Audio-3.0-ASR-Flash，医学术语识别率超 95%](https://x.com/Alibaba_Qwen/status/2083111834123407825) ⭐️ 7.0/10

7 月 31 日，阿里 Qwen 团队发布了新一代语音识别模型 Qwen-Audio-3.0-ASR-Flash，主打上下文一致性、领域术语识别、自定义热词以及语音润色输出为结构化文本等能力。内部测试显示，该模型医学术语召回率达 95.36%，工业术语召回率达 93.24%。 医疗和工业领域术语的高召回率直击通用 ASR 模型长期存在的痛点——专业术语识别错误频发。通过阿里云提供流式、文件转写和批量三种部署形态，使开发者能够在受监管或技术密集型行业中快速落地实时和离线语音应用。 模型提供三种部署形态：实时流式识别（Streaming）、录制文件转录（Filetrans）和非实时识别，均通过阿里云模型服务上线。GitHub 上还提供了配套的 Python 工具包 Qwen3-ASR-Toolkit，能够智能切分长音频文件并并行处理，突破了 API 单次 3 分钟音频长度的限制。

telegram · zaihuapd · 8月1日 03:29

**背景**: 自动语音识别（ASR）将口语转换为文本，是语音助手、转录服务和无障碍工具的基础技术。传统 ASR 模型在处理领域专有词汇——如医学术语、工业行话和专有名词——时表现不佳，导致错误累积并影响下游应用质量。自定义热词功能允许开发者在推理时提升特定术语的识别优先级，这一特性已被 NVIDIA Riva 和阿里 Qwen 系列等 ASR 提供商广泛采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3-ASR-Toolkit">GitHub - QwenLM/Qwen3-ASR-Toolkit: Official Python toolkit ...</a></li>
<li><a href="https://www.qwencloud.com/models/qwen-audio-3.0-asr-flash-streaming">Qwen-Audio-3.0-ASR-Flash-Streaming - QwenCloud</a></li>

</ul>
</details>

**标签**: `#Speech Recognition`, `#Qwen`, `#Alibaba Cloud`, `#AI Models`, `#ASR`

---

<a id="item-12"></a>
## [腾讯砍掉对标 GTA 的 3A 大作《Last Sentinel》](https://www.bloomberg.com/news/newsletters/2026-07-31/inside-tencent-s-failed-attempt-to-take-on-grand-theft-auto) ⭐️ 7.0/10

腾讯已于 7 月 28 日在旗下 Lightspeed LA 工作室裁员 80 人，并在历经六年开发后实质上叫停了高预算开放世界游戏《Last Sentinel》。尽管腾讯官方坚称游戏仍在制作中，但知情人士透露该项目已不再推进，留任员工将转往其他项目。 此次取消凸显了即便是腾讯这样财力雄厚的公司，开发能对标 Rockstar《侠盗猎车手》系列的 3A 开放世界游戏依然极为困难。它反映了游戏行业对缺乏明确创意方向的超大预算项目日益规避风险的趋势，也暴露了中国公司从零搭建西式 3A 工作室所面临的挑战。 该游戏是一款以重建后的东京为背景的赛博朋克开放世界作品，开发历时六年，耗资数亿美元。今年初的内部试玩反馈几乎全为负面；腾讯限定 7 月前交出改进版，但最终认定质量不达标且市场风险过高。工作室由 Rockstar 圣迭戈前负责人 Steve Martin 领导，团队规模数百人，远小于 Rockstar 数千人的体量。

telegram · zaihuapd · 8月1日 06:45

**背景**: Lightspeed LA 是腾讯在北美设立的首个 3A 级游戏开发工作室，2020 年成立于加州尔湾，隶属于腾讯光子工作室群。该工作室旨在为主机和 PC 平台开发叙事驱动的开放世界游戏，是腾讯进军传统上由欧美和日本发行商主导的 3A 级市场的重要战略布局。《Last Sentinel》作为工作室的首发作品对外公布，被定位为对标 Rockstar《侠盗猎车手》系列的产品——后者是史上最成功、开发成本最高的游戏系列之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LightSpeed_Studios">LightSpeed Studios - Wikipedia</a></li>
<li><a href="https://lastsentinelgame.com/">LAST SENTINEL</a></li>
<li><a href="https://ixbt.games/en/news/2026/07/31/425997-ambicioznyi-eksen-last-sentinel-ot-tencent-otmenen-posle-sesti-let-razrabotki-smi.html">Ambitious Tencent Action Game Last Sentinel Canceled After Six...</a></li>

</ul>
</details>

**标签**: `#gaming`, `#tencent`, `#project-management`, `#industry-news`, `#game-development`

---

<a id="item-13"></a>
## [中国在联合国峰会向全球南方推广开放权重 AI 模型](https://www.semafor.com/article/07/28/2026/token-diplomacy-how-china-is-shaping-the-worlds-ai-future) ⭐️ 7.0/10

2026 年 7 月底在日内瓦联合国&quot;智能向善&quot;峰会上，中国派出代表团向巴基斯坦、俄罗斯、赞比亚等全球南方国家推介中国开放权重 AI 模型，以低于美国对手的价格提供并承诺培训各国使用。阿里云架构师王坚在会上表示，中国 AI 可以成为其他国家发展的&quot;基石&quot;，而美国前沿实验室及特朗普政府官员则明显缺席。 这标志着全球 AI 地缘政治的重大战略分歧：中国利用开放权重模型作为外交工具在发展中国家建立影响力，而美国则坚持闭源前沿模型路线。这一策略可能决定全球南方数十亿人口最终采用何种 AI 标准、基础设施和生态系统，对技术主权和地缘政治走向具有深远影响。 开放权重模型与真正的开源模型不同：前者发布训练好的模型参数（权重）供推理和微调使用，但通常不包含训练代码、数据细节和复现模型所需的方法。美国国务院对此表示担忧，认为中国的做法将&quot;导致对中国基础设施和标准的依赖&quot;，并将其视为&quot;一带一路&quot;倡议向数字 AI 基础设施领域的延伸。

telegram · zaihuapd · 8月1日 10:06

**背景**: &quot;词元外交&quot;指的是中国向发展中国家输出 AI 词元和基础设施的策略，从&quot;一带一路&quot;倡议的物理基础设施出口（港口、铁路、电信网络）转向数字 AI 基础设施。前沿模型是由大规模算力和数据训练而成的最先进通用 AI 系统，通常由 OpenAI 和 Anthropic 等美国头部实验室以闭源方式开发。相比之下，开放权重模型允许用户下载并在本地运行模型权重，无需依赖中心化 API 提供商即可进行微调和定制化部署。开源与闭源之争对成本、主权以及各国发展独立 AI 能力具有重大影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.semafor.com/article/07/28/2026/token-diplomacy-how-china-is-shaping-the-worlds-ai-future">Token diplomacy: How China is shaping the world’s AI future ...</a></li>
<li><a href="https://carnegieendowment.org/research/2026/05/chinas-pivot-on-global-ai">China’s Pivot on Global AI - Carnegie Endowment for ...</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weights-vs-source-llms-why-difference-matters-more-kapil-uthra-6kanf">Open Weights vs . Open Source in LLMs: Why the Difference Matters...</a></li>

</ul>
</details>

**标签**: `#AI geopolitics`, `#open-weight models`, `#global south`, `#AI policy`, `#token diplomacy`

---

<a id="item-14"></a>
## [微软确认今年推出 Copilot「超级应用」](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 7.0/10

微软 CEO 纳德拉在财报电话会议上确认，公司将于今年推出一款 AI「超级应用」，将 Copilot 的聊天、编程和智能体能力整合到一个应用中，同时覆盖消费者和商用场景。 这一整合代表了从分散的 AI 工具向单一统一入口的重大战略转变，直接与 OpenAI 近期推出的 ChatGPT Work 应用竞争。它标志着行业正从独立的聊天机器人转向能够自主规划、执行和交付多步骤工作的集成化智能体平台。 该超级应用将整合四个此前独立的工具：Copilot 聊天机器人、用于编程的 GitHub Copilot、用于多步骤工作流执行的 Copilot Cowork，以及用于自主任务完成的 Autopilot 系统。Copilot Cowork 是由 Work IQ 驱动的智能体系统，它整合用户工作图谱中的信号，并在执行每项操作前需要用户批准。

telegram · zaihuapd · 8月1日 13:18

**背景**: 微软的 Copilot 经历了多个阶段的演进：从简单的聊天工具到 Copilot Cowork——一种能够跨应用、文件和数据规划和执行长时间运行的多步骤工作流的智能体系统；再到 Autopilot 系统——使用触发器、指令和护栏机制、无需等待用户提示即可自主执行操作的自主智能体。智能体 AI 指的是具有更高自主性和主动能力的系统，能够感知事件、做出决策并独立执行任务。微软的推进恰逢 OpenAI 近期也推出了整合 ChatGPT 与 Codex 的 ChatGPT Work 应用，加剧了 AI 生产力领域的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365/copilot/cowork/">Copilot Cowork overview | Microsoft Learn</a></li>
<li><a href="https://www.microsoft.com/en-us/microsoft-copilot/copilot-101/copilot-ai-agents">Copilot and AI Agents | Microsoft Copilot</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Copilot`, `#AI Super App`, `#Product Strategy`, `#Enterprise AI`

---

<a id="item-15"></a>
## [长鑫存储 LPDDR6 研发验证近尾声，速率达 12800 Mbps](https://finance.sina.com.cn/stock/t/2026-08-01/doc-inikuwea8878362.shtml) ⭐️ 7.0/10

长鑫存储首款 LPDDR6 产品研发验证已接近尾声，设计速率达 12800 Mbps（基础速率 10667 Mbps），颗粒容量 16 Gb、芯片容量 16 GB，采用 1295 Ball PoP 封装。长鑫早在今年 3 月已将样品送至核心客户，有望于 2026 年下半年实现量产导入。 若长鑫存储率先实现量产，将标志着国内存储产业从高端存储技术跟随者转变为前沿规格领跑者。这将为国产旗舰手机和端侧 AI 硬件提供自主可控的高速内存核心器件，降低对三星、SK 海力士等海外供应商的依赖。 相较于上一代 LPDDR5X，新品在低功耗设计与 RAS（可靠性、可用性和可维护性）功能上均有明显优化。1295 Ball PoP（叠层封装）技术可实现存储与处理器芯片的垂直堆叠，对空间受限的移动和端侧 AI 应用至关重要。

telegram · zaihuapd · 8月1日 15:30

**背景**: LPDDR（低功耗双倍速率内存）是专为移动和嵌入式设备设计的内存标准，每一代都带来更高的数据传输速率和更低的功耗。PoP（Package on Package，叠层封装）是一种集成电路封装方法，将两个或多个封装垂直堆叠，通常将内存放置在处理器上方，通过焊球实现层间信号传输。RAS（可靠性、可用性和可维护性）是计算系统中衡量正确运行、避免数据损坏和保持可用性的一组功能特性，在 AI 工作负载中日益重要。长鑫存储是中国领先的本土 DRAM 制造商，在长期由三星、SK 海力士和美光主导的市场中竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.theblockbeats.news/flash/359240">Changxin Technology&#x27;s LPDDR 6 Nearing R&amp;D Validation Culmination</a></li>
<li><a href="https://www.icdirectory.com/b/blog/what-is-a-package-on-package-pop.html">What is a package - on - package ( PoP )? | icDirectory Limited</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reliability,_availability_and_serviceability">Reliability , availability and serviceability - Wikipedia</a></li>

</ul>
</details>

**标签**: `#LPDDR6`, `#CXMT`, `#semiconductor`, `#memory-technology`, `#edge-AI`

---