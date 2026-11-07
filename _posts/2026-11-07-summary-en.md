---
layout: default
title: "Horizon Summary: 2026-11-07 (EN)"
date: 2026-11-07
lang: en
---

> From 39 items, 12 important content pieces were selected

---

1. [PwnEscape Part 2: Practical Firecracker VM Escape Walkthrough](#item-1) ⭐️ 8.0/10
2. [Muir: Linear Attention with Matched-Filter Readout Achieves 10M-Token Context in 25MB State](#item-2) ⭐️ 8.0/10
3. [Jev orchestrator queries Opus for LLM-judge identity resolution, matching accuracy at 4x lower cost](#item-3) ⭐️ 7.0/10
4. [Tesla to wind down Cybertruck production by mid-2027](#item-4) ⭐️ 7.0/10
5. [AI is dramatically accelerating AI research, sparking debate](#item-5) ⭐️ 7.0/10
6. [Tutorial Series on Bare-Metal UEFI Programming Sparks Discussion](#item-6) ⭐️ 7.0/10
7. [Anthropic IPO valuation expectations fall to $1.1T amid AI market rout](#item-7) ⭐️ 7.0/10
8. [Digital Antiquarian Retrospective on Deus Ex Sparks Discussion](#item-8) ⭐️ 7.0/10
9. [Allen AI Releases ToyBlocks: A Controlled Simulation for Robot Learning](#item-9) ⭐️ 7.0/10
10. [OpenAI reportedly raises an additional $11B at a $1.25T valuation](#item-10) ⭐️ 7.0/10
11. [Underdog demos 32MB speech and music model](#item-11) ⭐️ 7.0/10
12. [Boson AI releases Higgs Realtime Duplex, a 45B full-duplex multimodal model](#item-12) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [PwnEscape Part 2: Practical Firecracker VM Escape Walkthrough](https://pwn.ai/blog/firecracker-escape) ⭐️ 8.0/10

Pwn.ai published a detailed technical walkthrough (Part 2) demonstrating how to exploit the previously disclosed PwnEscape vulnerability (CVE-2026-99999) to escape Firecracker microVMs and reach the host. The write-up provides step-by-step exploitation details, but notes that the tested configuration lacked Firecracker's jailer-based containment. Firecracker underpins AWS Lambda and Fargate, so a practical guest-to-host escape path raises serious concerns for multi-tenant cloud isolation. The article also sparks debate about whether microVM security should rely on additional containment layers like jailer, namespaces, and seccomp. The exploit was demonstrated on a Firecracker configuration without the jailer, which in production drops privileges and restricts the VMM via namespaces and seccomp; the authors acknowledge that a properly jailed deployment would require a separate assessment of post-compromise privileges. The underlying vulnerability was disclosed weeks earlier, so this is exploitation detail rather than a new break.

hackernews · SerCe · Nov 6, 19:33 · [Discussion](https://news.ycombinator.com/item?id=50397219)

**Background**: Firecracker is an open-source virtualization technology from AWS that creates lightweight microVMs using KVM, combining hardware-level isolation with fast startup and low memory overhead. It is widely used in serverless platforms to run thousands of workloads per host. PwnEscape (CVE-2026-99999) is a Linux kernel guest-to-host VM escape that lets an attacker controlling a guest VM break out to the host.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/firecracker-microvm/firecracker">GitHub - firecracker-microvm/firecracker: Secure and fast ...</a></li>
<li><a href="https://socprime.com/blog/cve-2026-99999-analysis/">CVE-2026-99999: Critical Linux PwnEscape Flaw</a></li>
<li><a href="https://www.pandastack.ai/blog/vm-escape-attacks-explained/">VM Escape Attacks Explained (microVMs) · PandaStack</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that the tested setup lacked the jailer, so a properly jailed Firecracker instance may not be escapable in the same way. Others advocated for formally verified microhypervisors like Nova, and one operator offered a public demo service for PoC testing. Some noted the vulnerability was already disclosed, making this an exploitation guide rather than a new finding.

**Tags**: `#virtualization`, `#security`, `#firecracker`, `#exploitation`, `#microvm`

---

<a id="item-2"></a>
## [Muir: Linear Attention with Matched-Filter Readout Achieves 10M-Token Context in 25MB State](https://www.reddit.com/r/MachineLearning/comments/1xplbuu/muir_linear_attention_with_sensitivityallocated/) ⭐️ 8.0/10

Google Research introduces Muir, a linear attention architecture that fixes three bottlenecks in channel-wise gated delta models (like GDN-2) through matched-filter readout, sensitivity-allocated gating, and a numerically stable large-chunk parallel kernel. It enables streaming 10M tokens in a fixed 25MB state and achieves 90.0% zero-shot passkey accuracy at 1M tokens, while training 2.7x faster than Splash Attention at 32K. This work addresses key limitations of linear attention for long-context modeling, offering a path to extreme context lengths with constant memory, which could significantly reduce the cost of processing very long sequences compared to Transformer KV caches that grow linearly. It impacts efficient transformer research and applications requiring long-document understanding or streaming data. Muir uses an inverse fractional power law to equalize slow and fast decay rows, relaxing write erasure by 17% and extending lookback horizon by 60%; it fuses all five gates into one rank-512 projection to widen the FFN by 30.4% at a strict parameter budget; and its boundary-pivoted multiplicative decays avoid fp32 underflow and NaNs that affect 25% of heads in unpivoted versions. The paper reports 1.2x token efficiency vs. GDN-2 and lifts RULER 5-hop variable tracking root retention from 28.4% to 48.0%.

reddit · r/MachineLearning · /u/CategoryNormal149 · Nov 6, 19:10

**Background**: Linear attention models aim to reduce the quadratic complexity of standard Transformers by compressing history into a fixed-size state, but they often struggle with long-term recall. Gated DeltaNet (GDN) improves memory control by combining gating with the delta rule, and GDN-2 further decouples erase and write operations. Muir builds on these by addressing issues like slow-channel glare and write-vs-erase sensitivity, which degrade performance at very long contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Gated_DeltaNet">Gated DeltaNet</a></li>
<li><a href="https://arxiv.org/abs/2412.06464">[2412.06464] Gated Delta Networks: Improving Mamba2 with ...</a></li>
<li><a href="https://arxiv.org/abs/2605.22791">[2605.22791] Gated DeltaNet-2: Decoupling Erase and Write in ...</a></li>

</ul>
</details>

**Tags**: `#linear-attention`, `#long-context`, `#efficient-transformers`, `#machine-learning-research`, `#kv-cache-compression`

---

<a id="item-3"></a>
## [Jev orchestrator queries Opus for LLM-judge identity resolution, matching accuracy at 4x lower cost](https://hightouch.com/blog/llm-judges-identity-resolution) ⭐️ 7.0/10

Hightouch published a blog post demonstrating that a hybrid of Jev (a TypeSafe AI decision model) and Claude Opus can match frontier accuracy on LLM-as-judge identity resolution tasks at over 4x lower cost. The setup uses Jev as a cheaper orchestrator that decides when to escalate queries to Opus, and the result was discussed on Hacker News with 295 points and 65 comments. This illustrates a practical model-orchestration pattern where a cheap, fast decision model routes only hard cases to an expensive frontier model, potentially cutting evaluation costs significantly for LLM-as-judge pipelines. If generalizable, it could make large-scale AI evaluation more affordable, though the result is currently specific to identity resolution. The experiment tested Jev and GPT-6 Luna as judges for identity resolution, and the hybrid Jev+Opus approach matched frontier accuracy at over 4x lower cost. Jev is not a traditional LLM; it returns typed decisions (choice, score, or yes/no probability) in 70–500ms, which makes it suitable as a fast orchestrator.

hackernews · theanomaly · Nov 6, 19:48 · [Discussion](https://news.ycombinator.com/item?id=50397429)

**Background**: LLM-as-a-judge is a technique where a large language model evaluates the quality or correctness of another model's output against predefined criteria. Identity resolution is the task of determining whether records from different sources refer to the same real-world entity, such as a person or company. Model orchestration assigns different roles (router, worker, evaluator) to models of varying cost and capability to optimize price and performance. Jev, by TypeSafe AI, is a 'System One' model that returns structured decisions rather than free text.

<details><summary>References</summary>
<ul>
<li><a href="https://hightouch.com/blog/llm-judges-identity-resolution">LLM Judges for Identity Resolution at 4x Lower Cost | Hightouch</a></li>
<li><a href="https://openrouter.ai/docs/guides/community/jev">Jev Documentation - TypeSafe Decision Model on OpenRouter</a></li>
<li><a href="https://en.wikipedia.org/wiki/LLM-as-a-Judge">LLM-as-a-Judge - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted the result is specific to identity resolution rather than a general claim, and some criticized the human-labeled errors and reductive logic in AI decisions. Others shared similar experiences with model orchestration, highlighting that cheap models can effectively decide when to escalate to stronger models, and discussed curated context management as a future direction.

**Tags**: `#llm-as-judge`, `#cost-optimization`, `#model-orchestration`, `#identity-resolution`, `#ai-evaluation`

---

<a id="item-4"></a>
## [Tesla to wind down Cybertruck production by mid-2027](https://www.nbcnews.com/tech/tech-news/tesla-wind-cybertruck-production-years-poor-sales-markets-rcna607817) ⭐️ 7.0/10

Elon Musk announced that Tesla will wind down Cybertruck production at Gigafactory Texas around mid-2027, freeing up factory space to increase output of the Cybercab robotaxi. The decision follows weaker-than-expected sales of the electric pickup. The Cybertruck was Tesla's flagship attempt to enter the lucrative pickup market, and its discontinuation signals challenges in EV truck demand and Tesla's shifting priorities toward autonomy. It affects Tesla's product lineup, factory utilization, and investor confidence in its growth story. The wind-down is planned for around mid-2027 at Gigafactory Texas, with the freed capacity dedicated to the Cybercab robotaxi. The move comes after the Cybertruck failed to meet sales expectations despite initial hype.

hackernews · PLenz · Nov 6, 12:13 · [Discussion](https://news.ycombinator.com/item?id=50391456)

**Background**: The Cybertruck is Tesla's angular, stainless-steel electric pickup, first unveiled in 2019 and launched in 2023 after years of delays. It was intended to compete in the US full-size truck segment, but its high price, polarizing design, and practicality concerns limited its appeal. Tesla has been pivoting toward autonomous driving and robotaxis, with the Cybercab as a key future product.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/06/tesla-cybertruck-texas-musk.html">Tesla to wind down Cybertruck production in Texas next year ...</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/rip-cybertruck-musk-says-tesla-110857447.html?fr=sycsrp_catchall">RIP Cybertruck. Musk Says Tesla Winding Down Production ...</a></li>
<li><a href="https://www.motortrend.com/news/tesla-cybertruck-production-canceled">So Long, Cybertruck: Tesla Announces It Will Wind Down ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters debated the Cybertruck's failure from multiple angles: some highlighted its impracticality as a truck (poor towing, small bed), while others noted its usefulness as a home backup power source during outages. Many pointed to broader EV market headwinds, including the end of federal tax credits, declining EV sales share, and Tesla's lack of affordable models, questioning the company's future direction.

**Tags**: `#tesla`, `#electric-vehicles`, `#automotive-industry`, `#business`, `#hacker-news`

---

<a id="item-5"></a>
## [AI is dramatically accelerating AI research, sparking debate](https://www.planned-obsolescence.org/p/ai-is-dramatically-accelerating-ai) ⭐️ 7.0/10

An article on planned-obsolescence.org argues that AI is dramatically accelerating AI research, and the piece sparked a lively Hacker News discussion with 173 points and 133 comments. If AI can meaningfully speed up its own research, it could compress timelines for model development and reshape how AI labs allocate talent and compute, affecting the entire tech industry. Commenters questioned whether the acceleration stems from genuine gains in model intelligence (vertical scaling) or from massive capital investment and parallel compute (horizontal scaling), and noted that training speed may remain a fundamental bottleneck regardless of research automation.

hackernews · yurivish · Nov 6, 20:27 · [Discussion](https://news.ycombinator.com/item?id=50397994)

**Background**: Neural scaling laws describe how model performance improves predictably as model size, data, and compute increase. AI research acceleration refers to using AI to automate or speed up the process of AI development itself, a concept often linked to recursive self-improvement. Training large models involves massive parallel compute and is subject to bottlenecks in hardware, data, and convergence time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2001.08361">[2001.08361] Scaling Laws for Neural Language Models</a></li>
<li><a href="https://www.ibm.com/think/topics/parallel-computing">What is parallel computing ? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the premise, with some arguing that gains come more from capital and parallel compute than from smarter models, and others pointing out that training speed remains a fundamental bottleneck. Some also shared alternative analyses and noted that AI's strength in optimization may be a key factor.

**Tags**: `#AI research`, `#AI acceleration`, `#scaling laws`, `#machine learning`, `#community discussion`

---

<a id="item-6"></a>
## [Tutorial Series on Bare-Metal UEFI Programming Sparks Discussion](https://kevinboone.me/efitest_index.html) ⭐️ 7.0/10

Kevin Boone published a tutorial series on developing bare-metal applications for UEFI firmware using a Linux workstation, aimed at experienced Linux developers with no prior UEFI knowledge. The series covers setting up the development environment, writing UEFI applications, and dealing with the lack of a standard C library. This guide lowers the barrier to entry for systems programmers interested in UEFI development, a niche but critical area for bootloaders and firmware. The accompanying Hacker News discussion adds practical tips and resources, making it a valuable community knowledge base. The tutorial emphasizes that UEFI lacks a standard C library and has a Windows-like coding style, which can be challenging for Linux developers. Community members suggest using edk2-libc for C library support and verifying no undefined symbols remain after linking with `nm -D --undefined-only`.

hackernews · LaSombra · Nov 6, 16:50 · [Discussion](https://news.ycombinator.com/item?id=50394855)

**Background**: UEFI (Unified Extensible Firmware Interface) is the modern firmware interface that replaces legacy BIOS, responsible for initializing hardware and booting the operating system. Bare-metal programming means writing code that runs directly on hardware without an underlying operating system, often used for bootloaders, firmware, and embedded systems. UEFI applications are typically written in C and run in a pre-boot environment with limited services.

<details><summary>References</summary>
<ul>
<li><a href="https://kevinboone.me/efitest_index.html">Kevin Boone: First steps in bare-metal programming using UEFI ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/UEFI">UEFI - Wikipedia</a></li>
<li><a href="https://www.baeldung.com/cs/uefi-bare-metal-program-development">How to Make a Bare-Metal Program With UEFI (No OS Required)</a></li>

</ul>
</details>

**Discussion**: Commenters praised the guide as a great starting point, with one sharing experience building a Zig bootloader and noting the 16-bit character quirks of UEFI. Others recommended resources like edk2-libc, uefi-rs, and a UEFI IRC client, while some expressed frustration with UEFI's complexity compared to Linux development.

**Tags**: `#UEFI`, `#bare-metal`, `#systems-programming`, `#bootloader`, `#firmware`

---

<a id="item-7"></a>
## [Anthropic IPO valuation expectations fall to $1.1T amid AI market rout](https://www.bloomberg.com/news/articles/2026-11-06/anthropic-ipo-valuation-expectations-pressured-after-ai-rout) ⭐️ 7.0/10

Reports indicate that valuation expectations for Anthropic's upcoming IPO have dropped to as low as $1.1 trillion, down from earlier estimates of $1.3 trillion or more, following a broader sell-off in AI-related stocks. The news has sparked intense debate on Hacker News about the sustainability of AI subscription economics and competition from local models. A trillion-dollar IPO for Anthropic would be a landmark event for the AI industry, signaling both the immense scale of investment in frontier AI and the market's sensitivity to profitability concerns. The valuation pressure reflects broader investor skepticism about AI business models, which could affect funding for other AI startups and the pace of innovation. The valuation is reportedly tied to an ambitious revenue forecast of $190-200 billion for 2028, and the IPO's success may hinge on the S-1 lockup schedule, which some commenters believe could lead to massive share unlocks at an unfavorable political moment. The reported $1.1T figure is still far above Anthropic's last private valuation of $965 billion.

hackernews · dgellow · Nov 6, 16:54 · [Discussion](https://news.ycombinator.com/item?id=50394906)

**Background**: Anthropic is an AI safety and research company behind the Claude family of large language models, and it has been rumored to be preparing for an IPO. An IPO (Initial Public Offering) is the process by which a private company sells shares to the public for the first time, and its valuation reflects investor expectations of future growth. The 'AI rout' refers to a recent sharp decline in AI-related stock prices, which has made investors more cautious about high valuations.

<details><summary>References</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lteHJYZUVSRzZCUDRjNlNHdTVpZ0FQAQ?hl=en-GB&gl=GB&ceid=GB:en">Google News - Anthropic IPO valuation - Overview</a></li>
<li><a href="https://www.linkedin.com/pulse/anthropic-ipo-2026-explained-from-965-billion-possible-2-pvgkc">Anthropic IPO 2026 Explained, From $965 Billion to a Possible...</a></li>
<li><a href="https://www.morningstar.com/markets/stock-market-outlook-where-we-see-opportunities-q2">Q2 2025 Stock Market Outlook: From Overheated to... | Morningstar</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the sustainability of AI subscription pricing, with one noting that $15 of extra credits only provided 30 minutes of Claude Code usage, suggesting prices are far below actual inference costs. Another user reported that running the local Qwen3.8-Flash-Next model on their PC has drastically reduced their Claude Pro usage, and they plan to cancel their subscription. Others questioned the sanity of calling $1.1 trillion a 'low' valuation and doubted the IPO's success due to lockup schedules and political risks.

**Tags**: `#anthropic`, `#ipo`, `#ai-economics`, `#llm`, `#industry-news`

---

<a id="item-8"></a>
## [Digital Antiquarian Retrospective on Deus Ex Sparks Discussion](https://www.filfre.net/2026/11/deus-ex/) ⭐️ 7.0/10

The Digital Antiquarian published a long-form retrospective on the 2000 game Deus Ex, which reached the front page of Hacker News with 333 points and 167 comments. Deus Ex is widely regarded as a landmark in game design, particularly for its player freedom and immersive sim mechanics, so this retrospective offers valuable insights for game developers and interactive narrative enthusiasts. The article delves into the game's development history, including its use of the Unreal Engine and the challenges that led to cut content, while the community discussion highlights mods like GMDX and The Nameless Mod, the acclaimed soundtrack, and a debate over the reason for the missing Twin Towers in the skyline.

hackernews · cybersoyuz · Nov 6, 15:44 · [Discussion](https://news.ycombinator.com/item?id=50393758)

**Background**: Deus Ex is a 2000 action role-playing game developed by Ion Storm and published by Eidos Interactive. It combines first-person shooter, stealth, and role-playing elements, and is set in a dystopian cyberpunk future. The game was created by Warren Spector and is often cited as a prominent example of the immersive sim genre, influencing many later games.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Deus_Ex_(video_game)">Deus Ex (video game)</a></li>
<li><a href="https://www.filfre.net/2026/11/deus-ex/">Deus Ex The Digital Antiquarian</a></li>
<li><a href="https://www.moddb.com/games/deus-ex/mods">Mods - Deus Ex - ModDB</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong nostalgia and appreciation for the game, with one quoting Warren Spector on the press's tendency to attribute games to a single person, another praising the dynamic soundtrack, and others recommending mods like GMDX and The Nameless Mod. A notable debate arose over the article's explanation for the missing Twin Towers, with one commenter linking to a video arguing the reason is more complex.

**Tags**: `#game-design`, `#retrospective`, `#deus-ex`, `#interactive-narrative`, `#hacker-news`

---

<a id="item-9"></a>
## [Allen AI Releases ToyBlocks: A Controlled Simulation for Robot Learning](https://huggingface.co/blog/allenai/toyblocks) ⭐️ 7.0/10

Allen AI has released ToyBlocks, an open simulation framework for robot learning that automatically generates training demonstrations and evaluation tasks in a controlled tabletop world. It is the first 'foundation world' built on the new FoundationWorlds framework, eliminating the need for time-consuming human teleoperation. ToyBlocks provides a standardized, reproducible benchmark that could help the robotics and ML community compare algorithms fairly and study how training data variation affects generalization. By automating demonstration generation, it lowers the barrier to conducting controlled robot learning experiments. The framework lets researchers easily vary training experiences—for example, generating more pushing or flipping demonstrations—and then evaluate performance on tasks held out from training. It is designed as a controlled testbed rather than a photorealistic simulator, prioritizing systematic experimentation over visual fidelity.

rss · Hugging Face Blog · Nov 6, 14:00

**Background**: Robot learning, especially via reinforcement learning and imitation learning, often relies on simulated environments to train and test policies safely and cheaply. Benchmarks like RLBench provide standardized tasks, but generating demonstrations typically requires human teleoperation, which is slow and costly. ToyBlocks addresses this by automatically generating demonstrations and offering a controlled world for systematic evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/allenai/toyblocks">ToyBlocks: A controlled world for robot learning and evaluation</a></li>
<li><a href="https://allenai.org/blog/toyblocks">ToyBlocks: A controlled world for robot learning and ...</a></li>
<li><a href="https://extrapolator.ai/2026/11/06/toyblocks-a-controlled-world-for-robot-learning-and-evaluation/">ToyBlocks: A controlled world for robot learning and ...</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#reinforcement-learning`, `#benchmark`, `#simulation`, `#machine-learning`

---

<a id="item-10"></a>
## [OpenAI reportedly raises an additional $11B at a $1.25T valuation](https://techcrunch.com/2026/11/06/openai-reportedly-raises-an-additional-11-billion-at-a-1-25-trillion-valuation/) ⭐️ 7.0/10

OpenAI has reportedly raised an additional $11 billion as part of an ongoing funding round that has not yet closed but is expected to close in the coming weeks. The new capital comes at a reported valuation of $1.25 trillion. This massive raise at a trillion-dollar valuation signals continued investor confidence in OpenAI and the broader AI sector, concentrating enormous capital in a single company and potentially widening its lead over competitors. It also underscores how AI is becoming one of the largest destinations for venture and growth capital. The round is still open and the final amount could change before closing; the $1.25 trillion valuation is reported and not officially confirmed by OpenAI. The additional $11 billion is part of a larger funding effort rather than a standalone round.

rss · TechCrunch · Nov 6, 22:53

**Background**: OpenAI is the AI research and deployment company behind ChatGPT and the GPT series of models. In recent years it has raised billions of dollars from investors including Microsoft and various venture capital firms to fund compute, research, and product development. A $1.25 trillion valuation would make it one of the most valuable private companies in the world, reflecting the intense investor appetite for leading AI firms.

**Tags**: `#OpenAI`, `#funding`, `#AI industry`, `#venture capital`, `#valuation`

---

<a id="item-11"></a>
## [Underdog demos 32MB speech and music model](https://techcrunch.com/2026/11/06/underdog-shows-off-a-32mb-speech-model-in-new-demo/) ⭐️ 7.0/10

Underdog has released a demo built with its new voice model called Woof, which is only 32 MB in size and can generate both speech and music. This comes weeks after the startup launched Bark, a 167 MB speech-to-text model designed for edge devices. A 32MB model that handles both speech and music generation marks a notable efficiency milestone for on-device and edge generative audio, potentially enabling low-latency, private audio generation on resource-constrained hardware. This could affect developers building voice assistants, games, and accessibility tools that cannot rely on cloud APIs. The demo is a game built with the Woof model, but TechCrunch's write-up provides limited technical detail on architecture, audio quality, or supported languages. The earlier Bark model is 167 MB and targets transcription and dictation on edge devices, suggesting Underdog is pursuing a family of small-footprint audio models.

rss · TechCrunch · Nov 6, 13:02

**Background**: Generative audio models typically require hundreds of millions to billions of parameters and run in the cloud, which adds latency and raises privacy concerns. Small-footprint models aim to shrink these systems enough to run locally on phones, laptops, or embedded devices. Underdog is a startup competing in this emerging edge-AI audio space, where efficiency and on-device privacy are key selling points.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/06/underdog-shows-off-a-32mb-speech-model-in-new-demo/">Underdog shows off a 32 MB speech model in new demo | TechCrunch</a></li>
<li><a href="https://huggingface.co/ConwayResearch/Underdog-Bark-3.0-Pro">ConwayResearch/ Underdog -Bark-3.0-Pro · Hugging Face</a></li>
<li><a href="https://gradium.ai/content/on-device-text-to-speech-2026">On-Device Text-to-Speech: How Edge Synthesis Works</a></li>

</ul>
</details>

**Tags**: `#speech-synthesis`, `#generative-audio`, `#small-models`, `#edge-ai`, `#music-generation`

---

<a id="item-12"></a>
## [Boson AI releases Higgs Realtime Duplex, a 45B full-duplex multimodal model](https://www.reddit.com/r/MachineLearning/comments/1xpn5pv/higgs_realtime_duplex_a_45b_moe_fullduplex_model/) ⭐️ 7.0/10

Boson AI has released Higgs Realtime Duplex, a 45B-parameter Mixture-of-Experts model that processes audio, video, and text streams simultaneously in 160 ms chunks while performing background thinking, tool calls, and delegation. The model is not open-weight, and its Duplex API is currently available only via a waitlist, while the earlier turn-based Higgs Realtime is generally available. This release represents a notable architectural direction for realtime voice and video AI, moving beyond turn-based interaction to continuous, full-duplex processing that can listen, watch, and speak at once. It could influence how future conversational agents handle natural turn-taking, interruptions, and background task execution, impacting developers building realtime multimodal applications. The model uses a chunked-stream design with 160 ms chunks, encoding audio input at 1 token per chunk and audio output at 2 tokens per chunk, and it represents silence as chunks to decide when to backchannel or interrupt. It is trained via multi-teacher on-policy distillation from specialist teachers and a self-improvement loop, and on benchmarks it leads on five of seven tasks but trails OpenAI's best settings by 1 to 5 points, with turn-taking being the weakest area.

reddit · r/MachineLearning · /u/Cali_Cobarde · Nov 6, 20:23

**Background**: Full-duplex models differ from traditional turn-based voice assistants by processing input and output streams simultaneously, enabling more natural conversation with interruptions and backchanneling. Mixture-of-Experts (MoE) is an architecture that uses multiple specialized sub-networks (experts) and activates only a subset for each input, improving efficiency at large parameter counts. Boson AI's model builds on its earlier Higgs Realtime speech-to-speech model and adds video and face generation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.boson.ai/blog/higgs-realtime-duplex">Higgs Realtime Duplex: Face to Face, Working in the ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.emergentmind.com/topics/full-duplex-speech-llms">Full - Duplex Speech LLMs</a></li>

</ul>
</details>

**Tags**: `#multimodal`, `#full-duplex`, `#MoE`, `#voice-ai`, `#realtime`

---