---
layout: default
title: "Horizon Summary: 2026-09-03 (ZH)"
date: 2026-09-03
lang: zh
---

> 从 39 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Meta 发布低成本编程模型 Muse Spark 1.3](#item-tech-news-1) ⭐️ 8.0/10
2. [Gemini 3.8 Flash 发布：快速廉价且性能强劲](#item-tech-news-2) ⭐️ 8.0/10
3. [三个网站生成 21 万条 AI 推荐页面，Perplexity 频繁引用](#item-tech-news-3) ⭐️ 8.0/10
4. [AI 助力 Paint.NET 重写 Direct2D](#item-tech-news-4) ⭐️ 8.0/10
5. [从零构建文生图模型的完整指南](#item-tech-news-5) ⭐️ 8.0/10
6. [多数开源 AI 检测器无法达到 0.5%误报率](#item-tech-news-6) ⭐️ 8.0/10
7. [美国法院驳回拆分谷歌广告技术业务的请求](#item-tech-news-7) ⭐️ 7.0/10
8. [Deepity：C++预测编码网络库匹敌反向传播性能](#item-tech-news-8) ⭐️ 7.0/10
9. [CABiNet 对比 YOLO26-sem：UAVid 基准显示精度与延迟权衡](#item-tech-news-9) ⭐️ 7.0/10
10. [网信办 AI 治理第二阶段清理 561 万条信息](#item-tech-news-10) ⭐️ 7.0/10
11. [阿里发布 Qwen3.8-Max-0902，CodeArena 编程榜夺冠](#item-tech-news-11) ⭐️ 7.0/10
12. [月之暗面与三大云厂商洽谈 Kimi K3 收入分成](#item-tech-news-12) ⭐️ 7.0/10
13. [马斯克预告 Grok 4.7 十天后上线，参数 2.1 万亿](#item-tech-news-13) ⭐️ 7.0/10
14. [Nexus 暗网兜售 1.53 亿驾照扫描件 FBI 介入调查](#item-tech-news-14) ⭐️ 7.0/10
15. [新国标规范 AI 客服协同，禁止隐藏转人工入口](#item-tech-news-15) ⭐️ 7.0/10
16. [纽约公立学校将全面限制低年级学生课堂使用生成式 AI](#item-tech-news-16) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Meta 发布低成本编程模型 Muse Spark 1.3](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 8.0/10

Meta 发布了轻量级 AI 模型 Muse Spark 1.3，并宣称这是该系列迄今在编程与智能体工作上的最大幅度升级。该模型在 DeepSWE 基准上取得 75.4 分，为迄今最高成绩，并将谷歌 Gemini 3.8 Flash 当天稍早保持的榜首位置挤至第二。其推理成本极低，示例显示完成一次 SVG 生成仅耗时 38 秒、花费约 4.23 美分。模型已在 Muse Code 与 API 中开放试用，官方表示后续还将推出 🍉 以及 Muse Spark 的开放权重版本。以极低成本提供接近前沿的性能，使其在开发者中收获大量好评。

hackernews · bvaldivielso · 9月2日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49541256)

**「背景」** Muse Spark 是 Meta 主打低成本、高速度的 AI 模型系列，定位为在无需顶级算力开销的场景下提供实用编程与智能体能力。DeepSWE 基准专门评测模型在长时程智能体编码任务上的表现，即模型能否在数分钟到数小时的多轮操作中持续追踪上下文、处理模糊输入并自主完成任务。此前该基准的头部位置常由 Google、OpenAI 和 Anthropic 的旗舰模型占据，而 Muse Spark 1.3 以 75.4 分超越 Claude Opus 5 的 74.0 分，Meta 声称这标志着该系列在编程和智能体任务上迄今最大幅度的提升，不过独立第三方验证仍在进行中。

**「影响」** 开发者现在可以以极低的价格在 Muse Code 与 API 中获取接近前沿的编程与智能体性能，而厂商之间的基准竞争正持续压低模型使用价格，并可能吸引更多用户接受让 Meta 训练数据的条款以换取更低成本。

**「社区讨论」** 社区开发者普遍称赞其速度极快、价格低廉，并在简单 UI 编程任务上表现出干净且实用的输出，同版本对比中 1.3 的生成质量明显优于 1.2。也有评论指出，DeepSWE 榜首的频繁更替说明厂商竞争正推动价格下降；另有用户调侃，尽管技术表现出色，Meta 仍面临关于儿童社交媒体成瘾的 180 亿美元诉讼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://officechai.com/ai/muse-spark-1-3-benchmarks/">Meta Releases Muse Spark 1.3, Beats Opus 5, GPT Sol 5.6 On Some Benchmarks</a></li>
<li><a href="https://developer.meta.com/ai/models/muse-spark/">Muse Spark 1.3 | Meta</a></li>
<li><a href="https://daily.dev/posts/meta-releases-muse-spark-1-3-claims-top-scores-on-deepswe-benchmark-sitagwxqs">Meta releases Muse Spark 1.3, claims top scores on DeepSWE benchmark | daily.dev</a></li>

</ul>
</details>

**标签**: `#ai`, `#machine-learning`, `#meta`, `#model-release`, `#benchmarks`

---

<a id="item-tech-news-2"></a>
### [Gemini 3.8 Flash 发布：快速廉价且性能强劲](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 8.0/10

Google 发布了 Gemini 3.8 Flash 和 3.8 Flash Cyber，这是一款快速且廉价的 AI 模型，强调编码和推理能力。据测试，该模型在 artificialanalysis.ai 上智能评分为 59，与 Opus 5 medium 持平，并在 deepswe.datacurve.ai 排名第一（超过 Opus 5）。开发者 Simon Willison 用 1.8 美分和 13 秒生成了高质量的 HTML/JavaScript 页面。该模型还支持音频和视频输入，而 OpenAI 和 Anthropic 的旗舰模型仍仅支持图像。此外，模型卡可在 deepmind.google/models/model-cards/gemini-3-8-flash 获取。

hackernews · bratao · 9月2日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49537553)

**「背景」** Gemini 是谷歌\(Google\)旗下的大语言模型系列，其中 Flash 定位为快速、低成本的推理层级。Gemini 3.8 Flash 基于上一代 Gemini 3.7 Flash 构建，而 3.8 Flash Cyber 则是在相同基础上针对漏洞检测与修复\(网络安全任务\)专门调优的版本。该模型按每百万输入 token 0.75 美元、每百万输出 token 3.75 美元的价格上线，该促销价延续至 2026 年 12 月 31 日，之后将上调至每百万输入 1.50 美元、每百万输出 7.50 美元；这也是谷歌在六周内推出的第三款 Flash 模型。

**「影响」** 对需要快速、低成本生成代码和进行多媒体分析的开发者而言，3.8 Flash 使此类任务成本大幅降低，并可能改变工具选择。

**「社区讨论」** 社区普遍对该模型的性能和速度感到惊讶，尤其称赞其在 HTML/JavaScript 生成和多模态支持方面的能力；有用户提到 3.8 Flash 在多个基准上优于 3.7，但也有评论指出 thinking 级别为低时相对 3.7 存在回归。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-8-flash/">Gemini 3.8 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://www.orcarouter.ai/blog/gemini-3-8-flash-leak">Gemini 3.8 Flash Is Official: $0.75 Intro Price, 1M Context</a></li>
<li><a href="https://arstechnica.com/ai/2026/09/google-releases-gemini-3-8-flash-its-third-flash-model-in-six-weeks/">Google releases Gemini 3.8 Flash, its third Flash model in six weeks - Ars Technica</a></li>

</ul>
</details>

**标签**: `#Gemini`, `#AI models`, `#Google`, `#LLM`, `#Machine Learning`

---

<a id="item-tech-news-3"></a>
### [三个网站生成 21 万条 AI 推荐页面，Perplexity 频繁引用](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 8.0/10

一份报告揭示，三个网站生成了 215,128 个由 AI 生成的“最佳软件”页面，而这些页面被 AI 搜索引擎 Perplexity 在回答中频繁引用为信息来源。这一现象暴露了 AI 搜索领域的系统性信任危机：低质量的 AI 生成内容正被另一个 AI 系统当作可靠资料，进一步加剧了内容生态的失真。报告指出，这些页面专门针对 AI 回答引擎的引用机制进行优化，用户在使用 Perplexity 获取软件推荐时，可能会得到由机器生成、缺乏人工验证的建议。该问题直接影响依赖 AI 搜索进行技术选型或产品比较的开发者和普通用户，同时也引发了对 AI 内容循环引用风险的广泛关注。

hackernews · jakobgreenfeld · 9月2日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=49536375)

**「背景信息」** 这则报道源于 trellner.com 发布的一份报告，该报告调查了人工智能搜索引擎（尤其是 Perplexity）在回答中引用和依据的网页来源。报告发现，在约 380 个软件类别中，AI 推荐所依据的来源中有 59.8% 不属于访问量排名前 10 万的网站，其中多个被频繁引用的站点是专门为被模型读取而非真人阅读而构建的。这一现象反映了一种被称为“答案引擎优化”（AEO）的策略：内容制作者生产大量 AI 生成的页面，目标并非吸引用户点击，而是为了被 AI 搜索引擎引用，从而影响其输出结果。

**「影响」** 依赖 Perplexity 获取软件推荐或技术比较的用户，将越来越可能收到基于 AI 生成的营销性页面而非真实用户评价的建议，从而做出误导性的选型决策；这一影响同样波及被推荐软件背后的开发者与公司，因为他们的产品排名可能被这些批量生成的页面系统性操纵。

**「社区讨论」** 评论者普遍认为，LLM 在对比和推荐时明显偏向 AI 生成的内容而非人工撰写的内容，并引用个人实验验证了这一点；有用户指出，Perplexity 等工具为追求响应速度而牺牲了结果质量，导致链接和引用经常不可靠。此外，多位评论者提到 AI 模型缺乏对信息来源动机的怀疑，例如对虚构地点的错误推荐，以及大量由被比较公司自身托管的 AI 生成对比页面在研究中被引用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/">Three sites made 215 , 128 &quot; best software &quot; pages for AI . Perplexity ...</a></li>

</ul>
</details>

**标签**: `#AI-generated content`, `#search engine quality`, `#Perplexity`, `#content spam`, `#LLM reliability`

---

<a id="item-tech-news-4"></a>
### [AI 助力 Paint.NET 重写 Direct2D](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 8.0/10

Paint.NET 作者 Rick Brewster 宣布，该软件现已包含一套从零开始、通过 AI 辅助的洁净室逆向工程重写的 Direct2D 实现，用于在 WINE 上运行。这套代码位于 PaintDotNet.Windows.Direct2D1.Managed.dll 中，由 Claude 编写，总计约 18 万行，而 Paint.NET 其余部分约 70 万行、开发了 20 多年。使用 /wine 参数可触发该重写，因为 Direct2D 一直是 Paint.NET 在 WINE 上运行的最大障碍，且无法被禁用。Brewster 指出大部分代码属于“vibe coded”，未经彻底审查，他还不得不监督 Claude 修复资源管理问题（如引用计数对象的 AddRef 缺失），但也称赞了 Claude 在逆向工程内置效果库公式时的聪明和勤奋。这一进展表明 AI 编码代理可能加速大型专有 API 兼容层的实现，但代码质量和可靠性仍需谨慎对待。

rss · Simon Willison · 9月2日 05:50

**「背景」** Direct2D 是 Windows 平台上的 2D 图形渲染 API，负责硬件加速绘图，而 WINE 是一个让 Windows 程序能在 Linux 等系统上运行的兼容层。洁净室逆向工程指在不接触原厂商专有代码的前提下，仅基于公开规范和行为观察独立实现兼容功能，以避免知识产权问题。Paint.NET 依赖 Direct2D，但 WINE 对它的支持长期不完整，这正是该重写项目的核心动机。

**「影响」** 对希望在 Linux 上使用 Paint.NET 的用户来说，这项实验性 WINE 支持提供了潜在路径，但因为它被明确标记为“极其实验性”且大量代码未经人工审查，实际使用时可能遇到稳定性和正确性问题，不应用于关键工作。

**标签**: `#Direct2D`, `#WINE`, `#Paint.NET`, `#AI-assisted coding`, `#reverse engineering`

---

<a id="item-tech-news-5"></a>
### [从零构建文生图模型的完整指南](https://www.reddit.com/r/MachineLearning/comments/1w5c9rd/detailed_explanation_of_how_to_create_a/) ⭐️ 8.0/10

Jasper Research 发布了从零构建文生图（text-to-image）模型的详细技术手册，包含了完整的推理过程和中间结果，适合希望深入了解文生图模型或了解前沿实验室构建方法的人。该手册还附带了一个包含 1 亿张图像的数据集（Monet Dataset）以及一个包含小型模型的代码库（nano-t2i），使得用户能够实际从头训练一个文生图模型。具体资源包括在线交互式技术报告（Hugging Face Space）、GitHub 上的 nano-t2i 代码库以及 Hugging Face 上的 Monet 数据集。尽管这不是一项突破性研究成果，但作为实用的开源资源，它为实践者和学习者提供了深入的技术细节和具体工具。

reddit · r/MachineLearning · /u/dh7net · 9月2日 14:40

**「背景」** 文本生成图像（Text-to-Image，T2I）模型通常依赖大规模数据集和复杂训练流程，但公开的高质量数据集和可复现的完整训练代码并不多。Jasper Research 于近期发布了 MONET 数据集，包含约 1.049 亿个图文样本，是目前最大的开放式文本-图像数据集之一，并配套提供了 nano-t2i 代码库，这是一个极简、可修改、遵循 Apache-2.0 协议的开源训练框架，可在单张 H200 GPU 上以低于 300 美元的成本端到端训练一个流匹配（flow-matching）T2I 模型。该项目的目标正是降低 T2I 模型的研究和复现门槛。

**「影响」** 对于希望从头构建文生图模型的研究人员和开发者，这套手册和数据/代码资源提供了一条完整且可复现的实践路径，降低了学习门槛并直接支持动手训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/gojasper/nano-t2i">gojasper/ nano - t 2 i : Minimal training code of a nano text - to - image ...</a></li>
<li><a href="https://huggingface.co/blog/jasperai/monet">MONET: Lowering the bar for World-Class Image Generation research .</a></li>
<li><a href="https://www.jasper.ai/blog/monet">Monet Lowering the Barrier to World Class Image ... | The Jasper Blog</a></li>

</ul>
</details>

**标签**: `#text-to-image`, `#machine-learning`, `#tutorial`, `#dataset`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [多数开源 AI 检测器无法达到 0.5%误报率](https://www.reddit.com/r/MachineLearning/comments/1w58erw/most_opensource_ai_detectors_cant_hold_a_05/) ⭐️ 8.0/10

一个社区驱动的基准测试表明，大多数开源 AI 检测器无法维持 0.5%的误报率\(FPR\)。测试使用公共数据集，包括 Jabarian &amp; Imas 2025\(NBER\)、Liang 2023 TOEFL 论文、1,060 篇前沿模型文本\(GPT-5.x、Claude Opus 5、Gemini 3.x\)以及 5,000 页 2018 年前 LLM 时代的 FineWeb 页面作为人类对照池，每个模型的阈值统一在同一份 6,930 篇人类文档上校准至 0.5%误报率。结果显示 6 个模型中 4 个无法达到目标：MAGE 对 26%的普通人类网络文本打出大于 0.9999 的分数，旧版 OpenAI RoBERTa 检测器在现代生成器上的 AUC 仅为 0.31\(劣于随机猜测\)。在经 humanizer 改写的文本上所有模型表现崩溃——最佳模型仅捕捉 42%，第二名仅 4%——且所有检测器标记非母语者论文的比率均高于母语者，表明此类模型存在系统性的非母语者偏见。披露称六个模型之一为作者自有模型\(wasitaigeneratedcom/ai-text-detector-small，以 Apache-2.0 开源权重发布\)，完整数据集与方法均附于模型卡片以便复现。

reddit · r/MachineLearning · /u/grumpyp2 · 9月2日 12:04

**「背景」** 人工智能文本检测器通过分类器输出分数来判定文本由人类还是 LLM 生成，评估常用 ROC-AUC 以及给定阈值下的误报率\(false-positive rate, FPR\)，即把人类文本误判为 AI 的比例。由于误报会令无辜作者被冤枉指控，实际应用要求误报率极低；本基准将全部模型阈值统一校准到 0.5%误报率，再分别评测其在原始 AI 文本、经 humanizer 改写文本与前沿模型文本上的召回率。

**「影响」** 对依赖开源检测工具的内容审核、学术诚信与招聘筛选等实践而言，本基准显示在 0.5%误报率校准下这些模型普遍会误伤相当比例的人类网络文本并对非母语写作者构成系统性误判，实际部署需重新权衡阈值设置与群体偏见。

**标签**: `#ai-detection`, `#benchmarking`, `#open-source`, `#llm-bias`, `#ml-evaluation`

---

<a id="item-tech-news-7"></a>
### [美国法院驳回拆分谷歌广告技术业务的请求](https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html) ⭐️ 7.0/10

美国一家法院驳回了司法部要求强制拆分谷歌广告技术业务的请求，使该公司的广告技术堆栈得以完整保留。谷歌广告技术业务去年收入约 300 亿美元，约占母公司 Alphabet 总营收的 8%，但其收入已连续 16 个季度下滑，分析师估计该业务仅占母公司利润的不到 1%。这一裁决是谷歌在反垄断诉讼中的一次重要胜利，意味着其广告技术服务不会被强制剥离，但案件的法律影响和行业潜在后果可能仍在发酵。此次判决的具体理由和条件尚未公开，司法部仍有权提出上诉，未来走向仍存不确定性。

hackernews · donohoe · 9月2日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=49537131)

**「背景」** 美国司法部此前起诉谷歌在数字广告技术市场非法维持垄断，并要求强制拆分其广告技术业务。法院虽认定谷歌存在垄断行为，但于 2026 年 9 月 2 日驳回了强制拆分的请求，改为下令对其数字广告业务的运营方式进行调整。谷歌方面对未遭拆分的结果表示满意，而行业组织 CCIA 则认为这一裁决体现了反垄断补救措施应精准针对已认定的损害。

**「影响」** 美国法院驳回了司法部强制谷歌剥离其广告技术业务的请求，谷歌的广告技术堆栈（2025 年为 Alphabet 创造约 300 亿美元收入、约占总营收 8%，但利润占比不足 1%）得以完整保留。

**「社区讨论」** 评论者对拆分相关的程序对称性提出质疑，认为当前法律让合并容易而拆分几乎不可能；也有人追问所谓“广告技术”的确切定义，因为该业务利润占比不到 1%，似乎缺乏反垄断意义。还有人提议用累进税制对付垄断企业，而另一些评论者则讽刺科技巨头总能规避重大执法，感叹“Lake America”这样的说法为谷歌提供了庇护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.capitalgazette.com/2026/09/02/google-advertising-monopoly-spared-breakup/">Judge orders changes to Google’s digital ads business but spares it from a breakup</a></li>
<li><a href="https://techcrunch.com/2026/09/02/google-spared-from-ad-business-breakup-but-judge-orders-changes-to-how-it-operates/">Google spared from ad-business breakup, but judge orders changes to how it operates | TechCrunch</a></li>
<li><a href="https://ccianet.org/news/2026/09/ccias-response-to-court-ruling-on-google-ad-tech-remedies-in-doj-antitrust-case">CCIA’s Response to Court Ruling on Google Ad Tech Remedies in DOJ Antitrust Case - CCIA</a></li>

</ul>
</details>

**标签**: `#google`, `#antitrust`, `#ad-tech`, `#legal`, `#policy`

---

<a id="item-tech-news-8"></a>
### [Deepity：C++预测编码网络库匹敌反向传播性能](https://www.reddit.com/r/MachineLearning/comments/1w5fuhm/deepity_a_c_library_showing_predictive_coding/) ⭐️ 7.0/10

一位开发者用一个月时间构建了名为 Deepity 的本地 C++ 机器学习库，用于测试替代性信用分配算法，尤其是生物合理性更强、更适合持续学习的预测编码网络（PCN）。通过实现近期研究中的直接 Kolen-Pollack 反馈对齐（DKPPCN）加速方法，并利用算法缓存跳过推理收敛阶段中冗余的前向投影，该库在 CPU 上训练 MNIST（50 轮）时显著缩小了与反向传播的性能差距：PyTorch 反向传播达到 98.27% 的测试准确率（约 70 秒），而 Deepity DKPPCN 达到 97.73% 的准确率（59.5 秒）。这一可复现结果表明，预测编码网络在速度和精度上均能匹敌反向传播。开发者计划下一步将内核移植到 CUDA 以扩展架构规模，并测试其在标准反向传播难以处理的持续学习场景中的表现。

reddit · r/MachineLearning · /u/Important-Home4431 · 9月2日 16:49

**「背景」** 预测编码网络（PCN）是一种受神经科学启发的学习框架：层级模型中的每一层通过反馈连接预测下一层的响应，并用误差信号逐层修正对输入的估计，兼具生物学合理性和持续学习潜力。然而朴素的 PCN 实现需要反复的推理迭代来收敛，训练速度远慢于反向传播。为此，近期研究提出的直接 Kolen-Pollack 反馈对齐（DKP-PC）方法引入从输出层到所有隐藏层的可学习反馈连接，为误差传递建立直接通路，从而大幅加快学习速度。

**「影响」** 该结果以可复现的实验证据表明，更具生物合理性的预测编码网络能够在 MNIST 上同时匹配反向传播的训练速度与精度，为持续学习等场景下探索高效替代信用分配方案提供了实际基础。不过该结论仅基于单一数据集和 CPU 环境，尚需在更大架构与 GPU 上验证其普适性与扩展性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Predictive_coding">Predictive coding - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2602.15571v1">Accelerated Predictive Coding Networks via Direct Kolen–Pollack Feedback Alignment</a></li>
<li><a href="https://arxiv.org/abs/2602.15571">[2602.15571] Accelerated Predictive Coding Networks via Direct Kolen-Pollack Feedback Alignment</a></li>

</ul>
</details>

**标签**: `#predictive coding`, `#backpropagation`, `#C++`, `#machine learning`, `#MNIST`

---

<a id="item-tech-news-9"></a>
### [CABiNet 对比 YOLO26-sem：UAVid 基准显示精度与延迟权衡](https://www.reddit.com/r/MachineLearning/comments/1w5cfv1/cabinet_icra_2021_vs_yolo26sem_on_uavid_accuracy/) ⭐️ 7.0/10

CABiNet（ICRA 2021）的原第一作者在重建仓库后，于 UAVid 测试集上发布了一项可复现的对比基准：在 1024×1024 单尺度、无测试时增强的统一评估协议下，CABiNet-L 以 67.14% mIoU、9.17M 参数、54.8G FLOPs 和 4.44ms FP16 前向延迟（RTX 4070 SUPER、批大小 1）胜过 YOLO26x-sem 的 64.41% mIoU 与 13.09ms 延迟。两类模型共享转换后的数据集与分割、ENet 逆对数类权重（cls\_pw=0.5）及 EMA 评估，但初始化、epoch 预算、优化器、损失与增强各不相同——YOLO26 享有 Cityscapes 与 ADE20K 预训练优势，CABiNet 则拥有更长的训练预算（5000 轮对 500 轮），作者直言这是受控基准而非架构消融。近等计算量对比中（约 44G FLOPs），CABiNet-S 比 YOLO26s 高出 3.6 个 mIoU 点（65.25 对 61.69），但 YOLO26s 延迟更低，属于明确的精度/延迟取舍；而在 VDD 与 AeroScapes 上，YOLO26s 及以上型号反而超越 CABiNet-Large。该结果覆盖单次训练、无方差估计，延迟为纯模型前向、不含 TensorRT/ONNX 或端到端分块成本，权重、Hydra 配置、评估脚本与在线演示均已开源。

reddit · r/MachineLearning · /u/Naive-Explanation940 · 9月2日 14:46

**「背景」** CABiNet 是 2021 年发表于 ICRA（DOI 10.1109/ICRA48506.2021.9560977）的双分支 CNN 实时语义分割模型，由高分辨率空间分支与基于 MobileNetV3 的轻量上下文分支（全局聚合+局部分布）经 FFM 融合而成，原始论文即以 UAVid 航拍数据集为目标。YOLO26 则是 2026 年的通用多任务模型，其专用语义分割变体从 Cityscapes 与 ADE20K 预训练出发。今年的对比由原作者在重构后的仓库（PyTorch 2.x、Hydra、AMP、EMA、poly-LR、OHEM 损失、CI 与测试）中完成，意在检验 2021 年专用架构相对 2026 年通用模型在效率权衡上的位置。

**「影响」** 对追求航拍语义分割效率的研究者与工程团队，该结果意味着 CABiNet-L 在 UAVid 上能以约 3 倍更低的 GPU 前向延迟换取更高精度（+2.7 mIoU），但这并非普适优越。由于结论基于单次训练、无统计显著性估计，且跨数据集（VDD、AeroScapes）与部署场景（TensorRT/ONNX、Jetson、端到端分块）的表现不一致或未评估，跨架构迁移时仍需谨慎验证。

**标签**: `#semantic-segmentation`, `#benchmarking`, `#UAVid`, `#YOLO`, `#efficient-deep-learning`

---

<a id="item-tech-news-10"></a>
### [网信办 AI 治理第二阶段清理 561 万条信息](https://www.cac.gov.cn/2026-09/02/c_1790099041364574.htm) ⭐️ 7.0/10

中央网信办通报“清朗·整治 AI 应用乱象”专项行动第二阶段成果，各平台累计清理违规信息 561 万余条，并发布治理公告 46 期。抖音、快手、微博、腾讯、百度、哔哩哔哩、小红书、知乎、豆瓣、淘宝等平台优化多模态识别模型，动态扩充人脸库、声纹库和违规样本库，上线人脸实时治理系统，提升违规内容智能检测和拦截效率。豆包、元宝、千问、文心一言等平台严把原始语料审核关，强化 AI 生成合成内容标识要求。华为、小米、OPPO、vivo 等应用商店制定严格 APP 开发者准入规范，并抽检复测在架应用以拦截违规应用入库。

telegram · zaihuapd · 9月2日 05:24

**「背景信息」** “清朗”系列专项行动是中央网信办针对网络生态突出问题开展的集中整治行动，此次聚焦 AI 应用领域，重点治理利用人工智能生成和传播违法违规信息、违规上架 AI 应用等乱象。此前第一阶段已取得一定成效，此次通报为第二阶段成果汇总，涉及内容审核技术升级和平台责任落实。

**「影响」** 对 AI 应用开发者而言，必须更严格地遵守内容审核和标识要求，否则可能面临应用被应用商店下架或账号被处置的风险；对平台和内容服务商来说，需要持续投入技术治理能力并承担常态化审核责任。

**标签**: `#AI监管`, `#内容审核`, `#平台治理`, `#政策合规`, `#AI应用`

---

<a id="item-tech-news-11"></a>
### [阿里发布 Qwen3.8-Max-0902，CodeArena 编程榜夺冠](https://mp.weixin.qq.com/s/BfKRXMAR5ykD58LDkBftLg) ⭐️ 7.0/10

阿里巴巴通义千问发布新版本模型 Qwen3.8-Max-0902，该模型针对编程与专业办公任务进一步后训练，在 CodeArena 前端编程总榜中以 1691 分夺冠，较旧版提升 22 分。新模型拥有 2.4T 参数与 1M 上下文长度，API 定价为每百万 tokens 输入 2 美元、输出 6 美元，综合均价约 5 美元，低于榜单第二、第三名模型的 20 美元和 12 美元。该版本已上线千问 AI 平台，并接入千问办公、Qoder 与千问 APP，覆盖 AI 编码与办公场景。此次发布标志着阿里在编程基准测试上的领先，并通过较低定价提升 API 性价比竞争力。

telegram · zaihuapd · 9月2日 06:05

**「背景」** Qwen 是阿里巴巴通义千问推出的开源大语言模型系列。此前发布的旗舰版 Qwen3.8-Max 采用稀疏混合专家（MoE）架构，总参数约 2.4 万亿、每个 token 激活约 950 亿参数，并支持 100 万 token 的超长上下文窗口。本次发布的 0902 版本是这一基础模型的升级快照，而 CodeArena 则是衡量模型前端编程与代码生成能力的评测榜单。

**「影响」** 开发者使用 Qwen3.8-Max-0902 API 进行编程任务时，可受益于 CodeArena 领先的 1691 分表现及更低定价，每百万 tokens 综合均价约 5 美元，显著低于竞争对手的 20 美元和 12 美元，可能加速阿里在 AI 编程工具市场的采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=BjRmcnSVUlc">Meet Qwen 3 . 8 - Max - 0902 : Better Than Original: A Massive... - YouTube</a></li>
<li><a href="https://aibreakfast.beehiiv.com/p/alibaba-releases-qwen-3-8-max-with-16-day-autonomous-execution-capabilities">Alibaba releases Qwen 3 . 8 Max with 16-day autonomous execution...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Qwen`, `#large language models`, `#coding benchmark`, `#Alibaba`

---

<a id="item-tech-news-12"></a>
### [月之暗面与三大云厂商洽谈 Kimi K3 收入分成](https://www.jiemian.com/article/15040119.html) ⭐️ 7.0/10

据消息人士透露，月之暗面正与微软、亚马逊、谷歌就开源模型 Kimi K3 的收入分成展开早期谈判，初期寻求最高 30% 的分成比例。若协议达成，这将成为中国 AI 公司与美国云巨头之间的首个大型模型收入分成协议。Kimi K3 于 2026 年 7 月发布，总参数达 2.8 万亿，是全球首个开源 3T 级模型，截至 6 月中旬其年度经常性收入已突破 3 亿美元。目前谈判仍处早期阶段，核心细节尚未敲定，相关各方均拒绝置评。

telegram · zaihuapd · 9月2日 07:36

**「背景」** 月之暗面（Moonshot AI）是中国领先的人工智能实验室，其开源的 Kimi K3 模型于 2026 年 7 月发布，总参数达 2.8 万亿，是全球首个开源 3T 级模型，截至 6 月中旬年度经常性收入已突破 3 亿美元。通常开源模型厂商依赖云平台托管并按使用量向用户收费，而由云厂商托管并直接与模型方分成、尤其是让美国云巨头托管中国模型，属于少见的新安排。据路透社报道，月之暗面此前已与多家较小规模云平台签署类似分成协议，阿里巴巴也在为其新的开源模型向主要用户寻求收入分成协议，显示这一模式可能正在行业内扩散。

**「影响评估」** 若谈判成功，月之暗面将成为首家借助美国主要云平台分销开源模型并获取收入分成的中国 AI 公司，为开源大模型的商业化开辟新路径；但协议能否落地仍取决于云厂商对推理成本与市场需求的评估，存在较大不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://money.usnews.com/investing/news/articles/2026-08-26/exclusive-chinas-moonshot-in-talks-with-microsoft-amazon-google-over-k3-revenue-sharing-sources-say">Exclusive-China&#x27;s Moonshot in Talks With Microsoft, Amazon, Google...</a></li>
<li><a href="https://www.odaily.news/en/newsflash/512869">Foreign media: Up to 30%, Moonshot AI reportedly in talks... - Odaily</a></li>
<li><a href="https://mezha.net/eng/bukvy/84dfc5a3_moonshot_ai_negotiates/">Moonshot AI Negotiates Revenue Sharing Deals to Bring Kimi K 3 to...</a></li>

</ul>
</details>

**标签**: `#AI industry`, `#cloud computing`, `#open source models`, `#Moonshot AI`, `#revenue sharing`

---

<a id="item-tech-news-13"></a>
### [马斯克预告 Grok 4.7 十天后上线，参数 2.1 万亿](https://x.com/elonmusk/status/2094983639780204846) ⭐️ 7.0/10

马斯克 9 月 2 日在 X 平台（原推特）预告，Grok 4.7 将于 10 天后、即 2026 年 9 月 12 日上线。该模型参数规模达 2.1 万亿，较 Grok 4.6 的 1.5 万亿增长 40%，除服务速度略慢外，各项表现均优于前代，且 Token 效率更高。马斯克另于 8 月 13 日表示，Grok 4.7 上线后将超越所有现有模型。需要注意的是，该信息来自社交网络转发，缺少官方技术细节，模型尚未实际发布，性能宣称有待实测验证。

telegram · zaihuapd · 9月2日 08:10

**「背景」** Grok 是马斯克旗下人工智能公司 xAI 开发的大语言模型系列，前作 Grok 4.6 于 2025 年 8 月 7 日发布，参数规模为 1.5 万亿。约 2.1 万亿参数的设计自 2025 年 7 月起就已在多个媒体报道中流传，马斯克在 8 月 13 日也曾宣称 Grok 4.7 发布后将超越所有现有模型。9 月 2 日的预告是马斯克首次亲自证实参数规模与 10 天后的上线时间（2026 年 9 月 12 日），把此前仅有模糊时间窗的传闻落实为具体的发布计划。

**「影响」** 若 Grok 4.7 如期于 9 月 12 日上线并兑现性能宣称，其 2.1 万亿参数规模将直接冲击 OpenAI、Google 等现有头部模型的竞争格局；但因该预告源自社交网络且未经第三方实测，实际影响力仍存不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.biggo.com/news/cdeb763e-3e82-4f0b-82bd-4f473881bf08">Musk Announces Grok 4.7 Launch in Ten Days with 2.1 Trillion Parameters, Claims It Will Surpass All Models — BigGo Finance</a></li>
<li><a href="https://tbreak.com/grok-4-6-4-7-xai-release-date-specs/">Grok 4.6 Release Date: August 7, 1.5T Parameters &amp; More</a></li>
<li><a href="https://www.orcarouter.ai/blog/grok-4-7-release-date">Grok 4.7 Release Date: Musk Confirms Mid-September Target</a></li>

</ul>
</details>

**标签**: `#Grok`, `#马斯克`, `#AI模型`, `#参数规模`, `#行业新闻`

---

<a id="item-tech-news-14"></a>
### [Nexus 暗网兜售 1.53 亿驾照扫描件 FBI 介入调查](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/) ⭐️ 7.0/10

据 KrebsOnSecurity 报道，FBI 正在调查一个名为 Nexus 的暗网身份信息兜售服务，该平台声称掌握超过 1.53 亿张来自美国与加拿大民众的驾照数字扫描件，并已开始对外售卖。这些驾照扫描件包含姓名、住址、出生日期等敏感信息，一旦被用于身份冒用，受影响人群规模可观。Krebs 指出，这批数据可能源自此前汽车经销商、保险公司等机构泄露的旧扫描文件，目前官方尚未公布具体来源与影响人数。

telegram · zaihuapd · 9月2日 09:31

**「背景」** 驾照扫描件包含姓名、住址、出生日期等可用于身份冒用的敏感信息，长期是暗网身份兜售市场的热门商品；此类服务通常批量转售历年来由机构泄露的旧扫描文件，而非首次作案的新手。据调查线索，Nexus 出售的美国与加拿大驾照数据可能源自身份扫描服务商 IDScan.net 的泄露，部分文件还涉及医疗卡、居留卡等证件。

**「影响」** 对于美国与加拿大民众，尤其是驾照信息可能已包含在上述机构旧泄露事件中的个人，面临身份冒用与欺诈风险显著上升；由于官方尚未确定具体受影响名单，相关用户应警惕可疑的信用查询或贷款申请，并及时核查自身信用报告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5mac.com/2026/09/02/fbi-investigates-as-hackers-sell-digital-scans-of-153m-drivers-licenses/">FBI investigates as hackers sell digital scans of 153M drivers licenses</a></li>
<li><a href="https://www.technadu.com/fbi-investigates-nexus-dark-web-service-selling-over-153-million-us-and-canadian-drivers-licenses/634891/">FBI Probes Nexus Over 153M US and Canadian Driver ’ s Licenses</a></li>
<li><a href="https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/">FBI Probes Service Selling 153M+ Drivers Licenses – Krebs on...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#data breach`, `#privacy`, `#dark web`, `#identity theft`

---

<a id="item-tech-news-15"></a>
### [新国标规范 AI 客服协同，禁止隐藏转人工入口](https://mp.weixin.qq.com/s/Agt4qI5tgQA4kCT1DJX6fg) ⭐️ 7.0/10

9 月 1 日起，我国首个聚焦人工与智能客服协同的国家标准《顾客联络服务 人工与智能客户服务协同要求》（GB/T 47746—2026）正式实施。该标准要求平台设置明确的转人工选项，不得层层隐藏，且企业对 AI 客服回复内容承担主体责任，不得以算法生成为由拒绝兑现承诺。中消协 2026 年上半年投诉分析显示，售后服务问题占总投诉量的 26.79%，AI 客服“人工接入困难”成为新热点。专家指出，AI 客服月租可低至 99 元，而一线城市单名人工客服年成本达 8 万至 12 万元。该标准虽属推荐性，但可作为监管检查和纠纷调解的参考。

telegram · zaihuapd · 9月2日 11:17

**「背景」** 随着 AI 客服在企业客户服务中广泛应用，部分平台为降低成本，隐藏转人工入口或让 AI 客服难以转接人工，导致消费者维权困难。中消协 2026 年上半年投诉数据显示，售后服务问题占比达 26.79%，AI 客服“人工接入困难”成为新的投诉热点，促使监管部门出台国家标准加以规范。

**「影响」** 对于 AI 客服平台和企业，新标准要求明确设置转人工入口，并对 AI 回复承担主体责任，可能增加合规成本；对消费者而言，转人工渠道的透明化有助于改善售后维权体验。由于该标准为推荐性标准，其实际约束力取决于监管检查和纠纷调解的应用情况。

**标签**: `#AI customer service`, `#regulation`, `#China standards`, `#human-AI collaboration`, `#industry news`

---

<a id="item-tech-news-16"></a>
### [纽约公立学校将全面限制低年级学生课堂使用生成式 AI](https://abc7ny.com/post/new-york-city-public-schools-banning-ai-use-middle-school-year/19778716/) ⭐️ 7.0/10

纽约市公立学校宣布将在 2026—2027 学年实施新的技术政策，禁止学前班至八年级的近 60 万名学生课堂使用聊天机器人、AI 辅导等生成式 AI 工具，高中生的使用也将受到严格限制。新规同时限制个人学习设备的屏幕时间：学前班至二年级课堂不使用个人设备，三至五年级每天最多 30 分钟，初中生每天最多 45 分钟。教师仍可使用获批准的 AI 辅助备课、翻译和撰写通知，但不得将 AI 用于评分、行为监控、危机辅导及制定特殊教育计划。这一政策为全美最大公立学区的 AI 教育治理设下明确边界，可能成为其他地区制定同类政策的参照。

telegram · zaihuapd · 9月2日 14:38

**「背景」** 生成式 AI 工具（如聊天机器人和 AI 辅导）自 2022 年以来迅速进入校园，但围绕作弊风险、数据隐私、内容准确性及对学生认知发展的影响，争议一直持续。纽约市公立学校此前曾一度禁止 ChatGPT 后又解禁，此次新政策是其对 AI 治理的进一步收紧，并首次将屏幕时间限制与 AI 使用限制捆绑出台。

**「影响」** 该政策将直接影响纽约市约 60 万名学生，限制其在课堂接触生成式 AI 的机会，同时保留教师端获批的 AI 应用，体现“教师可用、学生受限”的管理取向。作为全美规模最大的公立学区之一，其政策动向可能被其他地区效仿，从而影响教育领域 AI 工具的采用节奏。

**标签**: `#AI policy`, `#education`, `#generative AI`, `#New York City`, `#screen time`

---