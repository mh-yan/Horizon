---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 40 items, 15 important content pieces were selected

---

1. [Politician probing spyware abuses hacked with Pegasus](#item-1) ⭐️ 9.0/10
2. [Mistral Releases Leanstral-1.5 for Formal Verification](#item-2) ⭐️ 9.0/10
3. [llama.cpp patch runs DeepSeek V4 Flash with 1M context on RTX 5090](#item-3) ⭐️ 9.0/10
4. [Ubicloud Advocates Strict Memory Overcommit for PostgreSQL](#item-4) ⭐️ 8.0/10
5. [Wordgard: New Rich-Text Editor by ProseMirror Creator](#item-5) ⭐️ 8.0/10
6. [The Fall and Rise of Screwworm](#item-6) ⭐️ 8.0/10
7. [User Builds Extreme 448GB VRAM Rig for Local LLM](#item-7) ⭐️ 8.0/10
8. [Guide to Running SOTA LLMs Locally](#item-8) ⭐️ 7.0/10
9. [Costco's Anti-Amazon Strategy: Avoiding Last-Mile Delivery](#item-9) ⭐️ 7.0/10
10. [Valve open-sources Steam Machine e-ink screen design](#item-10) ⭐️ 7.0/10
11. [60% LLM Cost Cut by Converting Code to Images and OCR](#item-11) ⭐️ 7.0/10
12. [Half-Baked Product: A Startup Cautionary Tale](#item-12) ⭐️ 7.0/10
13. [Course Creator Reports 50%+ Revenue Drop Due to AI](#item-13) ⭐️ 7.0/10
14. [Private Space Pilots Fly Orbital Missions for US Space Force](#item-14) ⭐️ 7.0/10
15. [DeepSeek DSpark: Up to 85% Faster Inference](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Politician probing spyware abuses hacked with Pegasus](https://techcrunch.com/2026/07/02/politician-who-investigated-spyware-abuses-had-his-phone-hacked-with-pegasus-spyware/) ⭐️ 9.0/10

A European politician who served on an EU committee investigating the spyware industry had his iPhone infected with NSO Group's Pegasus spyware by a government customer of NSO in October 2022 and March 2023. This incident highlights the irony of spyware being used against those who investigate it, underscoring the grave threat to democratic oversight and privacy rights posed by commercial surveillance tools. The Citizen Lab confirmed the infection with high confidence, and the attack occurred while the politician was on the EU committee investigating spyware abuses. NSO Group markets Pegasus for crime and terrorism, but it has been routinely used against journalists, lawyers, and activists.

rss · TechCrunch · Jul 3, 05:05

**Background**: Pegasus is a sophisticated spyware developed by Israeli firm NSO Group, capable of remote zero-click surveillance, including reading messages, tracking location, and accessing microphones and cameras. It is typically deployed by government clients against high-value targets, and its use has sparked global controversy over human rights and privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/NSO_Group">NSO Group - Wikipedia</a></li>
<li><a href="https://www.theguardian.com/technology/2024/nov/14/nso-pegasus-spyware-whatsapp">NSO – not government clients – operates its spyware, legal documents reveal | Hacking | The Guardian</a></li>

</ul>
</details>

**Discussion**: Commenters noted that this is part of a broader pattern, with one pointing to a similar scandal in Greece where politicians were hacked by Pegasus, allegedly orchestrated by the prime minister's office. Another commenter expressed cynicism about the influence of lobbyists and US corporations on EU data.

**Tags**: `#cybersecurity`, `#spyware`, `#NSO Group`, `#Pegasus`, `#surveillance`

---

<a id="item-2"></a>
## [Mistral Releases Leanstral-1.5 for Formal Verification](https://www.reddit.com/r/LocalLLaMA/comments/1umgdhx/mistral_released_leanstral15119ba6b/) ⭐️ 9.0/10

Mistral released Leanstral-1.5-119B-A6B, a 6B active parameter model under Apache-2.0 license, achieving state-of-the-art results in formal verification by saturating the miniF2F benchmark, solving 587/672 PutnamBench problems, and scoring 87% on FATE-H and 34% on FATE-X. This release advances automated theorem proving and code verification, enabling developers to automatically verify software correctness and find real bugs, with the model uncovering 5 previously unknown bugs across 57 open-source repositories. The model was trained using mid-training, supervised fine-tuning, and reinforcement learning with CISPO (Clipped Importance Sampling Policy Optimization), and it excels in agentic proof engineering and real-world code verification.

reddit · r/LocalLLaMA · /u/Tall-Ad-7742 · Jul 3, 14:44

**Background**: Formal verification uses mathematical proofs to ensure software correctness. Benchmarks like miniF2F and PutnamBench test AI's ability to solve formal mathematics problems. CISPO is a reinforcement learning algorithm that clips importance sampling weights for stable training.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/openai/miniF2F">openai/miniF2F: Formal to Formal Mathematics Benchmark - GitHub</a></li>
<li><a href="https://swift.readthedocs.io/en/latest/Instruction/GRPO/AdvancedResearch/CISPO.html">Clipped Importance Sampling Policy Optimization (CISPO) — swift 4.4.0.dev0 documentation</a></li>
<li><a href="https://huggingface.co/datasets/amitayusht/PutnamBench">amitayusht/ PutnamBench · Datasets at Hugging Face</a></li>

</ul>
</details>

**Discussion**: The Reddit comments on this post are mostly unrelated to Leanstral-1.5, discussing other models like AMALIA and LongCat, as well as a user's experience with Qwen 27B. No direct discussion of Leanstral-1.5 is present.

**Tags**: `#AI/ML`, `#formal verification`, `#theorem proving`, `#open-source`, `#Mistral`

---

<a id="item-3"></a>
## [llama.cpp patch runs DeepSeek V4 Flash with 1M context on RTX 5090](https://www.reddit.com/r/LocalLLaMA/comments/1ulymml/llamacpp_patch_deepseek_v4_flash_running_with/) ⭐️ 9.0/10

A custom CUDA kernel patch for llama.cpp enables DeepSeek V4 Flash to run with full 1M token context on a single RTX 5090, reducing VRAM requirement from ~256GB to ~31GB and achieving prefill speeds of 159 t/s at 1M context. This breakthrough makes long-context inference (up to 1M tokens) feasible on consumer hardware, dramatically lowering the barrier for researchers and developers to experiment with state-of-the-art sparse attention models locally. The patch implements a CUDA kernel for the DSA lightning indexer, which was previously missing in llama.cpp. It achieves 263 t/s prefill at 256K context and 159 t/s at 1M context, with peak VRAM usage of ~31 GiB at 1M.

reddit · r/LocalLLaMA · /u/da_dragon321 · Jul 2, 23:54

**Background**: DeepSeek V4 Flash uses DeepSeek Sparse Attention (DSA) with a lightning indexer to reduce attention computation. The DSA lightning indexer was not properly supported in llama.cpp, causing excessive VRAM usage. This patch wires the indexer into the model graph and adds a CUDA path.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/lemyx/tilelang-dsa">DeepSeek-V3.2-Exp DSA Warmup Lightning Indexer training operator ...</a></li>
<li><a href="https://ninehills.github.io/jack-diary/articles/20260308-deepseek-dsa-analysis.html">20260308 / 稀疏的胜利：拆解 DeepSeek DSA 与 Lightning Indexer</a></li>

</ul>
</details>

**Discussion**: The community is excited about the achievement, with users noting that local models like DeepSeek V4 Flash now approach Sonnet quality while being faster in wall-clock time than API-based models. Some users are benchmarking further and sharing detailed comparisons.

**Tags**: `#llama.cpp`, `#DeepSeek`, `#CUDA`, `#LLM inference`, `#long context`

---

<a id="item-4"></a>
## [Ubicloud Advocates Strict Memory Overcommit for PostgreSQL](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud published a blog post explaining why they use strict memory overcommit (vm.overcommit_memory=2) for PostgreSQL to prevent the OOM killer from terminating the database process. The post details how this setting avoids system instability under memory pressure. This matters because PostgreSQL is a memory-intensive database that can trigger the Linux OOM killer under default overcommit settings, causing unexpected downtime. By adopting strict overcommit, database operators can improve reliability, but the approach requires careful capacity planning and may not suit all workloads. Strict overcommit (mode 2) refuses allocations that exceed CommitLimit, which is set via overcommit_kbytes or overcommit_ratio. The blog post notes that this setting can prevent fork() calls from succeeding if memory is tight, so thorough testing in QA is essential before production deployment.

hackernews · furkansahin · Jul 3, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48774509)

**Background**: The Linux kernel uses memory overcommit to allocate more virtual memory than physical RAM, assuming not all memory will be used simultaneously. When the system runs out of memory, the OOM killer selects and terminates a process to free memory. PostgreSQL's memory-intensive operations (e.g., sorting, hash joins) can trigger the OOM killer under default heuristic overcommit (mode 0), leading to database crashes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://news.ycombinator.com/item?id=48774509">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit | Hacker News</a></li>
<li><a href="https://utcc.utoronto.ca/~cks/space/blog/linux/StrictOvercommitCanOOM">Chris's Wiki :: blog/linux/StrictOvercommitCanOOM</a></li>

</ul>
</details>

**Discussion**: Community comments highlight caution: one user warns that mode 2 can prevent forks and advises thorough testing. Another user shares experience with mixed workloads (Go app + PostgreSQL) where mode 2 caused instability. The blog's author (Ozgun) acknowledges the title was too strong and notes that strict overcommit may have unanticipated side-effects in many scenarios.

**Tags**: `#PostgreSQL`, `#Linux`, `#memory management`, `#OOM killer`, `#database operations`

---

<a id="item-5"></a>
## [Wordgard: New Rich-Text Editor by ProseMirror Creator](https://wordgard.net/) ⭐️ 8.0/10

Wordgard is a new in-browser rich-text editor released by Marijn Haverbeke, the creator of ProseMirror, offering a modern alternative with improved design, documentation, and developer experience. This matters because ProseMirror is a widely used foundation for editors like Tiptap, and Wordgard aims to address its steep learning curve and documentation gaps, potentially becoming a new standard for web-based rich-text editing. Wordgard shares many concepts with ProseMirror but is not a drop-in replacement; there is no upgrade path, and switching requires significant work. The editor is designed with a focus on clean design and comprehensive documentation.

hackernews · indy · Jul 3, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48772573)

**Background**: ProseMirror is a battle-tested rich-text editor framework known for its semantic document model and high performance, but it has a steep learning curve and sparse documentation. Many popular editors like Tiptap are built on top of ProseMirror. Wordgard is a new project from the same author aiming to provide a more approachable alternative while retaining the core strengths.

<details><summary>References</summary>
<ul>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**Discussion**: The community response is positive, with users praising the design and documentation. Some express interest in the 'why' behind the new editor and note the lack of an upgrade path from ProseMirror. Others share experiences of building custom editors and find validation in Wordgard's approach.

**Tags**: `#rich-text editor`, `#ProseMirror`, `#web development`, `#WYSIWYG`, `#open source`

---

<a id="item-6"></a>
## [The Fall and Rise of Screwworm](https://www.construction-physics.com/p/the-fall-and-rise-of-screwworm) ⭐️ 8.0/10

A detailed historical account of screwworm eradication efforts using the sterile insect technique (SIT) and their recent collapse, with new cases confirmed in South Texas in 2026. 螺旋蝇的重新出现威胁到美洲的牲畜和公共卫生，可能造成数十亿美元的经济损失，并引发对基于昆虫不育技术的根除计划长期可持续性的质疑。 The sterile insect technique involves releasing massive numbers of radiation-sterilized male flies to mate with wild females, reducing reproduction. A maintenance barrier at the Darién Gap has failed multiple times, allowing re-infestation.

hackernews · crescit_eundo · Jul 3, 12:58 · [Discussion](https://news.ycombinator.com/item?id=48774492)

**Background**: New World screwworm (Cochliomyia hominivorax) larvae feed on living flesh of warm-blooded animals, including humans, and can be fatal if untreated. The USDA successfully eradicated it from the U.S. and Central America using SIT, but maintaining a barrier in Panama has proven challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aphis.usda.gov/sites/default/files/factsheet-eradicating-nws-sit.pdf">Eradicating New World Screwworm with Sterile Insect Technique</a></li>
<li><a href="https://www.aphis.usda.gov/sites/default/files/factsheet-sit-dispersal-methods.pdf">Sterile Fly Release Methods for Controlling Screwworm</a></li>
<li><a href="https://www.aphis.usda.gov/livestock-poultry-disease/cattle/ticks/screwworm">New World Screwworm Prevention for Animals</a></li>

</ul>
</details>

**Discussion**: Commenters discussed the cost-benefit of maintaining the Darién barrier versus continent-wide eradication, and raised concerns about radiation resistance selection in screwworm populations. Some praised the historical eradication efforts despite limited resources.

**Tags**: `#agriculture`, `#public health`, `#entomology`, `#science history`, `#pest control`

---

<a id="item-7"></a>
## [User Builds Extreme 448GB VRAM Rig for Local LLM](https://www.reddit.com/r/LocalLLaMA/comments/1umokhj/uh_honey_how_do_you_feel_about_takeout/) ⭐️ 8.0/10

A Reddit user shared a custom local LLM rig with 448GB VRAM, running MiniMax M3 in AWQ-INT4 on vLLM, achieving ~960 tokens per second in batch mode. This demonstrates that high-throughput local inference of frontier-level models is possible with sufficient hardware, potentially reducing reliance on cloud APIs for privacy-sensitive or latency-critical applications. The rig combines 2x RTX Pro 6000 Max-Q (96GB), 8x RTX 3090 (24GB), and 2x RTX 5090 (32GB), using pipeline parallelism (PP) over tensor parallelism (TP) groups of 2. The user aims for 4x concurrency with 1M context length.

reddit · r/LocalLLaMA · /u/MotorcyclesAndBizniz · Jul 3, 20:02

**Background**: MiniMax M3 is an open-weight multimodal MoE model with 1M context window, competitive on coding and agentic tasks. AWQ-INT4 quantization reduces GPU memory by ~50% with minimal accuracy loss. vLLM is a high-throughput inference engine supporting distributed execution.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/models/text/m3">MiniMax M 3 - Coding & Agentic Frontier, 1M Context, Multimodal</a></li>
<li><a href="https://github.com/mit-han-lab/llm-awq">GitHub - mit-han-lab/llm-awq: [MLSys 2024 Best Paper Award ... Quantization Techniques for LLM Inference: INT8, INT4, GPTQ ... 4-Bit Quantization Decoded: INT4 QAT, MXFP4, and NVFP4 [2306.00978] AWQ: Activation-aware Weight Quantization for ... LLM Quantization Explained: INT8, INT4, GPTQ & AWQ</a></li>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm-project/vllm: A high-throughput and memory-efficient ...</a></li>

</ul>
</details>

**Discussion**: The community reacted with humor and awe, joking about the cost to the user's marriage and the massive electricity bill. Some users discussed the practicality of such a setup for local inference versus cloud alternatives.

**Tags**: `#LocalLLM`, `#Hardware`, `#Inference`, `#VRAM`, `#VLLM`

---

<a id="item-8"></a>
## [Guide to Running SOTA LLMs Locally](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob published a comprehensive guide on GitHub detailing how to build and run state-of-the-art large language models on local hardware, including specific hardware bills of materials and model recommendations. This guide helps enthusiasts and professionals understand the real costs and performance trade-offs of running LLMs locally, which is crucial for privacy, offline use, and avoiding cloud subscription fees. The guide covers setups ranging from a $3,000 dual RTX 3090 configuration with 48GB VRAM to a $50,000+ multi-GPU build, and recommends models like Qwen3.6-27B for mid-range hardware.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Large language models (LLMs) require significant computational resources, especially VRAM, for inference. State-of-the-art models often need hundreds of GB of VRAM, making local deployment expensive. Quantization techniques reduce model size but may impact quality.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jamesob/local-llm">GitHub - jamesob/local-llm: Everything I know about running LLMs locally · GitHub</a></li>
<li><a href="https://enji.ai/tech-articles/how-to-switch-from-sota-llms-to-local-oss-llms/">Switching from SOTA to Local OSS LLMs: A Practical Guide</a></li>
<li><a href="https://www.pugetsystems.com/solutions/ai/enterprise-scale/hardware-recommendations/">Hardware Recommendations for Large Language Model Servers | Puget Systems</a></li>

</ul>
</details>

**Discussion**: Commenters warn that costs can balloon beyond initial estimates, with one noting a $40K budget build actually costing $50-55K. Others suggest alternatives like unified memory architectures (e.g., 128GB Mac) or cloud services as more cost-effective for most users.

**Tags**: `#LLM`, `#local inference`, `#hardware`, `#deep learning`, `#open source`

---

<a id="item-9"></a>
## [Costco's Anti-Amazon Strategy: Avoiding Last-Mile Delivery](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

An analysis argues that Costco's business model deliberately avoids the logistical complexity of last-mile delivery, contrasting with Amazon's approach of home delivery of single-packaged items. This comparison highlights fundamental strategic differences in retail, questioning the social value of the logistical complexity required for home delivery and underscoring Costco's resilience against e-commerce giants. Costco relies on customers driving to its warehouses and transporting bulk purchases themselves, while Amazon handles last-mile delivery to individual homes, a cost-intensive process.

hackernews · bookofjoe · Jul 3, 15:14 · [Discussion](https://news.ycombinator.com/item?id=48776044)

**Background**: Last-mile delivery refers to the final leg of the logistics process where goods are transported from a distribution center to the end customer's doorstep. It is a major cost and complexity driver for e-commerce companies like Amazon. Costco's warehouse club model, in contrast, shifts the transportation burden to customers, reducing logistical overhead.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Last_mile_(transportation)">Last mile (transportation) - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/why-costcos-business-model-is-so-great-2016-2">Costco is beating Walmart and Amazon with the 'best business model' in retail</a></li>
<li><a href="https://www.untaylored.com/post/how-costco-makes-money-business-model-explained">How Costco Makes Money: The Costco Business Model and Revenue Streams Explained | Untaylored</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Amazon also tries to concentrate purchases on fewer SKUs to gain similar benefits as Costco, but can support a long tail of SKUs. Some praised Costco's wisdom in avoiding the last-mile problem, while others pointed out non-US perspectives, such as Costco's UK membership restrictions and its focus on non-food items like electronics and tires.

**Tags**: `#business strategy`, `#logistics`, `#e-commerce`, `#retail`

---

<a id="item-10"></a>
## [Valve open-sources Steam Machine e-ink screen design](https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/) ⭐️ 7.0/10

Valve has open-sourced the design of the e-ink display used on the Steam Machine, allowing anyone to build their own compatible screen. The company will not produce the display itself but has released the necessary files for community fabrication. This move empowers the community to customize and repair the Steam Machine, fostering innovation and repairability. It aligns with Valve's broader open-source hardware strategy and could inspire similar practices across the industry. The e-ink panel is identified as a standard Adafruit 5.83-inch eInk display (product 6397). The open-source release includes design files and documentation, enabling users to 3D-print enclosures and integrate the screen with the Steam Machine.

hackernews · ahlCVA · Jul 3, 13:01 · [Discussion](https://news.ycombinator.com/item?id=48774518)

**Background**: The Steam Machine is Valve's upcoming gaming console, first showcased in late 2025 with an optional e-ink front panel for customization. Valve has a history of supporting open-source hardware and software, such as the Steam Deck and contributions to graphics drivers. Open-sourcing the e-ink screen design allows the community to create custom skins, animations, or functional displays.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/">Valve open source the Steam Machine e-ink screen so you can make your own | GamingOnLinux</a></li>
<li><a href="https://www.notebookcheck.net/Valve-showcases-Steam-Machine-with-e-ink-display.1162643.0.html">Valve showcases Steam Machine with e-ink display - Notebookcheck News</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users praising Valve's approach to letting the community run with optional add-ons. One user identified the specific Adafruit panel, while another expressed interest in adapting the design for the Framework Desktop form factor. A technical question about larger e-ink screens with HDMI input also emerged.

**Tags**: `#open-source`, `#hardware`, `#valve`, `#e-ink`, `#community`

---

<a id="item-11"></a>
## [60% LLM Cost Cut by Converting Code to Images and OCR](https://github.com/teamchong/pxpipe) ⭐️ 7.0/10

A developer discovered that converting code text into images and then using an LLM's OCR capability can reduce API costs by up to 60%, due to lower per-token pricing for image inputs compared to text tokens. This pricing loophole could significantly reduce operational costs for heavy LLM users, but it may also lead providers to adjust pricing or close the gap, potentially increasing OCR-related costs. The technique, implemented in the pxpipe tool, exploits the difference in token pricing between text and image inputs in LLM APIs, though it may require more completion tokens and be slower.

hackernews · dimitropoulos · Jul 3, 15:50 · [Discussion](https://news.ycombinator.com/item?id=48776464)

**Background**: LLM APIs typically charge per token, with text tokens and image tokens priced differently. OCR (Optical Character Recognition) is the process of extracting text from images. Some providers like Gemini process PDFs by OCR-ing them internally without charging extra text tokens, suggesting a potential accounting loophole.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48776464">60% Fable cost cut by converting code to images and having the model OCR it | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters noted that this hack exploits a token accounting loophole that may be closed, similar to how Gemini handles PDFs. Some reported trying similar approaches with OpenAI models last year, finding it reduced prompt tokens but required more completion tokens, ultimately being more expensive and slower.

**Tags**: `#LLM`, `#cost optimization`, `#OCR`, `#pricing hack`, `#AI`

---

<a id="item-12"></a>
## [Half-Baked Product: A Startup Cautionary Tale](https://weli.dev/blog/half-baked-product/) ⭐️ 7.0/10

A reflective essay uses a fictional oven company to illustrate how a startup fails due to misaligned incentives and lack of domain expertise. This story resonates broadly because it highlights common startup pitfalls—founder motivation misaligned with product reality, and organizational disconnect—that lead to failure despite funding and effort. The article scores 7.0/10 on Hacker News with 1163 points and 355 comments, indicating strong community engagement and recognition of the familiar yet valuable themes.

hackernews · weli · Jul 3, 08:23 · [Discussion](https://news.ycombinator.com/item?id=48772388)

**Background**: The essay is a cautionary tale about a startup that builds a 'half-baked' product—an oven that works technically but fails in the market. The story explores how the founder's primary motivation (wealth) clashes with the need for deep domain expertise, and how different teams (engineering, sales, management) operate in silos, leading to a product that satisfies no one.

**Discussion**: Commenters highlight the founder's misaligned motivation (wealth over domain expertise) as a core issue, and note the organizational disconnect between roles. Some humorously relate to similar experiences in other industries, while others point out that the story's themes are timeless and will recur.

**Tags**: `#startups`, `#product development`, `#entrepreneurship`, `#failure analysis`

---

<a id="item-13"></a>
## [Course Creator Reports 50%+ Revenue Drop Due to AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Josh W. Comeau, a well-known course creator, reported that his latest course launch sold only about one-third as many copies as typical, and his existing courses have seen revenue declines of over 50% year-over-year, which he attributes to AI-driven uncertainty about developer jobs and LLMs replacing paid learning resources. This firsthand data from a prominent educator highlights a tangible economic impact of AI on the developer education market, potentially signaling a broader trend that could affect many independent creators and the learning ecosystem. Comeau noted that other course creators he spoke with are seeing the same trend, with revenue down 50%+ and fewer people engaging with content, as learners switch to LLMs that consume creators' work without consent or compensation.

rss · Simon Willison · Jul 3, 21:25

**Background**: Josh W. Comeau is a well-respected front-end developer and educator known for high-quality interactive courses on CSS and React. The rise of large language models (LLMs) like ChatGPT has enabled personalized tutoring and code generation, potentially reducing demand for structured paid courses. Additionally, widespread layoffs and AI automation fears have created uncertainty about the future of software development jobs, discouraging investment in learning.

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#job market`, `#LLMs`

---

<a id="item-14"></a>
## [Private Space Pilots Fly Orbital Missions for US Space Force](https://techcrunch.com/2026/07/02/private-space-pilots-are-flying-orbital-missions-for-the-us-space-force/) ⭐️ 7.0/10

True Anomaly and Rocket Lab are conducting orbital satellite maneuvers for the U.S. Space Force, performing Top Gun-style fly-bys to test space domain awareness and rapid response capabilities. This marks a significant shift toward commercial-military collaboration in space, potentially accelerating the development of space combat tactics and satellite servicing technologies. In the Victus Haze mission, Rocket Lab's satellite Puma was activated and ready for its first orbital maneuver within 37 hours and 36 minutes of launch, demonstrating rapid on-orbit readiness.

rss · TechCrunch · Jul 2, 23:01

**Background**: True Anomaly is a defense technology company focused exclusively on space defense, founded in 2022 by ex-U.S. Space Force members. Rocket Lab provides dedicated small satellite launch services with precise orbital injection. The U.S. Space Force is increasingly leveraging commercial partners for space domain awareness and rapid response missions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.trueanomaly.space/">True Anomaly - Delivering Decisive Capabilities for Space Superiority.</a></li>
<li><a href="https://www.airandspaceforces.com/victus-haze-mission-rapid-maneuvers-satellites/">Satellites Maneuver on Rapid Timelines for Victus Haze Mission</a></li>
<li><a href="https://www.trueanomaly.space/careers">Careers - True Anomaly</a></li>

</ul>
</details>

**Tags**: `#space`, `#military`, `#private space industry`, `#satellite operations`

---

<a id="item-15"></a>
## [DeepSeek DSpark: Up to 85% Faster Inference](https://www.reddit.com/r/LocalLLaMA/comments/1um9j5q/deepseek_drops_another_huge_breakthrough_dspark/) ⭐️ 7.0/10

DeepSeek has open-sourced DSpark, a speculative decoding framework that accelerates LLM inference by up to 85% on V4-Flash and V4-Pro models without requiring new hardware or retraining. This breakthrough significantly reduces inference latency, making large language models more practical for real-time applications and lowering operational costs, which could accelerate adoption across industries. DSpark is part of the DeepSpec codebase and was released on June 27, 2026. The speedup depends on acceptance quality, meaning actual gains may vary in practice.

reddit · r/LocalLLaMA · /u/BringTea_666 · Jul 3, 09:19

**Background**: Speculative decoding speeds up LLM inference by using a smaller draft model to predict multiple tokens, which are then verified by the larger model. Multi-Token Prediction (MTP) is an alternative approach where the model itself predicts multiple tokens per step without a separate draft model. DSpark improves upon these methods by optimizing the drafting and verification process.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf">DeepSpec/DSpark_paper.pdf at main · deepseek-ai/DeepSpec</a></li>
<li><a href="https://www.techtimes.com/articles/319236/20260628/deepseek-releases-dspark-speculative-decoding-makes-v4-85-percent-faster.htm">DeepSeek Releases DSpark: Speculative Decoding Makes V4 Up to ...</a></li>
<li><a href="https://venturebeat.com/orchestration/deepseek-open-sources-dspark-a-new-framework-to-speed-up-llm-inference-by-up-to-85">DeepSeek open sources DSpark, a new framework to speed up LLM ...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AI`, `#efficiency`, `#breakthrough`

---