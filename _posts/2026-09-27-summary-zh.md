---
layout: default
title: "Horizon Summary: 2026-09-27 (ZH)"
date: 2026-09-27
lang: zh
---

> 从 29 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [SemiAnalysis 免费拆解英特尔 Panther Lake 与 18A 工艺](#item-tech-news-1) ⭐️ 8.0/10
2. [上诉法院维持五角大楼对 Anthropic 黑名单裁决](#item-tech-news-2) ⭐️ 8.0/10
3. [Reladraw：可指定布局的图表语言](#item-tech-news-3) ⭐️ 7.0/10
4. [苹果因 Apple Pay 收费面临反垄断集体诉讼](#item-tech-news-4) ⭐️ 7.0/10
5. [Excel 40 年来首次支持单元格内多值，新增四个数组函数](#item-tech-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SemiAnalysis 免费拆解英特尔 Panther Lake 与 18A 工艺](https://newsletter.semianalysis.com/p/intel-panther-lake-teardown) ⭐️ 8.0/10

半导体分析机构 SemiAnalysis（作者 Adith Shankar）发布了针对英特尔 Panther Lake 处理器的免费拆解报告，隶属于其 STEEL 系列技术分析。该拆解聚焦于英特尔 18A 工艺节点的实现方式，而 18A 是英特尔重振其代工业务所依赖的下一代制造技术。公开摘要未披露具体测量数据或工艺细节，但该报告标志着业界首次以独立拆解形式审视 18A 节点的关键设计取舍。对关注先进制程竞争与英特尔代工路线图的硬件工程师和分析师而言，这是一份高价值的一手技术资料。

rss · Semianalysis · 9月26日 13:36

**「背景」** Panther Lake 是英特尔的下一代笔记本电脑处理器，预计于 2025 年发布，按计划将采用全新的 Intel 18A 工艺节点制造。Intel 18A 是英特尔最先进的制造节点，引入了 RibbonFET（环栅晶体管）与 PowerVia（背面供电）两项关键技术。本次拆解正是为了从物理层面验证该节点与芯片设计的实际实现方式，而相关报道也确认 Panther Lake 将搭载 Cougar Cove 性能核与 Darkmont 能效核。

**「影响」** 该报告为芯片设计工程师和行业分析师提供了关于英特尔 18A 节点实际实现取舍的独立技术证据，可用于评估英特尔代工业务的技术竞争力；由于公开摘要不含具体数据，确切的工艺与性能结论仍需以报告全文为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/enigma-security_intel-pantherlake-pctechnology-activity-7382348178563473408-WJUJ"># intel # pantherlake #pctechnology #advancedchips #aiinhardware...</a></li>
<li><a href="https://wccftech.com/intel-panther-lake-confirmed-to-feature-cougar-cove-darkmont/">Intel &#x27;s Panther Lake SoCs Confirmed To Feature Cougar Cove...</a></li>

</ul>
</details>

**标签**: `#Intel`, `#Panther Lake`, `#Intel 18A`, `#semiconductor`, `#hardware teardown`

---

<a id="item-tech-news-2"></a>
### [上诉法院维持五角大楼对 Anthropic 黑名单裁决](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 8.0/10

美国华盛顿特区联邦上诉法院于 2026 年 9 月 25 日以 2 比 1 的投票结果，维持五角大楼将 AI 实验室 Anthropic 列入国家安全供应链风险黑名单的决定，从而禁止其参与美国军事合同。多数法官认为，Anthropic 拒绝允许其产品用于自主武器和大规模监控的做法，合理地引发了五角大楼的担忧。Anthropic 表示不同意该裁决，并正考虑请求全体上诉法院对此案进行复审。此前，旧金山联邦法官曾依据另一部法律推翻了相关列名，并阻止政府对 Anthropic 实施更广泛的禁令。这一裁决直接影响 Anthropic 的军事合作与商业边界，并牵涉 AI 安全、伦理及相关政策和法律争议。

telegram · zaihuapd · 9月26日 05:19

**「背景」** Anthropic 是一家人工智能安全研究公司，其产品条款中明确禁止用于自主武器和大规模监控等用途，这与五角大楼对军事 AI 能力的需求产生冲突。五角大楼依据国家安全供应链风险相关法规将 Anthropic 列名，意在限制其参与军事合同；此前旧金山联邦法院曾基于另一部法律推翻该列名，但本次上诉法院的裁决推翻了此前的部分司法结果。

**「影响」** 该裁决使 Anthropic 目前仍无法获得美国军事合同，其商业机会和政府合作将受到实质性限制，同时可能影响其与军方相关的产品开发路线及行业对 AI 伦理边界的讨论。

**标签**: `#AI政策`, `#Anthropic`, `#AI伦理`, `#军事AI`, `#法律`

---

<a id="item-tech-news-3"></a>
### [Reladraw：可指定布局的图表语言](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw 是一个开源的新图表语言，允许开发者通过代码精确定义节点位置，弥补了 Mermaid 或 Graphviz 等自动布局工具与 Draw.io 等手动编辑器之间的空白。该项目提供在线 playground 免安装试用，并支持通过 npm 安装，同时还提供了用于 Claude 或其他智能体的技能安装方式，适合人类与 AI 智能体协作。它强调在保持代码可维护性的同时，让用户对图表的最终外观拥有高度控制权。该语言针对流程图中位置至关重要的场景特别有用，而相对定位方式也被认为足够满足大多数精确布局需求。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**「背景」** 传统图表工具要么采用自动布局（如 Mermaid、Graphviz），开发者无法控制节点位置，结果常常难看；要么像 Draw.io 那样需要手动拖拽，耗时且不适合智能体操作。Reladraw 试图结合两者优势，让用户以代码形式定义图表，同时保留对布局的显式控制，从而服务于需要精确呈现的开发者与 AI 智能体。

**「影响」** 对于需要在开发流程中用图表对齐架构的开发者及其编程智能体，Reladraw 提供了一种既精确又可维护的图表编写方式，有望降低手动调整的耗时。

**「社区讨论」** 社区反馈认为该工具处于“甜蜜点”，并建议将拓扑结构与布局关注点解耦以便用于 C4 建模。也有用户报告了边线弯曲渲染的疑似 bug，但整体上对这一方向表示欢迎。

**标签**: `#diagramming`, `#developer tools`, `#AI agents`, `#open source`, `#visualization`

---

<a id="item-tech-news-4"></a>
### [苹果因 Apple Pay 收费面临反垄断集体诉讼](https://9to5mac.com/2026/09/25/apple-faces-class-action-over-apple-pay-fees-charged-to-card-issuers/) ⭐️ 7.0/10

美国联邦法官已认证一起针对苹果的反垄断集体诉讼，指控苹果就 Apple Pay 交易向支付卡发卡机构收取过高费用。集体成员涵盖所有在美国发行支持 Apple Pay 卡片并支付相关费用的机构。诉讼称，苹果对信用卡交易按 0.15%、借记卡交易按 0.5 美分收费，而安卓手机钱包不向发卡机构收费；苹果被指每年收取最高 10 亿美元费用，并阻止对手开发竞争性钱包。原告要求退还费用并寻求禁令。该诉讼若成立，可能重塑移动支付平台的经济模式。

telegram · zaihuapd · 9月26日 03:32

**「背景信息」** Apple Pay 是苹果公司自 2014 年起在 iPhone 等设备上提供的移动支付与数字钱包服务，依托 NFC（近场通信）完成非接触式交易。与安卓系统中 Google Pay 等竞争性钱包不同，苹果对每笔 Apple Pay 交易向发卡机构收取费用，因而被指利用其在移动钱包市场的地位获取垄断性收入。美国联邦法官 Jeffrey S. White 已批准将这一反垄断诉讼认证为集体诉讼，允许数千家美国银行和信用社联合起诉苹果，指控其收取过高的 Apple Pay 费用并阻碍竞争对手开发替代钱包。

**「影响」** 该集体诉讼认证意味着所有符合条件的美国发卡机构自动成为原告群体成员，若苹果败诉，将面临最高每年 10 亿美元的 Apple Pay 费用退还，并可能被禁令限制其对信用卡 0.15%、借记卡 0.5 美分的现行收费结构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hbsslaw.com/press/apple-pay-payment-card-issuer-antitrust/credit-unions-win-class-certification-in-class-action-lawsuit-against-apple-alleging-illicit-revenue-from-apple-pay-fees">Credit Unions Win Class Certification in Class-Action Lawsuit ...</a></li>
<li><a href="https://9to5mac.com/2026/09/25/apple-faces-class-action-over-apple-pay-fees-charged-to-card-issuers/">Apple faces class action over Apple Pay fees charged to card ...</a></li>
<li><a href="https://appleinsider.com/articles/26/09/25/thousands-of-banks-can-now-sue-over-apple-pay-fees-in-one-antitrust-case">Thousands of banks can now sue over Apple Pay fees</a></li>
<li><a href="https://perexpteamworks.com/en/apple-pay-fees-class-action-lawsuit/">Apple Pay Fees Lawsuit Certified for Banks and Credit Unions</a></li>
<li><a href="https://www.macrumors.com/2026/09/25/apple-pay-antitrust-lawsuit-advances/">Banks and Credit Unions to Team Up Against Apple Pay Fees</a></li>

</ul>
</details>

**标签**: `#apple`, `#apple-pay`, `#antitrust`, `#mobile-payments`, `#class-action`

---

<a id="item-tech-news-5"></a>
### [Excel 40 年来首次支持单元格内多值，新增四个数组函数](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 7.0/10

微软宣布在 Excel 中推出列表、单元格内数组与嵌套数组功能，率先面向 Windows 和 Mac 的 Beta 通道用户开放。这是 Excel 40 年来首次允许在一个单元格中存放多个值，用户可用 Ctrl+J 或通过「插入 &gt; 列表」写入以逗号或分号分隔的多个项目，并能按单项进行筛选与计算。与此同时新增了 FLATTEN、HAS、HASANY、HASALL 四个函数用于处理数组。这些均为预览功能，正式发布前行为可能调整，官方建议暂不要用于重要工作簿。

telegram · zaihuapd · 9月26日 16:26

**「背景」** 传统 Excel 中一个单元格只能存储一个值，数组运算通常需要借助多单元格公式或动态数组函数（如 FILTER、SORT）来实现，用户无法在单个单元格内直接存放并管理多项数据。本次更新打破了这一长期限制，并配合新增函数提供更灵活的数组处理方式，属于表格软件基础模型的重要扩展。

**「影响」** 对于依赖 Excel 进行数据整理和分析的 Windows 及 Mac Beta 通道用户，此功能可显著简化多值存储与筛选流程，但因其仍为预览状态且行为可能变动，建议避免在关键生产工作簿中使用。

**标签**: `#Excel`, `#微软`, `#数组`, `#数据分析`, `#预览功能`

---