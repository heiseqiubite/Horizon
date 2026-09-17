---
layout: default
title: "Horizon Summary: 2026-09-17 (ZH)"
date: 2026-09-17
lang: zh
---

> 从 40 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Nvidia 宣布在 Rust 中原生编写 GPU 内核](#item-tech-news-1) ⭐️ 8.0/10
2. [小米公开 MiMo 2.6 后训练实时仪表盘](#item-tech-news-2) ⭐️ 8.0/10
3. [黑客入侵 Flock 摄像头：硬编码凭据漏洞](#item-tech-news-3) ⭐️ 8.0/10
4. [TMLR 主编探访被拒稿作者，多数人无法解释自己的论文](#item-tech-news-4) ⭐️ 8.0/10
5. [GoBench：用围棋评测 LLM 推理能力，与 ARC-AGI 2 强相关](#item-tech-news-5) ⭐️ 8.0/10
6. [美光展示全球首款 512 GB DDR5 模组，2027 年量产](#item-tech-news-6) ⭐️ 8.0/10
7. [Mistral 与 Mozilla 合作推出多语言 AI 浏览器功能](#item-tech-news-7) ⭐️ 7.0/10
8. [DeepSeek Harness 沙箱逃逸漏洞 QVD-2026-52646 安全分析](#item-tech-news-8) ⭐️ 7.0/10
9. [Datasette 0.65.5 修复权限绕过安全漏洞](#item-tech-news-9) ⭐️ 7.0/10
10. [LARA：冻结 LLM 的轻量可组合行为适配](#item-tech-news-10) ⭐️ 7.0/10
11. [阶跃星辰发布 StepAudio 3 Music 音乐生成模型](#item-tech-news-11) ⭐️ 7.0/10
12. [新浪云 SAE 永久下线，早期 B 站 420TB 数据濒危](#item-tech-news-12) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Nvidia 宣布在 Rust 中原生编写 GPU 内核](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 8.0/10

Nvidia 官方宣布支持在 Rust 中原生编写 CUDA GPU 内核，并提供了两条不同的编写路径。这意味着 Rust 开发者可以直接使用 Rust 语言编写 GPU 内核，而无需依赖 CUDA C++。该举措有望借助 Rust 的内存安全特性提升 GPU 编程的安全性，并可能减少对单一供应商专用代码的依赖。具体版本和发布日期尚未公布，但社区反响积极，许多开发者认为这是 GPU 计算领域的一个重要里程碑。

hackernews · nonmaskable · 9月16日 11:15 · [社区讨论](https://news.ycombinator.com/item?id=49724881)

**「背景」** CUDA 是英伟达的并行计算平台与编程模型，此前 GPU 内核主要使用 CUDA C++ 或 CUDA Python 编写。Rust 是一门强调内存安全与性能的系统编程语言。根据英伟达的官方博客，其于 2026 年 9 月宣布为 Rust 提供原生 GPU 编程支持，推出两条内核编写路径：cuda-oxide（SIMT 风格）与 cutile-rs（Tile 风格），目标是在编译期实现更安全的内核代码。

**「影响」** 对于使用 Rust 进行高性能计算或需要 GPU 加速的开发者而言，这将降低 CUDA C++ 的使用门槛，并使内核编写具备更强的编译期安全保证，从而提升开发效率和可靠性。

**「社区讨论」** 社区整体持期待态度，认为 Rust 的内存安全特性可能为内核编程带来改变；但也有开发者对 CUDA 的专有性表示担忧，认为更好的做法是将内核与 CPU 代码分离并手动启动，如 Metal、OpenCL、D3D12，或使用 Triton 等 DSL。另有评论指出，由于大语言模型尚未充分训练过这一新特性，反而重新燃起了学习 Rust 的兴趣。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/">Introducing CUDA Rust: Two Tracks for Writing GPU Kernels | NVIDIA Technical Blog</a></li>
<li><a href="https://forums.developer.nvidia.com/t/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/382704">Introducing CUDA Rust: Two Tracks for Writing GPU Kernels - Technical Blog - NVIDIA Developer Forums</a></li>
<li><a href="https://www.marktechpost.com/2026/09/08/nvidia-announces-cuda-rust-with-cuda-oxide-simt-and-cutile-rs-tile-for-compile-time-safe-gpu-kernels/">NVIDIA Announces CUDA Rust with cuda-oxide (SIMT) and cutile-rs (Tile) for Compile-Time-Safe GPU Kernels - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#Rust`, `#CUDA`, `#GPU`, `#Nvidia`, `#Systems Programming`

---

<a id="item-tech-news-2"></a>
### [小米公开 MiMo 2.6 后训练实时仪表盘](https://mimo.xiaomi.com/rl/) ⭐️ 8.0/10

小米推出 MiMo 2.6 后训练（post-training）实时仪表盘，公开直播旗舰开源权重模型的训练过程，这一透明化做法在大型 AI 厂商中十分罕见，具有行业意义。仪表盘为外界提供了观察模型训练动态的直接窗口，也展现了开源 AI 持续推进的势头。网友 joelwallis 反馈已在实际软件工程工作中使用 MiMo-V2.5，成本极低、性价比极高，智能质量接近此前使用 Anthropic 模型的体验。另有网友指出 MiMo-v2.5-Pro 在 DeepSWE 1.1 基准上得分为 19%，低于 Fable（70%）、Kimi K3（69%）、Astra（74%）等模型。此次展示并非正式的新模型发布，但反映了小米在开放权重模型研发上的投入与社区的高度关注。

hackernews · krackers · 9月16日 20:09 · [社区讨论](https://news.ycombinator.com/item?id=49732270)

**「背景」** MiMo 是小米开发的系列大语言模型，于 2025 年 4 月首次发布 MiMo-7B，现通过 API 服务向开发者提供，并作为小米&quot;人车家&quot;生态的关键 AI 模型。本次页面展示的是 mimo-v2.6-pro 和 mimo-v2.6-flash 两个变体强化学习后训练的实时训练指标，直接取自训练器日志；&quot;后训练&quot;（post-training）指在基础预训练之后，通过强化学习等方式进一步调整模型行为以提升推理与编码等能力，而公开直播这类过程在大型 AI 厂商中极为罕见。此外，小米还通过开源仓库说明 MiMo 系列模型可适配 Cursor、Cline、Zed 等代理与编码工具，其中语音控制模式（mimo-v2.5）可在 OpenRouter 等兼容中继平台使用。

**「行业影响」** 小米公开直播 MiMo 2.6 后训练过程，是旗舰开放权重模型中罕见的透明度举措，让开发者能够直接观察真实训练动态，并给其他模型厂商施加了类似的开放压力；这一做法也与当前围绕 AI 训练透明度的政策趋势相呼应，从 OECD 对开放权重模型的分析到 TRAIN Act 等拟议立法均触及相关议题。

**「社区讨论」** 社区讨论整体呈正面：多位用户基于实际使用经验认可 MiMo 模型的性价比与智能质量，称其接近此前 Anthropic 模型的水平，但也有反映偶发幻觉循环和个别任务（如多任务处理）表现一般的不同体验；另有一位用户将其类比为“定时炸弹”，认为开源 AI 的进展对 OpenAI/Anthropic 构成潜在威胁，并质疑其他厂商为何不愿采取同样开放的做法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Xiaomi_MiMo">Xiaomi MiMo - Wikipedia</a></li>
<li><a href="https://mimo.xiaomi.com/rl/">mimo -v 2 . 6 RL</a></li>
<li><a href="https://github.com/XiaomiMiMo/MiMo-Code">GitHub - XiaomiMiMo/ MiMo -Code: MiMo Code: Where Models and...</a></li>
<li><a href="https://oecd.ai/en/wonk/balancing-innovation-transparency-and-risk-in-open-weight-models">AI openness: Balancing innovation, transparency and risk in ...</a></li>
<li><a href="https://btlj.org/2026/05/the-train-act-forcing-transparency-in-ai-training-data/">The “TRAIN Act”: Forcing Transparency in AI Training Data</a></li>

</ul>
</details>

**标签**: `#AI training`, `#open source AI`, `#Xiaomi MiMo`, `#LLM`, `#post-training`

---

<a id="item-tech-news-3"></a>
### [黑客入侵 Flock 摄像头：硬编码凭据漏洞](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 8.0/10

Wired 与 404media 合作披露，Flock 自动车牌识别摄像头存在硬编码 API 密钥和明文凭据等多个安全漏洞，攻击者可借此入侵摄像头并可能访问 Flock 服务器。安全研究员 micahflee 的深入分析指出，这些硬编码凭据可用来请求凭据，且明文存储的凭据可能允许以摄像头身份访问 Flock 系统。分布式拒绝秘密（DDoSecrets）已发布相关分区映像，进一步公开了漏洞证据。该问题凸显了广泛部署的监控摄像头在物理暴露环境下的安全设计缺陷，对使用 Flock 系统的机构和整个物联网安全生态具有重要意义。

hackernews · driverdan · 9月16日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49726586)

**「背景」** Flock Safety 是美国最大的自动车牌识别（ALPR）摄影机供应商之一，其摄影机安装于警察局、企业及屋主协会等场所，捕捉的车辆数据上传至云端供参与机构跨辖区搜寻与共享。安全分析发现这些摄影机韧体存在硬编码凭证等漏洞（包括 CVE-2025-47823），攻击者可利用硬编码的 API 金钥，根据摄影机的 MAC 位址向 Flock 的伺服器请求登入凭证，进而入侵装置并可能存取其资料。

**「影响」** 由于这些安全缺陷影响的是部署在美国各地、供执法机构使用的 Flock 车辆识别摄像头，攻击者一旦获得物理接触，即可利用硬编码 API 密钥和明文凭据入侵设备，进而可能访问 Flock 服务器上的敏感数据；关联事件已显示超过 230 万条车牌信息和执法查询记录遭到泄露，并促使圣克鲁斯等城市终止与 Flock 的合同、引发跨党派要求联邦调查的呼声。

**「社区讨论」** 评论者普遍批评硬编码凭据是彻底的无能表现，并指出 Flock 的漏洞披露政策（VDP）看似欢迎报告，实则通过“不得交互设备或下载数据”等条款规避真正的安全审计。还有评论强调这些摄像头部署在不受保护的公共场所，威胁模型本就包含本地物理访问，而数据甚至未适当加密，任何人无需授权即可获取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://micahflee.com/flock-cameras-are-riddled-with-security-vulnerabilities-and-hard-coded-credentials/">Flock cameras are riddled with security vulnerabilities and...</a></li>
<li><a href="https://deflock.org/">Find Nearby ALPRs | DeFlock</a></li>
<li><a href="https://deflockbhm.com/the-facts/">Information about Flock Safety use in the Birmingham metro area</a></li>
<li><a href="https://oecd.ai/en/incidents/2026-01-13-439e">Flock AI Surveillance Data Leak Exposes Millions, Triggers ...</a></li>
<li><a href="https://www.webpronews.com/flocks-surveillance-storm-error-ridden-cameras-ignite-bipartisan-backlash/">Flock’s Surveillance Storm: Error-Ridden Cameras Ignite ...</a></li>
<li><a href="https://abcnews.com/US/flock-cameras-trigger-nationwide-backlash-privacy-concerns-police/story?id=136084771">Flock cameras trigger nationwide backlash over privacy ...</a></li>

</ul>
</details>

**标签**: `#security`, `#IoT`, `#vulnerabilities`, `#surveillance`, `#credentials`

---

<a id="item-tech-news-4"></a>
### [TMLR 主编探访被拒稿作者，多数人无法解释自己的论文](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 8.0/10

机器学习期刊《Transactions on Machine Learning Research》\(TMLR\) 的联合主编主动联系了 10 篇被桌面拒稿（desk rejection）论文的作者，试图验证作者是否真正理解自己提交的工作，结果令人担忧。在这 10 篇论文中，一位作者撤回了投稿，一位作者因其他承诺无法安排会谈，一位作者约好会议却未出席；三位作者无法回答关于论文的基本问题，另三位作者虽然能回答论文的高层概念，但在进一步追问技术细节时遇到困难；仅有一位作者能回答所有提问，但主编仍在该论文中发现了重大缺陷。这一结果引发了对投稿作者身份真实性、论文质量以及可能存在的 AI 生成或伪造研究内容的严重关切。文章发布于 Medium 平台，由 TMLR 官方账号（@TmlrOrg）以“Asking Authors About Their Own Papers”为题公开，调查由该刊联合主编亲自执行，凸显了当前机器学习领域投稿诚信的潜在问题。

reddit · r/MachineLearning · /u/hihey54 · 9月16日 23:20

**「背景」** TMLR（Transactions on Machine Learning Research）是机器学习领域的学术期刊，其投稿与审稿流程托管于 OpenReview 平台。Desk rejection（直接拒稿）指稿件在进入完整同行评审之前，由编辑依据契合度与准备程度直接拒绝，并不反映研究本身是否成立，也通常不会提供深入的审稿意见。TMLR 近期正在通过年度作者投稿配额、加强编辑监督等措施整治低质量投稿，此次对拟拒稿作者的直接质询正是这一系列诚信与质量控制举措的一部分。

**「影响」** 这次访谈直接冲击了机器学习投稿生态：TMLR 联合主编对 10 篇被桌面拒稿论文作者的抽查显示，多数作者无法解释自己提交的研究（3 位答不出基本问题、3 位难以深入技术细节、1 位爽约、1 位撤稿、1 位称无暇），这加剧了学界对 AI 生成或代写稿件混入投稿流程的担忧，并可能推动 TMLR 等期刊在快速拒稿阶段强化对作者真实资质和稿件归属的实质核查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@TmlrOrg/annual-author-submission-quotas-for-tmlr-1db785e51548">Annual Author Submission Quotas for TMLR | by Transactions on Machine Learning Research | Medium</a></li>
<li><a href="https://openreview.net/group?id=TMLR">TMLR | OpenReview</a></li>
<li><a href="https://casrai.org/guides/desk-rejection">What Desk Rejection Means and Why It Happens — CASRAI</a></li>
<li><a href="https://researchramp.substack.com/p/why-research-papers-get-desk-rejected">Why Research Papers Get Desk Rejected — 10 Reasons and 10 Fixes</a></li>
<li><a href="https://casrai.org/news/neurips-2026-pangram-ai-detector-desk-rejection-controversy">NeurIPS 2026 Pangram AI-Detector Desk Rejections - CASRAI</a></li>
<li><a href="https://casrai.org/guides/desk-rejection">What Desk Rejection Means and Why It Happens — CASRAI</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#publishing ethics`, `#research integrity`, `#ML community`, `#TMLR`

---

<a id="item-tech-news-5"></a>
### [GoBench：用围棋评测 LLM 推理能力，与 ARC-AGI 2 强相关](https://www.reddit.com/r/MachineLearning/comments/1wi68jg/gobench_evaluating_llms_on_the_game_of_go_r/) ⭐️ 8.0/10

GoBench 是一个通过 9x9 围棋对局评测大型语言模型（LLM）推理能力的新基准，模型需与 KataGo 对手梯度（从随机到超人类水平）对弈。该基准与 ARC-AGI 2 相关性高（r=0.83），且当前尚未饱和，能有效区分模型推理水平。GPT-6 Astra 峰值达到 2500 Elo，远低于最强 KataGo 的 4400 Elo；而 Codex 搭配 Astra 在使用编码工具并提前两小时准备后可达到 3560 Elo。作者承诺在基准饱和前持续维护排行榜，并提供排行榜、代码和论文链接。

reddit · r/MachineLearning · /u/Roland31415 · 9月16日 18:54

**「背景」** 围棋长期被视为人工智能推理能力的试金石，因搜索空间巨大且依赖策略直觉。KataGo 是开源且强大的围棋程序，常作为对手来评估模型对弈水平，Elo 评分可反映相对棋力。ARC-AGI 2 则是衡量通用抽象推理的现有基准，GoBench 希望通过自然对弈场景提供一种可能更少饱和的推理评测方式。

**「影响」** 对于研究 LLM 推理能力的研究者和开发者，GoBench 提供了一种与 ARC-AGI 2 高度相关但尚未饱和的评测手段，可评估真实对抗场景中的模型表现；同时，当前模型（如 GPT-6 Astra）与超人类围棋 AI 的显著差距表明该基准仍有充足的上探空间。

**标签**: `#LLM evaluation`, `#benchmark`, `#Go`, `#KataGo`, `#reasoning`

---

<a id="item-tech-news-6"></a>
### [美光展示全球首款 512 GB DDR5 模组，2027 年量产](https://videocardz.com/newz/micron-says-worlds-first-512gb-ddr5-module-will-be-production-ready-for-2027) ⭐️ 8.0/10

美光展示了面向服务器的全球首款 512 GB DDR5 RDIMM，最高速率达 9200 MT/s，AMD 与 Intel 正为未来服务器平台验证该设计，预计 2027 年具备量产条件。该模组采用 3D 堆叠 DRAM 芯片，24 根可组成 12 TB 内存；美光称单根功耗为 16W，低于 4 根 128 GB 模组合计的 44.2W，降幅超过 60%。这一规格将显著提升未来服务器单机内存容量并降低功耗，但性能与功耗数据目前均为厂商宣称，量产和实际指标仍需等待 2027 年平台验证完成。

telegram · zaihuapd · 9月16日 16:15

**「背景」** 面向服务器的 RDIMM（带寄存器的双列直插内存模组）通常比消费级 UDIMM 提供更高容量与可靠性，而 DDR5 是当前主流的内存标准。过去服务器的单条 RDIMM 容量普遍停留在 128 GB 及以下，提升容量主要受制于 DRAM 芯片密度与接口针脚数；美光此次借助 3D 堆叠（TSV 硅通孔）技术将单条容量提升至 512 GB，属于内存堆叠工艺的容量里程碑。

**「影响」** 对数据库、内存计算和 AI 推理等需要高内存容量与带宽的服务器场景而言，该模组可在相同插槽数量下将单机容量提升至 12 TB，或以更少模组达成同等容量并节省超过 60% 的功耗；不过量产需等到 2027 年，实际落地节奏仍取决于 AMD、Intel 平台的验证进度。

**标签**: `#DDR5`, `#memory`, `#servers`, `#Micron`, `#hardware`

---

<a id="item-tech-news-7"></a>
### [Mistral 与 Mozilla 合作推出多语言 AI 浏览器功能](https://mistral.ai/news/mistral-x-mozilla/) ⭐️ 7.0/10

Mozilla 与 Mistral 宣布合作，为 Firefox 浏览器带来基于 AI 的多语言浏览功能，涵盖上下文感知搜索、页面摘要以及跨浏览器标签页的内容记忆与检索。据社区评论转述的公布内容，该功能已率先在法国和北美上线。此次合作的意义在于将生成式模型能力与开源浏览器结合，便于用户在阅读非英语开发文档等场景获得多语言辅助。社区讨论的核心争议在于推理方式：究竟是采用完全本地的轻量模型，还是将用户浏览历史上传至云端推理，前者更注重隐私，后者带来更多便利但要求用户付出信任。官方目前并未在营销中清晰区分本地与云端推理的具体差异，也未明确说明启用云端处理需要用户同意的隐私代价。

hackernews · vertigoruntime · 9月16日 08:08 · [社区讨论](https://news.ycombinator.com/item?id=49723408)

**「背景信息」** Mozilla 以开发开源 Firefox 浏览器和强调隐私保护著称，Mistral AI 则是总部位于法国的欧洲人工智能公司，以开发多语言大语言模型闻名。2026 年 9 月 16 日，双方宣布合作，将 Mistral 的模型整合进 Firefox 的新功能“Firefox Smart Window（测试版）”，该功能支持上下文搜索、页面摘要和跨标签页的记忆检索。该功能首先在法国和北美推出，后续计划扩展到英国和德国。

**「影响」** 对 Firefox 用户而言，这一功能在带来多语言 AI 便利的同时，将浏览历史和标签页数据的处理路径——本地或云端——与隐私信任问题摆到了台前；隐私敏感型用户可能因此对开启该功能持保留态度。

**「社区讨论」** 社区意见分歧明显：部分用户称赞多语言能力对查阅非英语开发文档的实用性，并认为相比直接信任其他服务，Mozilla 构建更注重隐私的云端推理框架是改进；但批评者质疑 Mozilla 倾向将浏览历史上传云端，认为官方未充分说明本地与云端推理的区别及启用云端的同意机制，且这类信任难以被终端用户验证。另有观点将此与 Chrome 内置 Gemini Nano 的方案类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.mozilla.org/en/firefox/mozilla-mistral-partnership/">Mozilla and Mistral partner to expand AI competition, user ...</a></li>
<li><a href="https://mistral.ai/news/mistral-x-mozilla/">Mistral x Mozilla: Private, Multilingual AI Browsing</a></li>
<li><a href="https://localmodelwatch.tsuchitsuchi.com/en/2026/09/16/mistral-mozilla-firefox-smart-window-2/">Mistral AI and Mozilla Partner for Firefox Smart Window</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#Mozilla`, `#privacy`, `#browser`, `#machine learning`

---

<a id="item-tech-news-8"></a>
### [DeepSeek Harness 沙箱逃逸漏洞 QVD-2026-52646 安全分析](https://xz.aliyun.com/news/92841) ⭐️ 7.0/10

先知社区（xz.aliyun.com）发布了一篇关于 DeepSeek Harness 安全问题的小型研究文章，其标题指向编号为 QVD-2026-52646 的沙箱逃逸漏洞，并聚焦于一条 exec 命令如何穿透沙箱这一技术路径。然而，本次提供的源内容仅包含一句简介，未给出漏洞原理、利用条件、受影响版本、攻击前提或缓解措施等可验证的技术细节。因此，关于该漏洞的严重程度、实际危害范围以及是否已被公开利用等信息目前仍不明确。要得出可靠结论，仍须查阅原文全文、漏洞库公告或官方安全披露，本文不应被当作对该漏洞的完整或权威描述。

rss · 先知社区 · 9月16日 02:40

**「背景信息」** DeepSeek Harness 是 DeepSeek 于 2026 年 8 月发布的开源 AI 编程代理运行时，发布后数周内在 GitHub 上累计约 21.5 万星标。2026 年 9 月，研究人员公开了其中的高危漏洞 CVE-2026-82533（CVSS 9.4），该漏洞允许沙箱内的代理通过调用工具的本地 Web 界面来关闭自身文件沙箱并绕过审批提示。本文介绍的研究（关联编号 QVD-2026-52646）聚焦于该运行时中的动态插件沙箱逃逸，追踪泄露的 exec.agent.ctx 对象来源及其设计成因。

**「影响」** 对于在 DeepSeek Harness 中运行动态插件、依赖其沙箱隔离子代理或任意代码的用户，最直接的后果是这一安全前提被打破：QVD-2026-52646 被证实可利用泄漏的 exec.agent.ctx 对象在插件沙箱内执行命令，使沙箱边界形同虚设，且 Ox Security 独立披露的同类逃逸路径可扩大到

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/PencilDaydream/-exec-DeepSeek-Harness-QVD-2026-52646-/tree/main">GitHub - PencilDaydream/-exec-DeepSeek-Harness-QVD-2026-52646 ...</a></li>
<li><a href="https://labs.cloudsecurityalliance.org/research/csa-research-note-deepseek-harness-sandbox-escape-20260910-c/">DeepSeek Harness Sandbox Escape and Agent Containment</a></li>
<li><a href="https://qpulse.quasarcybertech.com/news/5670/deepseek-harness-sandbox-escape-vulnerability-cve-2026-82533-allows-unauthenticated-session-hijacking">DeepSeek Harness Sandbox Escape Vulnerability (CVE-2026-82533 ...</a></li>
<li><a href="https://github.com/PencilDaydream/-exec-DeepSeek-Harness-QVD-2026-52646-">GitHub - PencilDaydream/-exec-DeepSeek-Harness-QVD-2026-52646 ...</a></li>
<li><a href="https://devops.com/flaw-in-deepseek-harness-ai-coding-tool-let-agents-disable-their-sandbox/">Flaw in DeepSeek Harness AI Coding Tool Let Agents Disable ...</a></li>

</ul>
</details>

**标签**: `#security`, `#sandbox-escape`, `#vulnerability`, `#DeepSeek`, `#AI-systems`

---

<a id="item-tech-news-9"></a>
### [Datasette 0.65.5 修复权限绕过安全漏洞](https://simonwillison.net/2026/Sep/16/datasette-2/) ⭐️ 7.0/10

Datasette 0.65.5 已发布，修复了一个安全漏洞：在请求表名时，尾随换行符可以绕过表级权限，从而暴露私有行数据。该漏洞由 dpfkdlemtp 报告，编号为 GHSA-h547-rmjf-5m2m。此次发布为补丁版本，主要面向依赖表权限保护数据的用户，建议他们立即升级以消除访问控制绕过风险。

rss · Simon Willison · 9月16日 23:51

**「背景」** Datasette 是一个开源的探索与发布数据工具，允许用户对表和行实施细粒度的权限控制。攻击者通过在请求的表名末尾添加换行符，可能导致权限检查中的表名匹配异常，进而绕过既有的访问限制。

**「影响」** 对于使用 Datasette 表级权限保护私有数据的用户，此漏洞可能导致未经授权的行数据泄露，因此应尽快升级至 0.65.5 版本。

**标签**: `#security`, `#datasette`, `#patch`, `#vulnerability`, `#access control`

---

<a id="item-tech-news-10"></a>
### [LARA：冻结 LLM 的轻量可组合行为适配](https://www.reddit.com/r/MachineLearning/comments/1whx9tr/lara_small_composable_behaviours_for_frozen_llms_p/) ⭐️ 7.0/10

LARA（轻量级加性残差自适应）为冻结语言模型引入了一种低秩残差适配方法，通过训练残差适配器而非修改模型权重，使多个行为可以在推理时加载、移除、混合或路由。该方法提出了混合行为（Mixture of Behaviors, MoBs）路由器，让单一冻结模型能够逐令牌地选择或组合多个独立训练的行为，例如编码、数学、医疗和摘要，从而免去为每个任务保留单独适配模型的需要。该项目已发布可用的 PyTorch 库，包含训练代码、示例和论文复现说明，并附带与 LoRA 的对比以及基于海明威、菲茨杰拉德和格特鲁德·斯坦写作风格的演示。这一方案将模型的后期训练模块化，提升了灵活性和资源效率，但尚属研究公告，未有独立验证。

reddit · r/MachineLearning · /u/kertara · 9月16日 13:28

**「背景」** 传统上，适配大型语言模型通常需要微调整个模型或采用低秩适配方法（如 LoRA）修改权重，且不同任务往往需要保存单独的适配器或模型副本。LARA 则另辟蹊径，在选定层上训练轻量残差适配器，并将每种行为作为独立的小模块保存，从而在推理时灵活组合，无需改动原始冻结模型。

**「影响」** 对于需要在同一基础模型上部署多种任务能力的开发者，LARA 支持将多个适配行为合并进一个模型，从而减少存储和切换多个独立模型的开销，并实现实时任务组合。

**标签**: `#LLM adaptation`, `#LoRA`, `#modular AI`, `#PyTorch`, `#machine learning research`

---

<a id="item-tech-news-11"></a>
### [阶跃星辰发布 StepAudio 3 Music 音乐生成模型](https://static.stepfun.com/blog/stepaudio3/music/) ⭐️ 7.0/10

阶跃星辰发布 AI 音乐生成模型 StepAudio 3 Music，用户只需用自然语言描述风格、人声、情绪、乐器、调性与速度，即可生成完整的 48 kHz 立体声歌曲。该模型采用 MoE 架构与 AR + DiT 生成范式，并通过名为 ABC-COT 的技术先将自然语言创作意图转化为歌曲结构规划，再逐段生成音乐。官方称其在 Audiobox 与 MuQ-Similarity 两项音频评测中均取得 SOTA（当前最优）结果，兼顾音乐质量与可控性。模型主要面向短视频配乐、词曲 Demo 与游戏主题曲等实际创作场景。

telegram · zaihuapd · 9月16日 08:48

**「背景」** AI 音乐生成是指通过模型根据文本或音符等输入自动创作旋律、和声与编曲的技术，此前多数模型侧重单轨旋律或较短片段，难以稳定把控整首歌的结构与多轨编排。阶跃星辰此前的 StepAudio 系列已在语音与音频生成领域有所积累，本次 StepAudio 3 Music 将重点放到“完整歌曲”的生成上，把歌词、编曲与结构规划纳入同一流程。

**「影响」** 对短视频创作者、独立词曲作者和游戏开发者而言，他们可直接用自然语言描述快速产出结构完整的 48 kHz 立体声歌曲，显著降低配乐与 Demo 制作的门槛。

**标签**: `#ai-music-generation`, `#machine-learning`, `#multi-modal-ai`, `#model-architecture`, `#audio-ai`

---

<a id="item-tech-news-12"></a>
### [新浪云 SAE 永久下线，早期 B 站 420TB 数据濒危](https://tracker.archiveteam.org/sinavideo/#show-all) ⭐️ 7.0/10

新浪云 SAE 将于 2026 年 9 月 16 日 24 时永久下线，所有用户数据将被彻底删除。该平台作为国内首个 PaaS 云平台于 2009 年上线，早期 B 站曾依赖其存储大量视频源文件，目前仍有约 420 TB 历史数据存于新浪云 S3 桶中。Archive Team 发起分布式归档项目，已累计抢救约 680 TB 数据，完成度达 96.26%。这意味着约 3.74% 的历史数据（约 15.7 TB）可能无法恢复，数亿条早期视频资源将面临永久消失。

telegram · zaihuapd · 9月16日 15:00

**「背景」** 新浪云 SAE（Sina App Engine）是新浪于 2009 年推出的国内首个 PaaS 平台，凭借低成本、免运维特性吸引大量开发者。早期 B 站因自身存储能力有限，将视频源文件托管于新浪云的存储服务中，形成约 420 TB 的历史数据积累。Archive Team 是一个专门抢救互联网数据的志愿者组织，通过分布式爬虫和下载任务尽可能在服务关闭前保存数据。

**「影响」** 对于依赖早期 B 站视频资源的创作者、研究者及历史数据归档机构，此次下线将导致约 15.7 TB（=420×3.74%）的未归档数据永久丢失，对应部分早期 B 站视频将无法在互联网上恢复。同时，所有曾使用新浪云 SAE 的开发者及其应用数据也将全部灭失，可能影响众多已依赖该平台运行的旧应用。

**标签**: `#cloud computing`, `#data preservation`, `#archive team`, `#bilibili`, `#sae`

---