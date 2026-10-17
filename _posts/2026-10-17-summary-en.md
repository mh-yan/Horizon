---
layout: default
title: "Horizon Summary: 2026-10-17 (EN)"
date: 2026-10-17
lang: en
---

> From 34 items, 15 important content pieces were selected

---

1. [DeepSeek Releases V4.1-Flash-1017 With Strong Coding Gains](#item-1) ⭐️ 8.0/10
2. [Solar generation overtakes nuclear power globally for the first time](#item-2) ⭐️ 8.0/10
3. [LWN's 7.2 kernel statistics show surge in bug fixes, sparking LLM debate](#item-3) ⭐️ 8.0/10
4. [OpenCode Reportedly Leaks User API Credentials, Sparking Security Debate](#item-4) ⭐️ 8.0/10
5. [Xolotl runs 552B DeepSeek-V4.1-Flash on a single RTX 4090 at 27 tok/s](#item-5) ⭐️ 8.0/10
6. [Qwen 27B runs full 262k context on 16GB RX 9070 XT via ROCm KV streaming](#item-6) ⭐️ 8.0/10
7. [Bleached corals can recover within days when touching a healthy clone](#item-7) ⭐️ 7.0/10
8. [Pele renders Mermaid diagrams as themeable SVG without a browser](#item-8) ⭐️ 7.0/10
9. [Estonia's i-voting source code now public on GitHub](#item-9) ⭐️ 7.0/10
10. [Open-source ESP32 emulator runs firmware in the browser](#item-10) ⭐️ 7.0/10
11. [Hobbyist runs 48-layer MoE model across five consumer devices at 37-39 tok/s](#item-11) ⭐️ 7.0/10
12. [Developer runs 35B Fish Audio Drama 3 TTS on 16GB AMD Radeon via MoE offloading](#item-12) ⭐️ 7.0/10
13. [Abliterated DeepSeek V4.1 Flash 1017 released with GGUF quants](#item-13) ⭐️ 7.0/10
14. [NVIDIA Releases Dory1.0-4B: A Looped Latent-Recurrent LLM with 256K Context](#item-14) ⭐️ 7.0/10
15. [ds4 adds DeepSeek V4.1 Flash 1017 support via PR #1225](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek Releases V4.1-Flash-1017 With Strong Coding Gains](https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash-1017) ⭐️ 8.0/10

DeepSeek released DeepSeek-V4.1-Flash-1017, an October 17, 2026 snapshot of its V4.1-Flash model, now live on its website, app, and API. The company claims stronger benchmark performance, faster task completion, and shorter outputs than the previous version, describing it as a Pareto improvement in performance and cost. The release intensifies competition among coding-focused LLMs, with community members noting it beats Sol 5.6 on 10 of 11 coding benchmarks and offers a fast, open alternative to proprietary models. Its speed and openness could make it a practical default for agentic coding workflows and cost-sensitive developers. The model is a multimodal Mixture-of-Experts (MoE) with 552B backbone parameters and support for contexts up to one million tokens, served under the deepseek-flash API name and also available via OpenRouter and Ollama. Community testing suggests it is fast at finding high-priority issues but may surface some irrelevant findings, and benchmark leadership does not guarantee superiority on every task.

hackernews · theykk · Oct 17, 08:21 · [Discussion](https://news.ycombinator.com/item?id=50129045)

**Background**: DeepSeek is a Chinese AI lab known for releasing capable models at low cost, and its V4.1-Flash line targets fast, efficient inference. Coding benchmarks such as SWE-bench and LiveCodeBench are standard ways to compare LLMs on real software engineering tasks, while OpenRouter is a unified API platform that lets developers route prompts across many models. Mixture-of-Experts models activate only part of their parameters per token, keeping inference cheaper despite a large total parameter count.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news261017/">DeepSeek - V 4 . 1 - Flash - 1017 : Wish-Driven Programming Made Real</a></li>
<li><a href="https://ollama.com/library/deepseek-v4.1-flash:1017-cloud">deepseek - v 4 . 1 - flash : 1017 -cloud</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4.1-flash-1017">DeepSeek V 4 . 1 Flash 1017 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters praised DeepSeek's speed, low time-to-first-token, and openness—such as visible chain-of-thought and fewer blocks—saying it 'feels' better than Sol and Gemini despite not topping every benchmark. Others highlighted off-peak cost savings and ecosystem diversity, while one user's hands-on comparison found it fast at spotting a P1 issue but also producing an irrelevant finding.

**Tags**: `#AI/ML`, `#LLM`, `#DeepSeek`, `#benchmarks`, `#model release`

---

<a id="item-2"></a>
## [Solar generation overtakes nuclear power globally for the first time](https://www.pv-magazine.com/2026/09/29/solar-surpasses-nuclear-power-globally-for-first-time/) ⭐️ 8.0/10

Global solar electricity generation has surpassed nuclear power for the first time, with solar capacity rising 27% year on year to 2,383 GW after adding 510 GW, while nuclear capacity grew only 1.5 GW to 399.5 GW. From March 2025 through June 2026, either solar or wind individually out-generated nuclear every month, and in March, April, and May 2026 both did so simultaneously. This milestone shows that rapidly scaling variable renewables can outpace slow-growing baseload nuclear in actual delivered energy, reshaping assumptions about which sources dominate future grids. It signals that solar is becoming a primary electricity source globally, with major implications for energy policy, investment, and decarbonization planning. The comparison is based on actual generated terawatt-hours, not nameplate capacity, and solar's lower capacity factor (roughly 20–30%) versus nuclear's high capacity factor (often near 90–100%) means solar needed far more installed capacity to overtake nuclear output. Wind is also nearing nuclear generation, and the next major milestone—solar surpassing hydroelectric generation—is expected to take several more years at current growth rates.

hackernews · xbmcuser · Oct 17, 14:01 · [Discussion](https://news.ycombinator.com/item?id=50131256)

**Background**: Capacity factor is the ratio of actual electricity produced over a period to the maximum possible output if a plant ran at full power continuously; solar's is limited by daylight and weather, while nuclear plants typically run near full output. Solar installations have grown more than tenfold since 2014, pushing total global capacity past 2 TW in 2024, and solar already accounted for about 22% of electricity generation versus nuclear's 21.6% in that year. These trends explain why solar's rapid capacity additions can translate into surpassing nuclear in total generated energy despite lower per-unit output.

<details><summary>References</summary>
<ul>
<li><a href="https://www.weforum.org/stories/energy-transition/solar-power-to-surpass-nuclear-and-more-top-energy-stories/">Solar power set to surpass nuclear – and more top energy stories</a></li>
<li><a href="https://www.statista.com/statistics/183680/us-average-capacity-factors-by-selected-energy-source-since-1998/">Capacity factor by energy source 2024 US | Statista</a></li>
<li><a href="https://www.linkedin.com/posts/johnanoonan_global-solar-power-installation-crosses-2tw-activity-7346043599853146112-63KZ">Global solar power installation crosses 2TW in 2024 . | John Noonan</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that the milestone reflects actual generated terawatt-hours despite nuclear's much higher capacity factor, and noted wind is close behind while solar races ahead. Some lamented decades of nuclear stagnation that delayed a fossil-free grid, while others stressed that clean energy deployment must accelerate further to replace all dirty energy sources, not just electricity, including synthetic petrochemical feedstocks.

**Tags**: `#energy`, `#solar`, `#nuclear`, `#renewables`, `#climate`

---

<a id="item-3"></a>
## [LWN's 7.2 kernel statistics show surge in bug fixes, sparking LLM debate](https://lwn.net/Articles/1088776/) ⭐️ 8.0/10

LWN published its development statistics for the 7.2 kernel, highlighting a sharp rise in bugs fixed per release—more than double the historical rate since April 2026—and prompting community debate about LLM-assisted kernel development and the reliability of such metrics. The surge in bug fixes suggests LLM tools are significantly accelerating kernel maintenance, potentially improving security and stability, but also raising concerns about the quality and review burden of AI-generated patches in a project as critical as Linux. The statistics show a more than 2× rise in bugs fixed per release since April 2026, with the kernel nearing 2,000 CVEs fixed per release compared to roughly 500 during much of the 6.x era; however, critics note the lack of experimental controls to isolate LLM impact from other factors.

hackernews · farlight · Oct 17, 17:14 · [Discussion](https://news.ycombinator.com/item?id=50132950)

**Background**: LWN.net regularly publishes development statistics for each Linux kernel release, analyzing git commit metadata to show who contributed changes and where they came from. The Linux kernel is a massive open-source project with a rigorous review process, and recent years have seen increasing use of LLM-based tools for code generation and bug fixing. This has led to debates about the balance between automation and human oversight, with figures like Linus Torvalds and Greg Kroah-Hartman weighing in on AI-assisted contributions.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1066723/">Development statistics for the 7.0 kernel - lwn.net</a></li>
<li><a href="https://tech.yahoo.com/ai/articles/linux-kernel-nears-record-2-093000473.html">Linux kernel nears record 2,000 vulnerabilities per release as AI bug ...</a></li>
<li><a href="https://www.tomshardware.com/software/linux/linus-torvalds-posts-his-first-llm-assisted-patch-to-the-linux-kernel-after-issuing-clear-pro-ai-directives-the-bossman-makes-use-of-ai-tooling-himself">Linus Torvalds posts his first AI- assisted patch to the Linux kernel ...</a></li>

</ul>
</details>

**Discussion**: Commenters shared that LLM agents help automate bug reproduction and fixing, making the process faster but reducing the number of bug reports as users rely on agents to work around issues. Others criticized the lack of controlled experiments to measure LLM impact, and some noted the need for limits on machine-generated code like amdgpu header files.

**Tags**: `#linux-kernel`, `#open-source`, `#llm`, `#software-development`, `#community-discussion`

---

<a id="item-4"></a>
## [OpenCode Reportedly Leaks User API Credentials, Sparking Security Debate](https://twitter.com/opencode/status/2111516673953935833) ⭐️ 8.0/10

OpenCode, an open-source AI coding agent, reportedly leaked user API credentials, with the incident reaching the front page of Hacker News (623 points, 98 comments). The post's author claims it was flagged by OpenCode fans or team members, and the company has not clearly disclosed the scope of the leak. This incident highlights the supply-chain and key-storage risks of hosted AI coding services that handle users' bring-your-own-key (BYOK) credentials for providers like Anthropic, Google, and OpenAI. It also underscores the lack of standardized API key invalidation mechanisms, forcing users to manually rotate keys in a race against time. Community members are unsure whether the leak affected only OpenCode Zen users who stored BYOK keys, or whether it was a supply-chain attack on the OpenCode program itself. The ambiguity is compounded by the post being flagged on HN and the absence of an official incident report from OpenCode.

hackernews · pranshuchittora · Oct 17, 18:01 · [Discussion](https://news.ycombinator.com/item?id=50133401)

**Background**: OpenCode is an open-source, local-first AI coding agent that runs in the terminal, IDE, or desktop and supports multiple model providers. Some users access it through a hosted service called OpenCode Zen, which works similarly to OpenRouter: users can bring their own API keys (BYOK) or use the service's keys and pay per token. API keys are sensitive credentials that grant access to paid model APIs, so leaks can lead to unauthorized usage and billing fraud.

<details><summary>References</summary>
<ul>
<li><a href="https://opencode.ai/">OpenCode | The open source AI coding agent</a></li>
<li><a href="https://opencode.ai/docs/">Intro | AI coding agent built for the terminal - opencode.ai</a></li>
<li><a href="https://open-code.dev/">OpenCode - Open-Source AI Coding Agent</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion about the scope, asking whether local users with their own credentials are affected and whether this was a supply-chain attack. One top suggestion was that every API key system should provide an 'invalidate_api_key' endpoint so whitehats or the storing party can revoke all leaked keys at once, rather than leaving everyone to act individually.

**Tags**: `#security`, `#api-keys`, `#credential-leak`, `#supply-chain`, `#incident-response`

---

<a id="item-5"></a>
## [Xolotl runs 552B DeepSeek-V4.1-Flash on a single RTX 4090 at 27 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1x8m0jj/xolotl_strata_based_deepseekv41flash_552b_on_a/) ⭐️ 8.0/10

A developer released Xolotl, a Strata-based inference engine that runs the full 552B-parameter DeepSeek-V4.1-Flash model on a single RTX 4090 (24GB VRAM), Ryzen 7 5700X, 90GB DDR4 and an NVMe drive, achieving 27 tok/s decode and 180–320 tok/s prefill with 512K context. The engine also runs GLM-5.3-Flash, Qwen3.8-Flash-Next and Qwen3.8-27B, and an uncensored 1017 quant is expected within a couple of days. This demonstrates that a 552B-parameter mixture-of-experts model can be served on consumer gaming hardware rather than a multi-GPU server, which significantly lowers the barrier to running frontier-scale local LLMs. If the approach generalizes, it could reshape how the local-LLM community thinks about memory hierarchy and model size limits. The engine spreads weights across VRAM, pinned RAM and NVMe, pulling in only the experts each token needs, and reports 21/21 on HumanEval, 10/10 tool calls and 3/3 agentic bug-fix loops through the real server with thinking enabled. The current uncensored quant is 152 GiB, while the upcoming 1017 update is a 510GB download requiring a full recalibration and quantization because the weights differ even though architecture and tokenizer are identical.

reddit · r/LocalLLaMA · /u/indrasmirror · Oct 17, 21:40

**Background**: Mixture-of-experts (MoE) models activate only a small subset of their parameters per token, which keeps compute low but still requires all expert weights to be stored somewhere. Strata is an open-source C++ inference engine designed to run large MoE models like Qwen3.8-Flash-Next on consumer GPUs with 12–24GB of VRAM by streaming dormant experts between VRAM, system RAM and NVMe storage. GSQ is a post-training scalar quantization method from ISTA's Das Lab that compresses weights to 2–3 bits per parameter with minimal accuracy loss, enabling models to fit into far less memory.

<details><summary>References</summary>
<ul>
<li><a href="https://github.locker/Niko1221/Strata">Strata on GitHub (Niko1221/ Strata ) — FAQ & Similar Projects...</a></li>
<li><a href="https://github.com/xero00000/expert-streaming-engine">GitHub - xero00000/expert-streaming-engine: Run oversized ...</a></li>
<li><a href="https://arxiv.org/abs/2604.18556">[2604.18556] GSQ: Highly-Accurate Low-Precision Scalar ... What Are GSQ and RCO? Das Lab's New LLM Quantization Method GitHub - IST-DASLab/GSQ: Gumbel-Softmax post-training ... GSQ: Highly-Accurate Low-Precision Scalar Quantization for ... LLM Quantization: GGUF vs AWQ vs GPTQ Compared 2026 — TeqVolt GSQ - a ISTA-DASLab Collection - Hugging Face LLM Quantization Guide 2026 — GGUF vs AWQ vs GPTQ</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#inference-engine`, `#model-quantization`, `#deepseek`, `#consumer-hardware`

---

<a id="item-6"></a>
## [Qwen 27B runs full 262k context on 16GB RX 9070 XT via ROCm KV streaming](https://www.reddit.com/r/LocalLLaMA/comments/1x89ptz/qwen_27b_iq4_xs_q8q4_kv_at_full_262k_context_on_a/) ⭐️ 8.0/10

A developer ported adaptive KV streaming from CUDA to ROCm/HIP, enabling Qwen3.8-27B (IQ4_XS weights, Q8_0/Q4_0 KV cache) to run at its full 262,144-token context on a single 16GB RX 9070 XT. The implementation achieves 80+ t/s decode with MTP and 585.8 t/s prefill at 262k, while keeping the full KV cache in host RAM and streaming bounded working sets over PCIe SDMA. This demonstrates that consumer AMD GPUs with only 16GB VRAM can handle extremely long contexts previously thought to require much larger memory, significantly lowering the barrier for local long-context inference. It also shows the ROCm/HIP ecosystem can catch up to CUDA-only optimizations through community ports, benefiting AMD users and pressuring broader llama.cpp support. The model's IQ4_XS weights are ~14.3GB, and an ASCII-condensed version trims non-ASCII vocabulary to ~13.6GB, leaving ~3.4GiB usable VRAM; the 262k KV cache needs ~7.4GiB, so it is kept in host RAM and streamed as ~450MiB prefill and ~2,100MiB decode working sets. Decode with MTP ranges from 71.8–86.5 t/s at 1k–4k tokens down to 31.1 t/s at 262k, and running the card at a 231W power limit (-24%) costs only 3.6% prefill latency with virtually identical decode throughput.

reddit · r/LocalLLaMA · /u/bottlestreet3d · Oct 17, 13:01

**Background**: llama.cpp is a popular open-source inference engine for running large language models locally, and quantization techniques like IQ4_XS shrink model weights to 4-bit to fit on consumer hardware. KV cache stores attention keys and values for all previous tokens, growing linearly with context length and quickly exhausting VRAM on long contexts. Adaptive KV streaming keeps the full cache in pinned host RAM and streams only the needed pages to the GPU, while HIP is AMD's CUDA-like API that lets developers port NVIDIA code to ROCm with modest changes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/RaymondHuang210129/llama.cpp-adaptive-kv-streaming">GitHub - RaymondHuang210129/ llama . cpp - adaptive - kv - streaming ...</a></li>
<li><a href="https://rocm.docs.amd.com/projects/HIP/en/latest/how-to/hip_porting_guide.html">Porting CUDA code to HIP — HIP 7.16.0 Documentation - AMD</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/5063">Even more quantization types? · ggml-org llama.cpp ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#ROCm`, `#KV-cache`, `#local-LLM`, `#AMD-GPU`

---

<a id="item-7"></a>
## [Bleached corals can recover within days when touching a healthy clone](https://www.nature.com/articles/d41586-026-03266-x) ⭐️ 7.0/10

A new study reported by Nature finds that bleached corals can recover within days when they are in direct contact with a healthy neighboring coral, but the rescue effect appears to require the two corals to be genetically identical clones. The finding offers a rare piece of good news for reef conservation and suggests a potential mechanism for assisted coral recovery, but its dependence on clonal neighbors limits how widely it can be applied in the wild. The recovery effect was observed only between genetically identical corals, meaning reef managers would need genetic testing to identify compatible clones, and clonal corals that reproduce by fragmentation may form clusters where a bleached fragment could be placed near a healthy clone.

hackernews · alkyon · Oct 16, 23:38 · [Discussion](https://news.ycombinator.com/item?id=50126253)

**Background**: Coral bleaching occurs when heat stress causes corals to expel their symbiotic algae, called zooxanthellae, which provide them with nutrients and color; without these algae, corals turn white and can die. The ongoing global bleaching event is the largest on record, with the previous record during 2014–2017 affecting 68.2% of the world's reef area. Corals of the same species can sometimes fuse tissues when they meet, and genetically identical clones can arise through fragmentation.

<details><summary>References</summary>
<ul>
<li><a href="https://scienmag.com/a-gentle-touch-healthy-corals-can-rescue-bleached-neighbors-in-days/">A Gentle Touch: Healthy Corals Can Rescue Bleached Neighbors ...</a></li>
<li><a href="https://coralreefwatch.noaa.gov/satellite/research/coral_bleaching_report.php">NOAA Coral Reef Watch Current Global Bleaching: Status Update ...</a></li>
<li><a href="https://lab.bluehub.jp/en/coral-zooxanthellae-symbiosis/">Coral and Zooxanthellae Symbiosis Explained: The Mechanism of...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely skeptical about real-world applicability: a diver noted that on the Great Barrier Reef, bleaching is so widespread that healthy neighbors are often absent for vast distances, while others pointed out that the clone-only requirement makes the finding of limited practical use. Some commenters also questioned the novelty of the result, citing existing knowledge in the coral propagation and saltwater aquarium communities.

**Tags**: `#coral-reefs`, `#marine-biology`, `#science-news`, `#climate-change`, `#hackernews-discussion`

---

<a id="item-8"></a>
## [Pele renders Mermaid diagrams as themeable SVG without a browser](https://pele.run/) ⭐️ 7.0/10

Pele is an open-source tool from Obsidian that renders Mermaid diagrams as themeable SVG using CSS variables, potentially eliminating the need for a headless browser. It was announced on its website (pele.run) and discussed on Hacker News, where users noted its potential for easier embedding. Mermaid is widely used for diagramming in documentation and note-taking apps, but its official library typically requires a browser environment for layout, complicating server-side or embedded rendering. Pele's approach could simplify embedding Mermaid diagrams in static sites, markdown editors, and other non-browser contexts, benefiting developers and tools like Obsidian. Pele is a lightweight library that themes SVG output with CSS variables, allowing easy customization. The source code is available on GitHub under the obsidianmd organization, confirming its open-source nature.

hackernews · dchest · Oct 17, 15:55 · [Discussion](https://news.ycombinator.com/item?id=50132193)

**Background**: Mermaid is a popular open-source diagramming and charting tool that lets users create diagrams from text using a markdown-like syntax. Traditionally, rendering Mermaid diagrams requires a browser environment (often headless) to compute the layout and produce SVG, which can be cumbersome for server-side or embedded use. Themeable SVG refers to SVG graphics that can be styled dynamically, for example with CSS variables, to match different visual themes.

<details><summary>References</summary>
<ul>
<li><a href="https://mermaid.js.org/">Mermaid | Diagramming and charting tool</a></li>
<li><a href="https://pele.run/">Pele · Mermaid diagrams as themeable SVG</a></li>
<li><a href="https://en.wikipedia.org/wiki/Headless_browser">Headless browser - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with Mermaid's layout quality for complex diagrams, seeing Pele's styling improvements as secondary. Others emphasized the importance of open-source visibility, suggesting projects display GitHub links prominently, and noted that 'pele' means 'mouse' in Latvian.

**Tags**: `#mermaid`, `#svg`, `#diagramming`, `#open-source`, `#obsidian`

---

<a id="item-9"></a>
## [Estonia's i-voting source code now public on GitHub](https://github.com/valimised/ivxv) ⭐️ 7.0/10

The source code for Estonia's Internet voting system (i-voting) has been made publicly available on GitHub under the valimised/ivxv repository, as highlighted in a Hacker News discussion. This release marks a significant transparency milestone for a national e-voting platform that has been used in legally binding elections since 2005, allowing security researchers and the public to scrutinize the system's implementation and potentially increasing trust in online voting. The IVXV system has been used in Estonian municipal elections since 2017, but individual verifiability remains a challenge; research has shown that a compromised voter device can defeat the individual verifiability mechanism by exploiting the revoting option.

hackernews · theanonymousone · Oct 17, 03:18 · [Discussion](https://news.ycombinator.com/item?id=50127586)

**Background**: Estonia was the first country to hold legally binding general elections over the Internet, in 2005, and has used i-voting extensively since 2007. The IVXV system is the current version of its i-voting software. End-to-end verifiable voting systems aim to provide strong integrity and tamper resistance, but achieving individual verifiability—allowing voters to confirm their vote was recorded correctly—is particularly difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electronic_voting_in_Estonia">Electronic voting in Estonia - Wikipedia</a></li>
<li><a href="https://eprint.iacr.org/2021/1098">Individual Verifiability and Revoting in the Estonian ... - IACR</a></li>
<li><a href="https://en.wikipedia.org/wiki/End-to-end_auditable_voting">End-to-end auditable voting - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters debated the security and trust implications: some argued that software alone cannot secure elections and that post-election verification via statistical sampling is needed, while others noted that Estonia's system is widely accepted and has been open source for years. A local Estonian expressed concern about the system's reliance on trust in the government, and another pointed to existing verifiable systems like ElectionGuard used in US elections.

**Tags**: `#e-voting`, `#security`, `#open-source`, `#elections`, `#verifiability`

---

<a id="item-10"></a>
## [Open-source ESP32 emulator runs firmware in the browser](https://github.com/mikroverk/esp32sim) ⭐️ 7.0/10

A developer has released esp32sim, an open-source ESP32 emulator that executes firmware entirely in the browser, as demonstrated by a demo where no physical ESP32 is involved. The project aims to make ESP32 software easier to experiment with, test, and simulate without needing connected hardware. This tool could significantly lower the barrier for embedded development by enabling rapid prototyping and CI/CD testing without physical boards, potentially accelerating IoT project workflows. It also adds to the growing trend of running complex emulation in the browser via WebAssembly. The emulator is built with WebAssembly and currently supports at least the ESP32-S3 board, as indicated by the project's documentation. The author is actively seeking feedback from embedded developers on what features would be needed for real-world development, testing, and CI use.

hackernews · joakimeriksson · Oct 17, 13:51 · [Discussion](https://news.ycombinator.com/item?id=50131189)

**Background**: The ESP32 is a popular family of low-cost, low-power microcontrollers with integrated Wi-Fi and Bluetooth, widely used in IoT devices. Emulators like this allow developers to run and debug firmware on a computer instead of flashing it to physical hardware, which is especially useful for testing and continuous integration. WebAssembly enables near-native performance for such emulators inside a web browser.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32 - Wikipedia</a></li>
<li><a href="https://www.espressif.com/en/products/socs/esp32">ESP32 Wi-Fi & Bluetooth SoC | Espressif Systems</a></li>

</ul>
</details>

**Discussion**: Commenters found the project impressive, with one sharing a similar drone simulator that runs actual ESP32 flight controller code as WebAssembly. Others noted potential uses in CI/CD testing and asked how it differs from Wokwi, while one criticized the README's dense AI-generated formatting.

**Tags**: `#ESP32`, `#emulator`, `#embedded-systems`, `#WebAssembly`, `#open-source`

---

<a id="item-11"></a>
## [Hobbyist runs 48-layer MoE model across five consumer devices at 37-39 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1x8ley0/2_gaming_pcs_an_m4_pro_macbook_over_ethernet_2/) ⭐️ 7.0/10

A hobbyist (u/StayLameBro) demonstrated running Qwen 3.8 Flash Next, a 48-layer mixture-of-experts model with 512 experts per layer, across two gaming PCs, an M4 Pro MacBook, and two iPhone 17 Pro Maxes connected via Ethernet and USB-C. The setup achieved 37-39 tokens/s decode at 60k context, with a second layout reaching 164k context at 31-33 tok/s. This experiment shows that heterogeneous consumer devices can be chained to run models far larger than any single machine's memory, pushing the boundaries of local LLM inference. It offers a practical blueprint for hobbyists and could inspire more accessible distributed inference tools. The model is split by layers: PC1 (RTX 2060 Super) handles layers 0-9 plus the output layer and draft head, the MacBook handles layers 10-29, the iPhones handle expert computation for layers 10-18, and PC2 (RX 9060 XT) handles layers 30-47. Pipelined speculation with a multi-token-prediction draft head yields about 2.2 tokens per step, and all weights reside in VRAM/RAM with no disk streaming.

reddit · r/LocalLLaMA · /u/StayLameBro · Oct 17, 21:13

**Background**: Mixture-of-experts (MoE) models activate only a subset of experts per token, reducing compute but requiring large memory to store all experts. Multi-token prediction (MTP) draft heads let a model guess several future tokens, which are then verified in a single pass, speeding up generation. Distributed inference frameworks like distributed-llama and Exo aim to pool consumer hardware over Ethernet to run large models collaboratively.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://github.com/b4rtaz/distributed-llama">GitHub - b4rtaz/distributed-llama: Distributed LLM inference ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#distributed-inference`, `#mixture-of-experts`, `#consumer-hardware`, `#model-sharding`

---

<a id="item-12"></a>
## [Developer runs 35B Fish Audio Drama 3 TTS on 16GB AMD Radeon via MoE offloading](https://www.reddit.com/r/LocalLLaMA/comments/1x8kces/fish_audio_drama_3_says_it_needs_a_48_gb_nvidia/) ⭐️ 7.0/10

A developer built 'Red Curtain', a tool that runs Fish Audio Drama 3—a 35B-parameter mixture-of-experts text-to-speech model—on a 16GB AMD RX 9070 GPU by caching FP8 experts in system RAM and only loading active experts onto the GPU. The tool achieves slower-than-realtime speech generation (e.g., 3.3 seconds of speech in 13 seconds) while using about 11–12 GB of VRAM and 35 GB of RAM. This demonstrates that large MoE models can run on consumer AMD hardware with far less VRAM than officially required, potentially broadening access to advanced TTS for users without high-end NVIDIA GPUs. It also highlights the growing role of MoE offloading techniques and AMD's ROCm ecosystem in local AI deployment. The model has 35B total parameters but only about 3B active per token, and the FP8 experts (~32 GB) are kept in system RAM while the rest runs in BF16 on the GPU. Known issues include occasional silence after the first line (a model-level quirk also noted in the vLLM recipe), and the tool has only been tested on the RX 9070 (gfx1201); weights must be downloaded separately from Hugging Face.

reddit · r/LocalLLaMA · /u/fechyyy · Oct 17, 20:27

**Background**: Mixture-of-Experts (MoE) models activate only a subset of their parameters for each token, which reduces compute but still requires all parameters to be stored in memory. Offloading techniques keep inactive experts in slower system RAM and load only the needed ones onto the GPU, enabling large models to run on GPUs with limited VRAM. FP8 is an 8-bit floating-point format that reduces memory usage compared to BF16 while maintaining reasonable accuracy. AMD's ROCm is an open-source software stack for GPU computing, serving as the counterpart to NVIDIA's CUDA.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2401.14361v2">MoE -Infinity: Offloading -Efficient MoE Model Serving</a></li>
<li><a href="https://www.spheron.network/blog/fp8-quantization-inference-performance-hardware-explained/">What is FP8 Quantization? AI Inference Performance, Accuracy ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AMD_ROCm">AMD ROCm</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#AMD-ROCm`, `#MoE-offloading`, `#TTS`, `#consumer-hardware`

---

<a id="item-13"></a>
## [Abliterated DeepSeek V4.1 Flash 1017 released with GGUF quants](https://www.reddit.com/r/LocalLLaMA/comments/1x8ke24/deepseek_v41_flash_1017_gguf_abliterated/) ⭐️ 7.0/10

A community member released an abliterated version of DeepSeek V4.1 Flash 1017 along with GGUF quantizations for both the base and abliterated models, using a rank-2 subspace removal technique that reduced refusals from 97/100 to 4/100 in chat mode and from 98/100 to 9/100 in think mode. This provides the local LLM community with an early, technically refined abliterated derivative of a newly released model, showing that multi-direction refusal removal can substantially cut refusals while preserving model quality, which matters for users running uncensored models locally. The author measured separate refusal directions for chat and think modes and removed the rank-2 subspace they span rather than a single direction, optimizing for model integrity over eliminating every refusal; GGUF quants are available (no imatrix yet, WIP) and a LoRA is provided for GGUF users to avoid redownloading weights.

reddit · r/LocalLLaMA · /u/mrfakename0 · Oct 17, 20:29

**Background**: Abliteration is a technique that removes a model's refusal behavior by projecting out specific activation directions from its weights, typically identified from harmful-prompt data. GGUF is a quantization file format used by llama.cpp for running LLMs locally with reduced memory. DeepSeek V4.1 Flash 1017 is a recently released model, and this post is a community-made derivative rather than an official release.

<details><summary>References</summary>
<ul>
<li><a href="https://vynaris.com/blog/what-is-abliteration-llm-refusal-removal">What Is Abliteration? LLM Refusal Removal Explained</a></li>
<li><a href="https://mbrenndoerfer.com/writing/gguf-format-quantized-llm-storage-inference">GGUF : Storage and Inference for Quantized LLMs - Interactive</a></li>
<li><a href="https://abliteration.org/wiki/academic-research/">Academic papers on abliteration and refusal removal ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#abliteration`, `#gguf`, `#deepseek`, `#model-quantization`

---

<a id="item-14"></a>
## [NVIDIA Releases Dory1.0-4B: A Looped Latent-Recurrent LLM with 256K Context](https://www.reddit.com/r/LocalLLaMA/comments/1x8bg1u/nvidianvidianemotronlabsdory104bbf16_hugging_face/) ⭐️ 7.0/10

NVIDIA has released NVIDIA-Nemotron-Labs-Dory1.0-4B-BF16, a 4-billion-parameter language model that uses a looped (latent-recurrent) normalized-GPT architecture with interleaved sliding-window and full-attention layers, supporting up to 256K tokens of context. The model is available on Hugging Face under the OpenMDW License Agreement version 1.1, permitting both commercial and non-commercial use. This is a notable release for the local LLM community because it demonstrates a recurrent-depth scaling approach in a small, openly licensed model, potentially offering strong reasoning per parameter. If the architecture proves effective, it could influence future efficient model designs and make long-context reasoning more accessible on consumer hardware. The model repeatedly applies a shared block of layers to spend more compute per token, and it interleaves sliding-window attention with full-attention layers to handle long contexts efficiently. It is released in BF16 precision, supports English only, and is positioned for general-purpose reasoning on a small footprint.

reddit · r/LocalLLaMA · /u/silenceimpaired · Oct 17, 14:20

**Background**: Looped language models reuse the same transformer blocks across multiple iterations, effectively increasing depth without adding parameters, which can improve reasoning at a lower memory cost. Sliding-window attention restricts each token to attend only to a local window of previous tokens, reducing computation for long sequences, while full-attention layers preserve global information. The OpenMDW license is a permissive license designed specifically for machine-learning models and their artifacts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/looped-language-models">Looped Language Models : Iterative Transformer Refinement</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/visual-attention-variants">A Visual Guide to Attention Variants in Modern LLMs</a></li>
<li><a href="https://openmdw.ai/license/1-1/">OpenMDW-1.1 | OpenMDW</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#NVIDIA`, `#recurrent-architecture`, `#local-llm`, `#model-release`

---

<a id="item-15"></a>
## [ds4 adds DeepSeek V4.1 Flash 1017 support via PR #1225](https://www.reddit.com/r/LocalLLaMA/comments/1x8koix/deepseek_v41_flash_1017_support_for_ds4_pr_1225/) ⭐️ 7.0/10

PR #1225 adds compatibility for the DeepSeek-v4.1-Flash-1017 checkpoint to the ds4 (dwarfstar) local inference project, including new engrams and an updated vision tower. The change verifies that vision and language model files match and raises an error on mixed pairings, while files quantized with the ds4 suite load without modification. This lets local-inference users run the newest DeepSeek Flash checkpoint on ds4 without waiting for core kernel changes, since the architecture is unchanged. It matters for the LocalLLaMA community because it keeps a fast-moving proprietary checkpoint usable on consumer hardware shortly after release. Roughly 40% of routed expert tensors changed, about 30% in the engrams, and around 50% of the vision tower's expert tensors changed, though the architecture remains the same and slots into existing kernels. The author plans a Q2–Q8 mixed quant for 128GB machines with minor SSD offloading (152GB wired, 366GB total with engrams), expecting about 20 tokens per second decode on an M5 Max.

reddit · r/LocalLLaMA · /u/returnity · Oct 17, 20:42

**Background**: ds4 (also called DwarfStar 4) is a native inference engine by antirez for running DeepSeek V4 Flash and PRO models locally, built on ideas from llama.cpp and GGML but not linking against them. DeepSeek's Engram module adds conditional n-gram memory to the model backbone, and the term 'engrams' here refers to those memory tensors. Quantization compresses model weights (e.g., Q2–Q8 formats) so large models fit in limited RAM, and mixed quantization assigns different precisions to different tensors.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash and PRO local ...</a></li>
<li><a href="https://github.com/deepseek-ai/Engram">GitHub - deepseek -ai/ Engram : Conditional Memory via Scalable...</a></li>
<li><a href="https://deepseek.ai/blog/deepseek-engram-v4-architecture">DeepSeek Engram — V4 Memory Architecture Explained</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#deepseek`, `#quantization`, `#inference`, `#llama-cpp`

---