---
layout: default
title: "Horizon Summary: 2026-11-28 (ZH)"
date: 2026-11-28
lang: zh
---

> 从 10 条内容中筛选出 7 条重要资讯。

---

1. [热门购物网站发现利用 WebRTC 的信用卡盗刷脚本](#item-1) ⭐️ 8.0/10
2. [Convex 技能插件被指未经披露上传用户应用创意](#item-2) ⭐️ 8.0/10
3. [多州总检察长起诉 SpaceX 和 xAI，指控 Grok 生成有害图像](#item-3) ⭐️ 8.0/10
4. [迈克尔·尼尔森因 AI 安全担忧下架神经网络书籍](#item-4) ⭐️ 8.0/10
5. [谷歌 DeepCrossAttention 实现 Transformer 训练最高 3 倍加速](#item-5) ⭐️ 7.0/10
6. [Show HN: Bouncemarket——弹跳球的实时预测市场游戏](#item-6) ⭐️ 7.0/10
7. [D.J. Bernstein 批评对计算机验证证明的依赖](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [热门购物网站发现利用 WebRTC 的信用卡盗刷脚本](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 8.0/10

安全研究人员在热门购物网站上发现了滥用 WebRTC 数据通道的信用卡盗刷脚本，这些脚本在黑色星期五期间特别针对移动设备进行攻击。脚本被注入到结账页面以窃取支付卡信息。 这一发现凸显了电子商务网站上第三方脚本的持续风险，并表明攻击者不断调整技术以逃避检测。它影响在线购物者，尤其是移动用户，并强调了加强客户端安全控制的必要性。 这些盗刷脚本利用 WebRTC 数据通道，因为该通道较少被监控恶意活动，并且针对移动设备，因为它们更难被检测。这种攻击也可以用简单的 HTTP 请求实现，表明核心漏洞在于第三方脚本的引入。

hackernews · scanr · 11月27日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50668145)

**背景**: WebRTC 是一种浏览器 API，支持实时点对点通信，包括可以传输任意数据的数据通道。信用卡盗刷脚本通常被称为 Magecart 攻击，是注入到结账页面的恶意 JavaScript，用于窃取支付信息。第三方脚本通常被嵌入电子商务网站用于分析、广告和功能，但如果被入侵会引入供应链风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-google-apps-script-to-steal-credit-cards-bypass-csp/">Hackers abuse Google Apps Script to steal credit cards , bypass CSP</a></li>
<li><a href="https://www.akamai.com/glossary/what-is-magecart">What Is Magecart ? | Akamai</a></li>
<li><a href="https://webrtc.org/getting-started/overview">Getting started with WebRTC</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了根本原因，一些人认为屏蔽广告是合理的，而另一些人指出问题不在于 WebRTC 的技术能力，而在于缺乏监控。一些人建议对广告进行沙箱隔离以阻止 JavaScript 执行，还有一些人批评网络允许第三方代码执行的设计，呼吁在支付中采用非对称加密。

**标签**: `#security`, `#web-security`, `#webrtc`, `#credit-card-skimming`, `#third-party-scripts`

---

<a id="item-2"></a>
## [Convex 技能插件被指未经披露上传用户应用创意](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 8.0/10

GitHub 议题（convex/convex-backend-skill#64）指控 Convex 的技能插件在未告知用户的情况下将应用创意上传至远程服务器，在 Hacker News 上引发 239 分、76 条评论的讨论。Convex CEO Jamie 回应称，该提示上传用于支持 Convex 的“快速入门”功能，是已停用的 Convex Chef 氛围编程产品的后继。 该事件凸显了 AI 辅助开发者工具中日益增长的隐私与透明度问题，插件可能默认将敏感用户输入传输至远程服务器。这影响了使用 Convex 代理插件的开发者，并引发了对 AI 工具数据处理和用户同意的更广泛质疑。 该插件的提示上传与 Convex 的“快速入门”功能相关，该功能允许开发者用一句话描述应用，由代理生成脚手架。披露问题的核心在于用户是否被充分告知其创意会被发送至远程服务器，讨论还涉及提示注入风险和自托管开放权重模型。

hackernews · MickyTheMouse · 11月27日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50669765)

**背景**: Convex 是一个全栈开发平台，提供数据库、服务器函数和用于构建与托管软件的 AI 网关。它为主要的编码代理发布官方技能和插件，使用户能够通过自然语言描述生成应用脚手架。提示注入是一种将恶意指令隐藏在输入中以操纵 AI 模型行为的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.convex.dev/">Convex | All gas, no breakages</a></li>
<li><a href="https://docs.convex.dev/">Convex Docs | Convex Developer Hub</a></li>
<li><a href="https://shir-man.com/llm-attack/">Prompt Injection Generator | Unicode Stealth Payload Builder</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了其影响：一人指出自托管开放权重模型可能是长期解决方案，另一人指出提示注入比模型自行发起恶意工具调用更常见，第三人则以“创意不值钱”淡化该担忧。还有人对某评论者在议题中推广个人媒体网站感到困惑。

**标签**: `#privacy`, `#security`, `#AI-tools`, `#prompt-injection`, `#developer-tools`

---

<a id="item-3"></a>
## [多州总检察长起诉 SpaceX 和 xAI，指控 Grok 生成有害图像](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 8.0/10

包括弗吉尼亚州和华盛顿特区在内的多位州总检察长对 SpaceX 及其子公司 xAI 提起诉讼，指控其 Grok 人工智能模型生成儿童性虐待材料和未经同意的私密图像。诉讼称这些公司未能实施充分的保护措施，引发了一场关于 AI 平台责任的法律战。 这起诉讼标志着对生成式 AI 监管审查的显著升级，可能为追究 AI 开发者对其模型造成伤害的责任树立先例。它可能影响平台审核内容的方式，并加速监管 AI 生成露骨材料的立法努力。 诉讼针对 Grok 的图像生成功能，该功能因审查极少且易于规避而受到批评。它还凸显了 AI 生成内容中年龄验证和同意的挑战，因为 Grok 需要关联 X 账户，引发了隐私担忧。

hackernews · DeepLogin · 11月27日 19:42 · [社区讨论](https://news.ycombinator.com/item?id=50670855)

**背景**: Grok 是由埃隆·马斯克于 2023 年创立的 xAI 开发的 AI 助手，现为 SpaceX 的子公司。与其他 AI 模型相比，它以内容限制极少而闻名。这起诉讼正值全球对 AI 生成的未经同意的私密图像日益关注之际，诸如《TAKE IT DOWN 法案》等新兴法律旨在追究平台责任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">XAI (company)</a></li>
<li><a href="https://olartemoure.com/en/ai-non-consensual-intimate-images/">Misuse of AI to generate non - consensual intimate images</a></li>
<li><a href="https://www.igniterstech.com/publications/the-take-it-down-act-a-new-era-of-combat-against-nonconsensual-intimate-imagery">The Take It Down Act: A New Era of Combat Against Nonconsensual ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对于 Grok 如何能生成此类内容表示困惑，因为它需要关联 Twitter 账户，并质疑用户是否必须欺骗模型。一些人还询问制作这些图像的个人应承担的责任，而另一些人则指出为尝试该模型而交出社交媒体账户的隐私风险。

**标签**: `#AI ethics`, `#content moderation`, `#legal`, `#xAI`, `#Grok`

---

<a id="item-4"></a>
## [迈克尔·尼尔森因 AI 安全担忧下架神经网络书籍](https://neuralnetworksanddeeplearning.com/) ⭐️ 8.0/10

迈克尔·尼尔森已从其网站下架免费在线书籍《神经网络与深度学习》，表示不再希望帮助为前沿 AI 工作培养人才。此举在 Hacker News 上引发了 267 条评论的讨论，涉及 AI 安全、开放获取以及这一决定背后的动机。 这本书曾是广泛使用的高质量教育资源，向许多从业者介绍了神经网络，因此其下架凸显了开放 AI 教育与对灾难性 AI 风险的担忧之间日益紧张的关系。这也引发了疑问：扣留知识究竟是有效的抗议形式，还是仅仅将学习者推向存档副本。 尼尔森给出的理由是不希望为前沿 AI 实验室培养人才，并将此举定位为抗议而非技术变革。由于该书多年来免费在线提供，存档版本仍可通过互联网档案馆访问，而下架可能反而增加人们对这些材料的兴趣。

hackernews · brandonb · 11月27日 19:31 · [社区讨论](https://news.ycombinator.com/item?id=50670757)

**背景**: 迈克尔·尼尔森是一位知名的开放科学和深度学习研究者与作家，他的《神经网络与深度学习》自 2010 年代中期以来一直是该领域广受欢迎的免费入门读物。近年来，尼尔森撰写了关于人工超级智能存在性风险的文章，认为前沿 AI 开发构成严重风险。Hacker News 上的讨论反映了 AI 社区关于安全、开放研究和教育者责任的更广泛辩论。

**社区讨论**: 评论者意见分歧：一些人认为下架这本书是失策，因为理解神经网络有助于公众了解大公司在构建什么；另一些人则认为这是一种象征性抗议，主要只会促使人们转向存档副本。几位评论者指出，巨额资本投资和广泛的 ETF 持仓意味着许多人都间接参与了前沿 AI 开发，还有一位评论者附上了该书的互联网档案馆快照链接。

**标签**: `#neural-networks`, `#AI-safety`, `#open-education`, `#community-discussion`, `#protest`

---

<a id="item-5"></a>
## [谷歌 DeepCrossAttention 实现 Transformer 训练最高 3 倍加速](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 7.0/10

谷歌研究院提出了 DeepCrossAttention（DCA），这是一种类似深度注意力（depthwise attention）的机制，用可学习的、依赖输入的权重动态组合跨层表示，替代 Transformer 中的标准残差连接。该方法在保持模型质量相当的同时，训练速度最高可提升 3 倍。 这项研究有望显著降低大型 Transformer 模型的训练成本和时间，使深度架构对资源受限的团队更加实用。它也顺应了通过重新设计残差连接和注意力原语来提升深度学习系统效率的更广泛趋势。 DCA 在深度方向上对 Query、Key 和 Value 组件使用依赖输入的交叉注意力，完整论文可在 arXiv（2502.06785）上获取。该工作发表于 2025 年，社区成员指出 AttnRes 和循环层等相关方法可能进一步放大收益。

hackernews · ComputedCamp995 · 11月27日 23:06 · [社区讨论](https://news.ycombinator.com/item?id=50672565)

**背景**: Transformer 依赖残差连接（跳跃连接）来有效训练深度网络，它像信息高速公路一样帮助梯度流动。注意力机制让模型能够权衡不同输入的重要性，而近期研究探索在深度方向（跨层而非仅跨 token）应用类似注意力的操作来改进表示学习。DeepCrossAttention 属于用学习到的动态组合替代静态残差加法的一系列工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.06785v1">DeepCrossAttention : Supercharging Transformer Residual Connections</a></li>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections - Google Research</a></li>
<li><a href="https://www.alphaxiv.org/overview/2502.06785v1">DeepCrossAttention : Supercharging Transformer Residual... | alphaXiv</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了完整的 arXiv 论文，并提到该工作来自 2025 年，因此并非全新。一些人讨论了 AttnRes 和循环层等相关技术，认为将它们与 DCA 结合可能带来更大收益，另一些人则分享了关于模型速度和成本的轶事经验。

**标签**: `#transformers`, `#attention-mechanisms`, `#machine-learning`, `#model-training`, `#google-research`

---

<a id="item-6"></a>
## [Show HN: Bouncemarket——弹跳球的实时预测市场游戏](https://bouncemarket.minhanhday.com/) ⭐️ 7.0/10

一位开发者推出了 bouncemarket，这是一个实时预测市场游戏，玩家对服务器模拟的弹跳球落点进行投注。游戏具有确定性回放、服务器发送事件流以及当超过五名真人玩家加入时退出的 AI 交易者。 该项目展示了预测市场机制在纯混沌物理模拟中的新颖应用，引发了关于机器人对战动态和事件合约法律地位的讨论。它同时也是通过 SSE 流式传输服务器端确定性模拟的技术展示。 球的下落由服务器端模拟，并通过带有小缓冲的服务器发送事件流式传输到客户端，确保从相同起始位置进行确定性回放。然而，由于混沌动力学，起始位置的微小变化可能大幅改变结果，而 AI 交易者使用基于规则的简单系统，很容易被击败。

hackernews · mday404 · 11月27日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=50667726)

**背景**: 预测市场是参与者交易二元合约的金融市场，合约根据事件结果支付。服务器发送事件（SSE）是一种网络技术，允许服务器通过持久 HTTP 连接向浏览器推送实时更新。混沌系统是确定性的，但对初始条件高度敏感，使得长期预测变得困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Server-sent_events">Server-sent events</a></li>

</ul>
</details>

**社区讨论**: 评论者认为游戏有趣，但指出赔率变化太快使投注困难，一些人发现低价买入两边股票可以保证盈利。其他人讨论了 AI 机器人主导的可能性以及预测市场对随机事件的法律影响。

**标签**: `#prediction-markets`, `#game-development`, `#server-sent-events`, `#chaotic-systems`, `#show-hn`

---

<a id="item-7"></a>
## [D.J. Bernstein 批评对计算机验证证明的依赖](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

D. J. Bernstein 发布了一个页面，列举了七种证明检查器（HOL Light、Mizar、Metamath、Isabelle、Lean、HOL98/HOL4 和 Coq/Rocq）中的健全性错误，认为这些错误削弱了对计算机验证证明的信任，并呼吁使用更小的可信检查器以及检查器正确性的机器验证证明。 这一批评很重要，因为形式验证在数学和软件中越来越多地被使用，而检查器中的健全性错误可能使许多证明失效；这场辩论凸显了对稳健验证实践的需求，并影响研究人员、工具开发者和依赖这些系统的用户。 该页面列出了每个检查器的具体健全性错误，并主张减少可信计算基础；然而，评论者指出，在实践中通常需要多个独立的验证器（例如，Metamath 证明必须通过五个独立创建的验证器），因此单个错误不足以导致广泛的错误接受。

hackernews · _tk_ · 11月27日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=50667989)

**背景**: 像 Lean 和 Metamath 这样的证明助手是用于形式化和验证数学证明的工具；它们的内核检查证明的正确性，但这些检查器中的错误（健全性错误）可能导致错误陈述被接受为已证明。形式验证社区早已意识到此类错误，并开发了使用多个独立检查器等实践来增加信心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metamath">Metamath - Wikipedia</a></li>
<li><a href="https://news.lavx.hu/article/d-j-bernstein-catalogs-soundness-bugs-in-seven-proof-checkers">D. J. Bernstein catalogs soundness bugs in seven proof ...</a></li>

</ul>
</details>

**社区讨论**: HN 评论者讨论了实际影响：twotwotwo 和 dwheeler 强调，多个独立验证器（例如 Metamath 有五个）使得单个健全性错误很难误导数学家，而 gr_norm 指出已知的健全性错误很少，并且需要进一步利用才能隐藏真正的问题。andai 提出了更深层的担忧：代理根据自己对问题的错误理解来证明正确性。

**标签**: `#formal-verification`, `#proof-assistants`, `#soundness`, `#lean`, `#metamath`

---