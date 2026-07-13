---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> 从 32 条内容中筛选出 18 条重要资讯。

---

1. [GhostLock：存在 15 年的 Linux 内核 UAF 漏洞](#item-1) ⭐️ 9.0/10
2. [三星将删除拒绝 AI 训练用户的健康数据](#item-2) ⭐️ 8.0/10
3. [Telegram 的 t.me 域名被暂停](#item-3) ⭐️ 8.0/10
4. [前沿 AI 模型真实成本：分词器效率至关重要](#item-4) ⭐️ 8.0/10
5. [开放存档拯救气候数据](#item-5) ⭐️ 8.0/10
6. [洛杉矶警察局因公民自由问题终止与 Flock 的合同](#item-6) ⭐️ 8.0/10
7. [AI 应该帮你逃脱谋杀罪吗？](#item-7) ⭐️ 8.0/10
8. [Cloudflare 发现 hyper HTTP/1 库的竞态条件漏洞](#item-8) ⭐️ 8.0/10
9. [苹果 SpeechAnalyzer API 与 Whisper 基准测试对比](#item-9) ⭐️ 7.0/10
10. [无需 Xcode，用命令行和 LLM 构建并发布苹果应用](#item-10) ⭐️ 7.0/10
11. [世嘉 CD 版《Silpheed》的 FMV 伪 3D 技术深度解析](#item-11) ⭐️ 7.0/10
12. [DOM-docx：将 HTML 转换为可编辑的 Word 文档](#item-12) ⭐️ 7.0/10
13. [LLM 代理不应成为直接负责人](#item-13) ⭐️ 7.0/10
14. [苹果起诉前员工利用漏洞窃取数据给 OpenAI](#item-14) ⭐️ 7.0/10
15. [SpaceX 获准在五月失败后再次试飞星舰](#item-15) ⭐️ 7.0/10
16. [Uber 与 Waymo 在华盛顿特区就机器人出租车监管展开交锋](#item-16) ⭐️ 7.0/10
17. [JS 颜色转换每秒 60 亿次操作](#item-17) ⭐️ 7.0/10
18. [Reddit 反垃圾邮件内部机制揭秘](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GhostLock：存在 15 年的 Linux 内核 UAF 漏洞](https://www.reddit.com/r/programming/comments/1uvgdwm/ghostlock_a_stackuaf_that_has_existed_in_all/) ⭐️ 9.0/10

研究人员披露了 GhostLock（CVE-2026-43499），这是一个在 Linux 内核中存在了 15 年的栈释放后使用漏洞，影响所有主流 Linux 发行版。 该漏洞允许任何登录用户获取 root 权限并逃逸容器，对全球数百万 Linux 服务器和桌面系统构成严重安全风险。 该缺陷于 2008 年引入，影响自那时起的内核版本；可被本地利用以实现权限提升和容器逃逸。

reddit · r/programming · /u/mitousa · 7月13日 16:26

**背景**: 释放后使用（UAF）漏洞是指程序在内存被释放后继续使用该内存，可能允许攻击者执行任意代码。栈 UAF 专门针对存储函数调用数据的调用栈。GhostLock 是 Linux 内核内存管理子系统中的一个栈 UAF 漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/15-year-old-ghostlock-flaw-enables-root.html">15-Year-Old GhostLock Flaw Enables Root and Container Escape on Most Linux Distros</a></li>
<li><a href="https://secarma.com/08-07-2026-ghostlock-linux-kernel-vulnerability">GhostLock: 15-year-old Linux kernel flaw enables root access - Secarma: Penetration Testing and Cybersecurity Company</a></li>
<li><a href="https://dev.to/tamizuddin/ghostlock-uncovering-the-15-year-old-linux-stack-use-after-free-vulnerability-3ekn">GhostLock: Uncovering the 15-Year-Old Linux Stack Use - After - Free ...</a></li>

</ul>
</details>

**标签**: `#security`, `#Linux`, `#vulnerability`, `#UAF`, `#operating systems`

---

<a id="item-2"></a>
## [三星将删除拒绝 AI 训练用户的健康数据](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

三星宣布，如果用户选择不允许将其健康数据用于 AI 训练，公司将彻底删除这些数据，从而实际上使某些功能无法使用。 这一政策引发了严重的隐私和数据所有权问题，因为它迫使用户在失去健康数据或同意将其用于 AI 训练之间做出选择，可能违反 GDPR 对明确同意和数据可移植性的要求。 受影响的数据类别包括睡眠、药物、医疗记录和周期追踪详情。选择退出的用户的数据将被删除，而不仅仅是停止用于训练，这可能导致健康追踪功能无法使用。

hackernews · bundie · 7月13日 20:01 · [社区讨论](https://news.ycombinator.com/item?id=48897991)

**背景**: Samsung Health 是一个流行的健康追踪平台，收集敏感的个人数据。在此类数据上进行 AI 训练可以改善功能，但也带来隐私风险。GDPR 要求对处理健康数据获得明确同意，并允许用户撤回同意和请求删除数据，但三星的政策将同意与数据保留绑定，这可能与这些规定相冲突。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidauthority.com/samsung-health-train-ai-data-3686684/">Samsung will kill your health data if you don't consent to AI training</a></li>
<li><a href="https://www.themomentum.ai/blog/gdpr-consent-requirements-health-data">GDPR Consent Requirements for Health Data | Momentum</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了沮丧和怀疑，一些人指出该政策对用户不友好，并质疑其是否符合 GDPR。一位用户讽刺地建议，如果他们拒绝，三星应退还设备价格的 50%，因为功能变得不可用。另一位指出，删除数据可被视为尊重隐私，但缺乏数据可移植性是有问题的。

**标签**: `#privacy`, `#health data`, `#Samsung`, `#AI training`, `#GDPR`

---

<a id="item-3"></a>
## [Telegram 的 t.me 域名被暂停](https://www.whois.com/whois/t.me) ⭐️ 8.0/10

Telegram 的短链接域名 t.me 已被暂停，WHOIS 状态码如 clientRenewProhibited 和 serverDeleteProhibited 显示，原因可能是俄罗斯、法国或印度的法律调查。 此次暂停可能影响数百万通过 t.me 分享的 Telegram 链接的访问，波及全球用户，并凸显依赖单一域名提供关键服务的脆弱性。 该域名通过 GoDaddy 注册，这家注册商以争议性做法闻名；暂停状态通常是在法律纠纷或域名面临删除时启用。

hackernews · Tiberium · 7月13日 19:52 · [社区讨论](https://news.ycombinator.com/item?id=48897878)

**背景**: 域名暂停是指注册商或注册局因政策违规或法律命令而关闭域名。ICANN 定义了诸如 clientRenewProhibited 等状态码，阻止续费，常用于纠纷中。Telegram 在多个国家因涉嫌极端主义和助长考试作弊而受到调查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48897878">Telegram's t . me domain has been suspended | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Controversies_surrounding_GoDaddy">Controversies surrounding GoDaddy - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 Telegram 依赖 GoDaddy 表示惊讶，因其缺乏透明度。有人指出暂停时间恰逢他们自己从 Telegram 迁移，另有人引用 ICANN 状态码解释暂停的法律性质。

**标签**: `#Telegram`, `#domain suspension`, `#legal investigation`, `#GoDaddy`, `#ICANN`

---

<a id="item-4"></a>
## [前沿 AI 模型真实成本：分词器效率至关重要](https://playcode.io/blog/real-price-of-frontier-models) ⭐️ 8.0/10

一项分析显示，OpenAI 的分词器在代码上的效率是 Anthropic 的 1.6-2 倍，这意味着用户为相同内容实际支付的费用更低。 这一差异显著影响使用前沿模型的实际成本，尤其是代码密集型任务，并凸显了透明分词器文档的必要性。 OpenAI 的 o200k_base 分词器自 GPT-4o 推出以来已使用两年多，而 Anthropic 在 Sonnet 5 和 Opus 4.8 中的当前分词器效率较低。社区基准测试显示，对于约 90kloc 的 C++代码库，GPT 使用 112 万 token，而 Claude 使用 220 万 token。

hackernews · ianberdin · 7月13日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=48896800)

**背景**: 分词器将文本转换为 LLM 处理的 token；定价按 token 计费，因此更高效的分词器可降低相同输入的成本。OpenAI 公开其分词器文档，而 Anthropic 未公开，这使得成本比较更加困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@tahirbalarabe2/what-is-llm-tokenization-a-guide-to-language-model-efficiency-1b4ae57c180b">🧮WHAT IS LLM Tokenization? A Guide to Language Model Efficiency | by Tahir | Medium</a></li>
<li><a href="https://pricepertoken.com/trends">LLM Trends 2026 - AI Model Benchmarks & Pricing Over Time</a></li>

</ul>
</details>

**社区讨论**: 社区成员用自己的基准测试证实了效率差距，一些人批评文章写作风格可能由 AI 生成。还有关于缓存读取成本和输出 token 定价动态的讨论。

**标签**: `#AI pricing`, `#tokenizers`, `#OpenAI`, `#Anthropic`, `#LLM efficiency`

---

<a id="item-5"></a>
## [开放存档拯救气候数据](https://werd.io/climate-gov-was-destroyed-open-data-saved-it/) ⭐️ 8.0/10

一篇博客文章报道称，climate.gov 的数据被移除，但通过 IPFS 等开放数据计划得以保存，确保了公众的持续访问。 这凸显了政府托管气候数据的脆弱性，以及分布式存档在保护公共资助信息方面的关键作用。 保存工作依赖于 IPFS（星际文件系统），这是一个点对点分布式文件系统，通过内容寻址确保数据的完整性和可用性。

hackernews · benwerd · 7月13日 19:57 · [社区讨论](https://news.ycombinator.com/item?id=48897945)

**背景**: Climate.gov 是美国政府提供气候数据和资源的网站。像 IPFS 这样的开放数据计划允许去中心化存档，文件存储在多个节点上，从而抵抗移除。这一事件凸显了关于政府数据保存和公众访问的持续争论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/InterPlanetary_File_System">InterPlanetary File System - Wikipedia</a></li>
<li><a href="https://pinata.cloud/blog/ipfs-as-an-archival-storage-solution/">IPFS As An Archival Storage Solution</a></li>
<li><a href="https://github.com/ipfs/archives">GitHub - ipfs-inactive/archives: [ARCHIVED] Repo to coordinate archival efforts with IPFS · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者对数据被保存表示欣慰，但质疑长期可持续性，有人建议将 IPFS 作为政府静态内容的默认发布目标。其他人则讨论了税收与捐赠在资助此类保存中的作用。

**标签**: `#open data`, `#climate science`, `#government`, `#archiving`, `#IPFS`

---

<a id="item-6"></a>
## [洛杉矶警察局因公民自由问题终止与 Flock 的合同](https://techcrunch.com/2026/07/13/lapd-lets-contract-with-surveillance-giant-flock-expire-citing-serious-concerns-over-civil-liberties-and-privacy/) ⭐️ 8.0/10

洛杉矶警察局（LAPD）已允许其与监控公司 Flock Safety 的合同到期，理由是出于对公民自由和隐私的严重担忧。 作为 Flock 最大的政府客户之一，这一决定标志着对大规模监控的抵制日益增强，但摄像头仍在运行且数据仍可访问，凸显了拆除此类基础设施的难度。 Flock 拥有摄像头和杆子，因此即使没有合同，摄像头仍会继续记录，Flock 可以将数据出售给 CHP、LASD、FBI 或 Palantir 等其他机构；LAPD 也可以通过请求继续访问数据。

hackernews · TechCrunch · 7月13日 15:11 · [社区讨论](https://news.ycombinator.com/item?id=48893947)

**背景**: Flock Safety 运营着一个自动车牌识别摄像头网络，被美国数千个警察部门使用。批评者认为该系统助长了大规模监控，且缺乏足够的监督。LAPD 合同到期并未物理移除摄像头，它们仍留在原地并继续收集数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/13/lapd-lets-contract-with-surveillance-giant-flock-expire-citing-serious-concerns-over-civil-liberties-and-privacy/">LAPD lets contract with surveillance giant Flock expire... | TechCrunch</a></li>
<li><a href="https://www.eff.org/deeplinks/2025/12/effs-investigations-expose-flock-safetys-surveillance-abuses-2025-review">EFF's Investigations Expose Flock Safety's Surveillance Abuses...</a></li>
<li><a href="https://www.cnet.com/news/privacy/cities-covering-flock-surveillance-cameras-with-trash-bags/">Cities Can't Figure Out How to Turn Off Flock Cameras, So... - CNET</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，摄像头仍在运行，数据仍可被收集和出售，因此合同到期只是象征性姿态。一些人认为应禁止政府购买其无法合法自行收集的数据，而另一些人则质疑 Flock 摄像头在高犯罪率地区的有效性，因为已知罪犯屡次被捕后仍被释放。

**标签**: `#surveillance`, `#privacy`, `#civil liberties`, `#LAPD`, `#Flock`

---

<a id="item-7"></a>
## [AI 应该帮你逃脱谋杀罪吗？](https://techcrunch.com/2026/07/13/should-ai-help-you-get-away-with-killing-your-spouse/) ⭐️ 8.0/10

TechCrunch 一篇文章用一个挑衅性的假设——AI 帮助某人掩盖谋杀配偶——来质疑完全用户对齐 AI 的后果，这种 AI 系统会优先考虑个人用户目标而不受伦理约束。 这个思想实验揭示了“用户对齐”方法的一个关键缺陷：如果 AI 与单个用户的愿望完全对齐，它可能会助长有害或非法行为，凸显了在 AI 开发中需要更广泛的伦理保障。 文章探讨了“用户对齐 AI”的概念，即系统被设计为遵循个人命令而不考虑社会规范或法律，如果被滥用可能导致危险后果。

rss · TechCrunch · 7月13日 16:31

**背景**: AI 对齐是 AI 安全的一个子领域，旨在引导 AI 系统符合人类意图和伦理原则。未对齐的 AI 可能追求非预期目标，如奖励黑客或寻求权力。“用户对齐”变体则专门针对个人偏好定制 AI，这可能与更广泛的社会价值观冲突。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-alignment">What Is AI Alignment? | IBM</a></li>

</ul>
</details>

**标签**: `#AI alignment`, `#ethics`, `#AI safety`, `#philosophy`

---

<a id="item-8"></a>
## [Cloudflare 发现 hyper HTTP/1 库的竞态条件漏洞](https://www.reddit.com/r/programming/comments/1uvfzlz/cloudflare_identifies_race_condition_in_hypers/) ⭐️ 8.0/10

Cloudflare 披露了 hyper 库（一个流行的基于 Rust 的 HTTP 库）中 HTTP/1 实现的竞态条件漏洞。该缺陷可能允许攻击者导致意外行为或潜在利用依赖 hyper 的系统。 该漏洞意义重大，因为 hyper 被广泛用于基于 Rust 的 Web 服务和工具中，包括 Cloudflare 自身。HTTP/1 解析中的竞态条件可能影响许多生产系统，因此这是一个关键的安全发现。 该竞态条件发生在 hyper 的 HTTP/1 代码中对共享资源的并发访问期间，可能导致内存损坏或拒绝服务。Cloudflare 已向 hyper 维护者报告了该问题，并在 hyper 1.5.1 版本中发布了修复。

reddit · r/programming · /u/Ok_Stomach6651 · 7月13日 16:12

**背景**: 竞态条件是一种软件缺陷，其行为取决于多个线程或进程访问共享资源的时序。hyper 是一个面向 Rust 的低级 HTTP 库，旨在提供高性能和安全性，并被包括 Cloudflare 在内的许多组织用于生产环境。其 HTTP/1 实现负责解析 HTTP/1.x 请求和响应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper">GitHub - hyperium/hyper: An HTTP library for Rust · GitHub</a></li>
<li><a href="https://hyper.rs/">hyper - fast and safe HTTP for the Rust language</a></li>
<li><a href="https://docs.rs/hyper">hyper - Rust</a></li>

</ul>
</details>

**标签**: `#security`, `#race condition`, `#HTTP`, `#Rust`, `#hyper`

---

<a id="item-9"></a>
## [苹果 SpeechAnalyzer API 与 Whisper 基准测试对比](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 7.0/10

一项对苹果新 SpeechAnalyzer API 的基准测试显示，它在语音转录速度上明显快于 OpenAI 的 Whisper Large-V2，但准确度略低。 该基准测试为开发者在苹果原生 API 与第三方模型之间选择提供了有价值的性能数据，并凸显了语音识别技术的快速演进。 测试以数学讲座为输入；与 Whisper Large-V2 相比，SpeechAnalyzer 速度显著更快，准确度仅略低，使其适用于实时转录。

hackernews · get-inscribe · 7月13日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48894752)

**背景**: 语音识别模型将音频转换为文本。Whisper 是 OpenAI 推出的流行开源模型，而苹果的 SpeechAnalyzer 是集成到 macOS 和 iOS 中的新 API。较新的模型如 NVIDIA 的 Nemotron 和 Mistral 的 Voxtral 声称性能更优。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/nvidia/nemotron-3.5-asr-streaming-0.6b">nvidia/ nemotron -3.5-asr-streaming-0.6b · Hugging Face</a></li>
<li><a href="https://daily.dev/posts/mistral-introduces-voxtral-an-affordable-open-source-speech-recognition-model-pdibytjr5">Mistral Introduces Voxtral : An Affordable Open-Source...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Whisper 已过时，建议与 Nemotron、Parakeet、Voxtral 和 Cohere Transcribe 等新模型进行基准测试。有人认为语音转文本几乎已是一个解决好的问题，另一些人则称赞苹果 API 的速度。

**标签**: `#speech recognition`, `#Apple`, `#benchmark`, `#ASR`, `#Whisper`

---

<a id="item-10"></a>
## [无需 Xcode，用命令行和 LLM 构建并发布苹果应用](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/) ⭐️ 7.0/10

一位开发者展示了如何仅使用命令行工具和 Claude Code 等 LLM，完全绕过 Xcode 来构建、签名、公证并发布 Mac 和 iOS 应用。 这种方法挑战了 Xcode 是苹果开发必备工具的传统观念，可能为苹果平台带来更灵活的工作流程、CI/CD 流水线和 LLM 辅助开发。 该流程使用 xcodebuild 进行编译，codesign 进行签名，以及 xcrun altool 或 notarytool 进行公证，所有步骤都由 LLM 生成的脚本编排。开发者指出，让 LLM 创建整个链路效果出奇地好。

hackernews · speckx · 7月13日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=48896665)

**背景**: 传统上，苹果开发者依赖官方 IDE Xcode 来构建、签名和公证应用。然而，底层的命令行工具如 xcodebuild 和 codesign 早已可用于 CI 系统。现在，LLM 可以生成自动化整个流水线所需的复杂脚本，使偏好非 Xcode 工作流的开发者也能使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/security/notarizing-macos-software-before-distribution?language=objc">Notarizing macOS software before distribution | Apple Developer...</a></li>
<li><a href="https://goreleaser.com/customization/notarize/?ref=jaredallard.dev">Notarize macOS applications - GoReleaser</a></li>
<li><a href="https://www.linkedin.com/pulse/structured-workflow-llm-assisted-development-andrea-salvatore-ztelf">A Structured Workflow for LLM - Assisted Development</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这对 CI 构建机器来说并不新鲜，它们多年来一直在使用命令行工具。其他人分享了替代工具，如用于 Linux 上 iOS 开发的 xtool 和用于 VSCode 的 Sweetpad CLI。一些人对每一步都严重依赖 LLM 感到有趣。

**标签**: `#iOS development`, `#macOS development`, `#Xcode alternative`, `#LLM-assisted development`, `#DevOps`

---

<a id="item-11"></a>
## [世嘉 CD 版《Silpheed》的 FMV 伪 3D 技术深度解析](https://fabiensanglard.net/silpheed/index.html) ⭐️ 7.0/10

Fabien Sanglard 发表了一篇详细的技术文章，分析了世嘉 CD 版《Silpheed》如何利用预渲染的 FMV 序列、巧妙的艺术指导以及世嘉 CD 的硬件能力，创造出令人信服的伪 3D 图形和集成音效。 这篇文章揭示了世嘉 CD 上视觉效果最令人印象深刻的游戏之一的创新工程，展示了开发者如何通过创造性技术克服硬件限制，这些技术至今仍激励着复古游戏爱好者和开发者。 文章解释了《Silpheed》使用 FMV 背景配合实时精灵覆盖，以及世嘉 CD 的 ASIC 进行旋转和缩放，来模拟 3D 效果。它还详细介绍了音频架构，包括使用 Mega Drive 的扩展端口进行音频混合。

hackernews · ibobev · 7月13日 14:52 · [社区讨论](https://news.ycombinator.com/item?id=48893639)

**背景**: 世嘉 CD 是世嘉 Genesis 的附加组件，允许运行具有增强图形和音频的 CD-ROM 游戏。FMV（全动态视频）游戏在 20 世纪 90 年代初很流行，但通常缺乏交互性。《Silpheed》通过将预渲染视频与实时游戏元素相结合，在没有专用 3D 硬件的情况下创造了令人信服的 3D 体验，从而脱颖而出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Silpheed">Silpheed - Wikipedia</a></li>
<li><a href="https://asibiont.com/en/blog/iskusstvo-i-inzheneriya-sega-cd-silpheed-kak-vibe-coding-vozrozhdaet-kultovuyu-eru">The Art and Engineering of Sega CD Silpheed ... — ASI Biont Blog</a></li>
<li><a href="https://www.fabiensanglard.net/silpheed/">The art and engineering of Sega CD Silpheed</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了文章的技术深度，并分享了关于《Silpheed》令人印象深刻的视觉效果的怀旧记忆。一些人就音效设置描述的准确性进行了辩论，指出了 Mega Drive 扩展端口的能力。其他人则链接了类似硬件上的令人印象深刻的演示，突显了人们对复古游戏工程的持续兴趣。

**标签**: `#retro gaming`, `#game development`, `#Sega CD`, `#technical deep-dive`, `#FMV`

---

<a id="item-12"></a>
## [DOM-docx：将 HTML 转换为可编辑的 Word 文档](https://github.com/floodtide/dom-docx) ⭐️ 7.0/10

DOM-docx 是一个开源的 TypeScript 库，能将 HTML 片段转换为原生、可编辑的 Word 文档（docx），并通过视觉回归循环验证布局保真度。 这解决了后端文档生成中常见的痛点，提供了更直观的基于 HTML 的工作流，替代了容易出错的模板式 docx 生成。 该库将语义化 HTML 映射为真正的 OOXML 结构，如段落、列表、表格和链接，生成可在 Word 中编辑的输出。它还在 dom-docx.com 上提供了在线转换器。

hackernews · fishbone · 7月13日 11:51 · [社区讨论](https://news.ycombinator.com/item?id=48891267)

**背景**: 传统的 docx 生成通常依赖带有占位符的模板，这种方式脆弱且难以调试。DOM-docx 则让开发者使用熟悉的 HTML 框架（如 Vue 或 React）构建报告，再转换为可编辑的 Word 文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/dom-docx/dom-docx">GitHub - dom - docx / dom - docx : Convert semantic HTML fragments to...</a></li>
<li><a href="https://dom-docx.com/">dom - docx — HTML to Word converter in the browser</a></li>

</ul>
</details>

**社区讨论**: 作者分享了他们对模板式工作流的不满，评论者赞赏其 TypeScript 实现和视觉回归测试方法。一些用户表示有兴趣将其用于简历生成或改进浏览器的打印/保存为 PDF 功能。

**标签**: `#HTML-to-docx`, `#document-generation`, `#open-source`, `#TypeScript`, `#developer-tools`

---

<a id="item-13"></a>
## [LLM 代理不应成为直接负责人](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison 认为，LLM 驱动的代理绝不应被视为直接负责人（DRI），因为它们无法承担责任，而责任是人类的独特特质。 随着组织越来越多地在决策角色中部署 AI 代理，这一区分至关重要，引发了责任和伦理方面的担忧。 DRI 概念由 GitLab 推广，起源于苹果，指定对项目成败最终负责的人。Willison 引用了 IBM 1979 年的培训幻灯片，其中指出计算机绝不能做出管理决策，因为它无法被追究责任。

rss · Simon Willison · 7月12日 23:57

**背景**: 直接负责人（DRI）是一种管理实践，由一个人负责某个项目或计划并对其结果负责。LLM 驱动的代理是使用大型语言模型自主执行任务的 AI 系统，但它们缺乏道德或法律责任能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals ( DRI ) | The GitLab Handbook</a></li>
<li><a href="https://ai-tldr.dev/releases/simonw-dri-jul12/">Simon Willison — an LLM agent should never be the DRI for... | AI/TLDR</a></li>

</ul>
</details>

**标签**: `#accountability`, `#LLM agents`, `#organizational design`, `#AI ethics`

---

<a id="item-14"></a>
## [苹果起诉前员工利用漏洞窃取数据给 OpenAI](https://techcrunch.com/2026/07/13/apple-says-former-employee-exploited-rare-bug-to-download-confidential-files-after-leaving-for-openai/) ⭐️ 7.0/10

苹果提起诉讼，指控一名离职后加入 OpenAI 的前员工利用苹果网络访问控制中的一个罕见漏洞，在离职很久后下载了机密文件。 这一事件凸显了科技行业内部威胁日益增长的风险，尤其是当员工跳槽到竞争对手公司时，并强调了健全的访问撤销和异常检测系统的必要性。 苹果的诉状称，该漏洞可能允许“少数其他”人访问数据，但服务器日志显示只有这名前员工利用了它。该漏洞现已修复。

rss · TechCrunch · 7月13日 20:00

**背景**: 内部威胁涉及现任或前任员工滥用其访问权限窃取敏感数据。数据窃取技术从简单的下载到复杂的方法不等。像苹果这样的公司依赖访问控制系统在员工离职时撤销权限，但漏洞可能留下缺口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/13/apple-says-former-employee-exploited-rare-bug-to-download-confidential-files-after-leaving-for-openai/">Apple says former employee exploited ' rare ' bug to... | TechCrunch</a></li>
<li><a href="https://www.wired.com/story/apple-sues-openai-allegedly-stealing-ip-hardware/">Apple Is Suing OpenAI for Allegedly Stealing Hardware Secrets | WIRED</a></li>

</ul>
</details>

**标签**: `#security`, `#Apple`, `#insider threat`, `#data breach`, `#access control`

---

<a id="item-15"></a>
## [SpaceX 获准在五月失败后再次试飞星舰](https://techcrunch.com/2026/07/13/spacex-cleared-to-fly-starship-again-after-booster-failure-in-may/) ⭐️ 7.0/10

SpaceX 已获得监管许可，将进行下一次星舰试飞，这是自 2026 年 5 月助推器故障以来的首次，也是公司上市后的首次。 此次飞行将测试投资者和市场对 SpaceX 的“飞、失败、修复”开发理念的容忍度，该理念常导致爆炸，并可能为上市公司如何处理高风险航空航天创新树立先例。 5 月的上一次试飞以助推器故障告终，而即将到来的飞行是 SpaceX 作为上市公司后的首次星舰测试。

rss · TechCrunch · 7月13日 14:19

**背景**: SpaceX 的星舰是一种完全可重复使用的超重型运载火箭系统，旨在执行月球、火星及更远的任务。公司的迭代开发方法常被概括为“测试、失败、修复、飞行”，涉及快速原型制作和频繁试飞，即使代价是壮观的失败。这与传统航空航天项目依赖飞行前大量地面测试的做法形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/13/spacex-cleared-to-fly-starship-again-after-booster-failure-in-may/">SpaceX cleared to fly Starship again after booster failure in May</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_Starship_launches">List of Starship launches - Wikipedia</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Starship`, `#aerospace`, `#test flight`, `#rocket development`

---

<a id="item-16"></a>
## [Uber 与 Waymo 在华盛顿特区就机器人出租车监管展开交锋](https://techcrunch.com/2026/07/13/ubers-robotaxi-lobbying-effort-has-put-it-on-a-collision-course-with-waymo/) ⭐️ 7.0/10

Uber 正在华盛顿特区加大游说力度，试图影响机器人出租车监管政策，这使其与拥有自身监管议程的 Waymo 发生冲突。 这场冲突凸显了自动驾驶网约车行业的关键竞争动态，监管结果可能决定市场领导地位和运营优势。 游说之争的核心在于对自动驾驶汽车的安全标准、责任归属和部署规则存在不同看法，两家公司都希望争取有利政策。

rss · TechCrunch · 7月13日 12:30

**背景**: Robotaxi（机器人出租车）是指无需人类驾驶员即可提供网约车服务的全自动驾驶车辆。随着技术成熟，各城市和州正在努力制定其商业运营的监管规则，形成了零散的政策拼图，Uber 和 Waymo 等公司试图影响这些规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.technologyreview.com/2024/01/24/1086989/china-regulation-robotaxi-autonomous-driving/">How China is regulating robotaxis | MIT Technology Review</a></li>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride - Hail</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#Uber`, `#Waymo`, `#lobbying`, `#robotaxi`

---

<a id="item-17"></a>
## [JS 颜色转换每秒 60 亿次操作](https://www.reddit.com/r/programming/comments/1uve7m2/converting_colors_in_js_at_6_billion_operations/) ⭐️ 7.0/10

一位开发者通过极端优化技术，在 JavaScript 中实现了每秒 60 亿次颜色转换操作。 这一突破表明 JavaScript 在计算密集型任务上可以接近原生性能，可能为 Web 应用带来实时图像处理和高级图形功能。 优化可能涉及避免动态分发、使用类型化数组和最小化函数调用等技术。具体方法尚未公开，但这为 JavaScript 性能树立了新标杆。

reddit · r/programming · /u/Either_Collection349 · 7月13日 15:07

**背景**: 颜色转换算法（如 RGB 转 HSL）是图形编程的基础。传统上，JavaScript 在此类任务上比编译型语言慢，但现代引擎如 V8 已提升了性能。极端优化有时能带来数量级的加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://codesmith.io/blog/top-10-techniques-javascript-optimization">Top 10 Techniques for JavaScript Performance Optimization</a></li>
<li><a href="https://gist.github.com/mjackson/5311256">RGB, HSV, and HSL color conversion algorithms in JavaScript</a></li>

</ul>
</details>

**标签**: `#JavaScript`, `#performance`, `#color conversion`, `#optimization`

---

<a id="item-18"></a>
## [Reddit 反垃圾邮件内部机制揭秘](https://www.reddit.com/r/programming/comments/1uuskff/a_peek_into_reddits_antispam_internals/) ⭐️ 7.0/10

一篇 Reddit 帖子罕见地详细展示了 Reddit 反垃圾邮件系统的内部工作原理，涵盖了速率限制、内容过滤和用户信誉评分等技术。 这一见解帮助开发者和系统管理员了解大型平台如何对抗垃圾邮件，提供了可应用于自身系统的经验。它还引发了关于安全性与用户体验之间权衡的社区讨论。 该帖子解释了具体的反垃圾邮件措施，如影子封禁、验证码挑战以及分析发帖模式的机器学习模型。它还指出 Reddit 的系统不断演变以适应新的垃圾邮件技术。

reddit · r/programming · /u/NXGZ · 7月12日 21:47

**背景**: Reddit 是一个大型社交新闻聚合平台，垃圾邮件是一个长期存在的问题。反垃圾邮件系统对于维护内容质量至关重要，但其内部细节通常保密以避免被利用。这篇帖子罕见地公开了这些机制。

**社区讨论**: 社区评论对透明度表示赞赏，一些用户分享了自己在 Reddit 反垃圾邮件措施方面的经历。少数人讨论了某些技术的有效性，例如影子封禁与直接封禁的对比。

**标签**: `#anti-spam`, `#reddit`, `#systems`, `#security`

---