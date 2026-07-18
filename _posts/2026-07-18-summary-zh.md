---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 32 条内容中筛选出 14 条重要资讯。

---

1. [LG 显示器通过 Windows Update 静默安装软件](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 解决凸优化领域 30 年猜想](#item-2) ⭐️ 8.0/10
3. [Kimi K3 引发 AI 模型竞争辩论](#item-3) ⭐️ 8.0/10
4. [PHK 以自行车棚效应反思告别开源](#item-4) ⭐️ 8.0/10
5. [一张图展示 Stack Overflow 的衰落](#item-5) ⭐️ 8.0/10
6. [运河底发现被遗忘的能力计算机](#item-6) ⭐️ 8.0/10
7. [TP-Link Kasa 摄像头通过未认证 UDP 泄露 GPS 长达 6 年](#item-7) ⭐️ 8.0/10
8. [Anthropic 改变计划，永久保留 Claude Fable 5](#item-8) ⭐️ 8.0/10
9. [Fable 5 与 GPT-5.6 Sol 在 NP 难问题上的对比：/goal 有效](#item-9) ⭐️ 7.0/10
10. [回归 JPEG 实现无需 JavaScript 的简易动画](#item-10) ⭐️ 7.0/10
11. [Simon Willison 构建交互式 SQLite 查询解释器](#item-11) ⭐️ 7.0/10
12. [教程：使用 Lean 进行形式化验证入门](#item-12) ⭐️ 7.0/10
13. [微软工程师在 SQL Server 工作 13 年后对 Postgres 代码质量感到惊讶](#item-13) ⭐️ 7.0/10
14. [韧性不总是重试](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [LG 显示器通过 Windows Update 静默安装软件](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 9.0/10

据报道，LG 显示器在未经用户同意的情况下，通过 Windows Update 安装软件，并在每次启动时以完全系统权限运行。 这构成了重大的安全和隐私风险，因为它允许第三方供应商在用户不知情的情况下以提升的权限执行代码，可能引发供应链攻击。 该软件在通过 HDMI 插入 LG 显示器时自动安装，并在重启后持续存在。解决方法是在 Windows 设置中禁用制造商应用的自动下载。

hackernews · baranul · 7月18日 10:21 · [社区讨论](https://news.ycombinator.com/item?id=48956688)

**背景**: Windows Update 旨在自动提供驱动程序和固件更新，以确保硬件兼容性。然而，这一事件表明，它也可以在未经用户同意的情况下推送来自硬件供应商的无关软件，引发了对更新机制信任和安全的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://asibiont.com/en/blog/monitory-lg-tayno-ustanavlivayut-po-cherez-windows-update-bez-vashego-soglasiya-chto-proiskhodit-i-kak-zashchititsya">LG Monitors Silently Install Software Through Windows Update ...</a></li>
<li><a href="https://lightmask.net/trending/lg-monitors-silently-install-software-through-windows-update-without-consent/">LG Monitors Silently Install Software Through Windows Update ...</a></li>
<li><a href="https://earnqa.com/quality-assurance/compliance-hub/lg-monitors-silently-install-software-through-windows-update-without-consent/">LG Monitors Silently Install Software Through Windows Update ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了愤怒，指出该软件以完全系统权限运行并随系统启动，类似于恶意软件。用户提供了通过组策略或设备安装设置进行解决的方法，一些人认为责任在于微软允许这种行为。

**标签**: `#security`, `#privacy`, `#Windows`, `#LG`, `#supply chain attack`

---

<a id="item-2"></a>
## [GPT-5.6 解决凸优化领域 30 年猜想](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

GPT-5.6 通过一个提示词，帮助解决了凸优化中一个长达 30 年的空白，证明了一个关于在球形域上优化凸 Lipschitz 函数时间复杂度的特定猜想。 这展示了人工智能在数学研究（即使是专业领域）中的潜力，并可能改变数学家处理低垂和中垂果实问题的方式。 该猜想比 OpenAI 最近解决的循环双覆盖猜想更为小众，但仍是一个实际贡献。该解决方案由 GPT-5.6 Sol Pro 而非 Ultra 完成，表明即使是较不先进的模型也能辅助研究。

hackernews · mbustamanter · 7月18日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48957779)

**背景**: 凸优化是数学优化的一个子领域，研究在凸集上最小化凸函数。30 年的空白指的是关于在 Lipschitz 连续约束下解决此类问题的最优时间复杂度的未解问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48957779">GPT-5.6 used a prompt to close a 30-year gap in convex optimization | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2512.22863v2">A Counterexample to the Optimality Conjecture in Convex ...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，AI 可以暴力破解数学逻辑，可能自动化低垂果实问题。一些人争论这是否会使初级研究人员过时，而另一些人澄清该解决方案使用了 Sol Pro 而非 Ultra，突显了不同模型的能力差异。

**标签**: `#AI`, `#mathematics`, `#convex optimization`, `#machine learning`, `#research`

---

<a id="item-3"></a>
## [Kimi K3 引发 AI 模型竞争辩论](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/) ⭐️ 8.0/10

Moonshot AI 于 2026 年 7 月 16 日发布了 Kimi K3，这是一个拥有 2.8 万亿参数、100 万 token 上下文窗口的开源权重混合专家模型。 Kimi K3 的性能和定价与 ChatGPT 5.6 和 Opus 4.8 等前沿模型接近，引发了关于这是否标志着 AI 竞争中的范式转变还是仅仅是趋同的讨论。 Kimi K3 拥有 2.8 万亿参数，定价为每百万 token 输入/输出 3/15 美元，而 ChatGPT 5.6 Sol 为 5/30 美元，Opus 4.8 为 5/25 美元。

hackernews · sbochins · 7月18日 17:32 · [社区讨论](https://news.ycombinator.com/item?id=48960218)

**背景**: 知识蒸馏将知识从大模型转移到小模型，使更便宜的模型在特定任务上达到先进性能。Kimi K3 是一个开源权重模型，其参数公开可用，与 OpenAI 和 Anthropic 的专有模型不同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>

</ul>
</details>

**社区讨论**: 社区评论存在分歧：一些人认为蒸馏使前沿实验室的护城河不可持续，而另一些人则认为 K3 只是与现有模型趋同。用户还报告了不同的实际体验，有人发现 K3 在复杂任务上更慢且更贵。

**标签**: `#AI`, `#large language models`, `#distillation`, `#model competition`, `#pricing`

---

<a id="item-4"></a>
## [PHK 以自行车棚效应反思告别开源](https://queue.acm.org/detail.cfm?id=3818307) ⭐️ 8.0/10

开源传奇人物 Poul-Henning Kamp（PHK）在 ACM Queue 上发表了一篇回顾性文章，反思其职业生涯和“自行车棚效应”现象，并就技术决策与社区动态提供了见解。 这篇文章提供了系统编程和开源领域关键人物的珍贵一手智慧，帮助开发者理解并避免协作决策中的常见陷阱。 PHK 是 MD5crypt 密码哈希算法（1994 年）的创建者，也是 FreeBSD 和 Varnish Cache 的主要贡献者；文章还涉及了 LLM 辅助代码审查和年龄验证法规等现代议题。

hackernews · Ygg2 · 7月18日 17:27 · [社区讨论](https://news.ycombinator.com/item?id=48960155)

**背景**: “自行车棚效应”（Bikeshedding），又称帕金森琐碎定律，指人们倾向于在琐碎问题上花费过多时间而忽视更重要的问题。PHK 在开源社区推广了这一术语。他的职业生涯跨越数十年，在 Unix 系统和互联网基础设施方面做出了基础性贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Poul-Henning_Kamp">Poul-Henning Kamp - Wikipedia</a></li>
<li><a href="https://www.urbandictionary.com/define.php?term=bikeshedding">Urban Dictionary: bikeshedding</a></li>
<li><a href="https://www.ic.work/article/poul-henning-kamp-open-source-running-freedom">Poul-Henning Kamp的告别预言：开源最先失去的可能是运行自由 - ic.wo...</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 PHK 创建 MD5crypt 的贡献，并对其“LLM 辅助代码审查不会成为巨大颠覆者”的预测展开辩论，有人认为该观点脱离现实。也有人表示多次阅读后更欣赏其 nuanced 视角。

**标签**: `#open source`, `#software engineering`, `#bikeshedding`, `#systems programming`, `#history`

---

<a id="item-5"></a>
## [一张图展示 Stack Overflow 的衰落](https://data.stackexchange.com/stackoverflow/query/1953768#graph) ⭐️ 8.0/10

来自 Stack Exchange Data Explorer 的一张图显示 Stack Overflow 活动急剧下降，社区将其归因于 ChatGPT 等 AI 工具、排他性政策以及 2021 年被 Prosus 收购。 这种下降标志着开发者寻求帮助的方式发生转变，从传统的问答平台转向 AI 驱动的解决方案，这可能重塑在线知识共享社区。 该图在 2014 年左右达到峰值，远在 AI 成为主流之前，并在 2021 年被 Prosus 收购后出现显著下降。社区评论指出，高参与门槛和缺乏社区参与导致了衰落。

hackernews · secretslol · 7月18日 11:12 · [社区讨论](https://news.ycombinator.com/item?id=48956949)

**背景**: Stack Overflow 是一个面向程序员的问答平台，成立于 2008 年。它于 2021 年被 Prosus 以 18 亿美元收购。该平台因严格的审核政策而受到批评，这些政策打击了新用户。ChatGPT 于 2022 年底发布，提供即时代码答案，减少了对 Stack Overflow 的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stack_Overflow">Stack Overflow - Wikipedia</a></li>
<li><a href="https://stackoverflow.blog/2021/06/02/prosus-acquires-stack-overflow/">Prosus’s Acquisition of Stack Overflow: Our Exciting Next Chapter - Stack Overflow</a></li>
<li><a href="https://techcrunch.com/2021/06/02/stack-overflow-acquired-by-prosus-for-a-reported-1-8-billion/">Stack Overflow acquired by Prosus for $1.8 billion | TechCrunch</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 Stack Overflow 的衰落是咎由自取，源于高门槛和反社区政策。一些人指出衰落始于 ChatGPT 之前，并将 Prosus 收购视为转折点。一位用户在尝试查看图表时讽刺地遇到了速率限制，凸显了 AI 对互联网的广泛影响。

**标签**: `#Stack Overflow`, `#AI impact`, `#community`, `#data analysis`, `#tech industry`

---

<a id="item-6"></a>
## [运河底发现被遗忘的能力计算机](https://negroniventurestudios.com/2026/07/18/the-computer-at-the-bottom-of-a-canal/) ⭐️ 8.0/10

一篇详细的历史文章讲述了在运河底部发现的一款被遗忘的基于能力（capability）的计算机设计，探讨了其技术架构以及对现代硬件专业化的启示。 这个故事凸显了专用硬件与通用计算之间的权衡，并表明随着摩尔定律放缓，专用架构可能再次变得可行，从而影响未来的硬件设计。 这台计算机是一台能力机器（capability machine），一种使用标记内存进行细粒度访问控制的架构，类似于 1970-80 年代的 Intel iAPX 432 和 CAP 计算机。文章认为，商品化曲线压垮了这类设计，但摩尔定律的终结可能会重新激发人们的兴趣。

hackernews · Kudos · 7月18日 08:33 · [社区讨论](https://news.ycombinator.com/item?id=48956231)

**背景**: 基于能力的寻址是一种安全方案，通过称为能力（capability）的不可伪造令牌来控制内存访问。早期的能力机器如 Intel iAPX 432 在技术上先进，但由于复杂性和通用处理器的快速改进而在商业上失败。CHERI 项目是对这些思想的现代复兴。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Capability-based_addressing">Capability-based addressing - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Capability_Hardware_Enhanced_RISC_Instructions">Capability Hardware Enhanced RISC Instructions - Wikipedia</a></li>
<li><a href="https://homes.cs.washington.edu/~levy/capabook/Chapter1.pdf">Capability-Based Computer Systems</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，能力机器在当时是前沿技术，但被商品化曲线和摩尔定律压垮。一些人认为作者关于专用硬件现在可行的观点很有趣，尤其是随着 AI 改变了平台投资的经济性。

**标签**: `#computer architecture`, `#capability machines`, `#history of computing`, `#hardware design`, `#retrocomputing`

---

<a id="item-7"></a>
## [TP-Link Kasa 摄像头通过未认证 UDP 泄露 GPS 长达 6 年](https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md) ⭐️ 8.0/10

安全研究员 BadChemical 披露，TP-Link Kasa Spot EC71 摄像头通过端口 9999 上未认证的 UDP 服务泄露精确 GPS 坐标，该漏洞存在六年之久，直至固件 2.4.1 版本才被修复。 此漏洞凸显了物联网安全长期存在的缺陷：一款流行的智能家居设备在无需任何认证的情况下泄露敏感位置数据，可能被用于物理监视或定向攻击。 GPS 泄露自 2016 年起就已被公开知晓，但直到 2022 年经过协调披露后才被修复；此外，该摄像头还使用了硬编码的全局 RSA 私钥和未加盐的 MD5 密码存储。

hackernews · BadChemical · 7月17日 21:42 · [社区讨论](https://news.ycombinator.com/item?id=48952565)

**背景**: 智能摄像头等物联网设备通常运行轻量级固件，安全功能有限。未认证的 UDP 服务常用于本地发现，但如果保护不当，可能泄露敏感数据。TP-Link Kasa EC71 是一款室内安防摄像头，可与云服务和本地应用通信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/BadChemical/IoT-Vulnerability-Research-Public/blob/main/TP-Link_Kasa_EC71/Kasa_EC71.md">TP-Link Kasa cameras leaked home GPS via unauthenticated UDP ...</a></li>
<li><a href="https://www.devdigest.org/articles/tp-link-kasa-ec71-leaks-home-gps-via-unauthenticated-udp-for-6-years">TP-Link Kasa EC71 Leaks Home GPS via Unauthenticated UDP for</a></li>
<li><a href="https://byteiota.com/tp-link-kasa-your-security-camera-leaked-home-gps/">TP-Link Kasa: Your Security Camera Leaked Home GPS</a></li>

</ul>
</details>

**社区讨论**: 社区评论对物联网安全表示担忧，有人指出许多廉价设备存在类似缺陷。其他人则对严重程度存在争议，认为该漏洞主要影响本地网络，除非设备暴露在互联网上，但仍然是隐私风险。

**标签**: `#IoT`, `#security`, `#vulnerability`, `#privacy`, `#TP-Link`

---

<a id="item-8"></a>
## [Anthropic 改变计划，永久保留 Claude Fable 5](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 8.0/10

Anthropic 宣布，Claude Fable 5 将永久包含在 Max 和 Team Premium 订阅计划中，使用额度为上限的 50%，推翻了此前移除该模型的计划。这一决定是在 OpenAI 的 GPT-5.6 Sol 和 Moonshot AI 的 Kimi 3 的竞争压力下做出的。 此举表明，AI 模型市场的激烈竞争正迫使公司重新思考定价和访问策略以留住订阅用户。它也缓解了用户对失去 Anthropic 最佳模型访问权限的焦虑，可能有助于稳定订阅收入。 Pro 和 Team Standard 用户将继续通过使用额度访问 Fable 5，并获得一次性 100 美元额度，但每月 20 美元计划的用户仍无法访问。最初的移除计划是出于计算能力考虑，目前尚不清楚 Anthropic 是否会缩减训练以释放 GPU。

rss · Simon Willison · 7月18日 06:00

**背景**: Claude Fable 5 是 Anthropic 最强大的公开可用模型，属于 Mythos 系列。它最初计划仅通过 API 提供，但 GPT-5.6 Sol（在某些基准测试上优于 Fable 5）和 Kimi 3（一个强劲的竞争对手）的发布使得该计划难以维持。这一决定反映了 AI 模型发布的快速节奏，以及保持旗舰模型对订阅用户可访问的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区反应普遍积极，对 'Fable 末日' 的结束感到宽慰。一些用户质疑 Anthropic 能否维持计算需求，而另一些用户指出每月 20 美元的计划仍无法访问，这可能会引发进一步讨论。

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#pricing`, `#competition`

---

<a id="item-9"></a>
## [Fable 5 与 GPT-5.6 Sol 在 NP 难问题上的对比：/goal 有效](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/) ⭐️ 7.0/10

一篇博客文章对比了 Anthropic 的 Fable 5 和 OpenAI 的 GPT-5.6 Sol 在一个 NP 难问题上的表现，发现 /goal 提示能提升单线调查的性能。 这一对比为两大领先 AI 模型如何处理复杂推理任务提供了早期见解，并凸显了提示工程对提升模型性能的重要性。 /goal 提示对单线调查有益，但可能对更广泛的搜索策略无帮助；作者建议采用具有并行调查能力的超模式可能更优。

hackernews · couAUIA · 7月18日 11:00 · [社区讨论](https://news.ycombinator.com/item?id=48956879)

**背景**: NP 难问题是一类尚无高效解法的问题，因此成为 AI 推理的挑战性基准。提示工程涉及设计输入提示以引导 AI 模型输出。Fable 5 和 GPT-5.6 Sol 分别是 Anthropic 和 OpenAI 于 2026 年中发布的最新旗舰模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://www.promptingguide.ai/">Prompt Engineering Guide | Prompt Engineering Guide</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，Claude（Fable）在长会话中容易忘记指令，而 GPT 在优化问题上被认为更强。一些用户建议，采用并行调查的超模式可能优于 /goal 方法。

**标签**: `#AI`, `#LLM`, `#benchmarking`, `#prompt engineering`, `#NP-hard`

---

<a id="item-10"></a>
## [回归 JPEG 实现无需 JavaScript 的简易动画](https://maurycyz.com/projects/bad_jpeg/) ⭐️ 7.0/10

Maurycy Z. 创造了一种名为“回归 JPEG”的技术，利用 JPEG 格式的渐进式编码，使较早的扫描行在较晚显示，从而实现无需 JavaScript 的简易动画或隐写术。 这一巧妙黑客技术展示了对普遍图像格式的新颖应用，为轻量级动画和隐写术开辟了可能性，可绕过典型内容过滤器且无需客户端脚本。 该技术通过构建一个 JPEG 文件实现，其中每次扫描明确设置其频谱范围，使后续扫描覆盖先前图像数据。播放时序依赖于网络延迟，但可通过服务器端分块传输来近似控制。

hackernews · vitaut · 7月18日 03:14 · [社区讨论](https://news.ycombinator.com/item?id=48954851)

**背景**: JPEG 是一种使用离散余弦变换（DCT）的有损图像压缩标准。渐进式 JPEG 通过多次扫描编码图像，每次扫描细化图像质量。通常后续扫描增加细节；回归 JPEG 则反过来，让后续扫描覆盖先前数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://maurycyz.com/projects/bad_jpeg/">Regressive JPEGs: (Maurycy's blog)</a></li>
<li><a href="https://news.ycombinator.com/item?id=48954851">Regressive JPEGs | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/JPEG">JPEG - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区认为该技术富有创意且“邪门”。评论者提出了应用场景，如利用隐写术绕过内容过滤器、为并行加载提供进度条，以及通过服务器端定时分块传输来近似控制动画时序。

**标签**: `#JPEG`, `#image processing`, `#steganography`, `#hacking`

---

<a id="item-11"></a>
## [Simon Willison 构建交互式 SQLite 查询解释器](https://simonwillison.net/2026/Jul/18/sqlite-query-explainer/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一个交互式 SQLite 查询解释器工具，该工具通过 Pyodide（一个用于 WebAssembly 的 Python 发行版）完全在浏览器中运行。该工具为 EXPLAIN 和 EXPLAIN QUERY PLAN 的输出提供了易于理解的解释。 理解 SQLite 查询计划是开发者的常见痛点，而该工具通过提供无需安装的便捷学习方式降低了门槛。它展示了 Pyodide 将基于 Python 的工具直接带入浏览器的实际应用。 该工具借助 Fable（一个代码生成工具）构建，灵感来源于 Julia Evans 关于学习 SQLite 的博客文章。Willison 指出他并非 SQLite 查询计划专家，因此用户应独立验证结果。

rss · Simon Willison · 7月18日 17:19

**背景**: SQLite 的 EXPLAIN 和 EXPLAIN QUERY PLAN 命令揭示了数据库引擎如何执行查询，但其输出可能难以理解。EXPLAIN QUERY PLAN 提供查询策略的高级摘要，而 EXPLAIN 则显示底层的虚拟机操作。Pyodide 允许 Python 代码通过 WebAssembly 在浏览器中运行，使得此类工具无需服务器端组件即可工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/en/stable/console.html">pyodide .org/en/stable/console.html</a></li>
<li><a href="https://www.sqlite.org/eqp.html">Explain query plan</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#query-plan`, `#developer-tools`, `#pyodide`, `#webassembly`

---

<a id="item-12"></a>
## [教程：使用 Lean 进行形式化验证入门](https://www.reddit.com/r/programming/comments/1uzvfar/tutorial_introduction_to_formal_verification_with/) ⭐️ 7.0/10

一个新的教程系列向程序员介绍如何使用 Lean 定理证明器进行形式化验证，第一部分现已在 Reddit 上发布。 形式化验证可以数学上证明软件的正确性，而 Lean 是一个现代、开源的工具，使这种方法对开发者更易用。 该教程面向没有形式化验证经验的程序员，涵盖 Lean 中的基本概念和动手示例。

reddit · r/programming · /u/badcryptobitch · 7月18日 13:06

**背景**: 形式化验证使用数学证明来验证系统是否符合其规范。Lean 是一个证明助手和函数式编程语言，支持交互式定理证明。它被用于 seL4 微内核和 CompCert 编译器等高可靠性软件项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#Lean`, `#tutorial`, `#programming languages`

---

<a id="item-13"></a>
## [微软工程师在 SQL Server 工作 13 年后对 Postgres 代码质量感到惊讶](https://www.reddit.com/r/programming/comments/1uzerp7/what_surprised_an_engineer_after_spending_13/) ⭐️ 7.0/10

微软杰出工程师 Panos Antonopoulos 在 Talking Postgres 播客上分享，他在 SQL Server 工作 13 年后发现 Postgres 的代码库更干净、更容易理解，并且 LLM 帮助他梳理 Postgres 邮件列表上多年的设计讨论。 这位资深 SQL Server 工程师的见解凸显了 Postgres 日益成熟和开发者友好的代码库，可能鼓励更多企业将 Postgres 作为默认数据库选择。 Antonopoulos 指出，事务和存储等基本概念在 SQL Server 和 Postgres 之间迁移得很好，但他惊讶地发现自己在 Postgres 中理解新领域的速度要快得多。他还讨论了他参与的 Azure HorizonDB 工作，这是一个具有共享存储架构的 Postgres 兼容数据库。

reddit · r/programming · /u/clairegiordano · 7月17日 22:50

**背景**: PostgreSQL 是一个开源关系型数据库，以其可扩展性和标准合规性而闻名。其开发严重依赖公开的邮件列表进行设计讨论，但由于讨论数量庞大且年代久远，难以梳理。LLM（大语言模型）可以帮助总结和搜索这些讨论，使新加入者更容易理解过去的决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://azure.microsoft.com/en-us/products/horizondb">Azure HorizonDB | Microsoft Azure</a></li>
<li><a href="https://techcommunity.microsoft.com/blog/adforpostgresql/azure-horizondb-enterprise-ready-postgres-engineered-for-the-ai-era/4524094">Azure HorizonDB: Enterprise-Ready Postgres, Engineered for the AI Era | Microsoft Community Hub</a></li>
<li><a href="https://postgres.email/lists">Postgres Email Lists</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论活跃且内容充实。许多用户同意 Postgres 的代码库干净且文档完善，而其他人则指出 SQL Server 在工具和集成方面有其自身优势。一些评论者对如何使用 LLM 来消化邮件列表档案表示好奇。

**标签**: `#PostgreSQL`, `#SQL Server`, `#database`, `#engineering`, `#LLM`

---

<a id="item-14"></a>
## [韧性不总是重试](https://www.reddit.com/r/programming/comments/1v05z0d/sometimes_the_most_resilient_thing_a_system_can/) ⭐️ 7.0/10

一篇 Reddit 帖子指出，有时不重试（例如快速失败或优雅降级）比自动重试更具韧性，因为重试可能加剧故障。 这挑战了分布式系统设计中的传统观念（重试常被作为默认韧性机制），并强调了需要精细化的故障处理以防止级联故障。 帖子强调重试可能使本已吃力的系统过载，并建议在某些场景下使用断路器、超时和优雅降级等替代方案更为有效。

reddit · r/programming · /u/madflojo · 7月18日 20:07

**背景**: 在分布式系统中，重试是处理瞬时故障的常见模式，但可能导致惊群问题或在故障期间放大负载。优雅降级意味着系统在部分组件故障时仍能提供部分功能，而快速失败则立即停止请求以避免资源浪费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.codecentric.de/en/knowledge-hub/blog/resilience-design-patterns-retry-fallback-timeout-circuit-breaker">Resilience Design Patterns: Retry , Fallback, Timeout</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fault_tolerance">Fault tolerance - Wikipedia</a></li>
<li><a href="https://www.systemdesignhandbook.com/blog/distributed-systems-principles/">Distributed Systems Principles Explained</a></li>

</ul>
</details>

**社区讨论**: 社区普遍认同这一观点，热门评论讨论了重试导致故障的真实案例，并称赞文章指出了权衡。部分评论讨论了指数退避和抖动在减轻重试风险中的作用。

**标签**: `#resilience`, `#distributed systems`, `#failure handling`, `#system design`

---