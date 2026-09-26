---
layout: default
title: "Horizon Summary: 2026-09-26 (ZH)"
date: 2026-09-26
lang: zh
---

> 从 29 条内容中筛选出 15 条重要资讯。

---

1. [陶哲轩：AI 时代需要更多数学家](#item-1) ⭐️ 8.0/10
2. [Hacker News 热议：在 LLM 时代如何保持编程乐趣](#item-2) ⭐️ 8.0/10
3. [Conversations 因支持不佳和费用问题离开 Google Play 并转为免费](#item-3) ⭐️ 8.0/10
4. [DeepSeek 发布面向大规模智能体训练的 DSec 沙箱系统](#item-4) ⭐️ 7.0/10
5. [Reladraw：让你掌控元素布局的图表语言](#item-5) ⭐️ 7.0/10
6. [十五年后回顾苹果 Cards 应用的起源故事](#item-6) ⭐️ 7.0/10
7. [《经济学人》警告：考试成绩下滑是一场缓慢发展的灾难](#item-7) ⭐️ 7.0/10
8. [Floci：免费开源工具可在本地模拟任意云服务](#item-8) ⭐️ 7.0/10
9. [Automattic 在试图让 CEO 马特·穆伦维格休假失败后组建新董事会](#item-9) ⭐️ 7.0/10
10. [保险公司称 AI 编码工具令医院成本增加 9.42 亿美元](#item-10) ⭐️ 7.0/10
11. [KoboldCpp 内置轻量级 Agent 框架，仅 9 个工具、2k 系统提示词](#item-11) ⭐️ 7.0/10
12. [修复版 GPT-OSS 聊天模板解决 Unsloth 推理历史 Bug](#item-12) ⭐️ 7.0/10
13. [4 块 RTX 3060 Ti 通过张量并行实现 120 t/s 本地大模型推理](#item-13) ⭐️ 7.0/10
14. [Ling Tiny 3.0 在无 GPU 的 2017 年笔记本上实现智能体编程](#item-14) ⭐️ 7.0/10
15. [Splash 1.1.0 发布，新增 GGUF 量化与 MLX 导入支持](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [陶哲轩：AI 时代需要更多数学家](https://terrytao.wordpress.com/2026/09/24/were-gonna-need-a-lot-more-mathematicians/) ⭐️ 8.0/10

陶哲轩在其博客上发表文章，主张随着 AI 系统能力不断增强，社会将需要更多数学家来理解、验证并论证 AI 驱动设计的安全性。该文章在 Hacker News 上引发了 458 条评论的热烈讨论，聚焦人类理解力不可替代的作用。 这篇文章将 AI 安全重新定义为对人类数学专业能力的需求，而不仅仅是追求更好的模型，其背景是菲尔兹奖得主和研究者们正在争论 AI 在数学中的角色。它影响着数学家、软件工程师，以及所有依赖 AI 生成设计、且必须向公众论证其正确性的人。 陶哲轩的核心论点是：批准一项设计需要人类群体理解它为何有效、以及凭什么相信其安全性，而随着 AI 产出速度超过人类审查能力，这一标准越来越难以满足。讨论还指出，Lean 等形式化验证工具可以检查 AI 生成的证明，但仍需要人类判断来决定什么值得证明以及如何解读结果。

hackernews · srcreigh · 9月26日 02:46 · [社区讨论](https://news.ycombinator.com/item?id=49852717)

**背景**: 陶哲轩是世界上最杰出的数学家之一，曾大量撰文讨论 AI 如何改变数学研究，包括 Lean 等形式化证明助手——它能让计算机机械地验证证明。近期研究表明，基于 LLM 的智能体可以生成证明并由 Lean 进行检查，但不可靠性仍是 AI 用于严肃研究的主要障碍。Hacker News 上的讨论反映了更广泛的争论：在没有深入人类理解的情况下，AI 生成的代码和设计是否值得信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://teorth.github.io/tao-web/ai-views.html">Terence Tao on AI in mathematics (and beyond)</a></li>
<li><a href="https://arxiv.org/abs/2605.22763">[2605.22763] Advancing Mathematics Research with AI-Driven Formal Proof Search</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同人类理解力至关重要，有人提到自己如今在 Claude 生成的代码中发现的 bug 越来越少，担心在交付压力下变得不够谨慎。另一些人认为，学习数学是为了改造思维而非生产商品，没有人类去理解，LLM 的产出毫无用处；还有人观察到，把一切都交给 Claude 的同事会遭遇 XY 问题、糟糕的用户体验和过度复杂的解决方案。

**标签**: `#AI`, `#mathematics`, `#software-engineering`, `#human-comprehension`, `#LLM`

---

<a id="item-2"></a>
## [Hacker News 热议：在 LLM 时代如何保持编程乐趣](https://discourse.haskell.org/t/how-to-keep-enjoying-programming-in-a-world-of-llms/14705) ⭐️ 8.0/10

一篇题为“How to keep enjoying programming in a world of LLMs”的 Hacker News 讨论获得了 134 分和 190 条评论，开发者们分享了 AI 编程助手如何改变他们的动力、技能和满足感的个人经历。该帖子最初来自 Haskell Discourse，讨论中呈现出多样观点，从技能退化、动力丧失，到把繁琐工作交给 LLM 后重新获得乐趣。 随着 GitHub Copilot、Cursor 和 Claude 等基于 LLM 的编程工具成为开发者工作流的标准配置，这场讨论凸显了生产力提升与动手技能、内在动力被侵蚀之间日益加剧的矛盾。这种情绪对工程团队、工具开发者和教育者都很重要，因为他们必须决定如何整合 AI，同时不掏空编程这门手艺的内核。 评论者描述了具体影响：一位开发者表示，把任何任务推给 LLM 都会导致该技能退化，并举例说自己突然难以规划一个小项目的架构；另一位则称在使用智能体编程后完全失去了动力，感觉自己像“在机器人之间搬运数据和权限的肉块”。相反的观点指出，使用速度极快、推理量低的模型（例如 GPT-6 Luna 低努力 + 快速模式）能让开发者全程保持动手，避免长时间等待。

hackernews · signa11 · 9月26日 09:41 · [社区讨论](https://news.ycombinator.com/item?id=49854875)

**背景**: Hacker News 是由 Y Combinator 运营的科技社交新闻网站，聚焦计算机科学与创业，其讨论常常影响行业情绪。GitHub Copilot、Cursor 和 Claude 等基于 LLM 的编程工具能够根据自然语言提示生成、补全和重构代码，自 2023 年以来被广泛采用。“技能退化”指的是当调试或架构规划等任务被委托给 AI 后，因长期不使用而导致已习得能力逐渐减弱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News</a></li>
<li><a href="https://blog.stackademic.com/skill-atrophy-the-engineers-who-cant-debug-without-ai-anymore-afe212162ef7">“ Skill Atrophy ” — the engineers who can’t debug... | Stackademic</a></li>
<li><a href="https://simonwillison.net/2025/Mar/11/using-llms-for-code/">Here’s how I use LLMs to help me write code</a></li>

</ul>
</details>

**社区讨论**: 社区情绪褒贬不一，但整体偏向担忧：多位开发者报告了技能退化、动力丧失以及对生成代码有 bug 的沮丧，而另一些人则表示 LLM 让他们能卸下无聊工作、更享受编程。一个反复出现的主题是汽车修理工的类比——有人喜欢手工工具，有人喜欢用软件调校——还有一位评论者建议使用快速、低推理的模型来保持动手参与感。

**标签**: `#LLM`, `#programming`, `#developer experience`, `#skill atrophy`, `#Hacker News`

---

<a id="item-3"></a>
## [Conversations 因支持不佳和费用问题离开 Google Play 并转为免费](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 8.0/10

知名开源 XMPP/Jabber 安卓即时通讯客户端 Conversations 的开发者宣布，该应用将离开 Google Play 并转为免费。这一决定源于 Google 对开发者支持不力以及平台收取的费用。 这凸显了独立开源开发者与 Google Play 在安卓应用分发领域主导地位之间日益加剧的矛盾，可能促使更多用户转向直接下载 APK 或使用替代应用商店。这也进一步引发了关于应用商店垄断和开发者待遇的更广泛讨论。 Conversations 是一款面向 Android 6.0+ 的免费开源 XMPP 客户端，强调开放标准，开发者的文章明确将支持不佳和费用列为离开的原因。此举意味着用户需要从 Google Play 之外获取该应用，例如直接下载 APK 或通过其他分发渠道。

hackernews · ezst · 9月26日 10:55 · [社区讨论](https://news.ycombinator.com/item?id=49855315)

**背景**: Conversations 是一款广泛使用的安卓即时通讯应用，基于开放的 XMPP（可扩展消息与存在协议）标准，而非专有协议。Google Play 是大多数安卓设备的默认应用商店，会向开发者收取服务费并执行内容和分发政策。离开它意味着该应用必须依赖直接下载或第三方商店，这可能降低曝光度，但让开发者拥有更多控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conversations_(software)">Conversations (software) - Wikipedia</a></li>
<li><a href="https://conversations.im/">Conversations : the very last word in instant messaging</a></li>
<li><a href="https://support.google.com/googleplay/android-developer/answer/112622?hl=en-EN">Service fees - Play Console Help</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同情开发者，认为如果 Google 能提供良好的支持和及时的审核，15% 的费用是可以接受的，而垄断地位让它得以忽视开发者。多人分享了对 Google 糟糕的客户支持和繁琐验证要求的沮丧，还有人警告安卓正在让 Play 商店之外的应用安装变得越来越困难。

**标签**: `#Google Play`, `#app distribution`, `#monopoly`, `#developer experience`, `#open source`

---

<a id="item-4"></a>
## [DeepSeek 发布面向大规模智能体训练的 DSec 沙箱系统](https://arxiv.org/abs/2609.22978) ⭐️ 7.0/10

DeepSeek 推出 DeepSeek Elastic Compute（DSec），这是一种沙箱基础设施，可在 160 个 AMD EPYC 节点上实现 38 万个并发沙箱，相关细节已在一篇 arXiv 论文中公布。该系统与 DeepSeek 的强化学习框架协同设计，并从 DeepSeek-V4.1 开始将 rollout 执行迁移到 DSec 上，拆分为智能体沙箱和 worker 容器两个组件。 DSec 的规模及其与强化学习训练的紧密耦合，可能大幅降低大规模智能体训练的成本和复杂度，而这是构建强大 AI 智能体的关键瓶颈。该系统的设计也暗示了更广泛的 serverless 计算意义，社区很快注意到了这一点。 DSec 将有状态的 rollout 执行与可抢占的 GPU 训练解耦，并协调沙箱生命周期与训练过程，以在回收空闲资源的同时保留 rollout 状态。该论文还因作者名单异常庞大（131 人）而引人注目，这主导了社区讨论。

hackernews · shenli3514 · 9月26日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=49859112)

**背景**: 在 AI 智能体训练中，沙箱是一个隔离环境，未测试的代码和智能体操作可以在其中运行而不影响生产系统。AMD EPYC 是 AMD 旗下的多核 x86-64 服务器处理器品牌，160 个此类节点承载 38 万个并发沙箱，体现了虚拟化层的密度。DeepSeek 是一家中国 AI 公司，以其大语言模型和强化学习研究而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://technode.com/2026/09/23/deepseek-dsec-agent-training-sandbox-infrastructure/">DeepSeek details DSec sandbox infrastructure for agent training · TechNode</a></li>
<li><a href="https://arxiv.org/html/2609.22978v1">DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者最震惊的是论文的 131 位作者，有人开玩笑说，比起论文主题，这么多作者如何沟通并完成发表更令人感兴趣。其他人对 160 个 EPYC 节点上 38 万个并发沙箱的规模表示难以置信，还有一位评论者直接发问这是否就相当于 serverless 计算。

**标签**: `#deepseek`, `#elastic-compute`, `#serverless`, `#distributed-systems`, `#arxiv`

---

<a id="item-5"></a>
## [Reladraw：让你掌控元素布局的图表语言](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw 是一款新的开源图表语言，它将声明式“图表即代码”工具的便捷性与手动控制元素位置的能力结合起来。它提供了无需安装即可试用的浏览器 Playground、npm 安装包，以及可供 Claude 等 AI 代理使用的 agent skill。 现有的“图表即代码”工具迫使用户做出取舍：Mermaid、Graphviz 等自动布局语言替你决定布局，而 Draw.io 等图形编辑器虽然强大却耗时，且难以被 AI 代理操作。Reladraw 同时面向人类作者和 AI 代理，随着代理驱动开发工作流的增长，它切中了真实的痛点。 该语言采用相对定位指令而非绝对坐标，早期用户认为这对大多数需求已经足够。社区成员报告了一些小 bug，例如某条边未能渲染成曲线箭头，并建议采用与渲染器无关的后端，让同一套布局指令可以适配多种渲染引擎。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**背景**: Mermaid、Graphviz（使用 DOT 语言）和 D2 等声明式图表工具让用户用文本描述图表，再由软件自动计算布局。这种方式快速且便于版本控制，但作者几乎无法决定节点的最终位置，而对于位置本身承载含义的流程图来说，这一点很重要。Reladraw 试图在保留文本工作流的同时，重新赋予用户对布局的控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49858513">Show HN: Reladraw – A diagram language where you... | Hacker News</a></li>
<li><a href="https://6ic.com/news/reladraw-a-new-precision-tool-for-diagram-design-emerges">Reladraw : A New Precision Tool for Diagram Design Emerges</a></li>
<li><a href="https://blog.logrocket.com/complete-guide-declarative-diagramming-d2/">A complete guide to declarative diagramming with D2 - LogRocket Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持正面态度。有人指出 Mermaid 适合时序图、甘特图等固定布局，但在位置至关重要的流程图中表现不佳，并认为相对定位可能已经够用。其他人报告了早期 bug，询问该工具是否必须自带渲染器、能否面向多种后端，并将其与 D2 等替代方案进行比较。还有用户观察到，AI 助手在编写 .dot 图表时遇到的布局问题与人类如出一辙。

**标签**: `#diagramming`, `#developer-tools`, `#visualization`, `#DSL`, `#AI-agents`

---

<a id="item-6"></a>
## [十五年后回顾苹果 Cards 应用的起源故事](https://lexontech.org/fifteen-years-later-the-apple-cards-origin-story) ⭐️ 7.0/10

一篇回顾性文章讲述了苹果 Cards 应用的起源故事，这是苹果于 2011 年推出的从 iPhone 到实体贺卡的服务，文章详细披露了其背后的技术与商业挑战。文章还附带了社区评论，其中包括竞争对手初创公司 Sincerely 联合创始人的亲身讲述，他当时感到自己的公司被苹果的发布"Sherlock 化"了。 这个故事难得地揭示了苹果如何开发和发布产品，以及一次大型平台发布如何颠覆正在构建类似功能的小型初创公司。它还凸显了苹果与美国邮政署之间不寻常的技术合作，表明一个看似简单的消费者功能背后需要多少定制工程。 由于苹果拒绝在信封上印制可见条形码，却又希望实现端到端追踪，苹果与其印刷合作方开发了一种喷涂在信封上的隐形条形码，只有在特定紫外光下才能看见，美国邮政署也同意在寄出时和邮件处理设施中扫描这些卡片。社区评论者还提到，该应用被用于向不上网的家人发送无缝、即兴的照片贺卡，并讨论了凸版印刷与压凹工艺的美学如何影响了这款产品。

hackernews · ksec · 9月26日 09:13 · [社区讨论](https://news.ycombinator.com/item?id=49854693)

**背景**: 苹果的 Cards 应用于 2011 年作为 iPhone 生态系统的一部分发布，允许用户在手机上设计实体贺卡，并由苹果负责印刷和邮寄。"Sherlocking"（Sherlock 化）是苹果开发者社区的一个术语，指苹果将某项功能内置到自己的操作系统中，从而复制第三方应用的功能，可能扼杀该业务。凸版印刷是一种将蘸墨的活字压入纸张的传统印刷工艺，压凹工艺是一种相关的、能产生凹陷压痕的方法，一些评论者认为它影响了从数字到实体贺卡产品的外观与质感。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Card">Apple Card - Wikipedia</a></li>
<li><a href="https://www.apple.com/apple-card/">Apple Card - Apple</a></li>

</ul>
</details>

**社区讨论**: 讨论内容丰富、语气多样：Sincerely 的联合创始人描述了在苹果发布 Cards 时感到被"Sherlock 化"，以及恐惧与愤怒交织的心情；其他人则分享了用该应用向不上网的老年亲属发送即兴照片的个人经历。评论者还批判性地反思了创始人主导型公司，以及凸版印刷和压凹工艺的美学如何塑造了这款产品，增添了个人与技术层面的细节。

**标签**: `#Apple`, `#startups`, `#product development`, `#USPS`, `#Hacker News`

---

<a id="item-7"></a>
## [《经济学人》警告：考试成绩下滑是一场缓慢发展的灾难](https://www.economist.com/leaders/2026/09/10/plunging-test-scores-are-a-slow-moving-catastrophe) ⭐️ 7.0/10

《经济学人》于 2026 年 9 月 10 日发表的一篇社论文章指出，学生考试成绩的持续下滑构成一场缓慢发展的灾难，并在 Hacker News 上引发了关于其原因的深入讨论。评论者就人工智能、算法驱动的社交媒体、基于屏幕的学习以及人口结构变化谁才是主因展开了辩论。 标准化考试成绩是衡量未来劳动力技能和经济竞争力的关键指标，因此持续多年的下滑意味着人力资本将遭受长期损害。这场辩论之所以重要，还因为诸如禁止手机、回归纸质教科书、用纸笔代替 Chromebook 等补救措施，都高度依赖于能否正确诊断根本原因。 一位评论者指出，2018 年至 2022 年的下滑幅度与 2022 年至 2026 年相当，因此人工智能的作用并不明确；他还观察到，科学成绩受影响的程度低于更依赖注意力和练习的数学与阅读。另一位评论者认为，若按 2024 年的人口结构重新加权 1998 年 NAEP 八年级阅读成绩，可预测出 4.6 分的下降，与实际 4 分的降幅接近，说明人口结构变化能解释大部分趋势。

hackernews · vinni2 · 9月26日 15:24 · [社区讨论](https://news.ycombinator.com/item?id=49857442)

**背景**: 这篇文章刊登在《经济学人》的社论版块，代表该杂志对重大议题的立场。讨论中提到的“注意力经济”指的是平台通过变现用户有限注意力而形成的竞争性市场；NAEP 即美国国家教育进展评估，常被称为“国家成绩单”，长期追踪美国学生的学业表现。讨论还涉及人工智能对教育影响的持续争论，以及社交媒体对学生注意力、睡眠和学业表现的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.coursera.org/articles/attention-economy">What Is the Attention Economy ? | Coursera</a></li>
<li><a href="https://www.publicschoolreview.com/blog/the-impact-of-social-media-on-students-2026-update">The Impact of Social Media on Students (2026 Update)</a></li>
<li><a href="https://www.clrn.org/how-does-social-media-affect-students-academic-performance/">How Does Social Media Affect Students’ Academic Performance?</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者普遍认同成绩下滑是真实存在的，但对主因看法不一：有人归咎于对人类注意力的优化变现和算法驱动的社交媒体，有人指向人工智能，还有人认为人口结构变化解释了大部分降幅。多位评论者分享了关于禁止手机、回归教科书与手写、乃至体能下降的个人观察，整体情绪是屏幕和在线社交环境已经重塑了孩子们的注意力。

**标签**: `#education`, `#test scores`, `#AI impact`, `#social media`, `#attention economy`

---

<a id="item-8"></a>
## [Floci：免费开源工具可在本地模拟任意云服务](https://floci.io/) ⭐️ 7.0/10

Floci 是一款由社区驱动、采用 MIT 许可证的工具，可在毫秒级本地模拟 AWS、Azure、GCP 和 OCI 服务，无需云账户、认证令牌或付费功能门槛。它提供了 LocalStack 之外的替代方案，并强调可扩展、AI 辅助的测试套件创建，让开发者能够编写自己的云兼容测试并实现相应功能。 本地云模拟解决了开发者的真实痛点，为开发、测试和 CI 提供快速、无需凭证的反馈循环，这对需要在未配置真实基础设施的情况下验证行为的 AI 编程代理尤其有价值。Floci 的社区驱动、AI 辅助方式可能降低贡献新服务模拟的门槛，并挑战 LocalStack 在该领域的主导地位。 Floci 采用 MIT 许可证且免费，无需账户或认证令牌，支持多种云平台，包括 AWS、GCP（Cloud Storage、Pub/Sub、Firestore、Datastore、Secret Manager、IAM、Managed Kafka、Cloud Tasks、Cloud Run）、Azure 和 OCI。讨论中提出的一个关键警告是模拟服务与真实云服务行为之间可能存在漂移，这可能在切换到生产环境时导致严重差异。

hackernews · theanonymousone · 9月26日 08:31 · [社区讨论](https://news.ycombinator.com/item?id=49854416)

**背景**: 像 LocalStack 这样的本地云模拟器在开发者机器上模拟云提供商 API，使应用程序无需配置真实云基础设施即可构建和测试。这对于单元测试、集成测试、CI 流水线和离线开发很有用，但模拟器可能无法完全匹配真实云行为。Floci 作为免费、开源的替代方案进入这一领域，支持多个云提供商并鼓励社区贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://floci.io/">Floci — Local Cloud Emulators</a></li>
<li><a href="https://github.com/floci-io/floci">GitHub - floci-io/floci: Light, fluffy, and always free - The ...</a></li>
<li><a href="https://docs.localstack.cloud/">Welcome to LocalStack Docs</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 Floci 的轻量特性以及编写自定义测试套件的便利性，一位用户指出它比 LocalStack 轻量得多，并且与 Testcontainers 配合良好。其他人则对模拟 API 与真实 API 之间的行为漂移表示担忧，并质疑当云特定代码已被抽象掉时是否还需要模拟器。还有一条幽默的评论指出，“Floci”在罗马尼亚语中意为“阴毛”。

**标签**: `#cloud-emulation`, `#local-development`, `#testing`, `#open-source`, `#developer-tools`

---

<a id="item-9"></a>
## [Automattic 在试图让 CEO 马特·穆伦维格休假失败后组建新董事会](https://techcrunch.com/2026/09/25/automattic-has-a-new-board-after-failed-attempt-to-put-ceo-on-leave/) ⭐️ 7.0/10

Automattic 在原董事会投票决定让 CEO 马特·穆伦维格带薪休假后，组建了一个新的董事会。穆伦维格随后夺回公司控制权，并让参与此事的人离职，他在 X 上将这一事件称为“政变企图”。由于穆伦维格持有约 84% 的投票权，这一事件引发了人们对董事会有效性的质疑。 这是 Automattic 的一则重要公司治理新闻，该公司旗下的 WordPress 支撑着互联网的很大一部分。此事凸显出，在创始人控制的多类别股权结构下，即便董事试图采取行动，董事会也可能形同虚设。其结果可能影响投资者、员工以及更广泛的开源社区对创始人主导型科技公司治理的看法。 据报道，穆伦维格持有 Automattic 约 84% 的投票权，这意味着原董事会让他休假的投票实际上注定失败；他几天后通过 Slack 告诉员工自己已重新掌控公司。社区成员还指出，即将离任的董事会成员据称在短暂的过渡期内为自己批准了丰厚的遣散费。

hackernews · ilamont · 9月26日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=49857572)

**背景**: Automattic 是 WordPress 背后的公司，WordPress 是一个开源发布平台，支撑着全球大量网站；马特·穆伦维格是 WordPress 的联合创始人，也是 Automattic 的创始人兼 CEO。公司董事会通常负责监督管理层并保护股东利益，但在创始人持有绝对多数投票权的多类别股权结构中，董事会的实际权力受到严重限制。这一事件是创始人控制的科技公司中治理机制难以约束创始人的更广泛模式的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/25/automattic-has-a-new-board-after-failed-attempt-to-put-ceo-on-leave/">Automattic has a new board after failed attempt to put... | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Matt_Mullenweg">Matt Mullenweg - Wikipedia</a></li>
<li><a href="https://cryptobriefing.com/mullenweg-regains-automattic-control-board-ouster/">Matt Mullenweg claims he's back in charge at Automattic days after...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍质疑，在穆伦维格持有 84% 投票权的情况下，董事会怎么可能指望成功；一些人称这一尝试是破坏价值的失职行为，另一些人则认为董事会的真正目的可能是获取丰厚的遣散费。少数人为穆伦维格的强势反击辩护，也有人表示这场风波让他们更不愿意使用 WordPress。

**标签**: `#Automattic`, `#WordPress`, `#corporate-governance`, `#Matt Mullenweg`, `#tech-industry`

---

<a id="item-10"></a>
## [保险公司称 AI 编码工具令医院成本增加 9.42 亿美元](https://techcrunch.com/2026/09/26/insurers-claim-ai-is-already-increasing-healthcare-costs/) ⭐️ 7.0/10

蓝十字蓝盾协会（BCBSA）发布了一项基于其理赔数据的分析，结论是医院日益广泛使用 AI 编码与计费工具，在两年内额外推高了 9.42 亿美元的医疗支出。该保险机构称，这些工具通过生成更严重的诊断编码来抬高账单，但并未伴随相应的治疗增加。 这是首批具体且量化的说法之一，指出医院采用 AI 反而推高而非降低了成本，直接挑战了业界关于 AI 会让医疗更便宜的叙事。这一发现可能影响支付方的审计、报销政策以及对 AI 计费工具的监管审查，从而波及医院、保险公司和患者。 9.42 亿美元这一数字来自 BCBSA 对自身理赔数据的分析，其指出的机制本质上是 AI 辅助的“高编码”（upcoding）——即按比实际提供的诊疗更严重或更复杂的病情来计费。医院方面对此解读表示异议，认为 AI 工具提高的是病历记录的准确性，而非虚增收费。

rss · TechCrunch · 9月26日 21:02

**背景**: 高编码（upcoding）是一种长期存在的计费做法，即医疗机构提交的编码所对应的病情比实际提供的诊疗更严重或更复杂，从而获得更高的报销。AI 编码工具可以听取医患对话、自动生成诊断编码并优化理赔提交，支持者称这能减轻行政负担并减少错误。保险公司则认为，同样的自动化可能系统性地抬高诊断和支出，这使其成为围绕 AI 对医疗真实经济影响争论的新焦点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bcbs.com/about-us/association-news/new-bcbsa-research-on-ai-hospital-billing-driving-higher-health-care-costs">New BCBSA Research Shows AI Billing Raises Health Care Costs</a></li>
<li><a href="https://www.medicaldaily.com/blue-cross-ai-coding-medically-complex-hospital-records-479102">Blue Cross Ties $942 Million in Added Hospital Costs to AI Coding...</a></li>
<li><a href="https://cryptobriefing.com/blue-cross-hospital-ai-billion-cost-rise/">Blue Cross report links hospital AI to $1B rise in costs</a></li>

</ul>
</details>

**标签**: `#AI in healthcare`, `#healthcare costs`, `#AI economics`, `#insurance`, `#AI policy`

---

<a id="item-11"></a>
## [KoboldCpp 内置轻量级 Agent 框架，仅 9 个工具、2k 系统提示词](https://www.reddit.com/r/LocalLLaMA/comments/1wqlyp8/introducing_koboldcpp_agent_and_a_plea_for_help/) ⭐️ 7.0/10

由 LostRuins（concedo）维护的流行本地大模型推理工具 KoboldCpp 现已内置 Agent 框架，只需在 Admin 标签页勾选一个复选框或添加 --agent 启动参数即可启用。它自带 9 个工具，包含全部工具定义的系统提示词仅约 2k token，同时还能连接任何兼容 OpenAI Chat Completions 的第三方后端，或通过加载 mcp.json 文件扩展 MCP 工具。 这降低了本地大模型用户使用智能体工作流的门槛，为 Claude Code、Codex 或 Opencode 等配置复杂、体量较重的框架提供了一个更轻量的替代方案。由于 KoboldCpp 在本地 AI 社区中被广泛使用，将智能体能力直接内置到工具中，能让更多用户轻松完成简单的自主任务。 为有效运行，该 Agent 至少需要 28k 上下文和 8k 生成 token（建议更大），并推荐至少 12GB 显存以获得良好体验；它还提供三种工具调用审批模式（on/auto/off），并支持 AGENTS.md 和上下文压缩。需要注意的是，MCP 工具在 KoboldCpp 服务端执行，而 Agent 工具在客户端执行，维护者也提醒用户在批准工具调用时要谨慎。

reddit · r/LocalLLaMA · /u/HadesThrowaway · 9月26日 09:13

**背景**: Agent 框架（也称 agent scaffolding）是包裹在语言模型外部的软件层，使模型能够作为智能体行动：它负责管理工具调用、记忆、状态持久化和多步反馈循环，因此可以理解为“智能体 = 模型 + 框架”。KoboldCpp 本身是一个自包含、易用的文本生成程序，支持 GGML 和 GGUF 模型，基于 llama.cpp 构建，并带有类似 KoboldAI 的界面。此前，想要使用智能体能力的本地用户通常必须额外配置 Claude Code、Codex 或 Opencode 等外部框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://github.com/LostRuins/koboldcpp">GitHub - LostRuins/koboldcpp: Run GGUF models easily with a ...</a></li>
<li><a href="https://grokipedia.com/page/KoboldCpp">KoboldCpp</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#koboldcpp`, `#ai-agents`, `#llm-tooling`, `#open-source`

---

<a id="item-12"></a>
## [修复版 GPT-OSS 聊天模板解决 Unsloth 推理历史 Bug](https://www.reddit.com/r/LocalLLaMA/comments/1wr0wki/improved_and_fixed_template_for_gptoss_again/) ⭐️ 7.0/10

LocalLLaMA 用户 arbv 在 Hugging Face 上发布了更新版的 GPT-OSS Jinja 聊天模板，修复了从 Unsloth 版本继承来的一个严重 bug：当一条消息同时包含推理内容和最终回答时，历史回放阶段只渲染推理部分，导致回答被丢弃。新模板还加入了 preserve_thinking 选项，使多轮推理时能完整保留此前的分析内容。 如今许多推理工具和 API 框架默认会回放此前的推理轮次，因此该 bug 会在常见的多轮对话和智能体工作流中悄悄降低 GPT-OSS 的输出质量。修复后模型能获得正确的上下文，而 preserve_thinking 还能借助前缀缓存加速多轮推理。 Unsloth 模板中出问题的分支在消息同时包含 thinking 和 content 时会丢弃模型的回答，而且其声称“丢弃思维链”的注释本身就是错误的；OpenAI 官方参考模板并没有这个分支。报告者发现 GPT-OSS 20B 会严重跑偏，而 GPT-OSS 120B 往往仅凭推理痕迹就能恢复，并指出 preserve_thinking 会增加 token 消耗，但换来更快的前缀缓存推理。

reddit · r/LocalLLaMA · /u/arbv · 9月26日 20:35

**背景**: GPT-OSS 是 OpenAI 推出的开放权重推理模型系列（20B 和 120B），采用结构化的 harmony 响应格式，将分析通道与最终回答通道分开。聊天模板是 Jinja 文件，负责把对话历史转换成模型期望的精确 token 序列，因此模板有缺陷时会在毫无报错的情况下破坏上下文。Unsloth 是广受欢迎的高效微调与量化推理库，其模板被社区大量复用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/openai/gpt-oss-120b/blob/main/chat_template.jinja">chat _ template .jinja · openai/ gpt - oss -120b at main</a></li>
<li><a href="https://github.com/openai/gpt-oss">GitHub - openai/ gpt - oss : gpt - oss -120b and gpt - oss -20b are two...</a></li>
<li><a href="https://huggingface.co/unsloth/gpt-oss-20b-GGUF">unsloth/gpt-oss-20b-GGUF · Hugging Face</a></li>

</ul>
</details>

**标签**: `#GPT-OSS`, `#chat-template`, `#Unsloth`, `#LocalLLaMA`, `#bug-fix`

---

<a id="item-13"></a>
## [4 块 RTX 3060 Ti 通过张量并行实现 120 t/s 本地大模型推理](https://www.reddit.com/r/LocalLLaMA/comments/1wqv9o8/getting_stupidly_good_results_on_my_4x3060ti_setup/) ⭐️ 7.0/10

一位 r/LocalLLaMA 的 Reddit 用户报告称，他用 4 块 RTX 3060 Ti（每块 8GB 显存，功耗限制在 110W）搭建了一套主机，通过 Exl3 的张量并行实现约 70 t/s 的推理速度，而在 vLLM 上使用 HyperQwen 时，bf16 精度下可达约 120 t/s，并支持最高 15 万 token 的上下文窗口。将 KV 缓存量化为 kv8 后可开启完整的 26.2 万上下文，但吞吐量会回落到约 70 t/s。 这表明消费级 Ampere 显卡（包括最初为挖矿购买的卡）可以被重新利用，组成性能不俗的本地大模型推理集群，而无需购买昂贵的新硬件。它也凸显了张量并行以及 Exl3、HyperQwen 等优化推理栈如何让高吞吐、长上下文的本地推理对爱好者和中小团队变得触手可及。 该配置在四块 8GB 显卡上使用张量并行（TP=4），而 llama.cpp 并不支持这一特性，因此用户转向了 Turboderp 的 Exl3，随后又使用了专为 Ampere 显卡设计的 HyperQwen 仓库。据称并发带来的性能下降几乎可以忽略，因此既可以单智能体以 120 t/s 运行，也可以两个智能体并发并保持大上下文窗口。

reddit · r/LocalLLaMA · /u/DontWinFrensWthSalad · 9月26日 16:47

**背景**: 张量并行将模型的张量拆分到多块 GPU 上，使参数和中间激活都被分片，从而让单卡放不下的模型能够协同运行。Exl3（ExLlamaV3）是 Turboderp 推出的量化与推理项目，把最前沿的量化技术带给消费级硬件；HyperQwen 则是一套针对消费级 Ampere 显卡优化的服务栈，通过 vLLM 高效运行大型 Qwen 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/turboderp-org/exllamav3">GitHub - turboderp -org/exllamav3: An optimized quantization and...</a></li>
<li><a href="https://github.com/syv-ai/HyperQwen">GitHub - syv-ai/HyperQwen: Serve large Qwen models fast on ...</a></li>
<li><a href="https://awsdocs-neuron.readthedocs-hosted.com/en/latest/libraries/nxd-inference/app-notes/parallelism.html">Parallelism Techniques for LLM Inference — AWS Neuron ...</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#multi-gpu`, `#tensor-parallelism`, `#exl3`, `#hardware`

---

<a id="item-14"></a>
## [Ling Tiny 3.0 在无 GPU 的 2017 年笔记本上实现智能体编程](https://www.reddit.com/r/LocalLLaMA/comments/1wqcrly/ling_tiny_30_is_a_glimpse_of_the_future/) ⭐️ 7.0/10

一位 Reddit 用户展示了 Ling Tiny 3.0——一个拥有 80 亿参数、但每次仅激活 10 亿参数的混合专家（MoE）模型——能够在 2017 年款、搭载第七代 i5 处理器和 8GB 内存、没有 GPU 和显存的笔记本上，通过 llama.cpp 自主编写、运行并迭代代码。模型生成速度约为每秒 10 个 token，并在约 20 分钟内完成了一个多轮智能体编程任务：扫描本地网络中的 llama.cpp 服务器。 这表明强大的智能体编程不再局限于昂贵的 GPU 设备，有可能让大量老旧 CPU 和边缘设备无需新硬件就能变成有用的 AI 机器。这标志着小型 MoE 模型正让本地 AI 在普通消费设备和边缘计算场景中变得切实可行。 该模型使用直接从 llama.cpp 构建的 Q6 量化版本运行，未做任何优化，仅靠 CPU 就达到约每秒 10 个 token。任务本身相对简单，用户也指出更昂贵的硬件在速度和能效上始终更优，因此旧硬件未必对所有工作负载都实用。

reddit · r/LocalLLaMA · /u/netherreddit · 9月26日 00:40

**背景**: 混合专家（MoE）是一种模型架构，其中包含许多专门的子网络（专家），但每次处理提示时只激活其中一小部分，因此一个 80 亿参数的模型在推理时只需激活 10 亿参数。llama.cpp 是一个开源的 C/C++ 推理引擎，已成为在消费级硬件（包括 CPU）上本地运行大语言模型的事实标准。智能体编程（agentic coding）指 AI 智能体能够在迭代循环中自主编写、运行和调试代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://www.microcenter.com/site/mc-news/article/mixture-of-experts-moe-for-ai-explained.aspx">Mixture of Experts ( MoE ) Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#moe`, `#llama.cpp`, `#edge-ai`, `#agentic-coding`

---

<a id="item-15"></a>
## [Splash 1.1.0 发布，新增 GGUF 量化与 MLX 导入支持](https://www.reddit.com/r/LocalLLaMA/comments/1wqw9rn/splash_110_released_gguf_quants_support_mlx/) ⭐️ 7.0/10

Splash 1.1.0 正式发布，新增对 GGUF 量化模型的支持以及 MLX 导入功能，该消息在 r/LocalLLaMA 板块公布。有用户报告称，在配备 64GB 统一内存的 M5 Pro 上，以 Unsloth UD-Q4_K_XL 量化的 Qwen3 27B 模型运行智能体工作流，速度可达约 50 tokens/秒。 此次发布的重要性在于，它将优化内核、投机解码、前缀缓存和混合权重支持整合到一个面向 Apple Silicon 的工具中，使高质量的本地大模型推理更加实用。这降低了 Mac 用户在本地运行大模型的门槛，无需依赖云端 API。 50 tokens/秒的数据来自一位用户在 M5 Pro 64GB 设备上运行 27B 模型（Q4_K_XL 量化）的单一报告，实际性能会因硬件和模型不同而变化。Splash 整合了多种加速技术——优化内核、投机解码、前缀缓存和混合权重支持——共同带来了速度提升。

reddit · r/LocalLLaMA · /u/wojtek15 · 9月26日 17:27

**背景**: GGUF 是一种用于存储量化大语言模型的文件格式，因能在保持质量的同时减小模型体积和内存占用，被本地 AI 社区广泛使用。MLX 是苹果为 Apple Silicon 打造的机器学习数组框架，针对 M 系列芯片的统一内存架构进行了优化。投机解码是一种通过小型草稿模型预测多个 token，再由大模型并行验证来加速推理的技术。Splash 似乎是一个将这些技术整合在一起、面向 Mac 用户的新型推理引擎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ggufloader.github.io/what-is-gguf.html">What is GGUF? Complete Guide to GGUF Format & Quantization</a></li>
<li><a href="https://github.com/ml-explore/mlx">GitHub - ml-explore/mlx: MLX: An array framework for Apple ...</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency ...</a></li>

</ul>
</details>

**社区讨论**: 该 Reddit 帖子将 Splash 视为 Apple Silicon 本地推理的突破，作者强调了优化内核、投机解码、前缀缓存和混合权重支持的结合。尽管讨论氛围积极，但性能数据仅基于单一用户的体验，尚待更广泛的社区验证。

**标签**: `#local-llm`, `#apple-silicon`, `#gguf`, `#mlx`, `#inference-optimization`

---