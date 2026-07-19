---
layout: default
title: "Horizon Summary: 2026-07-19 (ZH)"
date: 2026-07-19
lang: zh
---

> 从 23 条内容中筛选出 13 条重要资讯。

---

1. [SRE 用 1600 美元的 ESP32 替代 12 万美元的保龄球计分系统](#item-1) ⭐️ 8.0/10
2. [阿里巴巴发布 Qwen 3.8，2.4 万亿参数开源大模型](#item-2) ⭐️ 8.0/10
3. [Minecraft Java 版切换至 SDL3](#item-3) ⭐️ 8.0/10
4. [Claude Code 现在使用用 Rust 重写的 Bun](#item-4) ⭐️ 8.0/10
5. [OpenAI 将 Codex 上下文大小降至 272k tokens](#item-5) ⭐️ 8.0/10
6. [AI 狂热正在摧毁全球决策能力](#item-6) ⭐️ 8.0/10
7. [GPT-2 词汇表以双曲树形式可视化](#item-7) ⭐️ 8.0/10
8. [软件工程师发现硬件比想象中简单](#item-8) ⭐️ 7.0/10
9. [Moonshot AI 因需求过大暂停 Kimi K3 订阅](#item-9) ⭐️ 7.0/10
10. [最后一个 MPEG-4 视觉专利到期](#item-10) ⭐️ 7.0/10
11. [无人出租车监管之争升温](#item-11) ⭐️ 7.0/10
12. [非营利组织 Current AI 致力于为所有人构建免费 AI 网络](#item-12) ⭐️ 7.0/10
13. [通过 SFT 和 RLVR，开源权重 LLM 通过瑞典医学执照考试](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [SRE 用 1600 美元的 ESP32 替代 12 万美元的保龄球计分系统](https://news.ycombinator.com/item?id=48968606) ⭐️ 8.0/10

一位 SRE 使用 ESP32 微控制器、ESPNow 网状网络和树莓派，以每对球道约 200 美元的成本构建了一套功能完整的保龄球计分与控制系统，替代了原价 12 万美元的专有系统。该项目名为 OpenLaneLink，计划开源。 这展示了现代嵌入式系统如何大幅降低成本并消除小众老旧设备的供应商锁定。它使小型保龄球馆业主能够以可负担的方式升级和定制系统，有望振兴当地娱乐选择。 该系统使用 ESP32 节点，通过 ESPNow 星型拓扑连接传感器和继电器，并配有 RS485 有线备用方案。树莓派作为球道计算机运行 Redis 和状态机，用户界面基于 React 和 WebSocket 构建。

hackernews · section33 · 7月19日 14:41

**背景**: ESP32 是一款低成本、低功耗的微控制器，集成 Wi-Fi 和蓝牙，广泛用于物联网项目。保龄球计分系统是专用且昂贵的设备，常使业主陷入昂贵的服务合同并限制定制化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automatic_scorer">Automatic scorer - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了类似的使用现代技术改造老旧设备的经验，例如使用 1970 年代 Intel 微控制器的迷你保龄球道，以及改造大型机床的业务。爱好者们对添加 LED 追光灯和自助支付系统等功能表示兴趣。

**标签**: `#embedded systems`, `#ESP32`, `#retrofit`, `#cost reduction`, `#DIY`

---

<a id="item-2"></a>
## [阿里巴巴发布 Qwen 3.8，2.4 万亿参数开源大模型](https://twitter.com/Alibaba_Qwen/status/2078759124914098291) ⭐️ 8.0/10

阿里巴巴宣布推出 Qwen 3.8，这是一个 2.4 万亿参数的开源权重大型语言模型，以回应 Moonshot AI 发布的 Kimi K3（2.8 万亿参数）。该模型预计很快将公开发布，延续 Qwen 系列的开源传统。 这一公告加剧了开源大模型领域的竞争，为开发者和研究人员提供了具有宽松许可的前沿规模模型。这也表明中国主要 AI 实验室致力于开源发布，可能加速本地 AI 部署和创新。 Qwen 3.8 拥有 2.4 万亿参数，略小于 Kimi K3 的 2.8 万亿，但两者都是有史以来最大的开源权重模型之一。该模型将通过阿里云提供，并可能发布在 Hugging Face 上，但具体发布日期和更小的蒸馏版本尚未确认。

hackernews · nh43215rgb · 7月19日 08:44 · [社区讨论](https://news.ycombinator.com/item?id=48966120)

**背景**: 大型语言模型的参数是编码知识和推理能力的学习权重；参数越多通常表示能力越强，但计算成本也越高。开源权重模型允许任何人下载、本地运行和微调，与封闭 API 不同。阿里巴巴的 Qwen 系列是重要的开源权重模型家族，之前的 Qwen 3.6 和 3.7 版本因本地使用而广受欢迎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/17/moonshot-ai-kimi-k3-model-openai-anthropic-china.html">China's Moonshot AI unveils Kimi K3 that rivals OpenAI, Anthropic - CNBC</a></li>
<li><a href="https://venturebeat.com/technology/chinas-moonshot-ai-releases-kimi-k3-the-largest-open-source-model-ever-rivaling-top-u-s-systems">China's Moonshot AI releases Kimi K3, the largest open-source model ...</a></li>
<li><a href="https://iternal.ai/llm-parameter-size-guide">LLM Parameter Size Guide: 1B to 1T Explained | Iternal</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，用户对竞争和本地模型使用的潜力感到兴奋。一些用户对访问限制和定价表示不满，而另一些用户则称赞较小 Qwen 模型在本地部署中的性能。少数用户报告了 Qwen 3.7 Pro 的负面体验，认为其可用性不如 DeepSeek。

**标签**: `#LLM`, `#open-weights`, `#Alibaba`, `#Qwen`, `#AI competition`

---

<a id="item-3"></a>
## [Minecraft Java 版切换至 SDL3](https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4) ⭐️ 8.0/10

Minecraft Java 版在最新快照中采用了 SDL3 库，取代了旧的 SDL2 库来处理窗口和输入。 此次更新改进了 GPU API 抽象，更好地支持 Vulkan 和 Metal，有望修复 Linux 上长期存在的输入延迟和切换窗口问题，为数百万玩家提升跨平台性能。 SDL3 的 LWJGL 绑定由 GTNH 模组包团队成员贡献，延续了原版到模组再到原版的贡献循环。但已知问题包括在 Windows 多显示器环境下和 Wayland 上使用独占全屏模式时可能崩溃。

hackernews · ObviouslyFlamer · 7月19日 11:48 · [社区讨论](https://news.ycombinator.com/item?id=48967256)

**背景**: SDL（Simple DirectMedia Layer）是一个跨平台库，通过 OpenGL、Vulkan、Metal 和 Direct3D 提供对音频、键盘、鼠标、手柄和图形硬件的底层访问。SDL3 于 2025 年 1 月发布，是一次重大更新，改进了 GPU API 抽象并现代化了输入处理。Minecraft Java 版使用 LWJGL（轻量级 Java 游戏库）来绑定 SDL 等原生库供 Java 调用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SDL_library">SDL library</a></li>
<li><a href="https://en.m.wikipedia.org/wiki/Simple_DirectMedia_Layer">Simple DirectMedia Layer - Wikipedia</a></li>
<li><a href="https://wiki.libsdl.org/SDL3/Libraries">SDL3 /Libraries - SDL Wiki</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍持积极态度，认为鉴于 SDL2 的 GPU 抽象已显陈旧，切换到 SDL3 是合理的。一些人担心阻塞性 bug，如 Windows 和 Wayland 上的全屏崩溃，希望能在正式版发布前修复。还有一位技术型父亲询问为家人搭建 Minecraft 服务器的建议。

**标签**: `#Minecraft`, `#SDL3`, `#gaming`, `#cross-platform`, `#open source`

---

<a id="item-4"></a>
## [Claude Code 现在使用用 Rust 重写的 Bun](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 8.0/10

6 月 17 日发布的 Claude Code v2.1.181 现在使用 Bun 的 Rust 移植版本，而非原先基于 Zig 的运行时，在 Linux 上启动速度提升了 10%。通过检查二进制文件中的 Rust 源文件路径和 Bun 版本号（1.4.0，高于最新公开发布版本）确认了这一变化。 这一从 Zig 到 Rust 的转变凸显了系统编程领域的一个主要趋势：Rust 的安全性保证越来越受到青睐。这也展示了 AI 辅助的重写如何以最小干扰部署到生产环境中，尽管工程和沟通选择引发了社区的重大讨论。 Bun 的 Rust 移植版本目前作为 canary 版本提供，嵌入在 Claude Code 中的版本（1.4.0）尚未在 canary 之外公开标记。该重写在一个月内作为大型 PR 合并，社区对过程的透明度和成熟度提出了担忧。

rss · Simon Willison · 7月19日 03:54 · [社区讨论](https://news.ycombinator.com/item?id=48966569)

**背景**: Bun 是一个快速的全能 JavaScript 运行时、打包器和包管理器，最初用 Zig 编写。Claude Code 是 Anthropic 的 AI 辅助软件开发工具。将 Bun 用 Rust 重写的决定源于对更好内存安全性和减少 bug 的需求，因为 Zig 需要手动管理内存生命周期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://moony01.com/javascript/2026/05/05/bun-rust-port-debate.html">Bun Rust Port Exposes The AI Rewrite Problem - Moony01 Studio</a></li>
<li><a href="https://www.stork.ai/blog/buns-rust-rewrite-the-betrayal-that-killed-zig">Bun 's Rust Rewrite: An Analysis of the Zig vs. Rust Debate | Stork.AI</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些人质疑为什么一个 TUI 工具需要 JavaScript 运行时，而另一些人则讨论 Zig 与 Rust 的工程优劣。很大一部分人批评重写过程中的沟通方式，认为其不专业且缺乏透明度，尤其是在合并速度如此之快的情况下。

**标签**: `#Claude Code`, `#Bun`, `#Rust`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-5"></a>
## [OpenAI 将 Codex 上下文大小降至 272k tokens](https://github.com/openai/codex/pull/33972/files) ⭐️ 8.0/10

OpenAI 在 GitHub 的一个拉取请求中，将 Codex 模型的上下文窗口从 372k tokens 减少到了 272k tokens。 这一变化引发了关于上下文大小与模型性能之间权衡的讨论，因为更大的上下文可能会降低质量并增加成本，而更小的上下文可能会丢失细节。 上下文从 372k tokens 减少到 272k tokens，而模型的最大上下文据称为 1,050,000 tokens，Codex 仅使用其中一部分。

hackernews · AmazingTurtle · 7月19日 07:54 · [社区讨论](https://news.ycombinator.com/item?id=48965850)

**背景**: 上下文压缩是一种减少模型上下文窗口中 token 数量同时保留重要信息的技术。它用于管理 LLM 应用中的内存和成本。然而，压缩可能导致细节丢失，尤其是在复杂任务中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://getunblocked.com/blog/codex-context-window/">Codex Context Window: How It Works (2026) - Unblocked</a></li>
<li><a href="https://github.com/openai/codex/discussions/1999">How large is the context window when Codex is used via a ChatGPT Plus or Pro plan? · openai/codex · Discussion #1999</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了复杂的感受：一些用户更喜欢 Anthropic 的长上下文，而另一些用户指出模型在更大上下文下会变笨，主张将上下文保持在 300k tokens 以下。一些用户认为压缩效果不佳，更倾向于重新开始。

**标签**: `#OpenAI`, `#Codex`, `#context size`, `#LLM`, `#model performance`

---

<a id="item-6"></a>
## [AI 狂热正在摧毁全球决策能力](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 8.0/10

Nik Suresh 发表了一篇批判性分析，其中充满了来自顾问和工程师的匿名轶事，展示了非理性的 AI 狂热如何导致大型组织做出糟糕的决策。 这篇文章揭示了一个危险趋势：高管们在不懂技术的情况下制定以 AI 为中心的战略，可能浪费数十亿美元并损害真正的创新。 一则轶事描述了一位从未使用过 ChatGPT 的高管为一家市值超过 20 亿美元的公司制定了以 AI 为中心的战略；另一则提到一个 token 排行榜，工程师们为了显得高产而用 Zig 重写代码。

rss · Simon Willison · 7月19日 05:06

**背景**: 文章认为，AI 狂热形成了一个反馈循环，供应商和客户都夸大生产力提升，使得诚实讨论对职业生涯构成风险。这种现象并不新鲜，但被当前的炒作周期放大了。

**社区讨论**: Hacker News 上的评论（文章中提及）可能包括对批评的赞同，分享类似经历，但此处未提供具体评论。

**标签**: `#AI`, `#corporate strategy`, `#tech criticism`, `#engineering culture`

---

<a id="item-7"></a>
## [GPT-2 词汇表以双曲树形式可视化](https://www.reddit.com/r/MachineLearning/comments/1v0pv45/follow_up_gpt2s_vocabulary_as_a_hyperbolic_tree/) ⭐️ 8.0/10

一项新的交互式可视化利用双曲几何将 GPT-2-small 的 32,070 个词元嵌入映射到庞加莱球中，揭示出一个包含一棵大树和许多孤立词元的森林状结构。 这提供了一种直观的方式来探索 GPT-2 嵌入空间中的语义关系，有助于研究人员更好地理解语言模型如何组织词汇。 该布局在嵌入表的压缩表示上使用 t-SNE，边为最小生成树；无需优化或训练，且可视化可在移动设备上运行。

reddit · r/MachineLearning · /u/Limp-Contest-7309 · 7月19日 12:54

**背景**: 双曲几何是一种非欧几何，其空间呈指数级扩展，非常适合嵌入树状结构。庞加莱球模型在单位球内表示双曲空间，而莫比乌斯平移允许在空间中自然导航。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperbolic_tree">Hyperbolic tree - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区称赞该可视化在技术上令人印象深刻且富有洞察力，一些用户讨论了双曲几何的选择以及孤立词元的含义。

**标签**: `#GPT-2`, `#hyperbolic geometry`, `#token embeddings`, `#visualization`, `#NLP`

---

<a id="item-8"></a>
## [软件工程师发现硬件比想象中简单](https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard) ⭐️ 7.0/10

一位软件工程师分享了设计、制造并销售 2500 台名为 JamCorder 的简易 MIDI 录音机的经验，认为如果设计保持极简，硬件可能比软件更简单。 这篇第一手经验挑战了硬件创业天生比软件更难的普遍看法，为考虑硬件产品的独立创客和小团队提供了实用见解。 JamCorder 是一款极简 MIDI 录音机，PCB 上仅有 25 个元件，外壳采用两件式注塑翻盖设计，刻意避开了蓝牙或显示屏等复杂功能。

hackernews · chipweinberger · 7月19日 10:34 · [社区讨论](https://news.ycombinator.com/item?id=48966713)

**背景**: MIDI（乐器数字接口）是一种标准协议，允许电子乐器、计算机和音频设备传输演奏数据，如音符事件和控制信号。MIDI 录音机捕获这些数据用于回放或编辑，通常不录制实际音频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MIDI">MIDI - Wikipedia</a></li>
<li><a href="https://learn.sparkfun.com/tutorials/midi-tutorial/all">MIDI Tutorial - SparkFun Learn</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为硬件难度随复杂度增加；许多人称赞作者的极简方法，但指出大多数产品无法如此简单。一些人还强调了扩大生产和处理真实用户场景的挑战。

**标签**: `#hardware`, `#entrepreneurship`, `#MIDI`, `#product design`, `#software engineering`

---

<a id="item-9"></a>
## [Moonshot AI 因需求过大暂停 Kimi K3 订阅](https://twitter.com/kimi_moonshot/status/2078855608565207130) ⭐️ 7.0/10

Moonshot AI 因过去 48 小时内需求激增，暂时暂停了其 Kimi K3 模型的新订阅，优先保障现有用户的计算资源。 此举突显了以客户为中心的增长策略，并表明像 Kimi K3 这样采用 RNN/线性注意力层以实现高效长上下文处理的新型 AI 架构需求旺盛。 Kimi K3 的 RNN/线性注意力层数量是全注意力层的三倍，特别适合长上下文任务。现有订阅用户不受影响，暂停是暂时的。

hackernews · serialx · 7月19日 16:02 · [社区讨论](https://news.ycombinator.com/item?id=48969291)

**背景**: Moonshot AI 是一家开发 AI 模型和智能工作空间的公司。Kimi K3 是其最新旗舰模型，专为编程、分析和复杂工作流设计，采用了结合 RNN/线性注意力与传统注意力机制的混合架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/en">Kimi AI with K3 | Built for Agentic Coding & Knowledge Work</a></li>
<li><a href="https://www.moonshot.ai/">Moonshot AI</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，称赞 Moonshot AI 以客户为先的做法。一些用户分享了使用 Kimi 进行编程的个人经历，另一些则讨论了 RNN/线性注意力架构的技术优势，并将其与 xLSTM 模型进行比较。

**标签**: `#AI`, `#LLM`, `#subscription`, `#customer experience`, `#RNN`

---

<a id="item-10"></a>
## [最后一个 MPEG-4 视觉专利到期](https://www.phoronix.com/news/Last-MPEG-4-Patent-Expired) ⭐️ 7.0/10

MPEG-4 Part 2（DivX 和 Xvid 背后的编解码器）的最后一个专利已到期，最后一个在巴西有效的专利现已失效。这意味着该编解码器现在在全球范围内可完全免费使用，无需担心专利许可问题。 这一里程碑消除了 21 世纪初最广泛使用的视频编解码器之一的专利障碍，使其可在开源软件、存档项目和旧媒体播放中不受限制地使用。这也凸显了向无专利视频环境缓慢但稳定的进展，尽管 H.264 等较新编解码器仍受专利限制。 到期的专利在巴西持有；美国及欧盟的 MPEG-4 Part 2 专利已于前几年到期。MPEG-4 Part 2 与 H.264（MPEG-4 Part 10）不同，后者在全球仍有有效专利。

hackernews · LorenDB · 7月19日 16:45 · [社区讨论](https://news.ycombinator.com/item?id=48969635)

**背景**: MPEG-4 Part 2，也称为高级简单框架（Advanced Simple Profile），是 1999 年标准化的视频压缩标准。它通过专有的 DivX 和开源的 Xvid 编解码器普及，使 DVD 质量的视频能够放入一张 CD 中。该编解码器在 21 世纪初广泛用于视频分享和 BT 下载，但后来被 H.264 和 H.265 等更高效的编解码器取代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MPEG-4_Part_2">MPEG-4 Part 2 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/MPEG-4">MPEG-4 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，虽然这是积极的一步，但 H.264 专利仍将活跃多年，限制了实际影响。一些人澄清 MPEG-4 Part 2 是 H.263/DivX/Xvid，而非 H.264，另一些人指出 Xvid 解码器已销售数十年，仅对超过一个 B 帧有限制。

**标签**: `#video codecs`, `#patents`, `#MPEG-4`, `#open source`, `#software patents`

---

<a id="item-11"></a>
## [无人出租车监管之争升温](https://techcrunch.com/2026/07/19/techcrunch-mobility-the-battle-over-robotaxi-rules/) ⭐️ 7.0/10

TechCrunch Mobility 报道了围绕无人出租车规则的监管之争日益激烈，凸显了行业参与者与政策制定者之间的紧张关系，同时新的截止日期和州级规则相继出台。 这场监管之争将塑造自动驾驶汽车部署的未来，影响特斯拉、Zoox 和 Nuro 等公司，并决定无人出租车安全扩展的速度。 美国国家公路交通安全管理局（NHTSA）设定了 2028 年发布新无人出租车安全规则手册的截止日期，而加利福尼亚州最近允许无人出租车违反交通法规而不受罚款，引发了争议。

rss · TechCrunch · 7月19日 16:05

**背景**: 当前的联邦规则假设有人类驾驶员，因此没有标准控制装置的车辆需要获得 NHTSA 的临时豁免。目前只有 Zoox 和 Nuro 持有有效的豁免。像加利福尼亚这样的州也在制定自己的规则，导致法规碎片化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.automotiveworld.com/news/nhtsa-sets-2028-deadline-for-new-robotaxi-safety-rulebook/">NHTSA sets 2028 deadline for new robotaxi safety rulebook | Automotive World</a></li>
<li><a href="https://www.mercurynews.com/2026/05/01/robotaxis-can-break-traffic-laws-without-fines-under-new-california-rules/">Robotaxis can break traffic laws without fines under new California rules – The Mercury News</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#regulation`, `#robotaxi`, `#transportation`, `#AI`

---

<a id="item-12"></a>
## [非营利组织 Current AI 致力于为所有人构建免费 AI 网络](https://techcrunch.com/2026/07/19/nonprofit-current-ai-is-racing-to-build-the-world-wide-web-of-ai-free-for-all/) ⭐️ 7.0/10

非营利组织 Current AI 正致力于构建一个免费、包容的 AI 生态系统，使其能在所有文化和设备上运行，类似于 AI 领域的万维网。 这一举措可能使 AI 访问民主化，避免未来 AI 被少数大型企业控制，并确保多元文化的代表性。 Current AI 在跨设备和 AI 聊天方面取得了进展，但公告缺乏具体的技术细节或项目时间表。

rss · TechCrunch · 7月19日 14:00

**背景**: 万维网通过开放和免费的方式彻底改变了信息共享。Current AI 旨在为人工智能复制这一模式，创建一种无论语言、文化或设备能力如何，所有人都能访问的基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/19/nonprofit-current-ai-is-racing-to-build-the-world-wide-web-of-ai-free-for-all/">Nonprofit Current AI is racing to build the World Wide Web of ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#nonprofit`, `#open source`, `#inclusivity`, `#infrastructure`

---

<a id="item-13"></a>
## [通过 SFT 和 RLVR，开源权重 LLM 通过瑞典医学执照考试](https://www.reddit.com/r/MachineLearning/comments/1v0pnoq/passing_the_swedish_medical_licensing_exam_by/) ⭐️ 7.0/10

研究人员对开源权重的大型语言模型进行后训练，应用监督微调（SFT）和基于可验证奖励的强化学习（RLVR），使其能够通过瑞典医学执照考试。 这表明开源权重 LLM 可以有效专用于医学执照等高风险的特定领域任务，可能降低 AI 在受监管领域部署的门槛。 该方法结合了 SFT 进行初始任务适应和 RLVR，后者使用客观、外部可验证的信号（如正确答案）作为奖励，无需人工反馈即可提升推理能力。

reddit · r/MachineLearning · /u/AccomplishedCat4770 · 7月19日 12:44

**背景**: 开源权重 LLM 的参数公开可用，允许针对特定任务进行微调。SFT 使用标注示例调整预训练模型，而 RLVR 使用可验证奖励优化模型，该技术因 DeepSeek-R1 的 Group Relative Policy Optimization 而流行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2506.14245">[2506.14245] Reinforcement Learning with Verifiable Rewards Implicitly ...</a></li>
<li><a href="https://labelstud.io/blog/reinforcement-learning-from-verifiable-rewards/">Reinforcement Learning from Verifiable Rewards | Label Studio</a></li>
<li><a href="https://github.com/opendilab/awesome-RLVR">Awesome RLVR — Reinforcement Learning with - GitHub</a></li>

</ul>
</details>

**标签**: `#LLM`, `#fine-tuning`, `#RLVR`, `#medical AI`, `#SFT`

---