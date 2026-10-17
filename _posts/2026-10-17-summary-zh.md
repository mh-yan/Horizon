---
layout: default
title: "Horizon Summary: 2026-10-17 (ZH)"
date: 2026-10-17
lang: zh
---

> 从 34 条内容中筛选出 15 条重要资讯。

---

1. [DeepSeek 发布 V4.1-Flash-1017，编码能力显著提升](#item-1) ⭐️ 8.0/10
2. [全球太阳能发电量首次超过核能](#item-2) ⭐️ 8.0/10
3. [LWN 7.2 内核统计显示 bug 修复激增，引发 LLM 争论](#item-3) ⭐️ 8.0/10
4. [OpenCode 被曝泄露用户 API 凭证，引发安全讨论](#item-4) ⭐️ 8.0/10
5. [Xolotl 在单张 RTX 4090 上以 27 tok/s 运行 552B DeepSeek-V4.1-Flash](#item-5) ⭐️ 8.0/10
6. [Qwen 27B 在 16GB RX 9070 XT 上通过 ROCm KV 流式实现完整 262k 上下文](#item-6) ⭐️ 8.0/10
7. [白化珊瑚与健康克隆体接触后可在数天内恢复](#item-7) ⭐️ 7.0/10
8. [Pele 将 Mermaid 图表渲染为可主题化的 SVG，无需浏览器](#item-8) ⭐️ 7.0/10
9. [爱沙尼亚网络投票系统源代码在 GitHub 上公开](#item-9) ⭐️ 7.0/10
10. [开源 ESP32 模拟器让固件在浏览器中运行](#item-10) ⭐️ 7.0/10
11. [爱好者用五台消费设备分布式运行 48 层 MoE 模型，达 37-39 tok/s](#item-11) ⭐️ 7.0/10
12. [开发者通过 MoE 卸载在 16GB AMD Radeon 上运行 35B Fish Audio Drama 3 TTS](#item-12) ⭐️ 7.0/10
13. [DeepSeek V4.1 Flash 1017 的去审查版与 GGUF 量化版发布](#item-13) ⭐️ 7.0/10
14. [NVIDIA 发布 Dory1.0-4B：具备 256K 上下文的循环潜在递归 LLM](#item-14) ⭐️ 7.0/10
15. [ds4 通过 PR #1225 新增对 DeepSeek V4.1 Flash 1017 的支持](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek 发布 V4.1-Flash-1017，编码能力显著提升](https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek-V4.1-Flash-1017，这是其 V4.1-Flash 模型在 2026 年 10 月 17 日的快照版本，现已在官网、应用和 API 上线。官方称该版本在基准测试中表现更强、任务完成更快、输出更短，是性能与成本上的帕累托改进。 此次发布加剧了面向编码的大模型竞争，社区成员指出它在 11 项编码基准中的 10 项上击败了 Sol 5.6，为专有模型提供了一个快速且开放的选择。其速度与开放性可能使其成为智能体编码工作流和成本敏感开发者的实用默认选项。 该模型是多模态混合专家（MoE）架构，主干参数 552B，支持最长一百万 token 的上下文，以 deepseek-flash 的 API 名称提供服务，也可通过 OpenRouter 和 Ollama 获取。社区测试表明它能快速发现高优先级问题，但也可能给出一些无关结果，且基准领先并不保证在每个任务上都更优。

hackernews · theykk · 10月17日 08:21 · [社区讨论](https://news.ycombinator.com/item?id=50129045)

**背景**: DeepSeek 是一家以低成本发布强能力模型著称的中国 AI 实验室，其 V4.1-Flash 系列主打快速高效的推理。SWE-bench、LiveCodeBench 等编码基准是衡量大模型在真实软件工程任务上表现的标准方式，而 OpenRouter 是一个统一 API 平台，让开发者可以在多个模型之间路由请求。混合专家模型每个 token 只激活部分参数，因此尽管总参数量很大，推理成本仍然较低。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news261017/">DeepSeek - V 4 . 1 - Flash - 1017 : Wish-Driven Programming Made Real</a></li>
<li><a href="https://ollama.com/library/deepseek-v4.1-flash:1017-cloud">deepseek - v 4 . 1 - flash : 1017 -cloud</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4.1-flash-1017">DeepSeek V 4 . 1 Flash 1017 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者称赞 DeepSeek 的速度、低首 token 延迟和开放性——例如可见的思维链和更少的拦截——认为尽管它并非每项基准都领先，但“感觉”比 Sol 和 Gemini 更好。其他人强调了非高峰时段的成本节省和生态多样性，而一位用户的实际对比发现它能快速发现一个 P1 问题，但也给出了一个无关结果。

**标签**: `#AI/ML`, `#LLM`, `#DeepSeek`, `#benchmarks`, `#model release`

---

<a id="item-2"></a>
## [全球太阳能发电量首次超过核能](https://www.pv-magazine.com/2026/09/29/solar-surpasses-nuclear-power-globally-for-first-time/) ⭐️ 8.0/10

全球太阳能发电量首次超过核能，太阳能装机容量在新增 510 GW 后同比增长 27%至 2,383 GW，而核能装机容量仅增长 1.5 GW 至 399.5 GW。从 2025 年 3 月到 2026 年 6 月，太阳能或风能每月都单独超过核能发电量，并且在 2026 年 3 月、4 月和 5 月两者同时超过核能。 这一里程碑表明，快速扩张的间歇性可再生能源在实际发电量上可以超过增长缓慢的基荷核能，从而改变关于未来电网主导电源的假设。它标志着太阳能正成为全球主要电力来源，对能源政策、投资和脱碳规划具有重大影响。 该比较基于实际发电的太瓦时数，而非铭牌容量；太阳能容量系数较低（约 20–30%），而核能容量系数很高（通常接近 90–100%），这意味着太阳能需要多得多的装机容量才能超过核能发电量。风能也正接近核能发电量，而下一个重大里程碑——太阳能超过水力发电——按当前增速预计还需数年时间。

hackernews · xbmcuser · 10月17日 14:01 · [社区讨论](https://news.ycombinator.com/item?id=50131256)

**背景**: 容量系数是指一段时间内实际发电量与电厂连续满功率运行可能的最大发电量之比；太阳能受日照和天气限制，而核电站通常接近满功率运行。自 2014 年以来，全球太阳能装机容量增长了十倍以上，2024 年总装机容量突破 2 太瓦，当年太阳能已占发电量约 22%，而核能占 21.6%。这些趋势解释了为何太阳能快速新增装机能够在总发电量上超过核能，尽管其单位容量出力较低。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.weforum.org/stories/energy-transition/solar-power-to-surpass-nuclear-and-more-top-energy-stories/">Solar power set to surpass nuclear – and more top energy stories</a></li>
<li><a href="https://www.statista.com/statistics/183680/us-average-capacity-factors-by-selected-energy-source-since-1998/">Capacity factor by energy source 2024 US | Statista</a></li>
<li><a href="https://www.linkedin.com/posts/johnanoonan_global-solar-power-installation-crosses-2tw-activity-7346043599853146112-63KZ">Global solar power installation crosses 2TW in 2024 . | John Noonan</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，尽管核能容量系数高得多，这一里程碑反映的是实际发电的太瓦时数，并提到风能紧随其后，而太阳能正快速领先。一些人惋惜核能数十年的停滞延误了无化石燃料电网的实现，另一些人则强调必须进一步加速清洁能源部署，以替代所有肮脏能源而不仅是电力，包括合成石化原料。

**标签**: `#energy`, `#solar`, `#nuclear`, `#renewables`, `#climate`

---

<a id="item-3"></a>
## [LWN 7.2 内核统计显示 bug 修复激增，引发 LLM 争论](https://lwn.net/Articles/1088776/) ⭐️ 8.0/10

LWN 发布了 7.2 内核的开发统计数据，指出每个版本修复的 bug 数量急剧上升——自 2026 年 4 月以来增长超过一倍——并引发了社区关于 LLM 辅助内核开发及此类指标可靠性的争论。 bug 修复数量的激增表明 LLM 工具正在显著加速内核维护，可能提升安全性和稳定性，但也引发了人们对 AI 生成补丁的质量和审查负担的担忧，尤其是在 Linux 这样关键的项目中。 统计数据显示，自 2026 年 4 月以来，每个版本修复的 bug 数量增长了 2 倍以上，内核每个版本修复的 CVE 接近 2000 个，而 6.x 时代大部分时间约为 500 个；然而，批评者指出缺乏实验对照来将 LLM 的影响与其他因素区分开来。

hackernews · farlight · 10月17日 17:14 · [社区讨论](https://news.ycombinator.com/item?id=50132950)

**背景**: LWN.net 定期发布每个 Linux 内核版本的开发统计数据，通过分析 git 提交元数据来展示谁贡献了更改以及更改的来源。Linux 内核是一个庞大的开源项目，拥有严格的审查流程，近年来基于 LLM 的工具在代码生成和 bug 修复中的使用日益增多。这引发了关于自动化与人工监督之间平衡的争论，Linus Torvalds 和 Greg Kroah-Hartman 等人物也对 AI 辅助贡献发表了看法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/1066723/">Development statistics for the 7.0 kernel - lwn.net</a></li>
<li><a href="https://tech.yahoo.com/ai/articles/linux-kernel-nears-record-2-093000473.html">Linux kernel nears record 2,000 vulnerabilities per release as AI bug ...</a></li>
<li><a href="https://www.tomshardware.com/software/linux/linus-torvalds-posts-his-first-llm-assisted-patch-to-the-linux-kernel-after-issuing-clear-pro-ai-directives-the-bossman-makes-use-of-ai-tooling-himself">Linus Torvalds posts his first AI- assisted patch to the Linux kernel ...</a></li>

</ul>
</details>

**社区讨论**: 评论者分享说，LLM 代理有助于自动化 bug 复现和修复，使过程更快，但减少了 bug 报告的数量，因为用户依赖代理来绕过问题。其他人批评缺乏对照实验来衡量 LLM 的影响，还有人指出需要对机器生成的代码（如 amdgpu 头文件）设置限制。

**标签**: `#linux-kernel`, `#open-source`, `#llm`, `#software-development`, `#community-discussion`

---

<a id="item-4"></a>
## [OpenCode 被曝泄露用户 API 凭证，引发安全讨论](https://twitter.com/opencode/status/2111516673953935833) ⭐️ 8.0/10

开源 AI 编程代理 OpenCode 被曝泄露用户 API 凭证，该事件登上 Hacker News 首页（623 分，98 条评论）。发帖作者称帖子遭到 OpenCode 粉丝或团队成员的标记（flag），而官方尚未清晰披露泄露范围。 该事件凸显了托管型 AI 编程服务在处理用户自带密钥（BYOK，涉及 Anthropic、Google、OpenAI 等提供商）时的供应链与密钥存储风险。它也暴露出缺乏标准化的 API 密钥失效机制，迫使用户在争分夺秒中手动轮换密钥。 社区成员尚不清楚泄露仅影响在 OpenCode Zen 中存储 BYOK 密钥的用户，还是针对 OpenCode 程序本身的供应链攻击。帖子在 HN 上被标记以及 OpenCode 缺乏官方事件报告，进一步加剧了这种不确定性。

hackernews · pranshuchittora · 10月17日 18:01 · [社区讨论](https://news.ycombinator.com/item?id=50133401)

**背景**: OpenCode 是一款开源、本地优先的 AI 编程代理，可在终端、IDE 或桌面运行，并支持多种模型提供商。部分用户通过名为 OpenCode Zen 的托管服务使用它，其模式类似 OpenRouter：用户可自带 API 密钥（BYOK），或使用服务方密钥并按 token 计费。API 密钥是访问付费模型 API 的敏感凭证，一旦泄露可能导致未授权使用和账单欺诈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>
<li><a href="https://opencode.ai/docs/">Intro | AI coding agent built for the terminal - opencode.ai</a></li>
<li><a href="https://open-code.dev/">OpenCode - Open-Source AI Coding Agent</a></li>

</ul>
</details>

**社区讨论**: 评论者对事件范围表示困惑，询问仅本地使用自有凭证的用户是否受影响，以及这是否为供应链攻击。一个高赞建议是每个 API 密钥系统都应提供“invalidate_api_key”端点，以便白帽或存储方在泄露时一次性吊销所有密钥，而不是让每个人各自行动。

**标签**: `#security`, `#api-keys`, `#credential-leak`, `#supply-chain`, `#incident-response`

---

<a id="item-5"></a>
## [Xolotl 在单张 RTX 4090 上以 27 tok/s 运行 552B DeepSeek-V4.1-Flash](https://www.reddit.com/r/LocalLLaMA/comments/1x8m0jj/xolotl_strata_based_deepseekv41flash_552b_on_a/) ⭐️ 8.0/10

一位开发者发布了 Xolotl，这是一个基于 Strata 的推理引擎，能在单张 RTX 4090（24GB 显存）、Ryzen 7 5700X、90GB DDR4 内存和一块 NVMe 硬盘上运行完整的 552B 参数 DeepSeek-V4.1-Flash 模型，解码速度达到 27 tok/s，预填充速度为 180–320 tok/s，支持 512K 上下文。该引擎还能运行 GLM-5.3-Flash、Qwen3.8-Flash-Next 和 Qwen3.8-27B，预计几天内会推出基于 1017 版本的未审查量化模型。 这表明 552B 参数的混合专家模型可以运行在消费级游戏硬件上，而不再需要多 GPU 服务器，从而大幅降低了运行前沿规模本地大模型的门槛。如果该方法能够推广，可能会改变本地 LLM 社区对内存层级和模型规模上限的认知。 该引擎将权重分布在显存、锁页内存和 NVMe 之间，只按每个 token 的需要拉取相应的专家，并在真实服务器上开启思考模式后报告 HumanEval 21/21、工具调用 10/10、智能体修 bug 循环 3/3 的成绩。当前未审查量化模型为 152 GiB，而即将推出的 1017 更新是 510GB 的下载，尽管架构和分词器相同，但权重不同，因此需要完整重新校准和量化。

reddit · r/LocalLLaMA · /u/indrasmirror · 10月17日 21:40

**背景**: 混合专家（MoE）模型每个 token 只激活一小部分参数，因此计算量较低，但仍然需要将所有专家权重存储在某个地方。Strata 是一个开源 C++ 推理引擎，旨在通过将休眠专家在显存、系统内存和 NVMe 存储之间流式传输，让 Qwen3.8-Flash-Next 等大型 MoE 模型能在 12–24GB 显存的消费级 GPU 上运行。GSQ 是 ISTA Das 实验室提出的一种训练后标量量化方法，可将权重压缩到每参数 2–3 比特，且精度损失极小，使模型能够装入远小于原始大小的内存中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.locker/Niko1221/Strata">Strata on GitHub (Niko1221/ Strata ) — FAQ & Similar Projects...</a></li>
<li><a href="https://github.com/xero00000/expert-streaming-engine">GitHub - xero00000/expert-streaming-engine: Run oversized ...</a></li>
<li><a href="https://arxiv.org/abs/2604.18556">[2604.18556] GSQ: Highly-Accurate Low-Precision Scalar ... What Are GSQ and RCO? Das Lab's New LLM Quantization Method GitHub - IST-DASLab/GSQ: Gumbel-Softmax post-training ... GSQ: Highly-Accurate Low-Precision Scalar Quantization for ... LLM Quantization: GGUF vs AWQ vs GPTQ Compared 2026 — TeqVolt GSQ - a ISTA-DASLab Collection - Hugging Face LLM Quantization Guide 2026 — GGUF vs AWQ vs GPTQ</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#inference-engine`, `#model-quantization`, `#deepseek`, `#consumer-hardware`

---

<a id="item-6"></a>
## [Qwen 27B 在 16GB RX 9070 XT 上通过 ROCm KV 流式实现完整 262k 上下文](https://www.reddit.com/r/LocalLLaMA/comments/1x89ptz/qwen_27b_iq4_xs_q8q4_kv_at_full_262k_context_on_a/) ⭐️ 8.0/10

一位开发者将自适应 KV 流式从 CUDA 移植到 ROCm/HIP，使 Qwen3.8-27B（IQ4_XS 权重，Q8_0/Q4_0 KV 缓存）能在单张 16GB RX 9070 XT 上以完整的 262,144 token 上下文运行。该实现借助 MTP 达到 80+ t/s 的解码速度，在 262k 上下文下预填充为 585.8 t/s，同时将完整 KV 缓存保留在主机内存中，并通过 PCIe SDMA 流式传输有限的工作集。 这表明仅有 16GB 显存的消费级 AMD GPU 也能处理此前被认为需要大得多的内存才能实现的超长上下文，显著降低了本地长上下文推理的门槛。它还说明 ROCm/HIP 生态可以通过社区移植追上仅限 CUDA 的优化，使 AMD 用户受益，并推动 llama.cpp 更广泛的支持。 模型的 IQ4_XS 权重约 14.3GB，经 ASCII 精简版将非 ASCII 词表裁剪至约 13.6GB，留下约 3.4GiB 可用显存；262k 的 KV 缓存需要约 7.4GiB，因此被保留在主机内存中，并以预填充约 450MiB、解码约 2,100MiB 的工作集进行流式传输。启用 MTP 的解码速度在 1k–4k token 时为 71.8–86.5 t/s，在 262k 时降至 31.1 t/s；将显卡功耗限制在 231W（降低 24%）仅带来 3.6% 的预填充延迟损失，解码吞吐几乎不变。

reddit · r/LocalLLaMA · /u/bottlestreet3d · 10月17日 13:01

**背景**: llama.cpp 是一个流行的开源推理引擎，用于在本地运行大语言模型，而 IQ4_XS 等量化技术将模型权重压缩到 4 位以适应消费级硬件。KV 缓存保存所有先前 token 的注意力键和值，随上下文长度线性增长，在长上下文下会迅速耗尽显存。自适应 KV 流式将完整缓存保留在锁定的主机内存中，仅将所需页面流式传输到 GPU；HIP 是 AMD 类似 CUDA 的 API，允许开发者以较小改动将 NVIDIA 代码移植到 ROCm。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/RaymondHuang210129/llama.cpp-adaptive-kv-streaming">GitHub - RaymondHuang210129/ llama . cpp - adaptive - kv - streaming ...</a></li>
<li><a href="https://rocm.docs.amd.com/projects/HIP/en/latest/how-to/hip_porting_guide.html">Porting CUDA code to HIP — HIP 7.16.0 Documentation - AMD</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/5063">Even more quantization types? · ggml-org llama.cpp ... - GitHub</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#ROCm`, `#KV-cache`, `#local-LLM`, `#AMD-GPU`

---

<a id="item-7"></a>
## [白化珊瑚与健康克隆体接触后可在数天内恢复](https://www.nature.com/articles/d41586-026-03266-x) ⭐️ 7.0/10

《自然》新闻报道的一项新研究发现，白化珊瑚在与健康的邻近珊瑚直接接触时可在数天内恢复，但这种救援效应似乎要求两者是基因完全相同的克隆体。 这一发现为珊瑚礁保护带来了难得的好消息，并提示了一种辅助珊瑚恢复的潜在机制，但其对克隆邻近体的依赖限制了它在野外的广泛应用。 这种恢复效应仅在基因相同的珊瑚之间观察到，这意味着珊瑚礁管理者需要通过基因检测来识别相容的克隆体，而通过断裂繁殖的克隆珊瑚可能形成集群，从而可将白化片段放置在健康克隆体附近。

hackernews · alkyon · 10月16日 23:38 · [社区讨论](https://news.ycombinator.com/item?id=50126253)

**背景**: 珊瑚白化是热应激导致珊瑚排出其共生藻（虫黄藻）的过程，这些藻类为珊瑚提供营养和颜色；失去这些藻类后，珊瑚会变白并可能死亡。当前全球白化事件是有记录以来最大的一次，此前的纪录是 2014 至 2017 年影响全球 68.2%的珊瑚礁区域。同种珊瑚在接触时有时可以融合组织，而基因相同的克隆体可通过断裂繁殖产生。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scienmag.com/a-gentle-touch-healthy-corals-can-rescue-bleached-neighbors-in-days/">A Gentle Touch: Healthy Corals Can Rescue Bleached Neighbors ...</a></li>
<li><a href="https://coralreefwatch.noaa.gov/satellite/research/coral_bleaching_report.php">NOAA Coral Reef Watch Current Global Bleaching: Status Update ...</a></li>
<li><a href="https://lab.bluehub.jp/en/coral-zooxanthellae-symbiosis/">Coral and Zooxanthellae Symbiosis Explained: The Mechanism of...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者对该发现的实际应用普遍持怀疑态度：一位潜水员指出，在大堡礁，白化范围如此之广，以至于在很大距离内往往找不到健康的邻近珊瑚；其他人则指出，仅限克隆体的要求使这一发现的实用价值有限。一些评论者还质疑该结果的新颖性，并提到珊瑚繁殖和海水水族爱好者社区已有相关知识。

**标签**: `#coral-reefs`, `#marine-biology`, `#science-news`, `#climate-change`, `#hackernews-discussion`

---

<a id="item-8"></a>
## [Pele 将 Mermaid 图表渲染为可主题化的 SVG，无需浏览器](https://pele.run/) ⭐️ 7.0/10

Pele 是 Obsidian 推出的一款开源工具，它使用 CSS 变量将 Mermaid 图表渲染为可主题化的 SVG，可能无需无头浏览器。该工具在其网站（pele.run）上发布，并在 Hacker News 上引发讨论，用户指出其易于嵌入的潜力。 Mermaid 广泛用于文档和笔记应用中的图表绘制，但其官方库通常需要浏览器环境进行布局，这给服务器端或嵌入式渲染带来了复杂性。Pele 的方法可以简化在静态网站、Markdown 编辑器和其他非浏览器环境中嵌入 Mermaid 图表的过程，使开发者和 Obsidian 等工具受益。 Pele 是一个轻量级库，使用 CSS 变量为 SVG 输出设置主题，便于自定义。源代码已在 GitHub 的 obsidianmd 组织下公开，确认了其开源性质。

hackernews · dchest · 10月17日 15:55 · [社区讨论](https://news.ycombinator.com/item?id=50132193)

**背景**: Mermaid 是一个流行的开源图表绘制工具，允许用户使用类似 Markdown 的语法从文本创建图表。传统上，渲染 Mermaid 图表需要浏览器环境（通常是无头浏览器）来计算布局并生成 SVG，这对于服务器端或嵌入式使用可能很麻烦。可主题化的 SVG 指的是可以动态设置样式的 SVG 图形，例如使用 CSS 变量，以匹配不同的视觉主题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mermaid.js.org/">Mermaid | Diagramming and charting tool</a></li>
<li><a href="https://pele.run/">Pele · Mermaid diagrams as themeable SVG</a></li>
<li><a href="https://en.wikipedia.org/wiki/Headless_browser">Headless browser - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Mermaid 在复杂图表中的布局质量表示失望，认为 Pele 在样式上的改进是次要的。其他人强调了开源可见性的重要性，建议项目突出显示 GitHub 链接，并指出“pele”在拉脱维亚语中意为“老鼠”。

**标签**: `#mermaid`, `#svg`, `#diagramming`, `#open-source`, `#obsidian`

---

<a id="item-9"></a>
## [爱沙尼亚网络投票系统源代码在 GitHub 上公开](https://github.com/valimised/ivxv) ⭐️ 7.0/10

爱沙尼亚网络投票系统（i-voting）的源代码已在 GitHub 的 valimised/ivxv 仓库中公开，并在 Hacker News 上引发了讨论。 此次发布是一个重要的透明度里程碑，因为该国家电子投票平台自 2005 年以来已用于具有法律约束力的选举，允许安全研究人员和公众审查系统的实现，可能增强对在线投票的信任。 IVXV 系统自 2017 年以来已用于爱沙尼亚地方选举，但个人可验证性仍然是一个挑战；研究表明，受感染的投票设备可以通过利用重新投票选项来破坏个人可验证性机制。

hackernews · theanonymousone · 10月17日 03:18 · [社区讨论](https://news.ycombinator.com/item?id=50127586)

**背景**: 爱沙尼亚是第一个在 2005 年通过互联网举行具有法律约束力的大选的国家，并自 2007 年以来广泛使用网络投票。IVXV 系统是其网络投票软件的当前版本。端到端可验证投票系统旨在提供强大的完整性和防篡改能力，但实现个人可验证性——允许选民确认其选票被正确记录——尤其困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electronic_voting_in_Estonia">Electronic voting in Estonia - Wikipedia</a></li>
<li><a href="https://eprint.iacr.org/2021/1098">Individual Verifiability and Revoting in the Estonian ... - IACR</a></li>
<li><a href="https://en.wikipedia.org/wiki/End-to-end_auditable_voting">End-to-end auditable voting - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者就安全性和信任影响展开辩论：一些人认为仅靠软件无法确保选举安全，需要通过统计抽样进行选举后验证；另一些人指出爱沙尼亚的系统已被广泛接受，并且多年来一直是开源的。一位爱沙尼亚当地人表达了对系统依赖政府信任的担忧，另一位提到了美国选举中使用的 ElectionGuard 等现有可验证系统。

**标签**: `#e-voting`, `#security`, `#open-source`, `#elections`, `#verifiability`

---

<a id="item-10"></a>
## [开源 ESP32 模拟器让固件在浏览器中运行](https://github.com/mikroverk/esp32sim) ⭐️ 7.0/10

一位开发者发布了 esp32sim，这是一个完全在浏览器中执行固件的开源 ESP32 模拟器，演示中没有任何物理 ESP32 参与。该项目旨在让 ESP32 软件更容易进行实验、测试和模拟，而无需连接硬件。 该工具通过支持无需物理板卡的快速原型设计和 CI/CD 测试，可能显著降低嵌入式开发的门槛，从而加速物联网项目的工作流程。它也顺应了通过 WebAssembly 在浏览器中运行复杂模拟的日益增长的趋势。 该模拟器基于 WebAssembly 构建，根据项目文档，目前至少支持 ESP32-S3 开发板。作者正在积极寻求嵌入式开发者的反馈，了解在实际开发、测试和 CI 使用中需要哪些功能。

hackernews · joakimeriksson · 10月17日 13:51 · [社区讨论](https://news.ycombinator.com/item?id=50131189)

**背景**: ESP32 是一款广受欢迎的低成本、低功耗微控制器系列，集成了 Wi-Fi 和蓝牙，广泛用于物联网设备。此类模拟器允许开发者在计算机上运行和调试固件，而不是将其烧录到物理硬件上，这对于测试和持续集成特别有用。WebAssembly 使得此类模拟器能在网页浏览器中达到接近原生的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32 - Wikipedia</a></li>
<li><a href="https://www.espressif.com/en/products/socs/esp32">ESP32 Wi-Fi & Bluetooth SoC | Espressif Systems</a></li>

</ul>
</details>

**社区讨论**: 评论者认为该项目令人印象深刻，有人分享了一个类似的无人机模拟器，该模拟器以 WebAssembly 运行真实的 ESP32 飞控代码。其他人指出了在 CI/CD 测试中的潜在用途，并询问它与 Wokwi 有何不同，还有一人批评了 README 中密集的 AI 生成格式。

**标签**: `#ESP32`, `#emulator`, `#embedded-systems`, `#WebAssembly`, `#open-source`

---

<a id="item-11"></a>
## [爱好者用五台消费设备分布式运行 48 层 MoE 模型，达 37-39 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1x8ley0/2_gaming_pcs_an_m4_pro_macbook_over_ethernet_2/) ⭐️ 7.0/10

一位爱好者（u/StayLameBro）展示了如何通过以太网和 USB-C 将两台游戏 PC、一台 M4 Pro MacBook 和两台 iPhone 17 Pro Max 连接起来，分布式运行 Qwen 3.8 Flash Next——一个每层 512 个专家的 48 层混合专家模型。该配置在 60k 上下文下达到 37-39 tokens/s 的解码速度，另一种布局在 164k 上下文下达到 31-33 tok/s。 该实验表明，异构消费设备可以串联起来运行远超单机内存的大模型，推动了本地 LLM 推理的边界。它为爱好者提供了实用蓝图，并可能启发更易用的分布式推理工具。 模型按层拆分：PC1（RTX 2060 Super）负责第 0-9 层及输出层和草稿头，MacBook 负责第 10-29 层，iPhone 负责第 10-18 层的专家计算，PC2（RX 9060 XT）负责第 30-47 层。利用多令牌预测草稿头的流水线投机解码平均每步产出约 2.2 个令牌，所有重量都驻留在显存/内存中，无需磁盘流式加载。

reddit · r/LocalLLaMA · /u/StayLameBro · 10月17日 21:13

**背景**: 混合专家（MoE）模型每个令牌只激活部分专家，降低了计算量但需要大量内存来存储所有专家。多令牌预测（MTP）草稿头让模型猜测后续多个令牌，然后通过单次前向传播验证，从而加速生成。像 distributed-llama 和 Exo 这样的分布式推理框架旨在通过以太网汇聚消费硬件，协作运行大模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://github.com/b4rtaz/distributed-llama">GitHub - b4rtaz/distributed-llama: Distributed LLM inference ...</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#distributed-inference`, `#mixture-of-experts`, `#consumer-hardware`, `#model-sharding`

---

<a id="item-12"></a>
## [开发者通过 MoE 卸载在 16GB AMD Radeon 上运行 35B Fish Audio Drama 3 TTS](https://www.reddit.com/r/LocalLLaMA/comments/1x8kces/fish_audio_drama_3_says_it_needs_a_48_gb_nvidia/) ⭐️ 7.0/10

一位开发者构建了“Red Curtain”工具，通过将 FP8 专家缓存到系统内存并仅将活跃专家加载到 GPU，在 16GB AMD RX 9070 显卡上运行了 Fish Audio Drama 3——一个 350 亿参数的混合专家文本转语音模型。该工具实现了慢于实时的语音生成（例如 13 秒生成 3.3 秒语音），同时使用约 11-12 GB 显存和 35 GB 内存。 这表明大型 MoE 模型可以在显存远低于官方要求的消费级 AMD 硬件上运行，可能让没有高端 NVIDIA 显卡的用户也能使用先进的 TTS 技术。同时，它也凸显了 MoE 卸载技术和 AMD 的 ROCm 生态系统在本地 AI 部署中日益重要的作用。 该模型总参数为 350 亿，但每个 token 仅激活约 30 亿参数，FP8 专家（约 32 GB）保留在系统内存中，其余部分在 GPU 上以 BF16 运行。已知问题包括偶尔在生成第一行后静音（这是模型本身的怪癖，vLLM 配方中也有提及），且该工具仅在 RX 9070（gfx1201）上测试过；权重需从 Hugging Face 单独下载。

reddit · r/LocalLLaMA · /u/fechyyy · 10月17日 20:27

**背景**: 混合专家（MoE）模型对每个 token 仅激活一部分参数，这减少了计算量，但仍需将所有参数存储在内存中。卸载技术将不活跃的专家保留在较慢的系统内存中，仅将需要的专家加载到 GPU，从而使大型模型能在显存有限的 GPU 上运行。FP8 是一种 8 位浮点格式，相比 BF16 可减少内存占用，同时保持合理的精度。AMD 的 ROCm 是一个用于 GPU 计算的开源软件栈，相当于 NVIDIA CUDA 的对应物。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2401.14361v2">MoE -Infinity: Offloading -Efficient MoE Model Serving</a></li>
<li><a href="https://www.spheron.network/blog/fp8-quantization-inference-performance-hardware-explained/">What is FP8 Quantization? AI Inference Performance, Accuracy ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AMD_ROCm">AMD ROCm</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#AMD-ROCm`, `#MoE-offloading`, `#TTS`, `#consumer-hardware`

---

<a id="item-13"></a>
## [DeepSeek V4.1 Flash 1017 的去审查版与 GGUF 量化版发布](https://www.reddit.com/r/LocalLLaMA/comments/1x8ke24/deepseek_v41_flash_1017_gguf_abliterated/) ⭐️ 7.0/10

一位社区成员发布了 DeepSeek V4.1 Flash 1017 的去审查（abliterated）版本，并为原始模型和去审查模型提供了 GGUF 量化文件；该方法采用秩-2 子空间移除技术，使聊天模式下的拒绝率从 97/100 降至 4/100，思考模式下从 98/100 降至 9/100。 这为本地 LLM 社区提供了一个新发布模型的早期、技术精细的去审查衍生版本，表明多方向拒绝移除可以在保持模型质量的同时大幅降低拒绝率，对在本地运行无审查模型的用户具有重要意义。 作者分别测量了聊天模式和思考模式下的拒绝方向，并移除了它们所张成的秩-2 子空间，而非单一方向，优先保证模型完整性而非消除所有拒绝；GGUF 量化文件已提供（imatrix 尚未完成，仍在进行中），并为 GGUF 用户提供了 LoRA 以避免重新下载权重。

reddit · r/LocalLLaMA · /u/mrfakename0 · 10月17日 20:29

**背景**: 去审查（abliteration）是一种通过从模型权重中投影移除特定激活方向来消除拒绝行为的技术，这些方向通常从有害提示数据中识别。GGUF 是 llama.cpp 用于在本地以更低内存运行 LLM 的量化文件格式。DeepSeek V4.1 Flash 1017 是近期发布的模型，本帖是社区制作的衍生版本，而非官方发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vynaris.com/blog/what-is-abliteration-llm-refusal-removal">What Is Abliteration? LLM Refusal Removal Explained</a></li>
<li><a href="https://mbrenndoerfer.com/writing/gguf-format-quantized-llm-storage-inference">GGUF : Storage and Inference for Quantized LLMs - Interactive</a></li>
<li><a href="https://abliteration.org/wiki/academic-research/">Academic papers on abliteration and refusal removal ...</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#abliteration`, `#gguf`, `#deepseek`, `#model-quantization`

---

<a id="item-14"></a>
## [NVIDIA 发布 Dory1.0-4B：具备 256K 上下文的循环潜在递归 LLM](https://www.reddit.com/r/LocalLLaMA/comments/1x8bg1u/nvidianvidianemotronlabsdory104bbf16_hugging_face/) ⭐️ 7.0/10

NVIDIA 发布了 NVIDIA-Nemotron-Labs-Dory1.0-4B-BF16，这是一个 40 亿参数的语言模型，采用循环（潜在递归）归一化 GPT 架构，交替使用滑动窗口注意力和全注意力层，支持高达 256K 个 token 的上下文。该模型以 OpenMDW 许可协议 1.1 版在 Hugging Face 上发布，允许商业和非商业使用。 这对本地 LLM 社区来说是一个值得关注的发布，因为它在一个小型、开放许可的模型中展示了循环深度扩展方法，可能以较少的参数提供强大的推理能力。如果该架构被证明有效，它可能影响未来高效模型的设计，并使长上下文推理在消费级硬件上更易实现。 该模型通过重复应用共享层块来为每个 token 投入更多计算，并交替使用滑动窗口注意力和全注意力层来高效处理长上下文。它以 BF16 精度发布，仅支持英语，定位为小体积下的通用推理模型。

reddit · r/LocalLLaMA · /u/silenceimpaired · 10月17日 14:20

**背景**: 循环语言模型在多次迭代中重用相同的 Transformer 块，从而在不增加参数的情况下有效增加深度，能以更低的内存成本提升推理能力。滑动窗口注意力限制每个 token 只关注先前 token 的局部窗口，从而减少长序列的计算量，而全注意力层则保留全局信息。OpenMDW 许可证是专为机器学习模型及其相关产物设计的宽松许可证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/looped-language-models">Looped Language Models : Iterative Transformer Refinement</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/visual-attention-variants">A Visual Guide to Attention Variants in Modern LLMs</a></li>
<li><a href="https://openmdw.ai/license/1-1/">OpenMDW-1.1 | OpenMDW</a></li>

</ul>
</details>

**标签**: `#LLM`, `#NVIDIA`, `#recurrent-architecture`, `#local-llm`, `#model-release`

---

<a id="item-15"></a>
## [ds4 通过 PR #1225 新增对 DeepSeek V4.1 Flash 1017 的支持](https://www.reddit.com/r/LocalLLaMA/comments/1x8koix/deepseek_v41_flash_1017_support_for_ds4_pr_1225/) ⭐️ 7.0/10

PR #1225 为 ds4（dwarfstar）本地推理项目新增了对 DeepSeek-v4.1-Flash-1017 检查点的兼容支持，包括新的 engrams 和更新后的视觉塔。该改动会校验视觉模型与语言模型文件是否匹配，并在混搭时抛出错误；而使用 ds4 量化套件量化的文件无需任何修改即可加载。 由于架构未变，本地推理用户无需等待核心内核改动即可在 ds4 上运行最新的 DeepSeek Flash 检查点。这对 LocalLLaMA 社区很重要，因为它让一个快速迭代的专有检查点在发布后不久就能在消费级硬件上使用。 约 40% 的路由专家张量发生变化，engrams 中约 30% 变化，视觉塔的专家张量约 50% 变化，但架构保持不变，可直接套用现有内核。作者计划为 128GB 机器发布 Q2–Q8 混合量化版本，并辅以少量 SSD 卸载（常驻 152GB，含 engrams 共 366GB），预计在 M5 Max 上解码速度约为每秒 20 个 token。

reddit · r/LocalLLaMA · /u/returnity · 10月17日 20:42

**背景**: ds4（又称 DwarfStar 4）是 antirez 开发的本地推理引擎，用于在本地运行 DeepSeek V4 Flash 和 PRO 模型，它借鉴了 llama.cpp 和 GGML 的思路，但并不链接这些库。DeepSeek 的 Engram 模块为模型主干加入条件式 n-gram 记忆，这里的“engrams”指的就是这些记忆张量。量化会压缩模型权重（如 Q2–Q8 格式），使大模型能装入有限内存，而混合量化则对不同张量采用不同精度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash and PRO local ...</a></li>
<li><a href="https://github.com/deepseek-ai/Engram">GitHub - deepseek -ai/ Engram : Conditional Memory via Scalable...</a></li>
<li><a href="https://deepseek.ai/blog/deepseek-engram-v4-architecture">DeepSeek Engram — V4 Memory Architecture Explained</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#deepseek`, `#quantization`, `#inference`, `#llama-cpp`

---