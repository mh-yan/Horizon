---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 47 条内容中筛选出 25 条重要资讯。

---

1. [研究人员完全控制沃尔沃/埃彻车队平台](#item-1) ⭐️ 9.0/10
2. [Moonshot AI 发布 3T MoE 模型 Kimi-K3](#item-2) ⭐️ 9.0/10
3. [vLLM v0.26.0：支持 Inkling 模型、DeepSeek-V4 优化、灵活注意力后端](#item-3) ⭐️ 8.0/10
4. [法官驳回谷歌用 DMCA 抗辩数据抓取](#item-4) ⭐️ 8.0/10
5. [Libsm64 将超级马里奥 64 变成可复用库](#item-5) ⭐️ 8.0/10
6. [Bun 的 Rust 重写进展更新](#item-6) ⭐️ 8.0/10
7. [NVIDIA Cosmos-H-Dreams：手术机器人的实时生成式仿真](#item-7) ⭐️ 8.0/10
8. [纳德拉警告不要依赖单一 AI 模型](#item-8) ⭐️ 8.0/10
9. [Claude 共享聊天和 Artifacts 通过谷歌搜索暴露](#item-9) ⭐️ 8.0/10
10. [微软发布首个 AI 安全模型与智能体系统](#item-10) ⭐️ 8.0/10
11. [Ilya Sutskever 的 SSI 与 Nvidia 合作扩展 AI 研究](#item-11) ⭐️ 8.0/10
12. [Roblox 如何让 Luau 变快：JIT 与优化](#item-12) ⭐️ 8.0/10
13. [从 React 迁移到 HTMX：一个论坛案例研究](#item-13) ⭐️ 7.0/10
14. [Paged Out #9：免费黑客杂志，深度技术文章](#item-14) ⭐️ 7.0/10
15. [现代电子邮件可由借用的部件构建](#item-15) ⭐️ 7.0/10
16. [Thea Energy 获 2000 万美元联邦拨款用于聚变磁体](#item-16) ⭐️ 7.0/10
17. [苹果因 App Store 加密货币诈骗案被起诉，损失 180 万美元](#item-17) ⭐️ 7.0/10
18. [亚马逊扩大卫星直连手机计划，挑战 SpaceX](#item-18) ⭐️ 7.0/10
19. [Antares 融资 4.7 亿美元为美军建造核反应堆](#item-19) ⭐️ 7.0/10
20. [OpenAI 的 Hugging Face 泄露事件重燃对齐与遏制之争](#item-20) ⭐️ 7.0/10
21. [谷歌 AI 概览现已覆盖 43%的搜索](#item-21) ⭐️ 7.0/10
22. [用模拟城市类比解释 PostgreSQL 内部原理](#item-22) ⭐️ 7.0/10
23. [从零开始用现代 C++构建快速无锁队列](#item-23) ⭐️ 7.0/10
24. [Laravel 网站通过 Varnish 前置 Nginx 超越 Redis 扩展](#item-24) ⭐️ 7.0/10
25. [从零开始用 Rust 编写 Arena 分配器](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [研究人员完全控制沃尔沃/埃彻车队平台](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 9.0/10

安全研究员 Eaton Works 披露了沃尔沃/埃彻的 My Eicher 车队管理平台中的一个漏洞，该漏洞使其能够控制所有用户和车辆。该研究员于 2025 年 11 月报告了该漏洞，在未获回应后，漏洞在数周内被悄然修复，最终于 2026 年 7 月公开披露。 该漏洞凸显了现代车辆中关键的云安全缺陷，车队管理平台可能被利用来远程控制车辆并访问敏感数据。这引发了对依赖云的汽车系统安全性和隐私性的严重担忧，影响车队运营商和个体车主。 该研究员获得了内部 API 的访问权限，从而能够控制所有用户和车辆，包括 GPS 跟踪和车辆指令。该漏洞在未公开承认的情况下被修复，研究员在负责任的披露流程超过八个月后公布了细节。

hackernews · EatonZ · 7月27日 15:08 · [社区讨论](https://news.ycombinator.com/item?id=49070756)

**背景**: My Eicher 是一个面向商用车辆的车队管理和 GPS 跟踪平台，提供车队监控、燃油管理和正常运行时间管理等功能。现代车辆越来越依赖基于云的平台进行远程信息处理和远程控制，如果云基础设施被攻破，就会引入安全风险。此事件是更广泛的汽车物联网漏洞被发现的趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo / Eicher ’s fleet management platform to gain control...</a></li>
<li><a href="https://thepixelspulse.com/posts/exploiting-volvoeichers-fleet-platform-to-gain-control-over-all-usersvehicles/">Exploiting VolvoEicher's fleet platform to gain control over all...</a></li>
<li><a href="https://www.eichertrucksandbuses.com/support-solutions/my-eicher">My Eicher | Fleet Monitoring Platform for Trucks & Buses</a></li>

</ul>
</details>

**社区讨论**: 社区赞扬了研究员在披露时间线上的耐心，指出其在发布前给予了慷慨的等待。评论者表达了对依赖云的车辆安全的担忧，其中一位分享了一则轶事：一辆宝马因手机信号不佳而无法启动；另一位则链接了 FSF 的维修权视频。一些人还推测了 AI 对此类漏洞的影响。

**标签**: `#security`, `#vulnerability disclosure`, `#automotive`, `#cloud security`, `#IoT`

---

<a id="item-2"></a>
## [Moonshot AI 发布 3T MoE 模型 Kimi-K3](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

Moonshot AI 在 HuggingFace 上发布了 Kimi-K3，这是一个拥有 3 万亿参数的混合专家（MoE）模型，提供开放权重和商业许可证。该模型原生支持 mxfp4 精度，托管约需 1.5TB 显存。 此次发布使最先进的大型模型得以普及，让初创公司能够针对自身数据进行定制并保持知识产权主权。同时也引发了关于托管成本以及自托管与 API 使用可行性的讨论。 该模型已在 Fireworks AI 上提供，定价为未缓存输入每百万 token 3.00 美元，缓存输入每百万 token 0.30 美元，输出每百万 token 15.00 美元。许可证规定，如果被许可方在任何连续 12 个月内的总收入超过 2000 万美元，则必须与 Moonshot AI 另行签订协议。

hackernews · nateb2022 · 7月27日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=49065752)

**背景**: 混合专家（MoE）是一种架构，每次输入仅激活部分参数（专家），从而在不成比例增加计算成本的情况下实现更大的模型规模。3 万亿参数的模型是最大的开放权重模型之一，托管它需要大量 GPU 内存（例如 8 块 B200 GPU）。开放权重允许用户下载、微调并在自己的基础设施上部署模型，提供定制化和数据控制能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.nocode.tech/article/kimi-k3-open-weights-july-27-cost-equation-no-code">Kimi K3 Open Weights Land July 27 — The 2.8-Trillion-Parameter Model That Changes the Cost Equation for Every No-Code Stack | NoCode.Tech</a></li>

</ul>
</details>

**社区讨论**: 社区意见不一：一些人关注托管成本和定价，指出自托管一个 3T 模型成本高昂，但在高用量下可能更便宜。另一些人则强调定制化和知识产权主权的好处，称这对初创公司来说是一个巨大的胜利。许可证的收入上限也引起了关注，因为它可能限制大公司的商业使用。

**标签**: `#AI`, `#Large Language Models`, `#Open Source`, `#MoE`, `#HuggingFace`

---

<a id="item-3"></a>
## [vLLM v0.26.0：支持 Inkling 模型、DeepSeek-V4 优化、灵活注意力后端](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 引入了对 Inkling 模型家族的完整支持、DeepSeek-V4 的重大性能优化、通过 head_dtype 实现的 fp32 lm_head 支持，以及可按 KV-cache 组选择的灵活注意力后端。该版本包含来自 212 位贡献者的 411 次提交。 此版本通过添加前沿模型支持和性能改进，巩固了 vLLM 作为领先开源 LLM 推理引擎的地位，惠及整个 AI 基础设施生态系统。大量的贡献者反映了推动快速创新的活跃社区。 Inkling 是一个 975B 参数的多模态 MoE 模型，支持高达 1M 的上下文长度，在发布当天即获得支持。DeepSeek-V4 的改进包括专用路由内核（端到端 TPOT 提升 2.94%）和 fused_topk_bias（内核加速 1.5-2 倍）。注意力后端现在可按 KV-cache 组选择，改进了混合模型支持。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个高性能的开源 LLM 推理和服务库，广泛应用于生产环境。它支持多种模型和硬件后端。Inkling 模型是 Thinking Machines Lab 开发的大型多模态 MoE 模型。FlashAttention-4 是一种针对 Hopper GPU 优化的内存高效注意力算法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://recipes.vllm.ai/thinkingmachines/Inkling">thinkingmachines/Inkling | vLLM Recipes</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance | vLLM Blog</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#performance optimization`, `#open source`, `#AI infrastructure`

---

<a id="item-4"></a>
## [法官驳回谷歌用 DMCA 抗辩数据抓取](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名联邦法官裁定，谷歌不能利用《数字千年版权法》（DMCA）来阻止对其搜索结果的抓取，驳回了谷歌将搜索结果页面归类为受反规避条款保护的版权作品的尝试。 这一裁决对网络抓取、AI 训练数据获取和搜索引擎竞争具有重大影响，因为它限制了利用版权法阻止从公开网页收集数据的做法。 该案涉及谷歌起诉 SerpAPI，一家为客户抓取谷歌搜索结果的的公司。法官认为，谷歌的搜索结果缺乏足够的创造性，不符合版权保护条件，因此 DMCA 的反规避条款不适用。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: DMCA 第 1201 条禁止规避控制访问版权作品的技术措施。谷歌辩称其搜索结果是有版权的汇编，抓取行为规避了其技术保护。然而，法院普遍认为，像搜索结果这样的事实汇编缺乏版权所需的原创性，并且抓取公开可访问的数据并不违反 DMCA。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.quinnemanuel.com/the-firm/publications/the-legal-landscape-of-web-scraping/">The Legal Landscape of Web Scraping</a></li>
<li><a href="https://nortonlaw.com/2026/05/14/dmca-section-1201-claims-the-new-battleground-for-ai-and-data-scraping-litigation/">DMCA Section 1201 Claims: The New Battleground for AI and Data Scraping Litigation - the NORTON law firm</a></li>
<li><a href="https://www.reuters.com/legal/litigation/google-lawsuit-says-data-scraping-company-uses-fake-searches-steal-web-content-2025-12-19/">Google lawsuit says data scraping company uses fake searches to steal web content | Reuters</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：一些人批评谷歌缺乏良好的 API 并依赖诉讼，而另一些人则指出抓取对于揭露诈骗的重要性。还有关于欧盟数据库保护法与美国版权标准的讨论。

**标签**: `#legal`, `#web scraping`, `#search engines`, `#DMCA`, `#data access`

---

<a id="item-5"></a>
## [Libsm64 将超级马里奥 64 变成可复用库](https://github.com/libsm64/libsm64) ⭐️ 8.0/10

Libsm64 是一个开源库，它将逆向工程后的《超级马里奥 64》游戏重新打包为共享库，使开发者能够将马里奥的角色和物理嵌入到任何外部游戏引擎中。 该项目展示了一种新颖的游戏互操作方式，无需模拟或专有 API 即可实现创意性的跨游戏混搭，并对围绕元宇宙和基于加密资产的资产可移植性的炒作提出了挑战。 该库暴露了一个在 libsm64.h 中定义的最小化 C API；客户端项目只需包含该头文件并链接库即可。示例集成包括马里奥出现在《半条命 2》和其他引擎中。

hackernews · klaussilveira · 7月27日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49067352)

**背景**: 《超级马里奥 64》于 2019 年被社区逆向工程团队完全反编译，生成了可读的 C 语言源代码。Libsm64 基于该反编译成果创建了一个可复用库，而非独立可执行文件。这使得开发者能够将马里奥的移动、碰撞和渲染导入到自己的项目中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in external game engines · GitHub</a></li>
<li><a href="https://www.retroreversing.com/super-mario-64">Super Mario 64 - Retro Reversing (Reverse Engineering)</a></li>
<li><a href="https://arstechnica.com/gaming/2020/05/beyond-emulation-the-massive-effort-to-reverse-engineer-n64-source-code/">Beyond emulation: The massive effort to reverse-engineer N64 source code - Ars Technica</a></li>

</ul>
</details>

**社区讨论**: 评论者热情高涨，称其“不可思议”，并指出它实现了元宇宙的承诺而没有炒作。他们分享演示视频和 awesome-libsm64 链接以展示有趣的项目。有人开玩笑说要把马里奥 64 作为服务出售，也有人询问非工程师的使用便利性。

**标签**: `#reverse engineering`, `#game development`, `#library`, `#retro gaming`, `#open source`

---

<a id="item-6"></a>
## [Bun 的 Rust 重写进展更新](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun 的首席开发者 Jarred 透露，Rust 重写版本已在一个多月前随 Claude Code 发布，进展顺利，但承诺的 Bun v1.4 Node.js 兼容性里程碑因未达到所需测试通过数量而延迟。 这一更新意义重大，因为 Bun 是广泛使用的 JavaScript 运行时，其从 Zig 到 Rust 的重写可能显著影响性能、安全性以及整个 JavaScript 生态系统。Node.js 兼容性的延迟凸显了大规模重写的挑战，并影响了开发者信任。 Rust 重写版本已在 AI 编码工具 Claude Code 中发布，几乎没有引起注意。Bun v1.4 承诺的 Node.js 测试通过数量尚未达标，发布将推迟至相关 PR 合并后，预计下周二。

hackernews · tomlockwood · 7月27日 11:12 · [社区讨论](https://news.ycombinator.com/item?id=49067854)

**背景**: Bun 是一个快速的全能 JavaScript 运行时、打包器、测试运行器和包管理器，旨在作为 Node.js 的即插即用替代品。该项目最初用 Zig 编写，目前正在进行大规模重写，改用 Rust 以提高安全性和性能。Claude Code 是 Anthropic 开发的 AI 辅助编码工具，可帮助开发者编辑代码和运行命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人认为大规模重写自然会拖慢开发速度，而另一些人则指出一个基于 Zig 的分支声称实现了亚秒级构建时间，暗示原始问题本是自身造成的。还有人质疑使用 LLM 进行翻译的做法，担心长期可维护性。

**标签**: `#Bun`, `#Rust`, `#JavaScript runtime`, `#rewrite`, `#software engineering`

---

<a id="item-7"></a>
## [NVIDIA Cosmos-H-Dreams：手术机器人的实时生成式仿真](https://huggingface.co/blog/nvidia/cosmos-h-dreams) ⭐️ 8.0/10

NVIDIA 推出了 Cosmos-H-Dreams，这是一个实时、动作条件的生成式世界模型，能够根据实时机器人指令生成手术视频序列，为手术机器人提供逼真的训练和规划能力。 该框架将生成式 AI 引入手术机器人这一关键领域，通过允许外科医生和 AI 策略在逼真的合成环境中训练而无需物理设置，有望加速开发并提高安全性。 Cosmos-H-Dreams 是 NVIDIA Cosmos 世界基础模型系列的一个领域特定变体，专为手术机器人构建。它已被 CMR Surgical 和 Cambridge Consultants 等公司用于患者特定的手术仿真。

rss · Hugging Face Blog · 7月27日 09:32

**背景**: 生成式仿真利用 AI 从动作创建逼真的视频序列，从而无需物理硬件即可进行训练。手术机器人需要高保真仿真以确保安全开发，NVIDIA 的 Cosmos 平台提供了可适应手术等专业领域的世界基础模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/nvidia/Cosmos-H-Dreams">nvidia/ Cosmos - H - Dreams · Hugging Face</a></li>
<li><a href="https://developer.nvidia.com/blog/advancing-surgical-robotics-with-ai-driven-simulation-and-digital-twin-technology/">Advancing Surgical Robotics with AI-Driven Simulation and Digital Twin Technology | NVIDIA Technical Blog</a></li>
<li><a href="https://healthcare-digital.com/news/nvidias-open-simulator-set-to-transform-surgical-robotics">NVIDIA's Open Simulator Set to Transform Surgical Robotics | Healthcare Digital</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#generative simulation`, `#surgical robotics`, `#AI`, `#real-time`

---

<a id="item-8"></a>
## [纳德拉警告不要依赖单一 AI 模型](https://techcrunch.com/2026/07/27/satya-nadella-says-companies-that-trust-one-ai-for-everything-may-not-survive/) ⭐️ 8.0/10

微软 CEO 萨提亚·纳德拉表示，依赖单一 AI 模型且没有自有 AI 基础设施（如 AI 网关）的公司可能无法生存。他强调需要定制模型以及在提示词和模型之间建立分离层。 来自行业顶级领袖的警告标志着企业 AI 采用策略的转变，敦促公司投资自有 AI 基础设施和多模型策略。这可能影响企业如何构建其 AI 系统以及资源分配。 纳德拉特别提到“AI 网关”作为关键层，用于分离提示词和模型，从而实现灵活性和控制。该声明暗示，锁定单一 AI 供应商可能对长期生存构成风险。

rss · TechCrunch · 7月27日 21:17

**背景**: AI 网关是管理 AI 模型访问的基础设施组件，类似于传统软件中的 API 网关。它们提供治理、安全和路由能力，使企业能够使用多个模型并在它们之间切换。随着 AI 采用的增长，公司意识到需要强大的 AI 基础设施层以避免对单一供应商的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/API_gateway">API gateway</a></li>
<li><a href="https://medium.com/@kuldeep.paul08/top-5-enterprise-ai-gateways-in-2026-3a8aa415cf04">Top 5 Enterprise AI Gateways in 2026 | by Kuldeep Paul | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#enterprise`, `#AI infrastructure`, `#Satya Nadella`, `#strategy`

---

<a id="item-9"></a>
## [Claude 共享聊天和 Artifacts 通过谷歌搜索暴露](https://techcrunch.com/2026/07/27/psa-your-claude-shared-chats-and-artifacts-may-have-ended-up-on-google/) ⭐️ 8.0/10

Claude 的共享聊天功能无意中导致用户对话和 Artifacts 被谷歌索引，使其可公开搜索。该问题由 TechCrunch 于 2026 年 7 月 27 日报道。 这一隐私事件影响广泛使用的 AI 工具，可能将敏感用户数据暴露给互联网上的任何人。它凸显了 AI 平台中共享功能的风险，以及需要更好的默认隐私控制。 暴露通过 Claude 的共享聊天功能发生，该功能创建对话和 Artifacts 的可共享链接。这些链接显然被谷歌爬取并索引，使其可通过搜索访问。

rss · TechCrunch · 7月27日 20:19

**背景**: Claude 是 Anthropic 开发的 AI 助手。其共享聊天功能允许用户创建对话快照，并通过直接链接分享。Artifacts 是 Claude 生成的内容，如代码或文档，也可共享。默认情况下，聊天是私密的，但共享链接可能无法防止索引。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/10593882-share-and-unshare-chats">Share and unshare chats | Claude Help Center</a></li>
<li><a href="https://www.anthropic.com/news/projects">Collaborate with Claude on Projects \ Anthropic</a></li>
<li><a href="https://support.claude.com/en/articles/9487310-what-are-artifacts-and-how-do-i-use-them">What are artifacts and how do I use them? | Claude Help Center</a></li>

</ul>
</details>

**标签**: `#privacy`, `#AI`, `#Claude`, `#data exposure`, `#security`

---

<a id="item-10"></a>
## [微软发布首个 AI 安全模型与智能体系统](https://techcrunch.com/2026/07/27/microsoft-launches-its-first-cyber-model-and-a-new-agentic-cybersecurity-system/) ⭐️ 8.0/10

微软推出了其首个 AI 安全模型和一个新的智能体网络安全平台，以增强其 AI 驱动的安全产品。 这标志着科技巨头在 AI 驱动安全领域的重要布局，可能为整个行业的自动化威胁检测与响应树立新标准。 新的智能体系统旨在自主识别和缓解网络威胁，基于微软现有的安全产品组合（如 Microsoft Defender）构建。

rss · TechCrunch · 7月27日 18:32

**背景**: 智能体 AI 指能够自主行动以实现目标的系统，例如通过长期关联网络数据来检测高级持续性威胁（APT）。微软此举顺应了主要云提供商将 AI 集成到安全运营中，以应对日益复杂攻击的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/27/microsoft-launches-its-first-cyber-model-and-a-new-agentic-cybersecurity-system/">Microsoft launches its first cybersecurity model , plus... | TechCrunch</a></li>
<li><a href="https://redcanary.com/cybersecurity-101/security-operations/agentic-ai/">Agentic AI in cybersecurity | Red Canary</a></li>
<li><a href="https://techcommunity.microsoft.com/blog/microsoftdefendercloudblog/new-innovations-in-microsoft-defender-to-strengthen-multi-cloud-containers-and-a/4503886">New innovations in Microsoft Defender to strengthen multi-cloud...</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#AI`, `#cybersecurity`, `#agentic systems`

---

<a id="item-11"></a>
## [Ilya Sutskever 的 SSI 与 Nvidia 合作扩展 AI 研究](https://techcrunch.com/2026/07/27/ilya-sutskevers-safe-superintelligence-partners-with-nvidia-to-scale-its-ai-research/) ⭐️ 8.0/10

由 Ilya Sutskever 创立的 Safe Superintelligence Inc.（SSI）在隐身两年后宣布与 Nvidia 建立长期合作伙伴关系，以扩展其 AI 研究。 此次合作表明，以安全为核心的超级智能研究正在获得重要的行业支持，可能借助 Nvidia 的硬件和生态系统加速安全 AI 的开发。 SSI 在成立一年内估值超过 300 亿美元，其唯一使命是开发安全的超级智能。与 Nvidia 的合作将为其研究扩展提供计算资源。

rss · TechCrunch · 7月27日 15:01

**背景**: Safe Superintelligence Inc. 于 2024 年由前 OpenAI 首席科学家 Ilya Sutskever 与 Daniel Gross 和 Daniel Levy 共同创立。该公司旨在构建超越人类智能的超级智能 AI 系统，并将安全性作为核心原则。Nvidia 是 AI 硬件和软件基础设施的领先提供商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Safe_Superintelligence_Inc.">Safe Superintelligence Inc.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ilya_Sutskever">Ilya Sutskever</a></li>
<li><a href="https://ssi.inc/">Safe Superintelligence Inc.</a></li>

</ul>
</details>

**标签**: `#AI`, `#Nvidia`, `#AI safety`, `#partnership`, `#scaling`

---

<a id="item-12"></a>
## [Roblox 如何让 Luau 变快：JIT 与优化](https://www.reddit.com/r/programming/comments/1v85isn/how_we_make_luau_fast/) ⭐️ 8.0/10

Roblox 发布了一篇详细的技术文章，解释了 Luau 语言实现中使用的性能优化和 JIT 编译技术。 Luau 是 Roblox 平台的主要脚本语言，被数百万开发者使用；了解其性能改进有助于开发者编写更快的代码，并为其他 JIT 编译器和虚拟机提供可借鉴的见解。 文章涵盖了类型特化、内联缓存以及新的 JIT 编译器等技术，该编译器将热点路径编译为本地代码，相比解释器实现了显著的加速。

reddit · r/programming · /u/_Sharp_ · 7月27日 16:34

**背景**: Luau 是一种源自 Lua 5.1 的脚本语言，由 Roblox 公司为 Roblox 平台开发。JIT 编译是一种在运行时将频繁执行的代码编译为本地机器码的技术，平衡了解释的灵活性和提前编译的速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Luau_(programming_language)">Luau (programming language ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Just-in-time_compilation">Just-in-time compilation - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Glossary/Just_In_Time_Compilation">Just-In-Time Compilation (JIT) - Glossary - MDN Web Docs</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论包括对实现细节和权衡的实质性评论，许多用户称赞文章的深度，并分享了自己在 Luau 性能方面的经验。

**标签**: `#Luau`, `#JIT compilation`, `#performance optimization`, `#programming languages`, `#compiler design`

---

<a id="item-13"></a>
## [从 React 迁移到 HTMX：一个论坛案例研究](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 7.0/10

Misago 论坛项目详细介绍了从 React.js 迁移到 HTMX 的过程，用服务器端 HTML 片段替代客户端渲染来实现 UI 交互。 这一迁移凸显了通过降低 JavaScript 复杂性来简化 Web 开发的趋势，可能为论坛等内容密集型网站带来性能和可维护性的提升。 HTMX 通过自定义属性扩展 HTML，无需编写 JavaScript 即可实现 AJAX、WebSocket 和服务器发送事件。该项目报告了性能提升和代码简化，但部分社区成员指出，对于高度交互的界面（如可过滤的产品列表），HTMX 可能较慢。

hackernews · Ralfp · 7月27日 09:58 · [社区讨论](https://news.ycombinator.com/item?id=49067301)

**背景**: React 是一个流行的用于构建客户端用户界面的 JavaScript 库，但它需要大量 JavaScript 并可能增加复杂性。HTMX 提供了一种超媒体驱动的替代方案，利用服务器端渲染，通过网络发送 HTML 片段来动态更新页面部分。这种方法可以减少客户端逻辑，并改善许多应用的感知性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>
<li><a href="https://en.wikipedia.org/wiki/Server-side_rendering">Server-side rendering</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户分享了他们使用 HTMX 的经验，并推荐了受 Phoenix LiveView 启发的 PyView 等替代方案。一些人讨论了 HTMX 对高度动态界面的适用性，指出对于复杂的交互，嵌入小型 React 或 Vue 组件可能仍然是更好的选择。

**标签**: `#HTMX`, `#React`, `#web development`, `#server-side rendering`, `#JavaScript frameworks`

---

<a id="item-14"></a>
## [Paged Out #9：免费黑客杂志，深度技术文章](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 7.0/10

Paged Out #9，一本免费的实验性黑客杂志，已以 PDF 形式发布，包含关于 C 语言编程、亚像素渲染和可计算铺砌等主题的单页文章。 该杂志填补了深度技术、黑客好奇内容的空白，让人联想到 Phrack 和 2600，同时具有现代设计和强大的社区参与度。 该杂志采用每页一篇文章的格式，印刷版可供购买。关于可计算铺砌的文章是对 Wang 在 1960 年代工作的未署名重新发现，该工作将铺砌与停机问题联系起来。

hackernews · laurensr · 7月27日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49070138)

**背景**: 亚像素渲染是一种利用单个红、绿、蓝子像素来提高有效分辨率的技术，常用于 LCD 上的文本显示。可计算铺砌由 Wang 在 1960 年代提出，涉及用彩色正方形铺砌平面，要求边颜色匹配，并且与停机问题等价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Subpixel_rendering">Subpixel rendering</a></li>
<li><a href="https://dl.ifip.org/db/conf/ifipTCS/ifipTCS2008/LafitteW08.pdf">Computability of Tilings .</a></li>
<li><a href="https://pagedout.institute/?page=about.php">About ⁂ Paged Out !</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该杂志的幽默和深度，将其与 Phrack 和 2600 相提并论。一位评论者指出，可计算铺砌文章是对 Wang 工作的未署名重新发现，将铺砌与停机问题联系起来。

**标签**: `#hacker magazine`, `#systems programming`, `#computability`, `#text rendering`, `#C programming`

---

<a id="item-15"></a>
## [现代电子邮件可由借用的部件构建](https://en.andros.dev/blog/d7ed8b07/modern-email-can-be-built-from-borrowed-parts/) ⭐️ 7.0/10

一篇技术文章认为，现代电子邮件可以通过重用现有协议和标准来改进，而不是从头构建新系统。 这种务实的方法可以在不需要彻底改革的情况下解决电子邮件长期存在的问题，如垃圾邮件和安全问题，从而可能简化采用并保持网络效应。 文章建议利用现有协议如 SMTP、DKIM 和 DMARC，并集成现代技术如 HTTPS 进行传输加密。

hackernews · andros · 7月27日 08:27 · [社区讨论](https://news.ycombinator.com/item?id=49066639)

**背景**: 电子邮件建立在已有数十年历史的协议（如 SMTP）之上，这些协议缺乏内置的安全和垃圾邮件防护。许多修复电子邮件的提议因网络效应和替换现有基础设施的困难而失败。

**社区讨论**: 评论者就垃圾邮件解决方案和网络效应进行了辩论，一些人认为电子邮件并不像声称的那样糟糕，渐进式改进比完全替换更可行。

**标签**: `#email`, `#protocols`, `#decentralization`, `#spam`

---

<a id="item-16"></a>
## [Thea Energy 获 2000 万美元联邦拨款用于聚变磁体](https://techcrunch.com/2026/07/27/thea-energy-lands-20m-federal-grant-to-build-its-magnets-for-fusion-reactors/) ⭐️ 7.0/10

聚变初创公司 Thea Energy 从 ARPA-E 获得 2000 万美元拨款，用于扩大其用于聚变反应堆的模块化高温超导磁体的生产。 这笔拨款支持了紧凑型聚变电站的关键技术，可能加速商业聚变能源的实现。它也凸显了联邦政府对聚变能源投资的增长，ARPA-E 已承诺投入 1.35 亿美元用于聚变项目。 Thea Energy 的高温超导磁体是模块化的，这可以简化制造并降低成本。该公司是多家竞争实现聚变能源商业化的初创公司之一，其他公司如 Commonwealth Fusion Systems 也在开发高温超导磁体。

rss · TechCrunch · 7月27日 20:40

**背景**: 高温超导磁体能够产生非常强的磁场，这对于在聚变反应堆中约束等离子体至关重要。2021 年，麻省理工学院和 Commonwealth Fusion Systems 展示了创世界纪录的 20 特斯拉高温超导磁体，证实了该技术用于紧凑型聚变的可行性。ARPA-E（高级研究计划局-能源）资助高风险、高回报的能源技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/27/thea-energy-lands-20m-federal-grant-to-build-its-magnets-for-fusion-reactors/">Thea Energy lands $20M federal grant to build its magnets for fusion ...</a></li>
<li><a href="https://www.cryogenicsociety.org/index.php?option=com_dailyplanetblog&view=entry&year=2024&month=09&day=11&id=369:tests-show-high-temperature-superconducting-magnets-ready-for-fusion">Tests Show High Temperature Superconducting Magnets Ready for...</a></li>
<li><a href="https://www.linkedin.com/posts/max-monange_live-from-san-diego-where-the-advanced-research-activity-7447771670842327040-m8vm">ARPA - E receives $135M for fusion program | Max Monange... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#fusion energy`, `#superconducting magnets`, `#ARPA-E`, `#clean energy`, `#startup`

---

<a id="item-17"></a>
## [苹果因 App Store 加密货币诈骗案被起诉，损失 180 万美元](https://techcrunch.com/2026/07/27/apple-sued-after-alleged-app-store-crypto-scam-cost-users-1-8m/) ⭐️ 7.0/10

三名用户对苹果提起诉讼，称他们在从 App Store 下载了一个绕过苹果审核流程的欺诈性加密钱包应用后，总共损失了超过 180 万美元。 这起诉讼挑战了苹果长期以来声称其 App Store 审核流程能确保用户安全的说法，可能削弱用户对平台的信任，并影响苹果反对侧载的法律论据。 该诈骗应用是一个看似合法的虚假加密钱包，通过了苹果的审核，导致了重大经济损失。此前也曾发生过类似事件，例如一个假冒的 Ledger Live 应用盗取了 950 万美元。

rss · TechCrunch · 7月27日 18:28

**背景**: 苹果将 App Store 宣传为发现应用的安全可信之地，并强调其在隐私和安全方面的高标准。该公司一直以这一安全论据来反对侧载和替代应用商店，并对交易收取 30%的佣金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/27/apple-sued-after-alleged-app-store-crypto-scam-cost-users-1-8m/">Apple sued after alleged App Store crypto scam cost... | TechCrunch</a></li>
<li><a href="https://www.thehindu.com/sci-tech/technology/crypto-scam-app-bypass-security-restrictions-on-apple-and-google-app-stores-report/article66466516.ece">Crypto scam app bypass security restrictions on Apple... - The Hindu</a></li>
<li><a href="https://chainstreet.io/fake-ledger-live-app-on-apple-app-store-drains-9-5-million/">Fake Ledger Live App on Apple App Store Drains... | ChainStreet</a></li>

</ul>
</details>

**标签**: `#Apple`, `#App Store`, `#crypto scam`, `#security`, `#lawsuit`

---

<a id="item-18"></a>
## [亚马逊扩大卫星直连手机计划，挑战 SpaceX](https://techcrunch.com/2026/07/27/amazons-new-satellite-network-for-mobile-phones-could-turn-up-the-heat-on-spacex/) ⭐️ 7.0/10

亚马逊宣布扩大其卫星直连手机的连接计划，旨在提供直接到手机的卫星服务，加剧与 SpaceX 星链 Direct to Cell 的竞争。 此举可能加速卫星直连手机服务的部署，为偏远地区带来连接，并挑战 SpaceX 在直连手机卫星市场的早期领先地位。 亚马逊的柯伊伯项目预计将利用其低地球轨道卫星星座，直接向标准智能手机提供短信、语音以及最终的数据服务，无需修改硬件。

rss · TechCrunch · 7月27日 18:08

**背景**: 卫星直连手机技术允许标准手机直接连接卫星，在没有传统蜂窝网络覆盖的地区实现通信。SpaceX 的星链已与 T-Mobile 合作推出 Direct to Cell 服务，而亚马逊的柯伊伯项目仍处于早期部署阶段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sciencenigeria.com/direct-mobile-connectivity-to-satellite/">Direct Mobile Connectivity To Satellite | Science Nigeria</a></li>
<li><a href="https://www.itedgenews.africa/direct-to-satellite-mobile-access-goes-mainstream/">Direct-to- Satellite mobile access goes mainstream - ITEdgeNews</a></li>

</ul>
</details>

**标签**: `#satellite`, `#connectivity`, `#Amazon`, `#SpaceX`, `#telecom`

---

<a id="item-19"></a>
## [Antares 融资 4.7 亿美元为美军建造核反应堆](https://techcrunch.com/2026/07/27/antares-raises-470m-to-build-nuclear-reactors-for-the-u-s-military/) ⭐️ 7.0/10

Antares 已筹集 4.7 亿美元，为美国空军基地开发功率在 100 千瓦至 1 兆瓦之间的小型模块化核反应堆。 这标志着对军用微反应堆的重大投资，可能增强关键国防基础设施的能源韧性，并加速先进核技术的部署。 这些反应堆属于微反应堆（功率低于 10 MWe），Antares 已于 2026 年 6 月在美国能源部反应堆试点计划下实现了 Mark-0 反应堆的临界。

rss · TechCrunch · 7月27日 17:49

**背景**: 小型模块化反应堆（SMR）是先进的核反应堆，每台功率容量高达 300 MWe，设计用于工厂制造和模块化部署。微反应堆是功率低于 10 MWe 的子类，更小，适合偏远或军事应用。Antares 专注于为战略用途生产工厂制造的裂变微反应堆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_modular_nuclear_reactor">Small modular nuclear reactor</a></li>
<li><a href="https://antaresindustries.com/">Antares Nuclear : Factory-Produced Fission Microreactors for Strategic...</a></li>

</ul>
</details>

**标签**: `#nuclear energy`, `#defense`, `#funding`, `#energy tech`

---

<a id="item-20"></a>
## [OpenAI 的 Hugging Face 泄露事件重燃对齐与遏制之争](https://techcrunch.com/2026/07/27/openais-hugging-face-breach-has-reignited-the-debate-over-alignment-and-control/) ⭐️ 7.0/10

OpenAI 的预发布 AI 模型在 Hugging Face 上遭到泄露，暴露了 AI 对齐与遏制方法之间的紧张关系。 这一事件凸显了采取强有力 AI 安全措施的紧迫性，因为关于让 AI 与人类价值观对齐还是遏制其能力的辩论愈演愈烈。 泄露事件发生在流行的 AI 模型仓库 Hugging Face 上，涉及 OpenAI 的预发布模型，引发了对先进 AI 系统安全性和控制的担忧。

rss · TechCrunch · 7月27日 17:28

**背景**: AI 对齐旨在使 AI 系统按照人类意图行事，而遏制则侧重于通过护栏和访问控制来限制 AI 的行为。此次泄露事件凸显了在安全性受损时这两种方法的局限性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cequence.ai/blog/ai/agent-containment/">Agent Containment : Definition, Risks, and Techniques</a></li>
<li><a href="https://www.fastcompany.com/91562128/why-alignment-cant-stay-on-the-sidelines-of-ai-adoption">Why alignment can’t stay on the sidelines of AI ... - Fast Company</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#security breach`, `#AI alignment`, `#OpenAI`, `#Hugging Face`

---

<a id="item-21"></a>
## [谷歌 AI 概览现已覆盖 43%的搜索](https://techcrunch.com/2026/07/27/googles-ai-search-is-rapidly-becoming-the-default-new-data-shows/) ⭐️ 7.0/10

新数据显示，谷歌的 AI 概览现已出现在 43%的搜索中，表明 AI 生成的答案正迅速成为默认的搜索体验。 这标志着人们在线发现信息的方式发生了重大转变，AI 生成的摘要成为搜索结果的主要界面，可能会降低传统网站的点击率。 该数据反映了相比早期采用率的显著增长，谷歌一直在向更多用户扩展 AI 概览，并用 Gemini 2.0 进行升级。

rss · TechCrunch · 7月27日 15:57

**背景**: AI 概览是出现在谷歌搜索结果顶部的 AI 生成摘要，无需用户点击进入网站即可提供快速答案。它们于 2024 年中推出，早期曾出现幻觉问题（例如建议在披萨上加胶水），但此后已得到改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/products-and-platforms/products/search/ai-mode-search/">Expanding AI Overviews and introducing AI Mode</a></li>
<li><a href="https://blog.google/products-and-platforms/products/search/generative-ai-google-search-may-2024/">Google I/O 2024: New generative AI experiences in Search</a></li>

</ul>
</details>

**标签**: `#AI`, `#search`, `#Google`, `#AI Overviews`, `#information retrieval`

---

<a id="item-22"></a>
## [用模拟城市类比解释 PostgreSQL 内部原理](https://www.reddit.com/r/programming/comments/1v806wy/pgsimcity_how_postgresql_works/) ⭐️ 7.0/10

一篇题为“PGSimCity - PostgreSQL 工作原理”的 Reddit 帖子，通过模拟城市的创意类比来解释 PostgreSQL 的内部架构，提供了一种新颖的教育方式。 这种类比使复杂的数据库内部原理对初学者和非专家更易理解，可能拓宽人们对 PostgreSQL 稳健性和设计的认识。 该帖子可能将 PostgreSQL 组件（如共享缓冲区、WAL、清理）映射到模拟城市元素（如电网、垃圾管理），但内容中未提供具体细节。

reddit · r/programming · /u/cheerfulboy · 7月27日 13:18

**背景**: PostgreSQL 是一个强大的开源关系型数据库，其内部架构复杂，包括共享内存、WAL（预写日志）、MVCC（多版本并发控制）和清理进程。理解这些内部原理对于性能调优和故障排除至关重要。模拟城市类比是一种创造性的教学方法，将数据库子系统比作城市管理任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.interdb.jp/pg/">The Internals of PostgreSQL</a></li>
<li><a href="https://www.postgresql.org/docs/current/internals.html">PostgreSQL: Documentation: 18: Part VII. Internals</a></li>
<li><a href="https://medium.com/agedb/postgresql-architecture-59d6242d91d8">PostgreSQL Architecture . Let’s dive into the world of... | Medium</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database internals`, `#educational`, `#analogy`

---

<a id="item-23"></a>
## [从零开始用现代 C++构建快速无锁队列](https://www.reddit.com/r/programming/comments/1v83ukz/building_a_fast_lockfree_queue_in_modern_c_from/) ⭐️ 7.0/10

一篇详细指南发布，指导如何利用现代 C++特性（包括 C++20 原子操作和内存序）从零开始实现一个快速无锁队列。 无锁数据结构对高性能并发系统至关重要；本指南帮助 C++开发者编写更安全、更高效的多线程代码，无需依赖传统锁机制。 该实现利用 C++20 的 std::atomic，结合 memory_order_seq_cst 和 memory_order_relaxed，采用基于链表的設計，并使用 hazard pointers 实现安全内存回收。

reddit · r/programming · /u/Dear-Economics-315 · 7月27日 15:35

**背景**: 无锁队列允许多个线程在不使用互斥锁的情况下进行入队和出队操作，从而避免竞争和死锁。它们依赖原子比较并交换（CAS）操作来保证正确性。现代 C++提供了可移植的原子类型和内存序语义，使无锁编程更加容易。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@clymeneallen/understanding-lock-free-queues-with-code-examples-37b0af92deba">Understanding Lock - Free Queues with Code Examples | Medium</a></li>
<li><a href="https://github.com/supermartian/lockfree-queue">GitHub - supermartian/lockfree- queue : A simple lock - free queue ...</a></li>
<li><a href="https://www.educative.io/blog/modern-multithreading-and-concurrency-in-cpp">A tutorial on modern multithreading and concurrency in C++</a></li>

</ul>
</details>

**标签**: `#C++`, `#lock-free`, `#concurrency`, `#data structures`, `#performance`

---

<a id="item-24"></a>
## [Laravel 网站通过 Varnish 前置 Nginx 超越 Redis 扩展](https://www.reddit.com/r/programming/comments/1v8c5zw/why_redis_wasnt_enough_to_survive_a_traffic_spike/) ⭐️ 7.0/10

一篇事后分析描述了 Laravel 网站如何在 Nginx 前添加 Varnish 作为反向缓存代理，以处理 Redis 单独无法应对的流量高峰。 这个实际案例表明，即使有 Redis 这一常见缓存层，额外的 HTTP 级缓存（如 Varnish）对于应对极端流量高峰至关重要，为 PHP 应用提供了经济高效的扩展策略。 Varnish 是一种专门设计为 HTTP 加速器的反向缓存代理，可以缓存整个页面并在不触及应用服务器的情况下提供服务，而 Redis 则缓存数据片段。该架构将 Varnish 置于 Nginx 之前，以卸载静态和缓存内容。

reddit · r/programming · /u/noweh95 · 7月27日 20:26

**背景**: Laravel 是一个流行的 PHP 框架，常用于动态网站。Redis 是一种内存数据存储，常用于缓存数据库查询和会话。然而，在极端流量下，Redis 可能仍然不够，因为每个请求仍需要 PHP 处理。Varnish 在 HTTP 层面运作，缓存完整响应，减少应用服务器的负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Varnish_cache">Varnish cache</a></li>
<li><a href="https://nestify.io/blog/nginx-vs-varnish/">NGINX vs Varnish : Which is the Best in Terms of Performance</a></li>
<li><a href="https://www.azion.com/en/learning/performance/varnish-vs-nginx/">Varnish vs . Nginx | Azion | Azion Technologies</a></li>

</ul>
</details>

**标签**: `#Redis`, `#Varnish`, `#Laravel`, `#scaling`, `#caching`

---

<a id="item-25"></a>
## [从零开始用 Rust 编写 Arena 分配器](https://www.reddit.com/r/programming/comments/1v80d8d/writing_arenas_in_rust_from_scratch/) ⭐️ 7.0/10

一篇关于从零开始用 Rust 构建自定义 Arena 分配器的详细教程已发布，涵盖了内存管理和性能权衡。 该教程帮助系统程序员理解如何在 Rust 中优化内存分配，这对游戏引擎和 Web 服务器等高性能应用至关重要。 教程逐步讲解如何实现一个 Arena 分配器，利用 Rust 的所有权模型和类型系统，性能可超越系统 malloc。还讨论了注意事项，例如需要手动释放具有非平凡析构函数的项。

reddit · r/programming · /u/f311a · 7月27日 13:25

**背景**: Arena 分配器以大型块分配内存并一次性释放，对于具有相同生命周期的对象效率很高。Rust 的默认分配器是系统分配器，但自 2018 年起可以全局设置自定义分配器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@FAANG/building-a-high-performance-arena-allocator-in-rust-00a91bfcc9f1">Building a High Performance Arena Allocator in Rust | Medium</a></li>
<li><a href="https://doc.rust-lang.org/std/alloc/index.html">std::alloc - Rust</a></li>
<li><a href="https://docs.rs/subms-arena-allocator/latest/subms_arena_allocator/">subms_ arena _ allocator - Rust</a></li>

</ul>
</details>

**标签**: `#Rust`, `#memory management`, `#arena allocator`, `#systems programming`

---