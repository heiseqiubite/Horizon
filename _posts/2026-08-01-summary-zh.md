---
layout: default
title: "Horizon Summary: 2026-08-01 (ZH)"
date: 2026-08-01
lang: zh
---

> 从 38 条内容中筛选出 13 条重要资讯。

---

1. [MCP 2.0 转向无状态模式，重新激发开发者兴趣](#item-1) ⭐️ 9.0/10
2. [法官考虑永久撤销美政府对 Anthropic 的封禁](#item-2) ⭐️ 9.0/10
3. [Simon Willison 谈 AI 开放权重革命](#item-3) ⭐️ 8.0/10
4. [以 GPT-5.6 推进性价比前沿](#item-4) ⭐️ 8.0/10
5. [🤖 DeepSeek-V4-Flash 正式版 API 上线公测](#item-5) ⭐️ 8.0/10
6. [华为开源 505B 参数 MoE 大模型 openPangu-2.0-Pro](#item-6) ⭐️ 8.0/10
7. [德国法院裁定 AI 音乐公司 Suno 侵犯版权](#item-7) ⭐️ 8.0/10
8. [Tailscale 发布 Hugging Face 泄露认证密钥入侵事件的详细复盘](#item-8) ⭐️ 7.0/10
9. [电梯调度算法的交互式探索](#item-9) ⭐️ 7.0/10
10. [qm：YC 支持的多人协作 AI Agent 管理框架](#item-10) ⭐️ 7.0/10
11. [开源 Transformer 模型用于糖尿病血糖水平预测](#item-11) ⭐️ 7.0/10
12. [If reviewing is mandatory for paper submissions, low-quality reviews can no longer be justified as “volunteer work” \[D\]](#item-12) ⭐️ 7.0/10
13. [MiniMax 多模态视频模型 H3 将于 8 月 3 日开源](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [MCP 2.0 转向无状态模式，重新激发开发者兴趣](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 9.0/10

MCP 2.0 规范（正式名称为 2026-07-28 Model Context Protocol 规范）于 2026 年 7 月 28 日发布，将协议默认改为无状态模式，取消了初始化/会话握手，改用单次 HTTP 请求。受这一重大简化的启发，Simon Willison 构建了 mcp-explorer（用于交互式探测 MCP 服务器的命令行工具）和 datasette-mcp（Datasette 的 MCP 服务器）。 这是 MCP 规范自发布以来最重大的变更，大幅降低了客户端和服务端的实现复杂度，使协议更适合无需维护服务端会话状态的可扩展 Web 应用。它还将 MCP 重新定位为比给予 AI 代理不受限制的 shell 访问权限更安全、更易审计的替代方案，后者已被证明充满风险。 旧的有状态 MCP 需要两次 HTTP 请求——先通过 initialize 调用获取 Mcp-Session-Id，再发起第二次请求实际调用工具——而新的无状态方式使用单次 POST 请求并附带 MCP-Protocol-Version 头。仍需跨调用状态的服务端现在使用显式的、服务端生成的句柄作为普通工具参数传递（SEP-2567），而非依赖隐式会话管理。

rss · Simon Willison · 7月31日 23:13

**背景**: MCP（Model Context Protocol）由 Anthropic 于 2024 年 11 月推出，旨在为 LLM 驱动的代理框架提供一种标准化暴露工具的方式。它在 2025 年经历了巨大的关注热潮，但后来在一定程度上被 Anthropic 的 Skills 功能所掩盖——Skills 允许具备终端和 curl 访问权限的代理框架以更灵活的方式实现 MCP 的大部分功能。Willison 现在认为，给予代理 shell 访问权限存在风险且需要强模型支撑，而 MCP 工具更易审计和控制，甚至可以在笔记本电脑上运行的小型模型也能很好地驱动它们。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/">The 2026-07-28 MCP Specification Release Candidate | Model Context Protocol Blog</a></li>
<li><a href="https://modelcontextprotocol.io/specification/2026-07-28/changelog">Key Changes - Model Context Protocol</a></li>
<li><a href="https://devblogs.microsoft.com/dotnet/announcing-v20-of-the-official-mcp-csharp-sdk/">Announcing v2.0 of the official MCP C# SDK - .NET Blog</a></li>

</ul>
</details>

**标签**: `#MCP`, `#Model Context Protocol`, `#AI Agents`, `#LLM Tools`, `#Anthropic`

---

<a id="item-2"></a>
## [法官考虑永久撤销美政府对 Anthropic 的封禁](https://techcrunch.com/2026/07/30/judge-says-trump-admin-still-lacks-evidence-for-anthropic-supply-chain-risk-label/) ⭐️ 9.0/10

联邦法官 Rita Lin 在周四听证会上表示，特朗普政府仍未提供足够证据来证明将 Anthropic 列为「供应链风险」的合理性，目前正考虑永久撤销该禁令。法官称政府因 Anthropic 公开批评国防部而实施惩罚的逻辑「非常令人不安」，并表示案卷记录「在某些方面对政府而言变得更糟了」。 此案树立了重要的法律先例，保护联邦承包商在军事 AI 使用上设定伦理边界时免受政府报复，直接影响 AI 政策、国家安全与公民自由三者之间的平衡。该裁决可能重塑政府在采购权力与承包商对其技术施加伦理约束的权利之间如何取舍的方式。 争端源于 Anthropic 与国防部合同谈判破裂：Anthropic 要求其 AI 不被用于对美国人进行大规模监控或致命武器决策，国防部则认为私营企业不应规定军方如何使用技术。Anthropic 于 3 月提起两起诉讼，Lin 法官此前已发布临时禁令叫停封禁；政府律师表示计划在 9 月 30 日前完成停用 Anthropic 产品。

telegram · zaihuapd · 7月31日 08:00

**背景**: 2026 年 2 月 27 日，特朗普总统指示所有联邦机构在六个月内停用 Anthropic 的 AI 技术，国防部长 Hegseth 宣布即将实施供应链风险认定。「供应链风险」标签是一种联邦采购机制，允许政府将被认为对国家安全或供应链完整性构成风险的承包商排除在外。2026 年 3 月，法官最初已阻止政府将 Anthropic 列为供应链风险，这被视为 Anthropic 在与政府法律战中的初步胜利。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mayerbrown.com/en/insights/publications/2026/03/anthropic-supply-chain-risk-designation-takes-effect--latest-developments-and-next-steps-for-government-contractors">Anthropic Supply Chain Risk Designation Takes Effect — Latest ...</a></li>
<li><a href="https://www.cbsnews.com/news/anthropic-ruling-judge-trump-pentagon-ai/">Judge blocks Pentagon from labeling Anthropic AI a &quot;supply ...</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI Ethics`, `#Government Policy`, `#Legal`, `#National Security`

---

<a id="item-3"></a>
## [Simon Willison 谈 AI 开放权重革命](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 8.0/10

Simon Willison 做客 Bryan Cantrill 和 Adam Leventhal 的 Oxide and Friends 播客，讨论了 AI 领域具有里程碑意义的一周，包括 Kimi K3 证明开放权重模型可以媲美专有前沿模型、AI 驱动的意外网络安全攻击，以及除 Anthropic 外几乎所有 AI 巨头签署的关于开放权重的行业公开信。对话还涵盖了从 Golden Gate Claude 到齐齐安派等多个话题，甚至预测教皇将在年底前就开放模型发表评论。 Kimi K3 拥有 2.8 万亿参数的开放权重模型达到前沿级别性能，标志着一个关键时刻，表明免费可用的模型已经能够与 OpenAI 和 Google 的专有产品竞争。与此同时，业界近乎一致支持开放权重与 Anthropic 显著反对之间的尖锐分歧，预示着一场将影响未来数年 AI 监管、可及性和国家安全的根本性政策辩论。 Kimi K3 是一个拥有 2.8 万亿参数的模型，基于 Kimi Delta Attention 和 Attention Residuals 构建，具备原生视觉能力和 100 万 token 的上下文窗口，是全球首个开放的三万亿级别模型。该播客录制于 DeepSeek V4 Flash（一个拥有 2840 亿参数、130 亿激活参数的 MoE 模型）和 Anthropic 网络安全事件公布之前，Willison 表示这两件事如果录制时间稍晚都会被讨论到。

rss · Simon Willison · 7月31日 21:33

**背景**: 开放权重模型是指将训练好的参数（权重和偏置）公开发布的 AI 模型，允许任何人下载、检查、修改并在自己的基础设施上运行，这与仅提供 API 访问的专有模型形成对比。随着 Kimi（月之暗面）和 DeepSeek 等中国实验室的模型展现出媲美领先专有模型的性能，开放权重运动获得了显著动力。与此同时，政策层面的争论也在升温：微软发布了一封由大多数主要 AI 公司签署的信件，主张开放权重对美国 AI 领导地位至关重要，而 Anthropic 则发表了不同意见，援引威权政权利用开放模型带来的国家安全担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>
<li><a href="https://www.anthropic.com/news/position-open-weights-models">Our position on open-weights models \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Weights`, `#LLM`, `#Cybersecurity`, `#Podcast`

---

<a id="item-4"></a>
## [以 GPT-5.6 推进性价比前沿](https://simonwillison.net/2026/Jul/30/luna-price-drop/#atom-everything) ⭐️ 8.0/10

OpenAI 宣布大幅下调 GPT-5.6 模型的价格。这得益于使用 GPT-5.6 Sol，通过预计算和并行化技术优化了负载均衡与推理计算。

rss · Simon Willison · 7月30日 23:58

**标签**: `#openai`, `#llm-pricing`, `#inference-optimization`, `#gpt-5.6`, `#ai-economics`

---

<a id="item-5"></a>
## [🤖 DeepSeek-V4-Flash 正式版 API 上线公测](https://api-docs.deepseek.com/zh-cn/updates) ⭐️ 8.0/10

DeepSeek 宣布 V4-Flash 正式版 API 开启公测，其 Agent 能力得到显著增强，且基准测试性能超越了 V4-Pro-Preview。

telegram · zaihuapd · 7月31日 05:50

**标签**: `#DeepSeek`, `#LLM`, `#AI Agents`, `#API Release`, `#Benchmark`

---

<a id="item-6"></a>
## [华为开源 505B 参数 MoE 大模型 openPangu-2.0-Pro](https://huggingface.co/openpangu/openPangu-2.0-Pro) ⭐️ 8.0/10

华为在 Hugging Face 上发布了开源大模型 openPangu-2.0-Pro，该模型总参数约 505B，每 token 激活约 18B，基于昇腾 NPU 训练，采用 MLA 注意力机制、DSA+SWA 独立分层混合设计以及 3 头 MTP 自投机模块。Thinking 版本在 AIME 2026 测评中得分 95.4，GPQA-Diamond 得分 87.9。 这是目前最大的开源 MoE 模型之一，其训练基于华为昇腾 NPU 而非 NVIDIA GPU，证明了非 NVIDIA 硬件栈在前沿规模模型训练上的可行性，对 AI 硬件多元化具有重要意义。其具有竞争力的基准分数和完全开源的发布方式，降低了研究人员和开发者研究及部署最先进架构的门槛。 模型采用 MLA（多头潜在注意力）通过低秩潜在表示压缩 KV 缓存，而 DSA+SWA 混合设计将用于局部上下文的滑动窗口注意力与用于长距离依赖的动态选择注意力相结合，将注意力复杂度从二次降低到线性。3 头 MTP 模块无需单独的草稿模型即可实现自投机解码，后训练阶段采用快慢合一微调与多专项强化学习。

telegram · zaihuapd · 7月31日 06:50

**背景**: MoE（混合专家）架构每次只激活部分参数，从而在不按比例增加推理成本的情况下提升模型总容量。MLA（多头潜在注意力）最早由 DeepSeek-V2 提出，通过存储键值对的压缩潜在表示而非完整张量来减少 KV 缓存的内存占用。SWA（滑动窗口注意力）将每个查询限制在固定局部窗口内以实现线性复杂度，而 DSA（动态选择注意力）通过基于内容的选择保留远距离 token；两者结合可实现高效的长上下文处理。MTP（多 token 预测）是一种投机解码技术，利用模型自身的多 token 预测头提前生成多个未来 token，并在单次前向传播中验证，在不损失质量的前提下加速生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/mla/">Multi-Head Latent Attention (MLA) | Sebastian Raschka, PhD</a></li>
<li><a href="https://www.pythonalchemist.com/llm-architectures/attention-variants">Attention Variants Explained: MHA, GQA, MQA, MLA, SWA , DSA</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#open-source`, `#moe-architecture`, `#huawei`, `#ascend-npu`

---

<a id="item-7"></a>
## [德国法院裁定 AI 音乐公司 Suno 侵犯版权](https://www.dw.com/en/german-court-rules-that-ai-music-firm-suno-violated-copyrights/a-78152227) ⭐️ 8.0/10

慕尼黑地区法院周五裁定，美国 AI 音乐公司 Suno 未经许可使用受版权保护的音乐训练 AI 模型，构成版权侵权，须披露非法所得并支付数额待定的赔偿。该诉讼由 GEMA 于 2025 年 1 月提起，Suno 表示不认同判决，将评估包括上诉在内的所有选项。 这是全球首批检验版权法如何适用于 AI 音乐训练的重大法院裁决之一，树立的判例可能重塑整个欧洲乃至全球生成式 AI 公司的许可实践。该决定表明未经许可使用受版权保护的内容训练 AI 将承担法律后果，可能迫使行业转向许可数据协议模式。 庭审中，GEMA 演示了 Suno 生成的歌曲与原版权作品高度相似。GEMA 代表德国逾 9.5 万名音乐人及全球超 200 万名权利持有人，其表示目标是推动平等的许可谈判，而非完全阻止 AI 发展。

telegram · zaihuapd · 7月31日 13:11

**背景**: Suno 是一家美国 AI 音乐公司，允许用户通过文本提示生成完整歌曲，已成为生成式 AI 音乐领域最知名的公司之一。GEMA 是德国的音乐表演和机械复制权集体管理组织，类似于美国的 ASCAP 或 BMI。此案是全球内容创作者就 AI 公司未经授权使用版权作品训练模型提起诉讼的更广泛浪潮的一部分。

**标签**: `#AI Copyright`, `#Generative AI`, `#Legal`, `#Music AI`, `#Suno`

---

<a id="item-8"></a>
## [Tailscale 发布 Hugging Face 泄露认证密钥入侵事件的详细复盘](https://tailscale.com/blog/hugging-face-intrusion) ⭐️ 7.0/10

Tailscale 发布了一份详细的事件复盘，揭示了攻击者入侵 Hugging Face 后在环境文件中发现的 136 个凭据中找到了一个可复用的 Tailscale 认证密钥，并在数天内利用该密钥向 Hugging Face 的 tailnet 中注册了 181 个恶意节点，每个节点都继承了 CI 级别的访问权限。 这一事件突显了 CI/CD 流水线中密钥管理不当的连锁风险——单个泄露的可复用认证密钥就能让攻击者获得对整个 mesh VPN 网络的持久访问权限。Tailscale 在自身产品没有漏洞被利用的情况下仍选择公开分析该事件，体现了纵深防御的理念，也为整个行业在密钥管理和异常检测方面提供了实用借鉴。 泄露的认证密钥属于可复用类型，而 Tailscale 官方文档明确建议避免使用此类密钥，因为它可以被多次用于注册无限数量的节点；推荐的替代方案是使用一次性认证密钥或通过环境变量传递密钥。181 个恶意节点每个都获得了带有 CI 级别访问权限的 Tailscale 身份标签，且数天内的注册行为模式明显异常，可以通过设置节点创建告警来及时发现。

hackernews · bluehatbrit · 7月31日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49127306)

**背景**: Tailscale 是基于 WireGuard 构建的 mesh VPN，它将设备连接成一个称为&quot;tailnet&quot;的私有网络，其中每台设备都是一个可以与其他节点安全通信的节点。认证密钥是一种用于自动将新设备注册到 tailnet 中而无需手动认证的令牌，这在 CI/CD 流水线中尤其有用，因为自动化系统需要加入网络。可复用认证密钥可以被反复使用来注册多个节点，而一次性密钥在使用一次后即失效，因此一旦密钥泄露，后者的安全性要高得多。Hugging Face 的入侵事件发生在攻击者获取了 CI 沙箱的访问权限后，在环境文件中发现了存储的凭据——这是自动化测试环境中常见但存在风险的做法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys">Auth keys · Tailscale Docs</a></li>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys/how-to/secure-auth-keys">Securely handle an auth key · Tailscale Docs</a></li>
<li><a href="https://tailscale.com/learn/understanding-mesh-vpns">Understanding Mesh VPNs - Tailscale</a></li>

</ul>
</details>

**社区讨论**: 社区普遍赞赏 Tailscale 的透明度，指出该公司本可以保持沉默（因为其产品并未被利用漏洞），但选择将该事件视为自身责任来对待，体现了安全工具厂商应有的态度。多位评论者承认这篇文章是&quot;非常高明的营销&quot;，在教育用户的同时推广了 Tailscale 的高级安全功能；也有人争论当攻击者已经获得后门访问权限时，VPN 厂商是否还应承担责任。讨论中还出现了值得关注的特性请求，包括希望增加&quot;安全检查&quot;功能来验证推荐配置，以及建议对异常节点注册模式设置低门槛告警。

**标签**: `#security`, `#tailscale`, `#incident-analysis`, `#secrets-management`, `#mesh-vpn`

---

<a id="item-9"></a>
## [电梯调度算法的交互式探索](https://john.fun/elevators) ⭐️ 7.0/10

一个探索电梯调度算法的交互式项目被分享，允许用户可视化和比较不同的调度策略。该帖子引发了广泛的社区讨论，获得了 806 个赞和 207 条评论，涵盖了算法比较和实际应用场景。 电梯调度是一个经典的系统设计问题，其算法可以直接迁移到磁盘 I/O 调度等其他领域，使其成为理解资源分配中优化权衡的有价值视角。社区讨论将该项目从一个简单的可视化提升为对调度算法如何跨工程领域应用的更深层技术探索。 项目探索的 SCAN 算法与 HDD 中使用的同名磁盘调度算法直接对应，磁盘臂沿一个方向服务请求后再反向运动。评论者指出，项目的随机目的地模型可能未反映真实世界的交通模式，在现实中目的地调度系统按目的楼层对乘客分组以提高效率。

hackernews · Jrh0203 · 7月31日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49124218)

**背景**: 电梯调度算法决定电梯如何选择服务楼层及其顺序，需要在等待时间、运行时间和能效之间取得平衡。SCAN 算法又称电梯算法，沿一个方向服务请求直到终点再反向，这一原理同样用于硬盘磁头调度。目的地调度系统是一种现代方法，乘客在登梯前输入目的楼层，系统据此将前往同一楼层的乘客分配到同一电梯轿厢。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/dsa/scan-elevator-disk-scheduling-algorithms/">SCAN (Elevator) Disk Scheduling Algorithms - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 评论者深入指出电梯调度与 HDD 磁盘调度（SCAN 算法）之间的类比，电梯问题本质上是磁盘臂运动的一维版本。来自真实世界的观察包括目的地调度系统在集群交通模式（如午餐高峰前往底层）下表现优于随机模型所暗示的效果。用户还分享了 Elevator Saga 等相关交互资源，并提出了实际的 UX 痛点，如无法取消误按的按钮。

**标签**: `#algorithms`, `#scheduling`, `#simulation`, `#systems-design`, `#optimization`

---

<a id="item-10"></a>
## [qm：YC 支持的多人协作 AI Agent 管理框架](https://github.com/yc-software/qm) ⭐️ 7.0/10

qm 是一个获得 YC 支持的开源项目，作为多人协作的 Agent 管理框架发布，使团队能够通过个人作用域和共享房间来管理多个 AI 编程 Agent。该工具引入了组织级别的协调原语——如分级 Agent 访问权限和共享协作空间——专为全公司范围的 AI Agent 编排而设计。 随着团队越来越多地同时部署多个 AI 编程 Agent，最难的问题已被证明是作用域控制和访问管理，而非 Agent 循环本身，这使得 qm 的个人作用域和共享房间成为及时的架构解决方案。该工具诞生于行业从单 Agent 工作流向多 Agent 编演转变的关键时刻，来自邻近构建者如 AQ 的社区验证也证实了该品类的重要性。 qm 的核心设计围绕个人作用域（限定每个 Agent 可见和可操作的范围）以及共享房间（作为多个 Agent 和人类协作的空间）展开。该项目在 GitHub 上开源，由 YC 支持的团队构建，但部分社区成员指出其文档在说明工具功能和与 Claude Cowork 等替代方案的差异方面可以更清晰。

hackernews · tosh · 7月31日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=49126604)

**背景**: Agent 框架是围绕大语言模型构建的软件基础设施，使模型能够作为 AI Agent 运行——管理工具调用、记忆、状态持久化、执行环境和反馈循环。多 Agent 编排将此概念扩展为协调多个专业化 AI Agent 作为统一系统协同工作，将复杂问题分解为专门的工作单元。随着各组织采用 AI Agent 进行编程和其他任务，挑战已从构建能力强大的单个 Agent 转向管理多个 Agent 如何交互、共享上下文并尊重组织边界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/ai-agent-design-patterns">AI Agent Orchestration Patterns - Azure Architecture Center | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 讨论中浮现出一个关键洞察：构建者 knighthacker 指出多人 Agent 中最难的问题是作用域控制而非 Agent 循环本身，qm 的个人作用域加共享房间是&\#x27;全公司助手的合理方案&\#x27;。评论者将其与 Orca、Gary Tan 的 gstack 和 AQ 等邻近工具进行了比较，一位用户幽默地讲述了给 Agent 自己的 Slack 频道后它竟然自主开始与其他 Agent 安排会议的经历。也有评论对与 Claude Cowork 等现有产品的差异化表示质疑，呼吁进行直接对比。

**标签**: `#ai-agents`, `#multiplayer-agents`, `#developer-tools`, `#llm-orchestration`, `#yc-backed`

---

<a id="item-11"></a>
## [开源 Transformer 模型用于糖尿病血糖水平预测](https://www.reddit.com/r/MachineLearning/comments/1vc1txc/i_have_trained_a_model_to_predict_my_blood_sugar_p/) ⭐️ 7.0/10

一位爱好者训练了一个 BERT 风格的纯编码器 Transformer，使用 8 至 24 小时的变长上下文，结合过去的血糖、碳水化合物和胰岛素数据以及未来的餐饮和胰岛素输入来预测未来 2 小时的血糖水平。该项目使用 DILATE 损失拟合中位数、pinball 损失拟合不确定性区间并通过 Kendall-Gal 混合，还采用了 Kovatchev 风险空间重参数化，训练了四个模型尺寸（最大约 1700 万参数），并在模拟器和真实 T1DM 数据集上进行了训练。 该项目展示了 Transformer 架构如何有效应用于个性化医疗预测任务，提供了一个可在手机本地运行的血糖预测开源工具。以 MIT 许可证发布并附带训练权重和评估数据，为从事医疗时间序列预测的机器学习从业者提供了有价值的参考，尤其对糖尿病管理社区具有重要意义。 最大模型约有 1700 万参数（16 层 16 头），预训练耗时约 48 小时，微调不到 10 分钟；作者还在个人数据上微调了一个版本，目前在其手机上运行。一个显著的局限是模型始终需要输入未来已知的碳水化合物和胰岛素信息，尚无法在缺少这些输入的情况下进行预测，作者已将此列为待改进方向。

reddit · r/MachineLearning · /u/0xdeadf1sh · 7月31日 20:09

**背景**: DILATE（包含形状和时间的失真损失）是一种用于多步时间序列预测的可微分训练目标，同时考虑波形形状和事件时序，对于非平稳信号比标准均方误差更有效。Kendall-Gal 不确定性估计利用 dropout 作为贝叶斯近似，从神经网络中产生校准的不确定性估计，使模型能够输出概率性预测区间。Kovatchev 风险空间是一种血糖值重参数化方法，将读数映射到风险尺度，强调临床危险范围（低血糖和高血糖），而非对所有预测误差一视同仁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/vincent-leguen/DILATE">vincent-leguen/ DILATE | DeepWiki</a></li>
<li><a href="https://openreview.net/pdf?id=r1ld_NBxIB">Shape and Time Distortion Loss for Training Deep</a></li>
<li><a href="https://openreview.net/pdf?id=RTeIGQtIfq">Fast Calibrated Uncertainty for Regression</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#Healthcare`, `#Transformers`, `#Time Series Forecasting`, `#Diabetes`

---

<a id="item-12"></a>
## [If reviewing is mandatory for paper submissions, low-quality reviews can no longer be justified as “volunteer work” \[D\]](https://www.reddit.com/r/MachineLearning/comments/1vbeqhw/if_reviewing_is_mandatory_for_paper_submissions/) ⭐️ 7.0/10

The author argues that since AI conferences now mandate reviewing for paper submissions, reviewers must provide concrete, professional justifications rather than abstract, generic criticisms.

reddit · r/MachineLearning · /u/Kwangryeol · 7月31日 03:05

**标签**: `#Machine Learning`, `#Peer Review`, `#Academic Research`, `#Conferences`

---

<a id="item-13"></a>
## [MiniMax 多模态视频模型 H3 将于 8 月 3 日开源](https://modelscope.cn/models/MiniMax/MiniMax-H3) ⭐️ 7.0/10

MiniMax 宣布其全新多模态视频模型 H3 将于魔搭社区（ModelScope）平台开源。该模型能够理解和生成文本、图像、音频与视频，并具备商业编辑能力。

telegram · zaihuapd · 7月31日 12:37

**标签**: `#multimodal-ai`, `#video-generation`, `#open-source`, `#MiniMax`, `#ModelScope`

---