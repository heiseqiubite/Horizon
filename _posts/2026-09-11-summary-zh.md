---
layout: default
title: "Horizon Summary: 2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 45 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [零点击微信蠕虫 WeWorm 发布](#item-tech-news-1) ⭐️ 9.0/10
2. [Shopify 放弃 React Native，转向 Swift 和 Kotlin](#item-tech-news-2) ⭐️ 8.0/10
3. [微软将 Rust 列为一级语言](#item-tech-news-3) ⭐️ 8.0/10
4. [Web 缓存欺骗:URL 规范化错位下的 13 种变体验证](#item-tech-news-4) ⭐️ 8.0/10
5. [LangFlow 授权绕过漏洞可致任意 npm/PyPI 包执行](#item-tech-news-5) ⭐️ 8.0/10
6. [vLLM 资源耗尽漏洞 CVE-2026-71486 影响 0.26.0 之前版本](#item-tech-news-6) ⭐️ 8.0/10
7. [HN 精选：DeepSeek V4.1-Flash 发布与 Shopify 回归原生](#item-tech-news-7) ⭐️ 8.0/10
8. [数据中心表后供电为何如此困难（第一部分）](#item-tech-news-8) ⭐️ 8.0/10
9. [DeepSeek 发布 V4.1 Flash：552B 参数新架构](#item-tech-news-9) ⭐️ 8.0/10
10. [腾讯混元发布开源音频编辑模型 AuK](#item-tech-news-10) ⭐️ 8.0/10
11. [武器化 Windows Defender 修复驱动为内核攻击原语](#item-tech-news-11) ⭐️ 8.0/10
12. [研究人员能否信任 OpenAI 处理未发表数学成果](#item-tech-news-12) ⭐️ 7.0/10
13. [PlanetScale 发布分片 Postgres 产品 Neki 引发争议](#item-tech-news-13) ⭐️ 7.0/10
14. [内网 LLM API 流量纯流量侧识别检测实测](#item-tech-news-14) ⭐️ 7.0/10
15. [trynix.dev：浏览器中运行任意 Nix 包](#item-tech-news-15) ⭐️ 7.0/10
16. [真实果蝇连接组学玩 Pong 失败，审计比成功更有价值](#item-tech-news-16) ⭐️ 7.0/10
17. [蚂蚁国际联合 Visa、Mastercard 制定 AI 代理支付标准](#item-tech-news-17) ⭐️ 7.0/10
18. [DeepSelect v1.0.0：面向 DSA 与采样器的 TopK 内核库](#item-tech-news-18) ⭐️ 7.0/10
19. [HBM 短缺推高中国 AI 芯片价格](#item-tech-news-19) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [零点击微信蠕虫 WeWorm 发布](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research 于 2026 年 9 月发布 WeWorm 演示，宣称这是首个能够通过微信通话在 iOS 和 Android 设备间传播的零点击蠕虫。受害者无需接听电话或以任何方式与手机交互，即使接听也听不到任何声音，漏洞利用依然成功。研究团队借助 AI 在约两天内发现漏洞并编写出首个远程代码执行（RCE）漏洞利用，构建蠕虫又花了一周时间。团队表示，此前此类规模的蠕虫通常需要更大规模的团队耗时数月完成，而 AI 已经能承担大部分工作，他们的角色在于判断攻击目标与安全测试方式。这一成果凸显了 AI 在漏洞发现与漏洞利用开发中的加速作用，对移动安全与 AI 安全研究具有深远影响。

rss · Simon Willison · 9月10日 00:56

**「背景」** 零点击（zero-click）漏洞利用指无需受害者进行任何交互（例如接听电话或点击链接）即可触发的攻击，而蠕虫（worm）则是能自我复制并在设备或账号之间传播的恶意程序。总部位于加利福尼亚州的安全公司 Calif 宣布，其团队借助 AI 在约两天内发现漏洞并写出了首个远程代码执行（RCE）利用，再用约一周完成蠕虫构建；该公司的演示显示，WeWorm 仅通过一次微信来电即可在 iPhone 和 Android 设备上接管对方账号，受害者无需接听或触碰手机，且已在三台测试手机上验证了传播。此前这类规模的攻击研究通常需要更大的团队耗时数月才能完成，因此该成果被视为 AI 加速漏洞挖掘与利用开发的一个重要标志性案例。

**「影响」** 对 iOS 和 Android 平台上的微信用户而言，这证实了存在无需任何交互即可被远程攻破的潜在风险；对安全研究者与平台开发者而言，它提供了 AI 显著缩短漏洞利用开发周期的具体实例，并促使行业重新评估 AI 辅助攻击的实际门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm – First 0-Click Worm Spreading Through WeChat Calls ...</a></li>
<li><a href="https://www.heise.de/en/news/WeWorm-Zero-click-worm-could-have-taken-over-all-WeChat-accounts-11445510.html">&quot;WeWorm&quot;: Zero-click worm could have taken over all WeChat accounts | heise online</a></li>
<li><a href="https://thehackernews.com/2026/09/wechat-zero-click-worm-took-over.html">WeChat Zero-Click Worm Took Over Accounts on iPhone and Android via Incoming Calls</a></li>

</ul>
</details>

**标签**: `#zero-click exploit`, `#AI security research`, `#RCE`, `#mobile security`, `#worm`

---

<a id="item-tech-news-2"></a>
### [Shopify 放弃 React Native，转向 Swift 和 Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 宣布放弃 React Native，改为使用原生 Swift（iOS）和 Kotlin（Android）构建应用，这是移动开发领域一项具有广泛影响的大型商业决策。Shopify 工程团队表示，LLM（大语言模型）改变了其 2020 年选择 React Native 时所依赖的核心假设，因此公司决定重新评估并推翻原有技术路线。这一消息在 Hacker News 上引发高度关注，获得 735 分和 490 条评论，讨论焦点包括 LLM 辅助迁移的可行性与成本问题。Shopify 官方在工程博客中提供了详细的技术理由，但尚未披露具体的迁移时间表、涉及的应用规模或性能对比数据。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**「背景信息」** Shopify 于 2020 年将移动应用从原生框架迁移至 React Native，其动机有三：避免重复构建相同功能、允许开发者跨技术栈协作、减少在功能一致性上耗费的时间。如今公司宣布回归原生方案，理由是编码智能体（coding agents）改变了构建移动应用的成本结构，使得分别用 Swift 和 Kotlin 开发两套原生应用比维护单一 React Native 代码库更为经济。

**「影响」** 作为 React Native 最知名的大规模采用者之一，Shopify 回归原生 Swift 与 Kotlin 的决定削弱了该跨平台框架的一个关键背书，并可能促使其他团队重新评估跨平台方案的长期成本效益，因为官方明确将 LLM 降低原生迁移成本列为重新评估的核心原因。

**「社区讨论」** 多数开发者对 Shopify 的决定表示认同，尤其是有 iOS 工程师提到自己长期面对管理层提倡共享代码库的压力，如今感到“被验证”。但在 LLM 的作用上存在分歧：有评论者分享用 AI 辅助一夜之间完成中小型应用迁移的经历，也有人指出自己在无 LLM 辅助的情况下早已完成类似的 React Native 到原生应用的迁移，认为“LLM 让原本过于昂贵的迁移变得可行”这一叙事并不准确。作者 fnthawar2 回应称，LLM 改变了其 2020 年决策背后的一个核心假设，因此公司选择重新审视当初的判断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://simonwillison.net/2026/Sep/10/shopify-react-native/">Native is now the future of mobile at Shopify</a></li>
<li><a href="https://ebusexpert.com/case-studies/shopify-moves-back-to-native-from-react-native/">Shopify Moves Back To Native From React Native - E BusExpert</a></li>
<li><a href="https://news.ycombinator.com/item?id=49643982">Shopify moves back to Native from React Native | Hacker News</a></li>

</ul>
</details>

**标签**: `#React Native`, `#Swift`, `#Kotlin`, `#mobile development`, `#cross-platform`

---

<a id="item-tech-news-3"></a>
### [微软将 Rust 列为一级语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

微软正式宣布将 Rust 列为一级（tier-1）编程语言，这标志着 Rust 在企业级采用进程中的一个重大里程碑，也是科技巨头对 Rust 的一次强有力背书。一级地位意味着 Rust 在微软的编译工具链、平台支持与内部工程实践中将获得与 C/C++ 相当的一流待遇。此举主要源于 Rust 的内存安全设计，有望帮助微软改善那个长期受内存安全漏洞（约占其常见漏洞与暴露 CVE 的 70%）困扰的巨大产品组合。该决定对软件工程实践、工具链生态以及 Rust 在企业界的进一步普及都具有深远影响。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**「背景」** “一级语言（tier-1）”是微软内部对编程语言支持级别的工程认定，代表公司将为该语言提供从本地开发到生产环境的完整支持路径，包括安全的工具链构建、高效的开发者工具、质量工作流、深度平台集成和合规保障。Rust 以内存安全设计著称，在微软内部长期被视作替代 C/C++ 进行新项目开发的重要选择，尤其有助于降低因内存安全问题导致的大量常见漏洞。这一宣布标志着 Rust 从试验性采用走向官方基础设施级支持。

**「影响」** 对微软内部及更广泛的企业开发者而言，Rust 晋级一级语言意味着其在编译工具链、平台支持和内部标准中获得与 C/C++ 同级的一流待遇，将显著加速 Rust 在大型企业软件与系统编程领域的采用。

**「社区讨论」** 多位评论者认为这一里程碑表明 Rust 已经成熟，是 C++ 和 C\# 的有力竞争者，而不再是快速变动、容易破坏兼容性的新生语言；有五年 Rust 开发经验的从业者表示，在高级应用开发领域已看不到比 Rust 更好的技术选项。同时也有评论提到微软借助自动化工具在 2030 年前将 10 亿行 C 代码转换为 Rust 的雄心目标、DARPA 的相关自动化转换工作，以及 MSVC 工具链集成的传闻，但对这些目标的可行性仍持观望态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#programming languages`, `#software engineering`, `#industry adoption`

---

<a id="item-tech-news-4"></a>
### [Web 缓存欺骗:URL 规范化错位下的 13 种变体验证](https://xz.aliyun.com/news/92808) ⭐️ 8.0/10

该文提出 Web 缓存欺骗（WCD）的本质并非“缓存”本身，而是 URL 规范化错位：浏览器原样发送 URL，CDN 仅凭字符串外观判定缓存，源站却做宽容的归一化处理，三方对同一 URL 各有一套解释，导致私有响应落入公共缓存。文章穷举出 \`;.css\`、\`.css\`、URL 编码、大小写、双斜杠、query 后缀等 13 个攻击变体，并采用 Express + Nginx 真实组件进行交叉验证，随后通过四组对照实验测量各层修复方案的实际效果。分析指出，具体哪些变体能够奏效、各层修复覆盖了哪些场景，是这项研究落地时最需要关注的结论，但该文的相关细节在原文中未完整展开。

rss · 先知社区 · 9月10日 05:09

**「攻击原理与前置概念」** Web Cache Deception（网页缓存欺骗）是一种攻击手法：攻击者构造一个貌似静态资源（如以 .css、.js 等后缀或 /resources 这类静态目录规则命中）的 URL，欺骗 CDN 或反向代理认为请求可以公开缓存，从而把本应私有的响应（如个人资料页）存入公共缓存，其他用户即可读取。其根因在于浏览器、缓存服务器与源站对同一个 URL 的规范化（normalization）处理不一致，典型差异包括路径遍历中的点段（dot-segment）是否解码与解析、URL 编码方式，以及路径分隔符（如 ? 或 ;）的判定，攻击者正是利用这些错位让缓存规则与源站逻辑得出不同结论。

**「影响」** 凡是在 CDN 或反向代理后部署 Express/Nginx 且依赖字符串前缀（如 \`.css\`）判定缓存的服务，若缺乏统一的 URL 规范化与严格的缓存键约束，就存在将登录态或私有页面写入公共缓存而被他人读取的风险；由于源文未给出各修复项与 13 种变体之间的完整对应关系，具体防护效果仍存在不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/web-security/web-cache-deception">Web cache deception | Web Security Academy</a></li>
<li><a href="https://portswigger.net/web-security/web-cache-deception/lab-wcd-exploiting-cache-server-normalization">Lab: Exploiting cache server normalization for web cache deception | Web Security Academy</a></li>
<li><a href="https://portswigger.net/web-security/web-cache-deception/lab-wcd-exploiting-origin-server-normalization">Lab: Exploiting origin server normalization for web cache deception | Web Security Academy</a></li>

</ul>
</details>

**标签**: `#security`, `#web cache deception`, `#URL normalization`, `#CDN`, `#vulnerability`

---

<a id="item-tech-news-5"></a>
### [LangFlow 授权绕过漏洞可致任意 npm/PyPI 包执行](https://xz.aliyun.com/news/92807) ⭐️ 8.0/10

LangFlow 存在一项授权绕过漏洞，其 MCP stdio 服务器配置中的授权检查仅部署于 REST 层，无法保护其他访问路径。攻击者可经流程图组件参数路径完全绕过该授权校验，从而在服务端环境中执行任意 npm/PyPI 软件包代码。由于 LangFlow 是广泛使用的 AI 工作流编排工具，该漏洞对人工智能基础设施与软件供应链安全构成严重风险，实际影响取决于运行环境的暴露面与配置。本披露来自先知社区，信息较为有限，未给出具体受影响版本与修复版本，建议相关部署者审查 MCP stdio 服务器配置及流程图组件参数的可信来源。

rss · 先知社区 · 9月10日 04:47

**「背景」** LangFlow 是一个开源的低代码 AI 工作流编排平台，用户可通过可视化流程（flow）组件连接模型、工具与数据源。MCP（Model Context Protocol）是 Anthropic 提出的协议，用于让 AI 应用调用外部工具，其中 stdio 传输方式会把 MCP 服务器的配置与工具调用逻辑直接映射为操作系统级命令执行，因此一旦被滥用就可能转化为任意命令执行。本次披露的漏洞（CVE-2026-12940）正是源于 LangFlow 对 MCP stdio 服务器配置的授权检查仅部署在 REST API 层，攻击者可通过流程组件参数路径绕过该检查，从而以 LangFlow 服务账户身份执行任意命令，并可能读取数据库中的全部机密与流程数据。

**「影响」** 对于将 LangFlow 实例部署于可访问网络、且未封闭相关 REST/构建端点的用户，这一漏洞意味着实际可远程利用的任意代码执行风险：MCP stdio 服务器配置中的授权校验仅存在于 REST 层，可经流程组件参数路径被完全绕过，导致攻击者在服务器上执行任意 npm/PyPI 包。同类 LangFlow RCE 缺陷已证实可在野外被利用且 CVSS 评级为 9.8（CVE-2026-0768），CVE-2026-33017 亦允许通过未认证的 build\_public\_tmp 端点请求执行任意 Python 代码，表明该风险并非纯理论性的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/BiiTts/CVE-2026-12940-Langflow-Unauth-RCE">GitHub - BiiTts/CVE-2026-12940- Langflow -Unauth-RCE...</a></li>
<li><a href="https://www.linkedin.com/pulse/anthropics-model-context-protocol-mcp-langflow-have-chain-taxiarchis-5rgwe">Anthropic’s Model Context Protocol ( MCP ) and LangFlow have...</a></li>
<li><a href="https://github.com/EQSTLab/CVE-2026-33017">GitHub - EQSTLab/CVE-2026-33017: Langflow RCE</a></li>
<li><a href="https://threatprotect.qualys.com/2026/09/02/langflow-remote-code-execution-vulnerability-exploited-in-attacks-cve-2026-0768/">Langflow Remote Code Execution Vulnerability Exploited in ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#langflow`, `#AI infrastructure`, `#RCE`

---

<a id="item-tech-news-6"></a>
### [vLLM 资源耗尽漏洞 CVE-2026-71486 影响 0.26.0 之前版本](https://xz.aliyun.com/news/92805) ⭐️ 8.0/10

vLLM 在 0.26.0 之前的两个 derender 端点存在资源耗尽漏洞（CVE-2026-71486）：端点会在资源边界校验前接受调用方提交的嵌套 GenerateResponse，并执行去分词、logprob 处理和 OpenAI 兼容响应构造。拥有相应 API 权限的客户端可利用格式合法但规模异常的 JSON，与同服务上的其他请求竞争 CPU、内存、响应缓冲与带宽，造成拒绝服务。鉴于 vLLM 被广泛用于 LLM 推理服务，该漏洞对依赖其部署的 AI 系统构成实际风险，受影响用户宜升级至 0.26.0 及以上版本。

rss · 先知社区 · 9月10日 02:17

**「漏洞背景」** vLLM 是一个被广泛部署于生产环境的大语言模型（LLM）推理与服务框架，它通过统一的 API 端点处理模型加载、请求调度和响应构造，其中 derender 端点是负责解析调用方提交数据的入口。CVE-2026-71486 影响 vLLM 0.26.0 之前的所有版本，由于端点会在资源边界校验之前执行去分词、logprob 处理和 OpenAI 兼容响应构造，攻击者可通过提交格式合法但规模异常的嵌套 GenerateResponse 结构来消耗服务资源；官方给出的修复方案是升级到 0.26.0 或更高版本。

**「影响」** 对于运行 vLLM 0.26.0 之前版本、暴露了 /v1/completions/derender 和 /v1/chat/completions/derender 端点的服务，拥有相应 API 访问权限（低权限）的客户端提交格式合法但规模异常的嵌套 GenerateResponse，可在资源边界校验之前消耗 CPU、内存、响应缓冲和带宽，拖慢同一服务上的其他推理请求；该漏洞的 CVSS 评分为 4.3，被归类为低严重性拒绝服务，且只影响可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cvefeed.io/vuln/detail/CVE-2026-71486">CVE - 2026 - 71486 - vLLM : Derender endpoints decode caller-supplied...</a></li>
<li><a href="https://cvereports.com/reports/CVE-2026-71486">CVE-2026-71486: CVE-2026-71486: Uncontrolled Resource Consumption in vLLM Derender Endpoints | CVEReports</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#安全漏洞`, `#CVE`, `#拒绝服务`, `#AI推理`

---

<a id="item-tech-news-7"></a>
### [HN 精选：DeepSeek V4.1-Flash 发布与 Shopify 回归原生](https://zeli.app/zh/digest/2026-09-10) ⭐️ 8.0/10

DeepSeek 正式发布 DeepSeek-V4.1-Flash，这是其新架构家族中最小的模型，原生支持视觉理解，采用非对称 MoE 结构，总参数 552B，但推理时仅激活约 8B 输入与 16B 输出参数。相比上一代，V4.1-Flash 将 KV cache 的 HBM 占用降至 1/4、SSD 存储降至 1/8，目前已上线 API 并宣布降价，同时计划开源权重以支持社区部署。同日另一大新闻是 Shopify 宣布放弃 React Native、回归原生 Swift/Kotlin 开发，理由是 AI Agent 让双端开发不再等于双倍成本，并借助 Helix 系统保障代码质量。其他热点包括数学家 Andreas Thom 指控 OpenAI 潜在使用其未发表数学成果、Microsoft 将 Rust 提升为一级语言（推出 rustc\_codegen\_utc 对接 MSVC 后端），以及 Automattic 董事会强制 CEO Matt Mullenweg 带薪休假。

rss · Zeli · 9月10日 23:59

**「背景」** DeepSeek 以压缩推理成本见长，非对称 MoE 架构将输入与输出的激活参数分开处理，配合 KV cache 的内存优化，可在保持能力的同时显著压低显存与存储开销。Shopify 于 2020 年全面投入 React Native，认定跨平台能节省成本；而 LLM 爆发后这一假设被改写——借助 AI Agent 自动迁移代码，双端原生开发不再意味着双倍成本。

**「影响」** 对 AI/ML 工程团队而言，V4.1-Flash 的降价与大幅缩减的 KV cache 占用直接降低了推理与部署成本，计划中的开源权重则将支持社区自托管；Shopify 的迁移案例也表明 AI Agent 正在改写跨平台开发的经济模型。

**标签**: `#AI models`, `#DeepSeek`, `#LLM efficiency`, `#mobile development`, `#software engineering`

---

<a id="item-tech-news-8"></a>
### [数据中心表后供电为何如此困难（第一部分）](https://newsletter.semianalysis.com/p/what-is-so-hard-about-behind-the) ⭐️ 8.0/10

本文是分析师 Ellie Holbrook 在 SemiAnalysis 发表的系列技术分析的第一部分，聚焦数据中心自备（表后）供电在工程、监管和经济层面遇到的障碍，这一议题直接关系到 AI 基础设施建设面临的能源瓶颈。文章以“Dumb Science Experiments vs. Money Printing Machines”的短评作为引子，表明其讨论重心是实际部署与资本回报，而非实验室级别的技术设想。由于当前可见内容仅为导语，文中尚未给出具体的容量数字、设备型号、成本数据或时间表，相关细节有待该系列的后续部分补充。

rss · Semianalysis · 9月10日 14:28

**「背景知识」** 后台电力（behind-the-meter power，即位于电网电表之后、由数据中心自行发电的供电方式）不同于从公共电网购电，其核心形式包括燃气轮机、电池储能和现场可再生能源。这种供电模式之所以重要，是因为美国电网容量与新数据中心的总电力需求之间存在明显缺口；SemiAnalysis 此前预测，到 2028 年美国将有超过 40GW 的后台式数据中心容量，占当年新增数据中心的一半以上，到 2029 年相关设备市场规模将超过每年 50GW。理解这一背景，有助于把握本文所讨论的后台供电技术难点的缘由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/us-grid-constraints-towards-40gw">US Grid Constraints: Towards 40GW+ of Behind-The-Meter ...</a></li>
<li><a href="https://aiweekly.co/alerts/semianalysis-40gw-of-behind-the-meter-us-datacenters-by-2028">SemiAnalysis: 40GW+ of behind-the-meter US datacenters by ...</a></li>

</ul>
</details>

**标签**: `#datacenters`, `#power infrastructure`, `#AI infrastructure`, `#energy`, `#technology analysis`

---

<a id="item-tech-news-9"></a>
### [DeepSeek 发布 V4.1 Flash：552B 参数新架构](https://mp.weixin.qq.com/s/qg0NU3NNUbp1co2PdkAPAg) ⭐️ 8.0/10

DeepSeek 正式发布 V4.1 Flash，这是全新模型结构系列中尺寸最小的模型。该模型采用 552B 参数的 Causal-Encoder-Decoder 架构，输入与输出激活量分别为 8B 和 16B，并原生支持多模态视觉理解。模型已上线 DeepSeek API，模型名为 deepseek-flash；新价格于 2026 年 9 月 10 日 12:00 生效，9 月 14 日 12:00 后 deepseek-v4-pro 请求将自动路由至 V4.1 Flash 并按新价格计费。本次公告来自转载的 Telegram 消息，内容简短，未附带基准测试结果或独立验证数据。

telegram · zaihuapd · 9月10日 05:54

**「背景知识」** DeepSeek 的模型线中，「Pro」与「Flash」分别对应面向复杂任务的高性能大模型和面向高频、低成本场景的小尺寸模型，前者以 deepseek-v4-pro 为名提供 API 服务。V4.1 Flash 采用 Causal-Encoder-Decoder 结构，融合了传统编码器-解码器与因果（仅解码器）架构的特点，并以稀疏激活方式运行——552B 参数中每次推理仅激活部分参数（输入激活 8B、输出激活 16B），从而在保持能力的同时降低算力成本。该模型是官方「新架构家族」中尺寸最小的成员，原生支持多模态视觉理解，并已上线 API（模型名 deepseek-flash）。

**「主要影响」** V4.1 Flash 以每百万 token 低于 1 美分的定价掀起新一轮大模型价格战，直接加大对 OpenAI、Anthropic 及众多中国 AI 厂商的价格压力。市场反应已经显现：MiniMax 和 Z.ai 股价跌幅超过 8%，反映市场对 DeepSeek 定价策略压缩中国 AI 行业利润率的担忧，香港 AI 概念股以及存储芯片厂商 SK 海力士、美光股价亦随之下滑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/updates/">Change Log | DeepSeek API Docs</a></li>
<li><a href="https://www.deepseek.com/en/news/deepseek-v4-1-flash/">DeepSeek | Introducing DeepSeek-V4.1-Flash: smarter, faster, more efficient.</a></li>
<li><a href="https://technode.com/2026/09/10/deepseek-formally-launches-v4-1-flash-routes-v4-pro-requests-to-flash/">DeepSeek formally launches V4.1 Flash, routes V4 Pro requests to Flash · TechNode</a></li>
<li><a href="https://www.storyboard18.com/digital/deepseek-v4-1-flash-deepens-ai-price-war-with-anthropic-openai-110369.htm">DeepSeek V4.1 flash deepens AI price war with Anthropic, OpenAI - Storyboard18</a></li>
<li><a href="https://cryptobriefing.com/deepseek-v4-flash-low-cost-ai-model/">DeepSeek rolls out low-cost AI model to challenge rivals</a></li>
<li><a href="https://www.briefs.co/news/deepseek-s-v4-1-flash-cranks-up-the-ai-price-war-charging-un/">DeepSeek V4.1 Flash ignites AI price war under 1¢/M</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI Model Release`, `#Multimodal`, `#Sparse Activation`, `#API Pricing`

---

<a id="item-tech-news-10"></a>
### [腾讯混元发布开源音频编辑模型 AuK](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 8.0/10

腾讯混元正式发布开源音频编辑模型 AuK，该模型可通过自然语言指令与参考音频统一完成语音生成与编辑任务，具体支持零样本文本转语音、音色/风格/情绪编辑、去口音以及多人语音分离等功能。同期发布的 AuK-Flash 采用 4 步推理，在匹配条件下推理速度约提升 4.5 倍。目前该项目的代码、模型权重和演示均已上线，供开发者直接使用。

telegram · zaihuapd · 9月10日 11:56

**「背景」** 语音处理工具长期处于碎片化状态，文本转语音、去噪、人声分离、音色或情感编辑等任务通常需要多个专用模型分别完成，缺乏统一的开源方案。AuK 是腾讯混元团队于 2025 年 9 月开源的 1.5B 参数语音基础模型，基于约 30.31 亿条指令-音频实例和 195 万小时有效监督数据训练，覆盖语音生成、内容编辑等五大任务族。该模型通过“自然语言指令加参考音频”的统一接口，将语音生成与编辑能力合并到单一模型中，代表了开源语音工具从分散走向整合的技术路线。

**「影响」** 对于从事语音生成、音频编辑及口音归一化相关开发的工程师和研究者，这一开源模型可在无需微调的情况下覆盖多项音频处理任务，而 AuK-Flash 提供的约 4.5 倍速度提升则更适合对推理延迟敏感的应用场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Tencent-Hunyuan/AuK">GitHub - Tencent-Hunyuan/AuK: AuK: An Open-Source ...</a></li>
<li><a href="https://arxiv.org/abs/2609.08936">[2609.08936] AuK Technical Report: An Open-Source ...</a></li>
<li><a href="https://www.aimodeling.com/en/news/slug/tencent-hunyuan-auk-speech-editing">AuK: Tencent&#x27;s Open 1.5B Speech Generation and Editing Model</a></li>

</ul>
</details>

**标签**: `#audio editing`, `#open source`, `#speech synthesis`, `#Tencent Hunyuan`, `#AI model release`

---

<a id="item-tech-news-11"></a>
### [武器化 Windows Defender 修复驱动为内核攻击原语](https://twitter.com/CyberWarship/status/tweet-2097980655980204356) ⭐️ 8.0/10

Check Point Research 公布了一项名为 &quot;BTR Reforged&quot; 的安全研究成果，将 Windows Defender 的修复驱动程序（remediation driver）武器化为一种内核操作原语。该发现由安全研究员 Florian Hansemann 通过 Twitter 推文对外宣布，并附带了指向完整研究报告的链接。这项技术展示了如何将受信任的 Windows 系统组件转变为潜在的内核攻击面，对安全社区具有较高价值，既可能被攻击者用于内核级利用，也能帮助防御者识别并缓解相关风险。研究同时涉及红队与蓝队视角，具体技术细节和影响范围仍以官方报告为准。

twitter · Florian Hansemann · 9月10日 09:29

**「背景」** Windows 依赖带微软签名的内核驱动以最高权限（Ring 0）执行系统维护操作，BTR.sys 就是其中一个用于修复和清理的官方驱动程序。Check Point 研究人员发现，仅凭管理员账户与 SeLoadDriverPrivilege 权限即可加载这一合法签名的驱动，并让它代为执行任意的内核级文件和注册表操作，全程无需利用漏洞、内存破坏或编写自己的驱动。这种方式属于“自带易受攻击驱动”（BYOVD）类技术的变体，关键在于借助微软自家的合法签名驱动绕过了驱动签名校验，为后续绕过或禁用安全机制提供了基础。

**「影响」** 由于 BTR.sys 是 Windows 的必需组件，微软无法将其加入漏洞驱动阻止列表或通过 WDAC 阻止，攻击者因而可利用这一内核级文件与注册表操作能力关闭 Tamper Protection 和 EDR 配置、写入 Run 键或服务项以建立持久化，而防御方在不破坏 Defender 本身的情况下几乎没有可用的缓解手段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.checkpoint.com/2026/btr-reforged-weaponizing-defenders-remediation-driver-as-a-kernel-operation-primitive/">BTR Reforged : Weaponizing Defender ’s Remediation Driver as...</a></li>
<li><a href="https://thehackernews.com/2026/08/microsoft-defenders-own-driver-can-be.html">Microsoft Defender &#x27;s Own Driver Can Be Weaponized to Delete...</a></li>
<li><a href="https://www.csoonline.com/article/4212929/windows-defenders-own-driver-can-leave-systems-defenseless.html">Windows Defender ’s own driver can leave systems... | CSO Online</a></li>
<li><a href="https://thehackernews.com/2026/08/microsoft-defenders-own-driver-can-be.html">Microsoft Defender &#x27;s Own Driver Can Be Weaponized to Delete...</a></li>
<li><a href="https://www.csoonline.com/article/4212929/windows-defenders-own-driver-can-leave-systems-defenseless.html">Windows Defender ’s own driver can leave systems... | CSO Online</a></li>
<li><a href="https://research.checkpoint.com/2026/btr-reforged-weaponizing-defenders-remediation-driver-as-a-kernel-operation-primitive/">BTR Reforged: Weaponizing Defender ’s Remediation Driver as...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#kernel exploitation`, `#Windows Defender`, `#red team`, `#security research`

---

<a id="item-tech-news-12"></a>
### [研究人员能否信任 OpenAI 处理未发表数学成果](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 7.0/10

一篇在 Hacker News 引发热议（获 627 分、610 条评论）的讨论质疑研究人员能否信任 OpenAI 处理未发表的数学研究，忧虑集中在成果归属、数据污染以及 AI 发现结果的真实性上。讨论源自数学界人士的帖文，指出 OpenAI 邀请研究人员使用其模型（据报道至少为 10 万名研究人员提供免费访问），但内部模型据称在解决开放问题方面进展快得惊人。核心争议在于，研究人员在协作中把新想法与未发表思路提供给模型后，OpenAI 若沿着这些思路发表成果却不作归属，类比于人类合作者将极不道德；同时有研究者担忧未发表输入可能进入预训练数据，使所谓“AI 数学突破”实受训练数据中研究对话影响而非真正独立发现。模型参数规模庞大，理论上可能记住对话中的特定技巧；但也有观点认为，在可验证数学的强化学习与大规模算力下，模型确实可能独立发现与对话中提及技巧无关的超人类解法。整体而言，这一讨论反映了学术界与产业界对 AI 辅助研究信任与完整性的深层忧虑。

hackernews · pred\_ · 9月10日 06:49 · [社区讨论](https://news.ycombinator.com/item?id=49639408)

**「背景」** OpenAI 近期宣称其 AI 模型解决了流体力学领域的纳维-斯托克斯（Navier–Stokes）问题，并称这一数学突破可能竞逐相关奖项，但同时表示无意认领该奖项。在正式宣布前，数学界已有关于该证明来源的传言，争议焦点在于：研究人员在合作中向 OpenAI 的模型提供了未发表的思路，而 OpenAI 在发布成果时未给予相应署名，外界因此质疑其模型是否在预训练中使用了这些未发表内容，以及 AI 生成的解答是否存在真实性与归属不清的问题。

**「影响」** 研究人员若将未发表思路提供给 OpenAI 模型协作，将面临成果被使用却不获归属、输入可能进入训练数据以及“被 AI 抢先发表”的风险，这会动摇研究者参与协作式 AI 问题求解的意愿。

**「社区讨论」** 评论中有观点将 OpenAI 比作人类合作者，指出其沿协作思路发表成果却不归属在人类语境下高度不道德；也有人持两面立场，认为模型既可能因参数规模记住对话细节，也可能在可验证数学的强化学习中独立发现与对话技巧无关的超人类方法；还有评论更广泛地质疑公司保护用户数据动机的可靠性，认为泄露客户数据的惩罚过于轻微。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scientificamerican.com/article/openai-claims-blockbuster-math-breakthrough-amid-swirl-of-controversy/">OpenAI claims blockbuster math breakthrough amid swirl of ...</a></li>
<li><a href="https://www.science.org/content/article/how-ai-math-breakthrough-ignited-controversy">How an AI math breakthrough ignited a controversy - Science</a></li>
<li><a href="https://kingy.ai/blog/navier-stokes-ai-proof-claims-dispute/">OpenAI’s Navier–Stokes Proof Claim: Evidence and Dispute</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#OpenAI`, `#research integrity`, `#machine learning`, `#data privacy`

---

<a id="item-tech-news-13"></a>
### [PlanetScale 发布分片 Postgres 产品 Neki 引发争议](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale 正式推出 Neki，一款基于分片（sharding）架构的 Postgres 托管数据库产品，目标是应对分布式 Postgres 在大规模场景下的扩展性难题。不过，此次发布并未被视为突破性进展，因为市场上已有同类替代方案（如 multigres）存在。发布随即引发争议，焦点集中在产品描述含糊、未能清晰说明 Neki 究竟是什么及其适用场景，以及其闭源定位。社区反馈还指向 CEO 的对外言论造成的摩擦，进一步削弱了外界对该产品的评价。作为分布式数据库工程的一次新尝试，Neki 面临技术价值与公关层面质疑并存的局面。

hackernews · simon\_weber · 9月10日 15:43 · [社区讨论](https://news.ycombinator.com/item?id=49645686)

**「背景」** 分片（sharding）是一种将数据库横向切分到多台服务器、从而突破单机性能瓶颈的技术。Neki 是 PlanetScale 推出的分片 PostgreSQL 托管服务，每个分片都是真正的 PostgreSQL，由路由器、sidecar 和控制平面组成，可支撑数亿 QPS 和 PB 级数据量并保持无停机。PlanetScale 此前以基于 Vitess 的 MySQL 托管服务闻名，Neki 是其向 PostgreSQL 生态的扩展，公司表示在该产品经真实生产环境验证后会将其开源。

**「影响」** 正在评估分布式 Postgres 方案的开发团队将多出一个商业选项，但 PlanetScale 的闭源定位与其此前批评同类开源方案（如 multigres）的态度形成鲜明对照，这可能会促使部分看重开源与透明度的用户转向开源替代品。

**「社区讨论」** 评论者普遍批评发布文章通篇未说明 Neki 是什么及其用途，并质疑其闭源做法与 CEO 先前公开贬低同类开源方案（如 multigres）的态度自相矛盾。另有开发者关注 CAP 定理下的一致性取舍，询问 Neki 如何解决最终一致性对许多负载不适用的问题；也有用户以“连零用户业余项目都需要它”的调侃来表达对可扩展性的疑虑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neki.dev/?ref=upstract.com">Neki | Sharded Postgres by PlanetScale</a></li>
<li><a href="https://planetscale.com/neki">Neki — PlanetScale</a></li>
<li><a href="https://mcpservers.org/agent-skills/planetscale/neki">neki | Agent Skills Library | MCP Servers</a></li>

</ul>
</details>

**标签**: `#postgres`, `#database`, `#sharding`, `#distributed-systems`, `#planetscale`

---

<a id="item-tech-news-14"></a>
### [内网 LLM API 流量纯流量侧识别检测实测](https://xz.aliyun.com/news/92806) ⭐️ 7.0/10

本文实测在不解密 HTTPS、不安装终端插件的情况下，仅从流量侧识别内网 LLM API 调用。作者在隔离网段对照采集 DeepSeek API、Ollama 明文、普通浏览和文件下载流量，从 DNS、SNI、JA3、HTTP、SSE 五层提取特征。使用 Suricata 四道闸门回放混合 pcap，六条告警全部为真阳性，对 12 个主流站点及 pip 安装流量零误报。测试还发现 DoH 仅能绕过 DNS 闸门，而 IP 直连前置代理会使 DNS 和 SNI 检测同时失效。

rss · 先知社区 · 9月10日 03:55

**「背景」** 企业内网中员工或恶意程序可能私自调用外部大模型 API，带来数据泄露和合规风险。传统安全监控依赖 HTTPS 解密或终端代理来识别这类流量，但在加密和隐私约束下这些手段常常不可行，因此需要探索纯流量侧的特征识别方法。

**「影响」** 对于有内网安全监控需求的企业或组织，该方案提供了一条无需解密 HTTPS 的 LLM API 调用检测路径，可显著降低部署门槛和隐私风险；但 DoH 和 IP 直连前置代理等绕过手段提示该方案仍有局限性，需要结合其他安全措施。

**标签**: `#网络安全`, `#LLM API`, `#流量分析`, `#Suricata`, `#入侵检测`

---

<a id="item-tech-news-15"></a>
### [trynix.dev：浏览器中运行任意 Nix 包](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 7.0/10

trynix.dev 允许用户在浏览器中通过 WebAssembly 运行由 qemu-wasm 驱动的 x86\_64 Linux 完整虚拟机，并可在其中交互式启动过去 13 年中任意一个 Nix 包。该工具由 Farid Zakaria 开发，他称之为自己「Nix 工作的代表作」。包以 URL 形式寻址，例如访问 https://trynix.dev/?pkg=python3%403.6.2 并点击「Load」，即可进入运行 2017 年 Python 3.6.2 的交互式 shell 环境。Farid 还在其上构建了 trynix-preview：一个 GitHub Action，会在拉取请求上评论一个链接，让审阅者直接在浏览器中启动该 PR 的构建结果，「无需服务器，只需浏览器」。

rss · Simon Willison · 9月10日 23:44

**「背景」** Nix 是一种以可复现构建为核心理念的包管理器，其包定义和构建产物均强调确定性。qemu-wasm 是一个将 QEMU 模拟器编译为 WebAssembly、使完整操作系统可在浏览器中运行的项目；trynix.dev 将两者结合，使得历史上的 Nix 包能够以原样（包括原有的库和运行时）在浏览器内直接运行。

**「影响」** 对 Nix 开发者而言，该工具显著简化了拉取请求审阅与旧版本环境复现：无需部署任何服务器，仅凭一个链接即可在浏览器中启动 PR 构建或历史包。不过其运行依赖浏览器端的完整系统模拟，性能与原生环境可能存在差距，实际体验有待验证。

**标签**: `#Nix`, `#WebAssembly`, `#virtualization`, `#reproducibility`, `#developer-tools`

---

<a id="item-tech-news-16"></a>
### [真实果蝇连接组学玩 Pong 失败，审计比成功更有价值](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

一位研究者使用真实果蝇连接组 MaleCNS v1.0（166k 个神经元，EM 重建）的子图，通过多巴胺式可塑性驱动其学习玩 Pong（每帧一个二进制命中信号），最终未能学会。审计失败过程发现多个具体问题：neuPrint 正则表达式 bug（全匹配与子串语义混淆）导致两个神经元群体被静默置零；原始神经元选择使光感受器到任何运动检测器无路径，缺少中间层；半数可用的运动神经元没有来自感觉通路的突触（零连接），仅因数组索引被错误分组到“向下挡板”，永远无法激活。重建基于更合理生物学假设（将威胁检测通路替换为求偶追逐中的视觉目标追踪通路）后，假设被数据否定，但最终找到端到端连接的下降神经元，使学习开/关首次产生差异，不过效果表现为学习规则抑制整个系统而非技能提升。此外，检查了流行的 Doom、Minecraft 和 Beat Saber 项目，发现其验证失败（Doom 六次迭代未过验证门）、真实运动检测通路静默（Minecraft）、过拟合单一曲目（Beat Saber）。完整审计细节见 Medium 文章。

reddit · r/MachineLearning · /u/oPeraza2007 · 9月10日 02:28

**「背景」** 果蝇连接组（connectome）是通过电子显微镜重建的神经元间突触连接图谱，MaleCNS v1.0 是果蝇雄性中枢神经系统的完整重建，包含约 16.6 万个神经元。将真实连接组用于学习任务测试，旨在验证神经回路是否具备可塑性能力；多巴胺样可塑性模拟奖惩信号调节突触权重。Pong 因其二进制的正负反馈和对精确追踪的要求，被视为对学习算法和神经结构的严格考验。

**「影响」** 对使用连接组数据进行模拟或构建可塑性模型的 AI/ML 研究者，该审计揭示了数据管道中的隐性错误（如正则表达式语义、神经元索引分配）可能导致虚假的负结果，并提供了系统性排查示例；同时提醒社区对公开的“果蝇玩游戏”类演示应持批判态度，因多数项目未通过严谨验证。

**「社区讨论」** 无社区评论可供汇总。

**标签**: `#connectomics`, `#reinforcement learning`, `#neural plasticity`, `#debugging`, `#neuroscience`

---

<a id="item-tech-news-17"></a>
### [蚂蚁国际联合 Visa、Mastercard 制定 AI 代理支付标准](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 7.0/10

蚂蚁国际于 2026 年 9 月 10 日宣布与 Visa、Mastercard 合作，为 AI 代理支付制定通用标准。三方将建立&quot;了解你的代理&quot;（Know Your Agent）机制，通过将 AI 代理关联到有效实体、评估其行为并持续监测风险，提升不同支付系统间的互操作性和安全性。三方援引麦肯锡预测称，到 2030 年 AI 代理处理的全球消费者商业交易额可能达到 3 万亿至 5 万亿美元。该举措标志着传统卡组织与金融科技企业首次以联盟形式定义 AI 代理支付的风险治理框架，但当前仍属意向声明，尚未发布具体技术规范或可交付的标准版本。

telegram · zaihuapd · 9月10日 03:00

**「背景」** 传统支付与金融体系中，KYC（了解你的客户）要求机构核实交易参与方的真实身份，是反洗钱和风险控制的基础。随着 AI 代理开始独立发起支付，原有框架无法直接适用，行业需要新的识别、验证与监测机制来确认代理背后的有效实体并追踪其行为，“KYA（了解你的代理）”正是将这一理念延伸至自主代理的产物。此次蚂蚁国际与 Visa、Mastercard 的合作于 2026 年 9 月 10 日宣布，目标是制定统一标准以提升跨支付系统的互操作性，目前属于意向性声明而非已交付的技术标准。

**「潜在影响」** 该合作意味着 Visa、Mastercard 与蚂蚁国际（支付宝母公司）将共同主导 AI 代理支付规则，引入

<details><summary>参考链接</summary>
<ul>
<li><a href="https://political.org/2026/09/09/visa-mastercard-and-ant-international-develop-standards-for-ai-agent-payments/">Visa , Mastercard and Ant International Launch ‘Know Your Agent ...</a></li>
<li><a href="https://crypto.news/ant-international-joins-visa-mastercard-to-build-ai-agent-payment-standards/">Ant International joins Visa , Mastercard to build AI agent payment ...</a></li>
<li><a href="https://www.chaincatcher.com/en/article/2288780">Ant Group collaborates with Visa and...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#payments standards`, `#fintech`, `#interoperability`, `#AI infrastructure`

---

<a id="item-tech-news-18"></a>
### [DeepSelect v1.0.0：面向 DSA 与采样器的 TopK 内核库](https://github.com/deepseek-ai/DeepSelect) ⭐️ 7.0/10

DeepSeek-AI 于 2026 年 9 月 10 日发布 DeepSelect v1.0.0，这是一套面向 DeepSeek 稀疏注意力（DSA）与采样器的高性能 TopK 内核库，代码已托管于 GitHub。该项目声称相比 PyTorch 原生的 torch.topk 可实现 2 至 20 倍的提速；TopK 运算是稀疏注意力机制和采样流程的关键环节，这类性能优化直接影响模型推理与生成效率。需要注意的是，该消息仅来自一则简短的 Telegram 帖子，未附带基准测试细节或独立验证，实际加速效果有待社区复现确认。

telegram · zaihuapd · 9月10日 07:28

**「背景」** DeepSeek 稀疏注意力（DSA）是 DeepSeek 系列模型（包括 DeepSeek V3.2、V4 和 V4.1）中使用的稀疏注意力机制，其实现依赖 TopK 核函数来从压缩后的注意力 logits 中选取关键位置。NVIDIA cuDNN 文档显示，DSA 模块的核心多数针对 Hopper（SM90）和 Blackwell（SM100+）GPU，其中组合的压缩 logits 加 TopK 路径仅支持 SM100。DeepSelect 正是面向这一稀疏注意力路径及采样器场景的高性能 TopK 核函数实现，旨在替代 PyTorch 原生 torch.topk。

**「影响」** 对于在 DeepSeek V3.2、V4 与 V4.1 等模型中依赖 DeepSeek 稀疏注意力（DSA）及采样流程的开发者，集成 DeepSelect 可将 TopK 运算相对原生 torch.topk 提速 2 至 20 倍，从而缩短推理与采样延迟；不过该性能数据来自项目自身声明，尚无独立基准验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/deeplearning/cudnn/latest/fe-oss-apis/dsa.html">DeepSeek Sparse Attention (DSA) — NVIDIA cuDNN</a></li>
<li><a href="https://github.com/deepseek-ai/DeepSelect">GitHub - deepseek -ai/ DeepSelect : DeepSelect : TopK kernels for...</a></li>
<li><a href="https://github.com/AnnoCat/deepselect">GitHub - AnnoCat/deepselect: DeepSelect: TopK kernels for ...</a></li>

</ul>
</details>

**标签**: `#TopK`, `#DeepSeek`, `#sparse attention`, `#performance optimization`, `#kernel`

---

<a id="item-tech-news-19"></a>
### [HBM 短缺推高中国 AI 芯片价格](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

路透社报道，全球高带宽存储器（HBM）供应紧张正冲击中国 AI 芯片产业，华为、寒武纪等厂商已上调产品价格。华为升腾 950DT 芯片报价较两个月前上涨约 20%至 50%，部分老款芯片价格上涨约 30%；寒武纪新一代思元 690 价格预计上涨约 20%至 30%。HBM 主要由 SK 海力士、三星和美光供应，美国出口限制加剧了中国市场的供应压力。随着国内 AI 算力需求增长，HBM 短缺正成为制约国产 AI 芯片扩张的重要瓶颈。

telegram · zaihuapd · 9月10日 09:29

**「背景信息」** HBM 是一种高带宽存储器，通过堆叠 DRAM 芯片实现更快的数据传输速度，是 AI 训练和推理芯片的关键组件。美国对华出口管制限制了中国获取先进 AI 芯片和制造设备，而 HBM 作为核心部件受类似限制影响，使得中国厂商在扩大产能时面临供应链瓶颈。

**「影响分析」** 对采购华为升腾或寒武纪思元系列芯片的数据中心和企业用户而言，价格上涨将直接增加 AI 基础设施成本，并可能延缓国产 AI 算力规模的扩展；若 HBM 短缺持续，价格仍有上行风险。

**标签**: `#AI芯片`, `#HBM`, `#供应链`, `#中国科技`, `#半导体`

---