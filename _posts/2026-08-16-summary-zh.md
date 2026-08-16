---
layout: default
title: "Horizon Summary: 2026-08-16 (ZH)"
date: 2026-08-16
lang: zh
---

> 从 33 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [Anthropic 发布 Claude 模型系统提示词](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B：能力出色却默认过度思考的开放模型](#item-tech-news-2) ⭐️ 8.0/10
3. [SSOG-Attention：用可分离高斯和替代 SDPA 的次二次注意力](#item-tech-news-3) ⭐️ 8.0/10
4. [重新审视高效通道注意力论文：中心假设或存疑](#item-tech-news-4) ⭐️ 8.0/10
5. [Claude 母公司营收暴增 14 倍](#item-tech-news-5) ⭐️ 8.0/10
6. [模型刻意变“笨”：推理优先的新趋势](#item-tech-news-6) ⭐️ 7.0/10
7. [Cloudflare 在切换名称服务器时静默注入分析脚本](#item-tech-news-7) ⭐️ 7.0/10
8. [美国要求盟友 AI 选边站](#item-tech-news-8) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 发布 Claude 模型系统提示词](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 公开了旗下 Claude 模型（如 Opus、Sonnet）的系统提示词，这些提示词以版本化形式发布（例如 Opus 4.8 与 Opus 5），直接展示了模型行为约束的底层文本。此举旨在提升透明度，帮助开发者理解模型为何以特定方式响应，从而更有效地进行调试和提示工程。具体提示词包括检查对话中是否实际附带了图像、在用户处于危机时优先保障其福祉等明确指令，反映出 Anthropic 从多个层面塑造模型行为的策略。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**「背景信息」** 系统提示词（System Prompt）是每次对话开始时向 Claude 提供的一组指令，用于设定行为边界和提供最新信息（如当前日期）。Anthropic 自 2024 年 10 月起将 Claude 网页版和移动端的系统提示词公之于众，并持续在平台文档中更新，以提升模型行为的透明度，帮助开发者理解其约束与能力。

**「影响」** 开发者现在可以审查 Claude 的系统级约束，从而更精准地调试与优化提示词，提升应用可靠性。不过，这些提示词仅是模型行为控制体系中的一层，模型的最终响应还受其他机制影响。

**「社区讨论」** 部分社区成员已通过 Git 仓库追踪提示词版本差异（如 Opus 4.8 与 5 的变更），例如新加入的 Fable 5 和 Mythos 5 模型名称。有人觉得像检查图像是否存在这类提示显得过于基础，但其他人强调这仅是分层行为控制系统中的一环，公开举措本身仍具有积极意义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs - Anthropic</a></li>
<li><a href="https://hackaday.com/2024/10/12/all-system-prompts-for-anthropics-claude-revealed/">All System Prompts For Anthropic’s Claude, Revealed - Hackaday</a></li>

</ul>
</details>

**标签**: `#system-prompts`, `#anthropic`, `#claude`, `#transparency`, `#llm`, `#ai-engineering`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B：能力出色却默认过度思考的开放模型](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

阿里云 Qwen 研究团队发布 Apache 2 许可的 27B 视觉模型 Qwen 3.8 27B，自报基准测试成绩优于前代，并可在消费级硬件上本地运行。默认推理努力设置为“xhigh”导致模型在简单任务上也进行大量过度思考——例如绘制一个圆会引发对几何美学的长篇推理，生成一个自行车鹈鹕 SVG 用了 22,276 个推理 token、耗时 21 分钟。关闭推理后相同任务仅需 2 分多钟，且模型仍能生成高质量图像；在视觉边界框任务上表现同样出色。作者建议用户忽略默认设置，优先使用低推理努力模式。

rss · Simon Willison · 8月16日 22:00

**「背景」** Qwen 3.8 27B 是 Qwen 系列的大型语言模型，支持通过 reasoning\_effort 参数控制推理深度，“xhigh”模式旨在处理复杂任务，会生成大量思考链 token。该模型继承了 Qwen 3.6 27B 的视觉能力，能够处理图像并生成 SVG 或边界框，并支持在本地设备上部署。

**「影响」** 默认推理设置可能导致消费级硬件上数十分钟的生成延迟，用户必须手动将推理努力调至低或无才能获得可用的响应速度。

**标签**: `#AI`, `#LLM`, `#model release`, `#open source`, `#Qwen`

---

<a id="item-tech-news-3"></a>
### [SSOG-Attention：用可分离高斯和替代 SDPA 的次二次注意力](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 8.0/10

研究者提出了一种名为 SSOG（Sum Of Separable Gaussians）的注意力机制，它用可分离高斯原子的学习替代缩放点积注意力，将复杂度从 O\(N²·d\)降至 O\(N·√N·d\)。在 ImageNet-1k 上，SSOG 取得了与 SDPA 相当的性能且收敛更快，在 CIFAR-100 上则明显优于 SDPA。该方法在更大规模下具有更高的内存和计算效率，相关代码已开源（GitHub 仓库）。该工作尚未经过同行评审，作者声明部分代码与博文使用了 AI 辅助，但对其内容负责。

reddit · r/MachineLearning · /u/4rtemi5 · 8月16日 10:06

**「背景」** 缩放点积注意力（SDPA）是 Transformer 架构的核心，通过计算所有查询与键的相似度得分来聚合信息，导致计算复杂度随序列长度 N 呈二次增长。为支持长序列处理，研究者一直在探索次二次复杂度的注意力替代方案，如线性注意力、稀疏注意力等。SSOG 属于这一方向，通过引入可分离高斯函数实现高效近似。

**「影响」** 对于需要处理长序列或高分辨率图像的计算机视觉任务，SSOG 在保持精度的同时，显著降低了注意力模块的计算与内存开销，并可能加速模型训练收敛。

**标签**: `#machine learning`, `#attention mechanism`, `#efficient transformers`, `#sub-quadratic attention`, `#computer vision`

---

<a id="item-tech-news-4"></a>
### [重新审视高效通道注意力论文：中心假设或存疑](https://www.reddit.com/r/MachineLearning/comments/1vptaw9/revisiting_the_efficient_channel_attention_paper/) ⭐️ 8.0/10

一位 Reddit 用户对高效通道注意力（ECA）论文（2019 年，引用量约 12k）的核心假设提出质疑，认为在无序通道均值上应用一维卷积缺乏拓扑依据。作者在棋类六子残局数据库上的受控实验显示，ECA 的 k=1 变体（即无跨通道交互）与 k=3 标准版本性能几乎持平，且均优于 SE 模块。检查官方及社区代码仓库发现，几乎所有复现均未进行纯 k=1 消融实验，部分实现甚至将 k 强制限制在 3 及以上。此外，屏蔽中间通道的掩码卷积（\[1, 0, 1\]）和每个通道独立权重的门控也取得了相近效果，共同表明原论文“跨通道交互是关键”的解释可能不成立，需重新审视通道注意力机制的工作原理。

reddit · r/MachineLearning · /u/arkuto · 8月16日 10:13

**「背景」** SENet 通过全局平均池化与全连接降维层对通道特征进行重标定；ECA-Net 则直接对通道均值应用一维卷积，避免降维，并声称跨通道交互是提升性能的关键因素。该设计在 ImageNet 上取得显著效果，成为注意力模块中的常用方案。

**「影响」** 该分析提示 ECA 论文中强调的跨通道交互可能并非注意力提升的根本原因，要求后续研究在评估通道注意力机制时，必须包含 k=1 的退化情况作为基准，以防过度解读设计要素。

**标签**: `#machine learning`, `#computer vision`, `#attention mechanisms`, `#deep learning`, `#research critique`

---

<a id="item-tech-news-5"></a>
### [Claude 母公司营收暴增 14 倍](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

Anthropic 第二季度初步营收超过 115 亿美元，比去年同期的 7.87 亿美元增长逾 14 倍，较上一季度的 47.3 亿美元也大幅提升，同时调整后营业利润实现转正。该公司正在筹备可能于今年秋季启动的大型 IPO，但初步数据仍可能调整。这一增长凸显了 AI 市场的强劲需求，也标志着 Anthropic 在商业化上迈出关键一步。

telegram · zaihuapd · 8月16日 07:26

**「背景」** Anthropic 是一家由前 OpenAI 员工创立的 AI 安全公司，主打 Claude 系列大语言模型，与 OpenAI 的 GPT 等产品竞争。此前其营收已连续多个季度高速增长，从 2025 年第一季度的 47.3 亿美元跃升至第二季度的 115 亿美元，显示出在企业和开发者市场中的采用率快速提升。

**「影响」** Anthropic 的盈利能力转正和 IPO 计划，可能吸引更多企业客户信赖并部署 Claude 模型，同时加剧 AI 行业竞争，推动基础设施和 API 定价的进一步优化。

**标签**: `#Anthropic`, `#AI industry`, `#revenue`, `#IPO`, `#business`

---

<a id="item-tech-news-6"></a>
### [模型刻意变“笨”：推理优先的新趋势](https://w4g1.dev/blog/models-are-getting-dumber-on-purpose) ⭐️ 7.0/10

近期一篇分析文章指出，大语言模型正从依赖静态事实记忆转向强化推理与外部工具调用，以降低幻觉并提升适应性。这一趋势意味着模型不再将全部知识内嵌于权重，而是通过推理链和工具检索动态获取信息，使得知识截止日期变得不再关键。尽管所引用的 SimpleQA 基准和 Gemini 2.5 Pro 等示例被认为已过时，但该方向本身持续受到关注，并引发了对模型架构演变的讨论。

hackernews · hruvhwe · 8月16日 19:04 · [社区讨论](https://news.ycombinator.com/item?id=49322695)

**「背景」** 大型语言模型传统上通过将海量事实知识直接编码到模型参数中来实现问答，但这导致模型体积膨胀且容易产生幻觉。近期的趋势是有意剥离模型内部的世界知识，转而强化其推理和工具调用能力，使得推理得分上升的同时，每词元计算开销下降（tool-1-1）。此举并非模型质量下降，而是有意为之的设计权衡，旨在通过减少静态记忆来提升灵活性和可靠性。

**「影响」** 开发者将更倾向于构建模块化知识库与推理引擎分离的系统，模型部署可能转向小参数核心推理模型搭配外部工具，但这也对知识库的维护和工具集成提出了更高要求。

**「社区讨论」** 社区中有人提出可插拔知识库的设想，但也有评论指出文章在基准和模型版本上已过时；此外，部分观点质疑推理与事实能否真正脱钩，认为人类决策并非纯粹逻辑推理，该策略的适用范围仍需验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://w4g1.dev/blog/models-are-getting-dumber-on-purpose">Models Are Getting Dumber on Purpose - Walter van der Giessen</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLMs`, `#model-reasoning`, `#knowledge-distillation`, `#hallucination`

---

<a id="item-tech-news-7"></a>
### [Cloudflare 在切换名称服务器时静默注入分析脚本](https://news.ycombinator.com/item?id=49322107) ⭐️ 7.0/10

用户在将域名切换到 Cloudflare 名称服务器以启用 R2 子域名访问后，发现其原本无 JavaScript 的纯 HTML 网站被自动注入了 Cloudflare Web Analytics 的 JS 分析片段。该行为默认开启，用户需进入 Analytics 仪表板添加站点，然后手动关闭代码片段才能去除，属于 opt-out 而非 opt-in 机制。社区反馈指出，这一注入仅发生在启用 Cloudflare 代理（橙色云）时，若仅使用 DNS 解析（灰色云）则不受影响，被注入的脚本包含唯一令牌并通过 beacon 发送数据，对隐私合规构成潜在风险。

hackernews · stagas · 8月16日 17:49

**「背景」** Cloudflare 于 2025 年 9 月宣布，其 Web Analytics（真实用户监控，RUM）功能将自 2025 年 10 月 15 日起对所有免费域名默认开启，目标是在不收集个人数据的前提下提供性能洞察（欧盟和英国流量除外）。这项变更意味着当用户将域名接入 Cloudflare 并使用其代理功能时，Cloudflare 会自动向页面注入 JavaScript 分析脚本，用户需手动关闭。

**「影响」** 使用 Cloudflare 代理服务的网站，在更改名称服务器后会被默认注入 Web Analytics 脚本，须手动进入仪表板关闭，可能违反网站隐私声明或引入不必要的用户跟踪。仅 DNS 解析（灰色云）模式不受此影响。

**「社区讨论」** 社区确认注入仅在启用代理（橙色云）时发生，并建议通过内容安全策略（CSP）限制脚本来源来阻止该分析脚本加载，从而避免隐私泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/the-rum-diaries-enabling-web-analytics-by-default/">The RUM Diaries: enabling Web Analytics by default</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#web-analytics`, `#privacy`, `#dns`, `#javascript-injection`

---

<a id="item-tech-news-8"></a>
### [美国要求盟友 AI 选边站](https://www.neowin.net/news/us-warns-allied-nations-side-with-us-in-the-ai-race-against-china-or-face-the-consequences/) ⭐️ 7.0/10

美国据报要求盟友及希望进行 AI 合作的国家签署名为“Pax Silica”的宣言，在人工智能领域明确选边，不得加入与中国相关的冲突倡议，否则可能被排除在美国主导的 AI 联盟之外。该宣言不仅是加入联盟的承诺，更明令禁止签署国参与预期相冲突的其他倡议，旨在巩固美国在 AI 领域的领导地位并孤立中国。此举突显地缘政治正深刻影响全球 AI 合作与治理。

telegram · zaihuapd · 8月16日 02:30

**「背景」** “Pax Silica”是美国主导的旨在强化半导体、人工智能和稀土等关键技术供应链安全的国际倡议，于 2026 年 2 月首次与印度签署。在中美 AI 竞争加剧的背景下，美国近期向盟友及合作伙伴施压，要求其签署该宣言并与美国合作，旨在通过技术联盟限制中国获取先进 AI 资源。

**「影响」** 如果该政策推行，美国盟友可能被迫在中美 AI 生态之间做出选择，进而影响技术供应链、标准制定与开源协作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.neowin.net/news/us-warns-allied-nations-side-with-us-in-the-ai-race-against-china-or-face-the-consequences/">US warns allied nations: Side with us in the AI race against ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pax_Silica">Pax Silica - Wikipedia</a></li>
<li><a href="https://www.state.gov/pax-silica/">Pax Silica - United States Department of State</a></li>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/02/united-states-and-india-sign-pax-silica-declaration/">United States and India Sign Pax Silica Declaration</a></li>

</ul>
</details>

**标签**: `#地缘政治`, `#人工智能`, `#国际合作`, `#技术政策`, `#Pax Silica`

---