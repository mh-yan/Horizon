---
layout: default
title: "Horizon Summary: 2026-10-24 (EN)"
date: 2026-10-24
lang: en
---

> From 40 items, 18 important content pieces were selected

---

1. [Brotli flaw CVE-2026-111497, now HTTP2Shell, enables RCE in many HTTP libraries](#item-1) ⭐️ 8.0/10
2. [gpu-unlock exploits Nvidia firmware to double FP/BF16 issue rates on RTX 3000](#item-2) ⭐️ 8.0/10
3. [How close can pure functional programming get to C?](#item-3) ⭐️ 8.0/10
4. [OpenAI to stop training frontier models on live internet](#item-4) ⭐️ 8.0/10
5. [Ollama v0.40.11 adds macOS speech generation and d3 decision models](#item-5) ⭐️ 7.0/10
6. [Developer hides Bitcoin behind PHP RCE in public challenge](#item-6) ⭐️ 7.0/10
7. [Goose: A New Language with Multiple Data Stacks and Resizable Fields](#item-7) ⭐️ 7.0/10
8. [Apollo Analysis: AI Productivity Gains Confined to Tech Sector](#item-8) ⭐️ 7.0/10
9. [Twelve Years of Distributed SQLite: A Retrospective](#item-9) ⭐️ 7.0/10
10. [arXiv paper explains why AI-generated text is hard to understand](#item-10) ⭐️ 7.0/10
11. [Grok and GPT recommend opposing candidates in over 90% of races](#item-11) ⭐️ 7.0/10
12. [Kimi K3.1 open-weight release strips cyberattack training data](#item-12) ⭐️ 7.0/10
13. [KLD is misunderstood as a quantization quality metric](#item-13) ⭐️ 7.0/10
14. [Meta trains small byte-level models that scale better than token models](#item-14) ⭐️ 7.0/10
15. [Run Qwen-Flash-Next Coder with 262K context on an 8GB GPU via llama.cpp](#item-15) ⭐️ 7.0/10
16. [Open-source browser rhythm game runs four neural nets locally to build levels from your songs](#item-16) ⭐️ 7.0/10
17. [ANEMLL Forge 0.2.1 runs Qwen3.8-27B on M6 Neural Engine with 192K context](#item-17) ⭐️ 7.0/10
18. [ISTA Releases GSQ-RCO Quantized GGUFs for DeepSeek-V4.1-Flash-1017](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Brotli flaw CVE-2026-111497, now HTTP2Shell, enables RCE in many HTTP libraries](https://www.aikido.dev/blog/python-packages-vulnerable-node2shell-brotli-cve-2026-111497) ⭐️ 8.0/10

A critical buffer overflow in the Brotli decompression library (CVE-2026-111497), initially dubbed Node2Shell and now renamed HTTP2Shell, allows unauthenticated remote code execution via crafted Brotli-compressed streams. The vulnerability affects Brotli versions 1.0.3 through 1.2.0 and has a wide blast radius across HTTP libraries and applications, with fixes available in Brotli 1.0.10, 1.1.1, and 1.2.1. This vulnerability is significant because Brotli is widely used for HTTP compression, so many web servers, proxies, and applications that decode Brotli data are exposed to remote code execution without authentication. The broad blast radius means organizations need to urgently identify and patch affected components across their stack. The flaw is an out-of-bounds write (CWE-787) in the Brotli decoder (c/dec/decode.c) that can corrupt adjacent memory, disclose sensitive information, cause denial of service, or execute arbitrary code. Patches are available in Brotli 1.0.10, 1.1.1, and 1.2.1, and downstream projects like Node.js, Bun, Python, Ruby, and Envoy have released fixed versions.

hackernews · theanonymousone · Oct 24, 08:06 · [Discussion](https://news.ycombinator.com/item?id=50219177)

**Background**: Brotli is a compression algorithm developed by Google, commonly used to compress HTTP responses and sometimes requests to reduce bandwidth. The vulnerability arises because the decoder mishandles certain compressed inputs, leading to memory corruption. Many programming languages and frameworks bundle Brotli for HTTP support, so a flaw in the library propagates to all of them.

<details><summary>References</summary>
<ul>
<li><a href="https://app.opencve.io/cve/CVE-2026-111497">CVE-2026-111497 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://www.tenable.com/cve/CVE-2026-111497">CVE-2026-111497 | Tenable®</a></li>
<li><a href="https://brandefense.io/blog/http2shell-brotli-cve-2026-111497/">HTTP2Shell Fixed Versions by Stack - Brandefense</a></li>

</ul>
</details>

**Discussion**: Commenters criticized the name HTTP2Shell as overly broad and misleading, preferring Brotli2Shell or Broccoli2Shell since the issue affects any Brotli decoding, not just HTTP. Some questioned why the RCE wasn't recognized as a security issue when reported earlier, and others noted the sensationalism while emphasizing the need to patch.

**Tags**: `#security`, `#vulnerability`, `#brotli`, `#http`, `#rce`

---

<a id="item-2"></a>
## [gpu-unlock exploits Nvidia firmware to double FP/BF16 issue rates on RTX 3000](https://github.com/Zagitta/gpu-unlock) ⭐️ 8.0/10

A GitHub project called gpu-unlock, developed by Zagitta, has released a Linux kernel module that exploits a buffer overflow in Nvidia's boot firmware to remove the firmware cap on FP16 and BF16 instruction issue rates for GeForce RTX 3000-series GPUs. The unlock effectively doubles the instruction issuing speed of FP16/BF16 FMA into FP32 operations on GA102, GA104, and GA106 chips, with community reports of up to 80% performance gains in certain compute benchmarks. This unlock allows consumer RTX 3000 cards to achieve performance closer to their professional counterparts on matrix workloads, which is particularly valuable for neural network research and LLM training on consumer hardware. It highlights how manufacturers artificially limit consumer hardware via firmware, and the community's ability to bypass such restrictions. The exploit relies on a classic buffer overflow in the booter that allows code execution via Return Oriented Programming (ROP), and the module works on GA102, GA103, GA104, and GA106 chips covering cards like the RTX 3090 Ti, 3090, 3080 Ti, 3080, 3070, and 3060 12GB. Users report that achieving the full performance gain may require increasing the power limit to 450W and improving cooling, as the stock cooler is not designed for such power levels.

hackernews · fragebogen · Oct 24, 09:58 · [Discussion](https://news.ycombinator.com/item?id=50219700)

**Background**: Nvidia's consumer GPUs typically have firmware-level restrictions that limit the issue rate of FP16 and BF16 instructions, which are crucial for AI and scientific computing workloads. These restrictions differentiate consumer cards from professional models, but hackers have long sought ways to bypass them. The gpu-unlock project builds on previous efforts like CMP90/50 Windows unlocks and vGPU unlock tools, using firmware exploitation to remove these artificial limits.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Zagitta/gpu-unlock">GitHub - Zagitta/ gpu -unlock · GitHub</a></li>
<li><a href="https://aiweekly.co/alerts/zagitta-releases-gpu-unlock-lifts-fp16bf16-caps-on-rtx-3000s">Zagitta Releases gpu-unlock, Lifts FP16/BF16 Caps on RTX ...</a></li>
<li><a href="https://github.com/DualCoder/vgpu_unlock">GitHub - DualCoder/vgpu_unlock: Unlock vGPU functionality for ... VGPU Unlock - Open-IOV RTX 5090 Predecessor Unlock: BF16 Hits 129.6 TFLOPS [2026] GPU-unlock: FP/BF16 instruction issue rate on Nvidia... GPU Unlock — supported NVIDIA cards, measured speedups ... (omg)vflash | Fully Patched nvflash from X to Ada Lovelace ...</a></li>

</ul>
</details>

**Discussion**: The community response is largely positive, with users like Tiberium confirming legitimate performance gains and RandyOrion calling the unlock 'invaluable' for neural network research. However, jacquesm cautions that the mod requires running the card hotter and increasing power to 450W, necessitating better cooling, and notes it can be stacked with the existing p2p mod. The author Zagitta acknowledges the exploits aren't his original ideas but aims to provide a less annoying package than patching the Nvidia driver.

**Tags**: `#GPU`, `#Nvidia`, `#firmware`, `#performance`, `#hardware`

---

<a id="item-3"></a>
## [How close can pure functional programming get to C?](https://rtfeldman.com/fp-vs-c) ⭐️ 8.0/10

A blog post by Richard Feldman analyzes how close pure functional programming can get to C-level performance, using benchmarks like lean-zip versus miniz_oxide and discussing compiler optimizations such as copy elision. This analysis challenges the assumption that pure functional languages are inherently slower, showing that with modern compiler techniques they can approach C performance, which could influence language design and adoption in performance-sensitive domains. The discussion highlights that copy elision and memory bandwidth are core bottlenecks, and that comparing against miniz_oxide may be unfair since it is intentionally simple; zlib-rs is suggested as a more competitive baseline.

hackernews · stmonty · Oct 24, 03:43 · [Discussion](https://news.ycombinator.com/item?id=50218195)

**Background**: Pure functional programming avoids side effects and mutable state, which traditionally introduces overhead from copying and allocation. C and C++ allow aggressive optimizations like copy elision, where the compiler eliminates unnecessary object copies, often leading to better performance. Recent advances in compiler optimization and language design are narrowing the performance gap between functional languages and C.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Copy_elision">Copy elision - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters added valuable insights: jandrewrogers noted that C/C++ allows extreme copy elision which is crucial for memory bandwidth; VorpalWay pointed out that miniz_oxide is intentionally simple and zlib-rs would be a fairer comparison; WalterBright mentioned D's `pure` annotation as a compiler-checked alternative; andai questioned the use of immature technology in production.

**Tags**: `#functional-programming`, `#performance`, `#compilers`, `#optimization`, `#benchmarking`

---

<a id="item-4"></a>
## [OpenAI to stop training frontier models on live internet](https://techcrunch.com/2026/10/23/openai-says-it-will-no-longer-train-its-ai-models-on-the-live-internet-citing-significant-risks/) ⭐️ 8.0/10

OpenAI announced it will no longer train its frontier AI models on the live internet, citing "significant risks." The policy shift comes just weeks after one of its engineers said that cutting models off from the internet wouldn't work. As a leading AI lab, OpenAI's decision could set a precedent for how other companies train frontier models, potentially reshaping industry norms around data sourcing and AI safety. It may also affect model capabilities, data licensing practices, and regulatory expectations across the AI ecosystem. The announcement lacks technical specifics, such as what alternative data sources OpenAI will use or how it will keep models current without live web access. The timing is notable given the internal disagreement, suggesting the decision may be controversial even within OpenAI.

rss · TechCrunch · Oct 23, 23:05

**Background**: Frontier models are the most advanced AI systems available at a given time, trained on massive datasets to achieve state-of-the-art performance. Training on the live internet has been common because it provides fresh, diverse data, but it also exposes models to harmful content, misinformation, and security risks. OpenAI's move reflects growing concern about these risks and may signal a broader shift toward more controlled training data pipelines.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>
<li><a href="https://openai.com/">OpenAI | Research & Deployment</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI training`, `#AI safety`, `#policy`, `#frontier models`

---

<a id="item-5"></a>
## [Ollama v0.40.11 adds macOS speech generation and d3 decision models](https://github.com/ollama/ollama/releases/tag/v0.40.11) ⭐️ 7.0/10

Ollama v0.40.11 introduces native speech generation on macOS, allowing `ollama run` to play text or chat replies aloud and exposing an OpenAI-compatible `/v1/audio/speech` endpoint for streaming audio. It also adds the d3 family of decision models (2B, 4B, 9B, and 27B) for classification, yes/no answers, and probability scoring. This release expands Ollama beyond text generation into audio output and specialized decision-making, making the local LLM tool more versatile for developers building voice-enabled apps or routing/classification pipelines. The OpenAI-compatible endpoint lowers integration friction for existing tools. Speech models only generate speech; chat, completion, and embedding requests to them return a 400 error. The d3 models are derived from vLLM Semantic Router's decision models and accept text, structured state, or images as input.

github · github-actions[bot] · Oct 24, 00:30

**Background**: Ollama is a popular tool for running large language models locally. The OpenAI-compatible `/v1/audio/speech` endpoint follows the same API pattern as OpenAI's text-to-speech service, allowing apps to switch between providers easily. vLLM Semantic Router is an open-source project that routes requests to different models based on policy; its decision models are specialized for classification and scoring tasks rather than general chat.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.ollama.com/capabilities/speech">Turn text into spoken audio with text-to- speech models. - Ollama</a></li>
<li><a href="https://github.com/vllm-project/semantic-router">GitHub - vllm-project/semantic-router: An open, programmable ...</a></li>
<li><a href="https://vllm-sr.ai/blog/decision-models/">Introducing Decision 1.0: Open Decision Foundation Models</a></li>

</ul>
</details>

**Tags**: `#ollama`, `#llm`, `#speech-synthesis`, `#local-ai`, `#release`

---

<a id="item-6"></a>
## [Developer hides Bitcoin behind PHP RCE in public challenge](https://stealmybitcoin.com/) ⭐️ 7.0/10

A developer launched stealmybitcoin.com, a public challenge that hides a Bitcoin wallet worth about $502 on a server running a PHP version vulnerable to the recently disclosed PHP2SHELL remote code execution (RCE) flaws, with the key accessible to the PHP user account via a print-flag binary. The first person to exploit the RCE and retrieve the wallet wins the prize. The challenge serves as a real-world test of whether the PHP2SHELL vulnerabilities are actually being exploited in the wild, and it has become a focal point for debating claims that autonomous AI hacking agents can trivially compromise vulnerable servers. Its outcome could shape how defenders and the security community assess the practical risk of these critical PHP flaws. The server deliberately runs a PHP version predating the PHP2SHELL CVE disclosures, and the prize is only about $502, which critics argue is far too low to justify burning a working exploit or risking a honeypot. The challenge remained unclaimed for at least the first hour, and commenters noted the server was overloaded by traffic.

hackernews · cloudlandsdev · Oct 24, 20:30 · [Discussion](https://news.ycombinator.com/item?id=50224916)

**Background**: PHP2SHELL refers to two critical remote code execution vulnerabilities in core PHP, tracked as CVE-2026-109618 and CVE-2026-109619, publicly disclosed in October 2026; one involves out-of-memory handling that can interrupt PHP while internal request data is only partially initialized. Because PHP powers a huge share of the web, these flaws affect millions of independently managed servers. A honeypot is a decoy system designed to look like a legitimate target so defenders can observe attackers' methods, which is why some commenters suspect this challenge may be one.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vulncheck.com/blog/php2shell-vulnerabilities">PHP 2Shell Vulnerabilities : CVE-2026-109618 and... | VulnCheck</a></li>
<li><a href="https://www.wiz.io/blog/php2shell-php-rce">PHP 2Shell: AI uncovers critical RCE vulnerabilities ... | Wiz Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Honeypot_(computing)">Honeypot (computing) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly skeptical: some suspected the site is a honeypot and argued the low prize value makes it irrational for skilled attackers to reveal a working exploit, while others said the fact it stayed unclaimed undermines hype about autonomous AI agents compromising sites at scale. Several mocked people who had claimed the PHP exploits were trivial to use but declined to demonstrate it.

**Tags**: `#security`, `#PHP`, `#RCE`, `#honeypot`, `#AI-hype`

---

<a id="item-7"></a>
## [Goose: A New Language with Multiple Data Stacks and Resizable Fields](https://aardappel.github.io/goose/) ⭐️ 7.0/10

Goose is a new programming language created by Aardappel (Wouter van Oortmerssen) that eliminates the heap by using multiple data stacks and resizable fields, enabling automatic memory analysis. The language has sparked a technical discussion on Hacker News, including an AMA with the creator and praise from John Carmack. Goose challenges conventional memory management by showing that a restricted-purpose language without a heap can still handle many programs safely and efficiently. Its design could influence how languages approach memory safety and performance, particularly for parsing and network data processing. In Goose, every dynamic value lives inline on a data stack managed by the compiler; growth advances a pointer and memory is freed when its scope ends, with at most one resizable value live per stack. There is no garbage collection, so programmers must be careful about memory growth, and the language is intended for programs where the number of growable memory regions can be statically specified.

hackernews · bobbydigitales · Oct 24, 19:06 · [Discussion](https://news.ycombinator.com/item?id=50224100)

**Background**: Traditional languages use a heap for dynamic memory allocation, which requires manual management (as in C) or garbage collection (as in Java). Stack-based allocation is faster and automatically reclaimed but limited to last-in-first-out lifetimes. Goose extends this by allowing multiple stacks and resizable fields, enabling dynamic data without a heap.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/aardappel/goose/tree/master/">GitHub - aardappel/goose: The Goose Programming Language</a></li>
<li><a href="https://news.ycombinator.com/item?id=50224100">John Carmack on the Goose Language: multiple data stacks and ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stack-based_memory_allocation">Stack-based memory allocation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters discussed the limitations of fixed stacks for dynamically sized data, with some noting that Goose is suitable for restricted purposes and requires careful memory management due to lack of garbage collection. Others compared it to ML-style regions and highlighted John Carmack's praise for its potential in fast parsing.

**Tags**: `#programming languages`, `#memory management`, `#language design`, `#stack-based`, `#Hacker News`

---

<a id="item-8"></a>
## [Apollo Analysis: AI Productivity Gains Confined to Tech Sector](https://www.apollo.com/wealth/insights-news/insights/daily-spark/no-signs-of-ai-payoff-outside-the-tech-sector) ⭐️ 7.0/10

Apollo Wealth published an analysis arguing that there are no signs of AI-driven productivity payoffs outside the tech sector, sparking a Hacker News discussion with 391 points and 361 comments. This matters because trillions of dollars are being invested in AI on the assumption of broad economic gains, and if benefits remain confined to tech, it could reshape investment strategies and policy expectations across industries. The analysis notes that while some software companies have increased output without hiring, broader productivity gains have yet to materialize, and historical analogies to electrification suggest a decade-long lag between adoption and measurable impact.

hackernews · the-mitr · Oct 24, 19:47 · [Discussion](https://news.ycombinator.com/item?id=50224463)

**Background**: AI productivity refers to the expected increase in economic output per worker due to AI adoption. The debate echoes Robert Solow's 1987 paradox: 'You can see the computer age everywhere but in the productivity statistics.' Apollo Wealth is the wealth management arm of Apollo Global Management, providing investment insights.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bennettschool.cam.ac.uk/blog/ai-productivity-gains/">Where are the AI productivity gains? - Bennett School of ...</a></li>
<li><a href="https://www.pwc.com/gx/en/news-room/press-releases/2026/pwc-2026-ai-performance-study.html">Three-quarters of AI’s economic gains are being captured by ...</a></li>

</ul>
</details>

**Discussion**: Commenters offered diverse views: some argued the tech sector is naturally first due to being software-defined, others contended that AI vendors capture most of the gains as revenue, and some noted it's simply too early, citing the slow diffusion of past general-purpose technologies like electrification.

**Tags**: `#AI economics`, `#productivity`, `#industry analysis`, `#tech sector`, `#HN discussion`

---

<a id="item-9"></a>
## [Twelve Years of Distributed SQLite: A Retrospective](https://philipotoole.com/twelve-years-of-distributed-sqlite/) ⭐️ 7.0/10

Philip O'Toole, creator of rqlite, published a retrospective on twelve years of building distributed SQLite systems, which sparked a Hacker News discussion with 352 points and 60 comments comparing engines like rqlite, Cloudflare D1, and Paxos-based alternatives. This retrospective highlights the growing ecosystem of distributed SQLite solutions and the architectural trade-offs between them, which is valuable for developers choosing a database for edge, embedded, or cloud applications. The discussion revealed that rqlite does not officially support BEGIN/COMMIT multi-statement transactions, while other engines like D1 have reliability concerns, and alternatives such as zaxonlite use WAL replication with Paxos.

hackernews · otoolep · Oct 24, 01:16 · [Discussion](https://news.ycombinator.com/item?id=50217500)

**Background**: SQLite is a widely used embedded relational database, but it lacks built-in distribution. Projects like rqlite and Cloudflare D1 add replication and fault tolerance by layering consensus algorithms (e.g., Raft, Paxos) or durable objects on top of SQLite. Paxos is a family of protocols for achieving consensus in distributed systems, ensuring that a cluster agrees on a single value despite failures.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rqlite/rqlite">GitHub - rqlite/rqlite: The lightweight, fault-tolerant ...</a></li>
<li><a href="https://developers.cloudflare.com/d1/">Overview · Cloudflare D1 docs</a></li>
<li><a href="https://www.scylladb.com/glossary/paxos-consensus-algorithm/">What is Paxos Consensus Algorithm ? Definition & FAQs | ScyllaDB</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed experiences: one reported D1 as unreliable in production, another noted rqlite's lack of full transaction support as a key differentiator, and a third described building a Paxos-based multi-master SQLite using WAL replication. Some argued that with modern tooling, using PostgreSQL directly may be simpler than distributed SQLite for many use cases.

**Tags**: `#distributed-systems`, `#sqlite`, `#databases`, `#consensus`, `#replication`

---

<a id="item-10"></a>
## [arXiv paper explains why AI-generated text is hard to understand](https://arxiv.org/abs/2610.29162) ⭐️ 7.0/10

A new arXiv paper by Thomas Hikaru Clark, Matias B. Martin, and Kyle Mahowald (arXiv:2610.29162, submitted October 21, 2026) investigates why AI-generated text has become harder to understand, finding that models use psycholinguistic features linked to human processing difficulty and proposing that AI text is optimized for information density rather than successful communication. This research matters because LLM-generated text is increasingly used in education, customer service, and content creation, so understanding why it is hard to read can inform better model training and prompting; it also connects to broader debates about RLHF and alignment. The study uses a novel corpus of AI-generated text across diverse domains and measures features such as object relative clauses, long syntactic dependencies, and low-frequency n-grams; it hypothesizes that optimization for math, code, and reasoning creates pressure for information density over communicative clarity.

hackernews · canjobear · Oct 24, 18:04 · [Discussion](https://news.ycombinator.com/item?id=50223647)

**Background**: RLHF (Reinforcement Learning from Human Feedback) is a technique that trains a reward model from human preferences and then uses reinforcement learning to align LLM outputs with those preferences. Psycholinguistic features like object relative clauses and long dependencies are known to increase human reading difficulty. The paper argues that while human language is optimized for communication, AI text is optimized for other goals like reasoning and code.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.29162">Why is AI-generated language so hard to understand?</a></li>
<li><a href="https://arxiv.org/html/2610.29162v1">Why is AI-generated language so hard to understand? - arXiv.org</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning_from_human_feedback">Reinforcement learning from human feedback - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters offered distinct hypotheses: one technical writer argued RLHF optimizes for surface features that raters perceive as good writing (lists, headings, catchy phrases); another noted LLMs often use transitive verbs intransitively, causing ambiguity; a third suggested AI text lacks an underlying human intent or mental model, and others pointed to training data containing persuasive commercial and opinion writing.

**Tags**: `#LLM`, `#AI-generated text`, `#linguistics`, `#RLHF`, `#natural language processing`

---

<a id="item-11"></a>
## [Grok and GPT recommend opposing candidates in over 90% of races](https://techcrunch.com/2026/10/24/forced-to-pick-groks-ai-model-chooses-republicans-openais-picks-democrats/) ⭐️ 7.0/10

A new study found that Grok's AI model overwhelmingly recommends Republican candidates while OpenAI's GPT favors Democrats, with the two models disagreeing in more than 90% of nearly 500 election races. This finding highlights significant political bias in two major AI models, raising concerns about AI ethics, model alignment, and election integrity as more people turn to chatbots for political information. The study examined nearly 500 races and found that the models disagreed in over 90% of them, with Grok leaning Republican and GPT leaning Democratic; however, the article provides limited methodological details and no community discussion.

rss · TechCrunch · Oct 24, 15:00

**Background**: Large language models like Grok and GPT are trained on vast amounts of text data and fine-tuned with human feedback, which can inadvertently embed political biases. Previous research, such as studies from Brookings and UK think tanks, has documented a tendency for LLMs to lean left on political questions, but this study shows a stark divergence between two leading models. Grok is developed by xAI, while GPT is developed by OpenAI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.brookings.edu/articles/the-politics-of-ai-chatgpt-and-political-bias/">The politics of AI: ChatGPT and political bias | Brookings</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI bias`, `#political bias`, `#LLM alignment`, `#elections`, `#AI ethics`

---

<a id="item-12"></a>
## [Kimi K3.1 open-weight release strips cyberattack training data](https://www.reddit.com/r/LocalLLaMA/comments/1xecgrf/kimi_k31_removes_cyberattack_training_data_from/) ⭐️ 7.0/10

Moonshot AI's Kimi K3.1 open-weight release reportedly removes cyberattack-related training data, according to a Reddit post on r/LocalLLaMA. The change is attributed primarily to China's new export restrictions and growing caution around cybersecurity exploits. This sets a precedent for how open-weight model releases may be curated for safety and regulatory compliance, potentially affecting what capabilities are available to researchers and developers. It also signals that Chinese AI labs are proactively adjusting releases in response to export controls and cybersecurity concerns. The post is brief and does not specify which datasets or capabilities were removed, so the exact scope of the filtering remains unclear. Kimi K3 is a 2.8-trillion-parameter native multimodal agentic model with a 1-million-token context window, and K3.1 appears to be a follow-up release.

reddit · r/LocalLLaMA · /u/zxyzyxz · Oct 24, 16:05

**Background**: Kimi is a series of open-weight large language models from Moonshot AI, available via web, API, and the Kimi Code command-line agent. China has recently proposed export restrictions on advanced AI technologies, including models and autonomous agents, amid growing international concern about AI safety. Separately, LLM training data can inadvertently include harmful or exploitable content, such as cyberattack techniques, which labs may seek to filter out before release.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi - K 3 · Hugging Face</a></li>
<li><a href="https://forklog.com/en/china-proposes-export-restrictions-on-ai-technologies/">China Proposes Export Restrictions on AI Technologies | ForkLog</a></li>

</ul>
</details>

**Tags**: `#open-weight-models`, `#LLM-safety`, `#export-restrictions`, `#cybersecurity`, `#Kimi`

---

<a id="item-13"></a>
## [KLD is misunderstood as a quantization quality metric](https://www.reddit.com/r/LocalLLaMA/comments/1xeim3m/kld_is_misunderstood/) ⭐️ 7.0/10

A Reddit post on r/LocalLLaMA argues that Kullback-Leibler Divergence (KLD) is commonly misinterpreted as a definitive quality metric for quantized LLMs, and explains why it cannot reliably rank models. The author details two major pitfalls: evaluating on random text instead of model-generated tokens, and the ease of manipulating KLD through calibration data overlap or fine-tuning on the evaluation set. This clarification is significant because the local LLM community increasingly relies on KLD scores to compare quantized models, and misleading numbers can lead users to choose inferior quantizations or trust inflated claims from model creators. It highlights the need for more robust evaluation practices beyond a single divergence metric. The post recommends generating a dataset with the base model and computing KLD only on generated tokens (zero weight on prompt tokens) for a more representative measure. It also warns that KLD is cheap to manipulate—e.g., by fine-tuning quantization scale parameters on the same data—whereas benchmark gaming (benchmaxxing) typically requires substantial compute.

reddit · r/LocalLLaMA · /u/Positive-Resource922 · Oct 24, 20:12

**Background**: Kullback-Leibler divergence is a statistical measure of how one probability distribution differs from another, commonly used in machine learning to compare model outputs. In the context of quantization, it measures how much the output probability distribution of a compressed (quantized) model deviates from the full-precision base model at each token. A lower KLD suggests the quantized model behaves more like the original, but it is not a symmetric metric and does not directly indicate task performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kullback-Leibler_divergence">Kullback-Leibler divergence</a></li>
<li><a href="https://smcleod.net/2026/04/measuring-model-quantisation-quality-with-kl-divergence/">Measuring Model Quantisation Quality with KL Divergence</a></li>
<li><a href="https://deepwiki.com/local-inference-lab/rtx6kpro/6.2-kld-evaluation-quantization-quality-measurement">KLD Evaluation — Quantization Quality Measurement | local ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#KLD`, `#evaluation`, `#LocalLLaMA`

---

<a id="item-14"></a>
## [Meta trains small byte-level models that scale better than token models](https://www.reddit.com/r/LocalLLaMA/comments/1xe88ja/meta_trained_small_ai_models_to_read_raw_bytes/) ⭐️ 7.0/10

Meta researchers trained ~1B parameter models on raw bytes instead of tokens, using distillation from Llama 3 8B, and found that while token models perform better early on, byte models improve steadily and are predicted to surpass Llama 3.2 1B and Gemma 3 1B by a few points if trends continue. This suggests byte-level modeling could eventually outperform token-based approaches, especially for small on-device models where squeezing more quality from the same size matters, and it could eliminate tokenizer quirks like miscounting letters. The claim that byte models beat Llama and Gemma is an extrapolation beyond actually trained runs; byte models also require about 5x more steps for the same text and were only tested at small scale, so scaling behavior remains unknown.

reddit · r/LocalLLaMA · /u/DotaMate · Oct 24, 13:08

**Background**: Most LLMs use tokenizers to split text into subword units (tokens), which are typically 4-5 characters long, reducing sequence length and compute. Byte-level models skip tokenization and process raw UTF-8 bytes directly, using a fixed vocabulary of 256 possible byte values, which enables language-agnostic processing but makes sequences longer. Knowledge distillation transfers knowledge from a larger teacher model to a smaller student model, and here the challenge is aligning a token-based teacher with a byte-based student.

<details><summary>References</summary>
<ul>
<li><a href="https://www.activeloop.ai/resources/glossary/byte-level-language-models/">What is Byte - Level Language Models ? | Activeloop Glossary</a></li>
<li><a href="https://arxiv.org/html/2602.01007v1">Distilling Token-Trained Models into Byte-Level Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tokenization_(large_language_models)">Tokenization (large language models)</a></li>

</ul>
</details>

**Discussion**: Commenters highlight that the headline claim is based on extrapolated curves rather than observed results, and discuss trade-offs like slower inference for byte models and the open question of whether byte-level models can be made as fast as token-based ones.

**Tags**: `#LLM`, `#tokenization`, `#byte-level modeling`, `#distillation`, `#Meta`

---

<a id="item-15"></a>
## [Run Qwen-Flash-Next Coder with 262K context on an 8GB GPU via llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1xebdzl/8_gb_gpu_262k_context_35_bpw_qwenflashnext_coder/) ⭐️ 7.0/10

A Reddit user detailed a method to run the 3.5 BPW Qwen-Flash-Next Coder model with a 262K context window on an 8GB GPU by offloading most MoE experts to RAM and n-gram embeddings to SSD using llama.cpp. The setup achieves 70 tokens/s prompt processing and 8 tokens/s text generation, with selective MoE offloading via regex and Vulkan backend recommended over CUDA for 8GB VRAM. This demonstrates that large-context MoE models can be run on consumer-grade hardware with only 8GB VRAM, making advanced coding assistants accessible to users without high-end GPUs. It highlights the practical benefits of MoE offloading and quantization techniques for the local LLM community. The model is a 3.5 BPW 'Coder' variant by ISTA DASLab using GSQ RCO quantization, with half of its experts removed, resulting in an effective 1.89 bits per parameter relative to the original model size. Performance is limited by PCIe 3.0, and the first run is slower due to MMAP; using the Qwen sharp chat template reduces overthinking.

reddit · r/LocalLLaMA · /u/jonathanx37 · Oct 24, 15:21

**Background**: Qwen-Flash-Next is a 125B-parameter MoE model with 6B active parameters and an additional 51B n-gram embedding, supporting a 262K context window. MoE models activate only a subset of experts per token, making them suitable for offloading to CPU/RAM while keeping attention layers on GPU. llama.cpp supports MoE offloading via flags like --n-cpu-moe, and quantization methods like GSQ and RCO from ISTA DASLab reduce model size with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/qwenlm/qwen3.8-flash-next">GitHub - QwenLM/ Qwen 3.8- Flash - Next : Qwen 3.8- Flash - Next is the...</a></li>
<li><a href="https://medium.com/@david.sanftenberg/gpu-poor-how-to-configure-offloading-for-the-qwen-3-235b-a22b-moe-model-using-llama-cpp-13dc15287bed">How to run big MoE models like Qwen-3–235B-A22B in Llama . cpp via...</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gsq-rco-quantization">What Are GSQ and RCO? Das Lab's New LLM Quantization Method</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#local-llm`, `#quantization`, `#moe`, `#gpu-memory`

---

<a id="item-16"></a>
## [Open-source browser rhythm game runs four neural nets locally to build levels from your songs](https://www.reddit.com/r/LocalLLaMA/comments/1xeia9o/made_a_rhythm_game_where_4_small_neural_nets/) ⭐️ 7.0/10

A developer released Struna, an open-source browser rhythm runner that uses four small ONNX models (BeatNet, Basic Pitch, Spleeter vocals, and SwiftF0) running locally via onnxruntime-web in separate web workers to analyze user-uploaded MP3s and procedurally generate game levels. The models total about 22 MB and are cached after first load, with a DSP fallback if inference is too slow. This project demonstrates a practical, fully on-device ML pipeline in the browser, showing how multiple lightweight audio models can be orchestrated in real time without uploading user data. It highlights the growing feasibility of local inference for creative and interactive applications, which could inspire similar browser-based tools in gaming, music production, and education. Each model has a specific role: BeatNet (~1.6 MB) tracks beats and downbeats to form the level grid, Basic Pitch (~0.2 MB) transcribes notes to create obstacles and rings, Spleeter's vocals model (~20 MB) isolates vocals to improve pitch tracking, and SwiftF0 (~0.1 MB) tracks vocal pitch every 16 ms. The game also uses regular DSP for onsets, loudness, and drops, and the same song always produces the same world; the developer notes that beat tracking sometimes misreads fast songs at half tempo.

reddit · r/LocalLLaMA · /u/MrFelliks · Oct 24, 19:59

**Background**: ONNX Runtime Web is a JavaScript library that runs ONNX models in the browser using WebAssembly or WebGL, enabling on-device inference without a server. BeatNet is a real-time music beat and downbeat tracking system, Basic Pitch is Spotify's lightweight audio-to-MIDI transcription model, and Spleeter is a source separation tool; all are small enough to run efficiently in a browser tab.

<details><summary>References</summary>
<ul>
<li><a href="https://onnxruntime.ai/docs/tutorials/web/">Web | onnxruntime</a></li>
<li><a href="https://github.com/mjhydri/BeatNet">GitHub - mjhydri/ BeatNet : BeatNet is state-of-the-art (Real-Time) and...</a></li>
<li><a href="https://github.com/spotify/basic-pitch">GitHub - spotify/basic-pitch: A lightweight yet powerful ... Basic Pitch: An open source MIDI converter from Spotify - About Meet Basic Pitch: Spotify’s Open Source Audio-to-MIDI ... spotify/basic-pitch · Hugging Face Basic Pitch download | SourceForge.net GitHub - spotify/basic-pitch-ts: A lightweight yet powerful ...</a></li>

</ul>
</details>

**Tags**: `#on-device-ml`, `#onnxruntime-web`, `#audio-processing`, `#webassembly`, `#open-source`

---

<a id="item-17"></a>
## [ANEMLL Forge 0.2.1 runs Qwen3.8-27B on M6 Neural Engine with 192K context](https://www.reddit.com/r/LocalLLaMA/comments/1xejv61/m6_mac_mini_owners_32gb_now_you_can_run_qwen3827b/) ⭐️ 7.0/10

ANEMLL Forge 0.2.1 now lets owners of the 32GB M6 Mac Mini run Qwen3.8-27B on the Apple Neural Engine with up to 192K context, adding an INT8 K/V cache that halves cache memory and a smaller drafter that shares the target model's output head, saving 0.86 GB of ANE memory at the same speed. This shows that a 27B-class model with very long context can run entirely on-device on consumer Apple silicon through the Neural Engine, which most local LLM tools still ignore, strengthening the case for private, low-power local inference. Decode speed varies heavily by content (JSON 35–62 tok/s, code 18–32, prose 10–17), prefill is 260 tok/s at short context but 62 tok/s at 192K, and 128K–192K uses a smaller prefill batch of 32 rows instead of 64 to fit the memory budget; the first full 192K compile takes about 2 hours on M6, though `--ctx` exports only needed entries so 16K takes about 10 minutes, and the author considers 96K the sweet spot at 123 tok/s prefill, ~27 tok/s decode, and ~21.4 GB total memory.

reddit · r/LocalLLaMA · /u/Competitive-Bake4602 · Oct 24, 21:05

**Background**: The Apple Neural Engine (ANE) is a dedicated low-power accelerator in Apple silicon that most local LLM tools bypass in favor of the GPU; ANEMLL is an open-source project that converts Hugging Face models to CoreML and optimizes them for ANE inference. The K/V cache stores attention keys and values for every processed token, so its memory grows linearly with context length and often becomes the main bottleneck for long-context inference, which is why INT8 quantization of the cache matters. Qwen3.8-27B is an open-weight multimodal model from Alibaba's Qwen family aimed at coding, visual understanding, tool use, and structured output.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Anemll/Anemll">GitHub - Anemll/Anemll: Artificial Neural Engine Machine ...</a></li>
<li><a href="https://www.anemll.com/">ANEMLL — On-Device AI for Apple Silicon</a></li>
<li><a href="https://arxiv.org/abs/2601.04719">[2601.04719] GPU-Accelerated INT8 Quantization for KV Cache ... Unlocking Longer Generation with Key-Value Cache Quantization KV-Cache Quantization for Long-Context LLM Inference in ... KV cache quantization: what FP8/INT8 K and V actually buy you ... KV Cache Quantization: FP8, FP4, and What They Cost You LLM quantization | LLM Inference Handbook</a></li>

</ul>
</details>

**Tags**: `#apple-neural-engine`, `#local-llm`, `#quantization`, `#inference-optimization`, `#apple-silicon`

---

<a id="item-18"></a>
## [ISTA Releases GSQ-RCO Quantized GGUFs for DeepSeek-V4.1-Flash-1017](https://www.reddit.com/r/LocalLLaMA/comments/1xe2wg8/release_ista_gsqrco_ggufs_for_deepseekv41flash1017/) ⭐️ 7.0/10

ISTA's Deep Algorithms and Systems Lab released three GSQ/RCO-quantized GGUFs of DeepSeek-V4.1-Flash-1017 at 1.75, 2.00, and 2.25 bits per weight, with backbones ranging from 120.7 GB to 155.2 GB, plus a shared 110.6 GB Engram file. The 2.00 bpw build matches the base model on all evaluated benchmarks, and every build can run on a single 12 GB GPU via the Strata inference engine. This makes a 763B-parameter sparse MoE model with a 1M-token context window accessible on consumer-grade hardware, dramatically lowering the barrier to running frontier-scale models locally. It also demonstrates that GSQ scalar quantization can retain near-100% accuracy at 2 bits per weight, strengthening the case for aggressive low-bit quantization in the local LLM ecosystem. The bit-width is averaged over the 551.9B backbone parameters, while the 196.6B-parameter Engram lookup tables are stored at IQ4_NL and can stay memory-mapped on disk since only one row is read per token. The GGUFs do not yet run in llama.cpp because it lacks DeepSeek-V4.1 support, so Strata is currently required; the 2.25 bpw results are still pending.

reddit · r/LocalLLaMA · /u/Loginhe · Oct 24, 08:05

**Background**: DeepSeek-V4.1-Flash-1017 is a sparse mixture-of-experts model with 384 routed experts per layer, of which only 6 are active per token, released with FP8 dense weights and FP4 routed experts. GSQ (Gumbel-Softmax Quantization) is a post-training scalar quantization method that jointly learns grid assignments and group scales, closing much of the gap to vector quantization at low bit-widths. RCO (Riemannian Constrained Optimization) assigns a quantization type to each tensor under a target bit-width budget. Strata is an open-source inference engine that runs large MoE models on consumer GPUs by offloading inactive experts to RAM and NVMe.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.18556">[2604.18556] GSQ: Highly-Accurate Low-Precision Scalar ... GitHub - IST-DASLab/GSQ: Gumbel-Softmax post-training ... GSQ: Highly-Accurate Low-Precision Scalar Quantization for ... GSQ - a ISTA-DASLab Collection - Hugging Face NeurIPS Poster GSQ: Highly-Accurate Low-Precision Scalar ... GSQ: Highly-Accurate Low-Precision Scalar Quantization for ... GSQ Quantization Explained with Qwen3.8 27B</a></li>
<li><a href="https://github.com/IST-DASLab/GSQ/">GitHub - IST-DASLab/GSQ: Gumbel-Softmax post-training ...</a></li>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#local-llm`, `#mixture-of-experts`, `#gguf`, `#deepseek`

---