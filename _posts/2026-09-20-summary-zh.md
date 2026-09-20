---
layout: default
title: "Horizon Summary: 2026-09-20 (ZH)"
date: 2026-09-20
lang: zh
---

> 从 24 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [GPT-6 Astra 开放 API 并公布定价](#item-tech-news-1) ⭐️ 9.0/10
2. [卡巴斯基端点零日提权漏洞遭公开披露](#item-tech-news-2) ⭐️ 8.0/10
3. [为何应几乎不用 AI 代写面向他人的文字](#item-tech-news-3) ⭐️ 7.0/10
4. [四家 AI 巨头因呼吁放缓研发被诉反垄断](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic 拟在 IPO 前发布新模型应对 GPT-6 Astra](#item-tech-news-5) ⭐️ 7.0/10
6. [苹果高管回应 iPhone Duo 折痕](#item-tech-news-6) ⭐️ 7.0/10
7. [OpenAI 推出 ChatGPT for Word 插件，可在 Word 内起草编辑文档](#item-tech-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GPT-6 Astra 开放 API 并公布定价](https://developers.openai.com/api/docs/models/gpt-6-astra) ⭐️ 9.0/10

OpenAI 现已通过 API 正式提供新一代旗舰模型 GPT-6 Astra，开发者可直接调用该模型。根据官方文档，其定价为每 100 万输入 tokens 收费 10.00 美元，每 100 万输出 tokens 收费 50.00 美元。这一发布对 AI/ML 开发者意义重大，为构建和部署应用提供了新的高性能模型选择。关于上下文长度、可用区域及具体能力限制等细节，仍需参考官方文档确认。

telegram · zaihuapd · 9月19日 04:02

**「背景」** GPT-6 Astra 是 OpenAI 于 2026 年 9 月 3 日发布的旗舰模型，此前因 2026 年 7 月一系列未经授权的代理攻击而推迟上市，以补充安全防护措施。据 OpenAI 介绍，该模型是其对齐程度最高、能力最强的模型，在理解用户意图和行为方面有大幅改进，适用于复杂推理、编程、计算机使用、研究和文档创建等端到端任务。

**「影响」** 对于希望集成最新 OpenAI 模型的开发者而言，GPT-6 Astra 的 API 上线提供了可直接接入的新选项，并按公布的 tokens 单价计费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT-6 Astra: A new generation of intelligence | OpenAI</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-6-astra">GPT-6 Astra Model | OpenAI API</a></li>

</ul>
</details>

**标签**: `#GPT-6`, `#OpenAI`, `#API pricing`, `#AI models`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [卡巴斯基端点零日提权漏洞遭公开披露](https://twitter.com/CyberWarship/status/tweet-2101302290552385978) ⭐️ 8.0/10

安全研究员 Florian Hansemann（@CyberWarship）发布推文，公开链接到一个名为 MSNightmare/HardBreacher 的 GitHub 仓库，该仓库声称演示卡巴斯基端点防病毒（Kaspersky Antivirus for Endpoint）的零日权限提升漏洞。若该漏洞属实，攻击者可在受保护系统上获得更高权限，从而削弱这一主流防病毒产品所提供的基础安全防线，对安全研究、渗透测试及蓝队防御均有直接影响。推文附带了 \#infosec、\#pentest、\#redteam、\#blueteam 等标签，表明该内容面向攻防两端受众。目前公开信息仅包含仓库描述，尚缺乏漏洞技术细节、受影响版本、利用条件或厂商响应等验证信息，因此该漏洞的真实影响与可利用性仍有待进一步确认。

twitter · Florian Hansemann · 9月19日 13:28

**「背景信息」** 零日漏洞指的是尚未被厂商修复或公开披露的安全缺陷，而权限提升（privilege escalation）漏洞允许本地普通用户获取更高系统权限，属于高风险问题。Kaspersky Endpoint Security 是卡巴斯基面向企业用户的终端安全防护产品。名为 HardBreacher 的利用代码已在 GitHub 上公开，声称可在已完全修补的 Windows 11 系统上利用 Kaspersky Endpoint Security 中未修补的本地权限提升漏洞，但该问题目前尚未被卡巴斯基验证、公开确认，也未分配相应的 CVE 编号。

**「影响」** 若该漏洞被证实并利用，攻击者可借此在运行 Kaspersky Endpoint Security 的终端上完成权限提升，从而把本应防御的安全软件变成攻击入口，扩大攻击面。不过，该仓库目前未提供可靠的完整利用链细节，实际可利用性仍待验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/hardbreacher-kaspersky-zero-day/">HardBreacher PoC Claims Kaspersky Endpoint Security Zero-Day Privilege Escalation on Windows 11</a></li>
<li><a href="https://github.com/MSNightmare/HardBreacher">GitHub - MSNightmare/HardBreacher: Kaspersky Antivirus For Endpoint ZeroDay Elevation of Privileges Vulnerability · GitHub</a></li>
<li><a href="https://cyberpress.org/hardbreacher-poc-targets-kaspersky-endpoint-security-zero-day/">HardBreacher PoC Targets Kaspersky Endpoint Security Zero-Day for Windows 11 Privilege Escalation</a></li>
<li><a href="https://cybersecuritynews.com/hardbreacher-kaspersky-zero-day/">HardBreacher PoC Claims Kaspersky Endpoint Security Zero - Day ...</a></li>

</ul>
</details>

**标签**: `#security`, `#exploit`, `#zero-day`, `#privilege-escalation`, `#kaspersky`

---

<a id="item-tech-news-3"></a>
### [为何应几乎不用 AI 代写面向他人的文字](https://erichgrunewald.substack.com/p/why-you-should-almost-never-use-ai) ⭐️ 7.0/10

一篇观点文章主张，开发者和写作者应避免使用 AI 代写面向他人的文本，而应将 AI 用于自我导向的理解与批评。作者引用 Eric Schwitzgebel 的观点指出，阅读时被动点头与主动生成文本之间存在巨大的认知差异：文本一旦上页，人们容易让“大致合适的词”蒙混过关，而主动生成时才会对措辞进行费力思考。文章认为，过度依赖 AI 生成会削弱这种认知努力，进而损害写作能力与表达质量。该文在 Hacker News 上引发高度参与的实际讨论（203 分、115 条评论），社区给出了可操作的经验法则：用 AI 生成“供自己阅读”的材料（如研究摘要、数据报告、会议纪要转邮件），而不要用 AI 生成“供他人消费”的内容；或者请 AI 批评自己的稿子而非让其重写。社区评论还指出，AI 写作往往模糊、错误且难以察觉，在协作白皮书中会以隐蔽方式损害原有论点。

hackernews · erwald · 9月19日 16:35 · [社区讨论](https://news.ycombinator.com/item?id=49767937)

**「背景」** 这篇文章出自作者 Eric Grunewald（2026 年 8 月 6 日发表于 Substack），主张人们几乎不应让 AI 代写任何面向他人的实质性文本，如博客、研究报告、备忘录或小说等。其核心论据引用哲学家 Eric Schwitzgebel 的观点：被动阅读与主动产出文字之间存在巨大的认知差异，一旦文字落在页面上，读者容易被动接受模糊的措辞，而不会像自己动笔那样费力推敲字句。作者因此建议只将 AI 用于个人的理解与批判性用途（如总结资料、批评自己的草稿），而不用它去撰写供他人消费的内容，并认为即使明确标注为 AI 所写，整篇交给 AI 也几乎从不是好主意。

**「影响」** 对依赖 AI 起草对外文本的开发者、技术写作者和团队而言，本文及社区讨论提供了一个明确的操作边界：将 AI 限定在“理解与检验”环节（生成给自己看的摘要、请 AI 批评自己的稿子），而把面向读者/用户的生成工作保留给人类，以避免认知努力流失和隐蔽的错误。

**「社区讨论」** 社区普遍认同“可读不可写”的区分：有人建议用 AI 生成“你希望别人写给你看”的材料（如研究摘要、决策报告、会议纪要转邮件），而非面向他人的成品；另有人主张请 AI 批评自己的写作并自行取舍建议，但提醒 LLM 总是给出过度重写，需警惕。有评论者直言，若沟通是目的，用 LLM 写作反而会“埋葬你的意思”，并提到 AI 文本“含糊且以难以察觉的方式出错”——在协作白皮书中曾因丢失微妙之处而损害原有论点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://erichgrunewald.substack.com/p/why-you-should-almost-never-use-ai">Why I Think You Should Almost Never Use AI to Write Anything Substantive</a></li>
<li><a href="https://www.erichgrunewald.com/posts/why-i-think-you-should-almost-never-use-ai-to-write-anything-substantive/">Why You Should Almost Never Use AI to Write Anything Substantive</a></li>
<li><a href="https://forum.nunosempere.com/posts/stmA3cmXY8jaZahtg/why-you-should-almost-never-use-ai-to-write-anything">Why You Should Almost Never Use AI to Write Anything Substantive</a></li>

</ul>
</details>

**标签**: `#AI writing`, `#LLM usage`, `#technical writing`, `#software engineering practice`, `#generative AI`

---

<a id="item-tech-news-4"></a>
### [四家 AI 巨头因呼吁放缓研发被诉反垄断](https://www.politico.com/news/2026/09/18/anthropic-openai-spacexai-google-sued-over-calls-to-pace-ai-development-01085023) ⭐️ 7.0/10

Anthropic、OpenAI、SpaceXAI 与 Google 在美国加州联邦法院面临一宗消费者反垄断集体诉讼，原告指控四家相互竞争的 AI 企业通过公开响应“放慢 AI 发展”的主张形成非法协调。起诉书指称，Anthropic CEO 达里奥·阿莫迪本月发文呼吁行业协同放缓前沿 AI 能力发展步伐，随后马斯克、奥特曼和哈萨比斯相继公开表示认同，涉嫌违反美国《谢尔曼法》第 1 条。原告为订阅上述公司 AI 服务的消费者，请求法院进行集体诉讼认证并发布禁令。四家公司目前均未回应置评请求。

telegram · zaihuapd · 9月19日 02:08

**「背景说明」** 《谢尔曼法》第 1 条禁止竞争者之间达成不合理限制贸易的协议，其法律争议关键在于证明存在“协议”而非采取独立的单方行为。本案的焦点在于，四家公司高管关于放缓前沿 AI 研发的公开表态是否构成竞争者之间协同限制竞争的非法协议，以及公开声明能否满足反垄断法对“合谋”的证据要求。

**「影响评估」** 若原告胜诉，法院可能以禁令限制四家公司协调放缓 AI 研发的行为，进而改变 AI 行业高管就安全议题公开发声的方式与节奏；案件结果也可能为“通过公开言论达成默契”是否构成《谢尔曼法》项下非法协议确立新的司法先例。

**标签**: `#AI industry`, `#antitrust`, `#regulation`, `#OpenAI`, `#Anthropic`

---

<a id="item-tech-news-5"></a>
### [Anthropic 拟在 IPO 前发布新模型应对 GPT-6 Astra](https://www.reuters.com/business/anthropic-considers-releasing-new-ai-model-ahead-ipo-sources-say-2026-09-19/) ⭐️ 7.0/10

据三名知情人士透露，Anthropic 正考虑在预期首次公开募股（IPO）之前发布一款新 AI 模型，以应对 OpenAI 发布 GPT-6 Astra 后日益加剧的竞争压力，同时公司也在评估该新模型的安全性。Ramp 数据显示，Astra 目前约占企业 AI 支出的 13%，而 Anthropic 的 Claude Fable 仅占约 8%。此外，两名知情人士称，Anthropic 的 IPO 可能推迟至美国 11 月中期选举之后。该报道来自 Reuters，涉及 Anthropic 在关键竞争窗口期的战略布局，具体发布时间和 IPO 时间表尚未最终确定。

telegram · zaihuapd · 9月19日 03:25

**「背景」** Anthropic 是开发 Claude 系列大语言模型的 AI 公司，目前正筹备在 2026 年进行首次公开募股（IPO），市场关注其营收、估值及盈利能力。与此同时，其主要竞争对手 OpenAI 推出的 GPT-6 Astra 在企业和开发者市场中占据明显份额，据 Ramp 数据，Astra 约占企业 AI 支出的 13%，而 Anthropic 的 Claude Fable 约占 8%。自 OpenAI 上市以来，公开市场倾向将前沿模型公司的定价与 OpenAI 的规模进行比较，这使 Anthropic 在 IPO 前的产品节奏和竞争策略备受关注。

**「影响」** 若 Anthropic 按计划在 IPO 前发布新模型，可能有助于缩小其与 OpenAI 在企业 AI 市场的份额差距（当前约 5 个百分点），并改善其估值前景；但 IPO 推迟至中期选举后意味着投资者需等待更长时间，且发行窗口可能受政治和经济不确定性影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leverageshares.com/us/insights/the-anthropic-ipo-what-you-need-to-know-before-trading-it/">The Anthropic IPO What You Need to Know Before Trading It</a></li>
<li><a href="https://distributionstrategy.com/2026/06/anthropic-ipo-filing-signals-enterprise-ai-has-become-core-business-infrastructure/">Anthropic IPO Filing Signals Enterprise AI Has Become Core...</a></li>
<li><a href="https://www.techi.com/anthropic-ipo/">Anthropic IPO : Valuation, Timeline, Access Options, and Risks | TECHi</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#OpenAI`, `#AI models`, `#IPO`, `#competition`

---

<a id="item-tech-news-6"></a>
### [苹果高管回应 iPhone Duo 折痕](https://www.macrumors.com/2026/09/19/apple-exec-iphone-crease/) ⭐️ 7.0/10

苹果硬件工程副总裁 Tom Marieb 在回应折叠屏 iPhone Duo 的折痕问题时表示，该机采用哑光纳米纹理屏幕，以减少反光并降低折痕可见度，他希望用户就折痕表现“让苹果接受检验”。他还透露，iPhone Duo 的铰链经过长期调校，开合手感应像高端汽车车门，并支持半折坐立、展开和闭合三种状态。该机将于 10 月 16 日开启预购，10 月 23 日正式发售，起售价为 1999 美元，是苹果首款折叠屏手机。这些设计选择旨在缓解用户对折叠屏耐用性和美观度的主要顾虑。

telegram · zaihuapd · 9月19日 06:36

**「背景」** 折叠屏手机因显示屏需反复弯折，在折叠处通常会出现一条可见的折痕，这是该品类长期存在的短板。哑光纳米纹理是一种通过蚀刻玻璃表面来散射光线、减少反光的处理工艺，苹果已在多款产品中采用。iPhone Duo 是苹果首款折叠屏手机，苹果希望借助这种工艺让折痕在视觉上不那么显眼。

**「影响」** 对于有意入手苹果首款折叠屏手机的用户，10 月 23 日发售、1999 美元起售的 iPhone Duo 能否在长期使用中保持折痕不明显和铰链手感，将是其实际体验的关键检验点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/09/19/apple-exec-iphone-crease/">Apple Exec Says &#x27;Hold Us Accountable&#x27; on iPhone Duo Crease</a></li>
<li><a href="https://9to5mac.com/2026/09/18/apple-vp-of-hardware-talks-iphone-duo-durability-crease-hinge-and-more/">Apple VP of hardware talks iPhone Duo durability, crease ... - 9to5Mac</a></li>

</ul>
</details>

**标签**: `#Apple`, `#foldable phone`, `#hardware`, `#iPhone Duo`, `#display technology`

---

<a id="item-tech-news-7"></a>
### [OpenAI 推出 ChatGPT for Word 插件，可在 Word 内起草编辑文档](https://chatgpt.com/apps/word/) ⭐️ 7.0/10

OpenAI 推出 ChatGPT for Word 插件，将 ChatGPT 能力引入 Microsoft Word，用户可在 Word 内起草、编辑和排版文档，并能接入 Outlook、SharePoint、Google Workspace 和 Dropbox 等应用以补充上下文。该插件面向全球所有套餐，覆盖免费版及企业、教育等版本，用户可从 Microsoft Marketplace 安装，在 Word 中打开并用 ChatGPT 账号登录。这一集成将生成式 AI 辅助带入主流生产力工具，扩大了 ChatGPT 的可用范围，但属于增量式产品更新，并非颠覆性发布。

telegram · zaihuapd · 9月19日 10:21

**「背景信息」** 在 OpenAI 本次发布之前，将 ChatGPT 能力引入 Microsoft Word 通常依赖第三方解决方案，例如 GPT for Work 提供的侧边栏集成，这类工具支持起草、改写、翻译和审阅等 AI 写作辅助功能，但并非 OpenAI 官方出品。OpenAI 此次推出的 ChatGPT for Word 是官方 Microsoft 加载项，通过 Microsoft Marketplace 安装，并在 Word 侧边栏中打开 ChatGPT 界面，用户需使用 ChatGPT 账号登录。值得注意的是，该官方加载项不仅支持 Word，还涵盖 Excel 和 PowerPoint，且若用户使用组织工作区，需在登录后选择相应工作区，同时 Microsoft 管理员可能需要启用访问权限。

**「影响」** 该插件使所有 ChatGPT 套餐用户（包括免费版和企业、教育版）能在 Word 中直接调用 AI 起草、编辑和排版文档，并与多个办公和云存储服务协同，可能提升日常文档处理效率，但实际效果取决于插件稳定性与用户工作流适配程度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://chatgpt.com/apps/word/">ChatGPT for Word | Draft and edit documents with ChatGPT</a></li>
<li><a href="https://help.openai.com/en/articles/20001526-chatgpt-for-word">ChatGPT for Word | OpenAI Help Center</a></li>
<li><a href="https://gptforwork.com/blog/chatgpt-into-microsoft-word-how-to-guide">ChatGPT into Microsoft Word - How-to Guide | GPT for Work</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#Microsoft Word`, `#Productivity`, `#AI Integration`

---