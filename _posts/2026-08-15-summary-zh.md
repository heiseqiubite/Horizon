---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 24 条内容中筛选出 6 条重要资讯。

---

**科技新闻**
1. [Firefox 成唯一支持 uBlock Origin 的主流浏览器](#item-tech-news-1) ⭐️ 8.0/10
2. [BDH-CQ：基于循环隐式推理的上下文学习](#item-tech-news-2) ⭐️ 8.0/10
3. [阿里 Qwen 下载量半年破 30 亿](#item-tech-news-3) ⭐️ 8.0/10
4. [使用 Codex 自动研究实现 232 倍 GPU 内核加速](#item-tech-news-4) ⭐️ 7.0/10
5. [Jacobian 镜头零重构迁移至 Qwen3.8-27B](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Code 六大省钱技巧，缓存省 90% 成本](#item-tech-news-6) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Firefox 成唯一支持 uBlock Origin 的主流浏览器](https://zeli.app/zh/digest/2026-08-14) ⭐️ 8.0/10

2026 年 8 月 14 日，随着 Microsoft Edge 等 Chromium 内核浏览器逐步淘汰 Manifest V2 架构，Mozilla Firefox 成为唯一继续支持 uBlock Origin 等强力广告拦截扩展的主流浏览器，用户无需妥协即可获得纯净浏览体验。同日，阿里巴巴 Qwen 团队开源了 Qwen3.8-27B 稠密模型，仅 27B 参数就在 SWE-bench Pro、CoWorkBench 等基准上大幅超越前代 Qwen3.6-27B，甚至逼近 Opus 4.6 Max，并原生支持 256K 上下文、可扩展至 1M tokens，为本地部署高性能 AI 提供了极高性价比的选择。这两项进展分别标志着网页浏览隐私保护和开源 AI 能力的重要突破。

rss · Zeli · 8月14日 23:59

**「背景」** Chromium 浏览器的 Manifest V2 扩展架构允许广告拦截器深度拦截网络请求，而 Google 主导的 Manifest V3 迁移限制了相关 API，导致 uBlock Origin 等扩展拦截效果大打折扣。Qwen 是阿里巴巴通义实验室开发的开源大语言模型家族，Qwen3.8-27B 是其最新稠密模型，专为代码生成、Agent 任务等场景优化，采用 Apache 2.0 许可证开放权重。

**「影响」** 重视隐私和广告拦截的用户可能大规模转向 Firefox，而 Qwen3.8-27B 的发布则为开发者在本地部署高性能 AI 模型提供了绕过云端 API 的高性价比方案。

**标签**: `#web-browsers`, `#ad-blocking`, `#open-source`, `#language-models`, `#AI`

---

<a id="item-tech-news-2"></a>
### [BDH-CQ：基于循环隐式推理的上下文学习](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 8.0/10

BDH-CQ 提出了一种基于循环隐式推理的上下文学习系统，在推理时通过任务演示持续更新循环记忆，并在高维隐空间中迭代计算得到查询答案，无需显式解码中间推理步骤。该方法在训练中不使用任务标识符或评估任务演示对，推理时也不更新模型参数。一个 1.5 亿参数的模型在 ARC-AGI-1 上取得了 29.5% 的 pass@2 准确率，且单任务成本仅为 0.00070 美元，打破了此前报告的成本-准确率帕累托前沿。

reddit · r/MachineLearning · /u/moschles · 8月15日 06:18

**「背景」** BDH-CQ 是一种在 Dragon Hatchling \(BDH\) 后 Transformer 递归架构上扩展的推理模型，原有架构通过低秩交互的神经元单元维持演化的关联状态。ARC-AGI-1 是一个公开的抽象推理评估集，要求模型仅从少量示例中推断并应用规则，传统方法在此类任务上成本高昂。

**「影响」** 该结果表明，仅用 1.5 亿参数的小模型就能在极低推理成本下达到以往大规模模型在 ARC-AGI-1 上的准确率，为资源受限场景下的复杂推理提供了高效的新路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/pathwaycom/arc-task-gen">GitHub - pathwaycom/arc-task-gen: Generates original ARC-AGI-1-style ...</a></li>

</ul>
</details>

**标签**: `#in-context learning`, `#recurrent neural networks`, `#latent reasoning`, `#ARC-AGI`, `#machine learning research`

---

<a id="item-tech-news-3"></a>
### [阿里 Qwen 下载量半年破 30 亿](https://www.bloomberg.com/news/articles/2026-08-15/alibaba-ai-models-hit-3-billion-downloads-passing-meta-google) ⭐️ 8.0/10

阿里巴巴的 Qwen 开放权重 AI 模型在过去六个月内全球下载量突破 30 亿次，在采用规模上超过 Meta 和谷歌。根据 Hugging Face 报告，2026 年谷歌模型下载量为 4.18 亿次，Meta 仅为 2.27 亿次。阿里云已开源超过 460 个 Qwen 模型，并衍生出超过 30 万个社区版本。这一数据标志着开源 AI 生态的竞争格局发生显著变化，阿里 Qwen 系列迅速成为开发者社区的主流选择。

telegram · zaihuapd · 8月15日 15:18

**「背景信息」** Qwen（通义千问）是阿里巴巴自 2023 年 4 月内测、9 月公开发布的开源权重 AI 模型系列，其架构基于 Meta 的 Llama 模型。阿里采取将高性能模型以开放权重形式发布在 Hugging Face 和 ModelScope 等平台的策略，允许全球开发者免费下载、修改和部署，至今已开源超过 460 个模型，衍生出逾 30 万个版本。

**「影响」** 对于开发者而言，Qwen 下载量领先意味着可用的衍生模型已超过 30 万个，大幅提高了针对特定任务找到预调优变体的概率，从而加速应用落地。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://theaicronicle.com/en/news/companies/alibaba-open-vs-closed-ai-canary-coalmine">Alibaba: Open vs. Closed AI and the Qwen Model — The AI Chronicle</a></li>
<li><a href="https://www.aichatdaily.com/tools/qwen">Qwen Reviewed: Alibaba&#x27;s Open-Weight AI (2026) — AI Chat Daily</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-15/alibaba-ai-models-hit-3-billion-downloads-passing-meta-google">Alibaba AI Models Hit 3 Billion Downloads , Passing Meta , Google</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#Qwen`, `#Alibaba`, `#downloads`

---

<a id="item-tech-news-4"></a>
### [使用 Codex 自动研究实现 232 倍 GPU 内核加速](https://sankalp.bearblog.dev/autoresearch/) ⭐️ 7.0/10

一篇博客介绍了如何利用 AI 驱动的自动研究流程，通过 Codex 代理在 GPU 内核优化竞赛中取得了 232 倍的性能提升。该方案通过“基准测试→性能分析→验证→研究→改进”的循环，自动生成并调整 CUDA 代码，显著超过了人工实现的性能。然而，该方法的泛化能力受到质疑，社区反馈指出，在竞赛使用的特定输入形状之外，绝大多数优化后的内核会立即崩溃，仅由 GPU 专家手工调整的版本保持了鲁棒性。这一结果揭示了当前 AI 自动优化在追求极致指标时，容易过度拟合特定测试用例，而难以产出通用可靠的系统级代码。

hackernews · tosh · 8月15日 11:00 · [社区讨论](https://news.ycombinator.com/item?id=49309549)

**「背景」** 自动研究（auto-research）指利用 AI 智能体自主执行研究任务，比如 GPU 内核优化。这篇博客文章介绍了在 GPU Mode 的 qr\_v2 竞赛中，作者使用 Codex 智能体通过自动化的基准测试、性能分析和代码改进循环，将 CUDA 内核的基线性能提升了 232 倍。

**「影响」** 所报告的 232 倍加速仅适用于竞赛特定的输入形状，生成的核在分布外数据上完全失效，因此该技术当前无法直接用于需要通用性的生产环境。

**「社区讨论」** 社区普遍关注方案的鲁棒性：前 10 名中的 8 个 AI 优化方案在非竞赛输入下全部崩溃，只有专家依靠领域知识并保持代码规模可控的方案才通过了更广泛的测试，凸显出 AI 自动研究倾向于牺牲通用性来换取基准分数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sankalp.bearblog.dev/autoresearch/">Auto-research with codex: How I achieved a 232x Faster Kernel over baseline with Codex in GPU Mode&#x27;s qr_v2 problem – sankalp&#x27;s blog</a></li>

</ul>
</details>

**标签**: `#GPU-kernel-optimization`, `#AI-code-generation`, `#auto-research`, `#performance-tuning`, `#machine-learning`

---

<a id="item-tech-news-5"></a>
### [Jacobian 镜头零重构迁移至 Qwen3.8-27B](https://www.reddit.com/r/MachineLearning/comments/1vpa5cv/survival_of_the_fitted_qwen3627bs_jacobian_lens/) ⭐️ 7.0/10

实验将专为 Qwen3.6-27B 拟合的 Jacobian 镜头（源自 Anthropic 工作）直接应用于 Qwen3.8-27B，零重构测试读取与操控。在 40 个两跳潜层实体读取中，迁移镜头在层 48 的中位排名从本模型的 4 降至 17，但在层 24 反而更优（121 vs 38），远优于原始 logit 镜头的 1e3-1e4 排名；利用旧镜头提取的“悖论”方向在 3.8 上进行投影消除，成功从输出中移除“paradox”一词且保持描述连贯。结果表明，架构和分词器相同的模型版本间，解读工具可跨版本复用，监控管线无需每次重构镜头。

reddit · r/MachineLearning · /u/imstilllearningthis · 8月15日 18:24

**「背景」** Jacobian lens（雅可比透镜）是一种可解释性工具，通过计算模型输出对内部激活的雅可比矩阵，将隐层状态投影到词汇空间，从而读取模型在推理过程中产生的潜在概念。该技术由 Anthropic 在 2024 年 7 月关于语言模型“全局工作空间”（J‑space）的论文中提出，并提供了开源实现。通常，这类透镜针对特定模型检查点拟合，但版本更新后是否需要重新拟合尚不明确。

**「影响」** 对于依赖可解释性工具进行模型监控的团队，该发现意味着可直接测试已有镜头在版本间的迁移效果，而非默认每次更新都需要重构，从而降低维护成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://runtimewire.com/article/anthropic-found-a-hidden-workspace-inside-claude">Anthropic Found a Hidden Workspace Inside Claude - RuntimeWire</a></li>
<li><a href="https://unfinishablemap.org/research/anthropic-global-workspace-j-space-2026-07-07/">Research Notes - Anthropic &#x27;s Global Workspace / J- Space in LLMs</a></li>

</ul>
</details>

**标签**: `#interpretability`, `#Jacobian-lens`, `#Qwen`, `#model-versioning`, `#transfer`

---

<a id="item-tech-news-6"></a>
### [Claude Code 六大省钱技巧，缓存省 90% 成本](http://claude.md/) ⭐️ 7.0/10

Anthropic 博客分享了 Claude Code 的六项成本优化技巧，核心是利用提示缓存机制：在任务间用 /clear 清空上下文、提前锁定模型与推理强度以避免缓存失效、用 @ 方式引用文件而非手写路径、给冗长命令加静默参数或交给子 Agent、用 /context 检查并移除不必要内容、离开前运行 /compact 以利用缓存完成压缩。官方指出，提示缓存命中后读取成本仅为正常输入的 0.1 倍，可节省 90% 费用，而输出 token 比输入贵 5 倍，目前开发者日均 token 消耗约 13 美元。

telegram · zaihuapd · 8月15日 11:14

**「背景知识」** Claude Code 是 Anthropic 推出的终端 AI 编码工具，可通过自然语言协助开发者执行任务、解释代码并管理 Git 工作流（tool-1-3）。其 API 调用按 token 计费，输出 token 价格是输入 token 的 5 倍，而提示缓存是一种将已发送的上下文暂存并复用的机制，命中后读取成本仅为正常输入的 0.1 倍，可节省约 90% 的费用。不过，中途切换模型或推理强度会清空缓存，导致成本上升。

**「影响」** 使用 Claude Code 的开发者通过遵循这些技巧可直接降低 API 调用开销，尤其是将提示缓存命中率提升后，单次对话成本可减少高达 90%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/anthropics/claude-code/releases">Releases · anthropics/ claude - code · GitHub</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#成本优化`, `#提示缓存`, `#AI编码工具`, `#开发效率`

---