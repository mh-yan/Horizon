---
layout: default
title: "Horizon Summary: 2026-11-03 (EN)"
date: 2026-11-03
lang: en
---

> From 54 items, 18 important content pieces were selected

---

1. [Astra LLM reads and writes neural network weights to boost Qwen](#item-1) ⭐️ 9.0/10
2. [Subvocal's RF smart glasses decode silent speech to text](#item-2) ⭐️ 8.0/10
3. [Terry Tao Advocates 'Egoless Mathematics' in the AI Era](#item-3) ⭐️ 8.0/10
4. [Ubuntu leaves critical Linux kernel 0day RCE unpatched for nearly three weeks](#item-4) ⭐️ 8.0/10
5. [Anthropic warns it is very close to recursive self-improvement capability](#item-5) ⭐️ 8.0/10
6. [Marvell to acquire Lumentum for $115B in tech mega-deal](#item-6) ⭐️ 8.0/10
7. [Qwen Head Denies API-Only Rumors, Confirms Qwen 4.0 and 5.0 Will Stay Open Source](#item-7) ⭐️ 8.0/10
8. [Open-source sparse attention enables 10M token context on Qwen](#item-8) ⭐️ 8.0/10
9. [ISTA Releases 763B DeepSeek Coder at ~1 Bit Per Parameter via GSQ and RCO](#item-9) ⭐️ 8.0/10
10. [vLLM v0.33.0rc3: PyTorch 2.14, CUDA 13.0-only, and Many New Models](#item-10) ⭐️ 7.0/10
11. [Show HN: Interactive Voxel Map of Warsaw Built from Open Data](#item-11) ⭐️ 7.0/10
12. [Cloudflare halves DNS build delay and cuts memory use by 85%](#item-12) ⭐️ 7.0/10
13. [Oracle files to raise $20B in stock and bonds for AI buildout](#item-13) ⭐️ 7.0/10
14. [NYT and publishers sue Brave over AI content scraping](#item-14) ⭐️ 7.0/10
15. [Amazon Allegedly Cancels GPU Orders and Closes Accounts, Including Tim Sweeney's](#item-15) ⭐️ 7.0/10
16. [Local quants vs Claude benchmarked on 9 real C++/CUDA bugs](#item-16) ⭐️ 7.0/10
17. [Unsloth benchmarks DeepSeek-V4.1 GGUFs at 512K context, claims 10-20% gain over GSQ-RCO](#item-17) ⭐️ 7.0/10
18. [Uncensored DeepSeek-V4.1-Flash-1017 runs on 12GB VRAM](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Astra LLM reads and writes neural network weights to boost Qwen](https://rikiyat.github.io/blog/weight-space-programming/) ⭐️ 9.0/10

A blog post and Hacker News discussion describe Astra, a general-purpose LLM that can directly interpret and modify the weights of other neural networks without using an optimizer or gradient descent. Notably, Astra edited a small Qwen model's weights to improve its math skills by roughly 5x and traced a looping failure to specific MLP directions in layers 15 and 19. This capability suggests LLMs may have a native understanding of weight space, potentially enabling recursive self-improvement where AI systems directly edit their own or other models' weights to enhance performance. If validated, it could fundamentally change how models are fine-tuned and raise new safety concerns about AI self-modification. Astra identified that the base model looped by repeating text and rarely reached an answer (85 of its first 96 practice answers ran to the 32,768-token limit), then subtracted a specific direction from 64 output columns in each of layers 15 and 19 (131,072 weights) to fix it. The work was done without environment feedback in some cases, relying solely on the LLM's interpretation of the weights.

hackernews · dbreunig · Nov 2, 18:21 · [Discussion](https://news.ycombinator.com/item?id=50341174)

**Background**: Weight-space programming refers to a general-purpose LLM reading and writing a network's weights directly, around some natural language specification, rather than through traditional training with gradient descent. Recursive self-improvement (RSI) is a process where an AI system iteratively designs a more capable successor, potentially leading to an intelligence explosion. Qwen is a family of open-weight large language models developed by Alibaba, with architectures that include mixture-of-experts and hybrid thinking capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://rikiyat.github.io/blog/weight-space-programming/">Sparks of Weight -Space Programming: LLMs can natively read & write...</a></li>
<li><a href="https://news.ycombinator.com/item?id=50341174">Astra can read and write weights to improve Qwen | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>

</ul>
</details>

**Discussion**: Commenters expressed shock and awe at Astra's capabilities, with some calling it 'insane' and noting it can determine training games and edit weights without tooling. Others debated whether this is an emergent ability or the result of deliberate training on neural weight data for recursive self-improvement, drawing parallels to early GPT models trained on chess notation. Some raised concerns about the implications for AI safety and the nature of the achievement.

**Tags**: `#LLM`, `#weight manipulation`, `#emergent abilities`, `#recursive self-improvement`, `#AI research`

---

<a id="item-2"></a>
## [Subvocal's RF smart glasses decode silent speech to text](https://news.ycombinator.com/item?id=50340088) ⭐️ 8.0/10

The Subvocal Company (YC F26), founded by two Georgia Tech CS students, presented smart glasses that use RF sensing to decode silently mouthed or internal speech into text at speech speed. The team pivoted from EMG electrodes to RF after finding EMG impractical due to sweat, interference, and placement variability. This is a notable technical and product milestone for silent speech interfaces, potentially enabling discreet, hands-free text input in public or quiet environments and offering accessibility benefits for users who cannot speak aloud. It also sparks important debate on privacy, inference location, and form factor in wearable computing. The glasses emit radio waves similar to Bluetooth that pass through the face and are modulated by the tongue, lips, and soft palate during silent mouthing; foundation models trained on this data decode the perturbations to text. The team had to build a low-noise RF sensing stack, optimize antenna placement for maximal field overlap with articulators, and address cross-user generalization due to varying facial anatomy.

hackernews · aarushyadav · Nov 2, 17:16

**Background**: Silent speech interfaces aim to enable communication without audible vocalization by sensing articulatory or neural signals. Subvocal recognition (SVR) converts subvocalization—internal speech typically made when reading—into digital output. Prior academic work like MIT's AlterEgo used EMG electrodes on the face, but practical wearables require non-invasive sensing like RF.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Subvocal_recognition">Subvocal recognition - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/s44460-025-00010-2">Sensing technologies for silent speech interfaces - Nature</a></li>

</ul>
</details>

**Discussion**: HN commenters were largely enthusiastic, calling the tech sci-fi-like and phenomenal for accessibility, while requesting more detail on how it works and better glasses fit for non-standard nose shapes. Others raised privacy concerns about inference location and offline operation, and compared it to open-source silent speech projects like LipFlow and LipNet.

**Tags**: `#silent-speech`, `#smart-glasses`, `#RF-sensing`, `#accessibility`, `#human-computer-interaction`

---

<a id="item-3"></a>
## [Terry Tao Advocates 'Egoless Mathematics' in the AI Era](https://terrytao.wordpress.com/2026/11/02/egoless-mathematics-in-the-ai-era/) ⭐️ 8.0/10

In a blog post published on November 2, 2026, Fields Medalist Terry Tao argues that mathematicians should adopt an 'egoless' approach to research as AI increasingly solves major problems, and he calls for a 'Maths 2.0' era that prioritizes human understanding over ego-driven competition. Tao is one of the most influential mathematicians alive, and his argument could reshape how the mathematical community evaluates research, credit, and career incentives as AI tools become central to theorem proving and problem solving. The essay builds on Tao's earlier September 2026 post 'A Severe Misalignment of AI in Mathematics,' which warned that AI companies treating math problems as benchmarks harms the science, and it has sparked debate over whether prioritizing 'truth over people' neglects the human and societal dimensions of mathematical work.

hackernews · smilelamp · Nov 2, 18:54 · [Discussion](https://news.ycombinator.com/item?id=50341736)

**Background**: Large language models have recently made dramatic progress in solving outstanding mathematical problems, prompting concern among researchers about the field's future. The term 'egoless' echoes 'egoless programming,' a concept introduced by Gerald Weinberg in 1971 that encourages detaching personal ego from one's work to enable collaboration and error detection. Tao's proposal extends this idea to mathematics, suggesting researchers should focus on collective understanding rather than personal credit.

<details><summary>References</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2026/11/02/egoless-mathematics-in-the-ai-era/">Egoless Mathematics in the AI Era | What's new</a></li>
<li><a href="https://terrytao.wordpress.com/2026/09/11/a-severe-misalignment-of-ai-in-mathematics/">A Severe Misalignment of AI in Mathematics | What's new</a></li>
<li><a href="https://grokipedia.com/page/egoless_programming">Egoless programming</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News offered diverse and critical perspectives: some argued that human pursuits cannot be separated from the humans who pursue them and that 'egoless' claims often mask a different kind of ego, while others worried the essay implies 'people don't matter; all that matters is truth' and feared for the future of mathematics if that view prevails. Several commenters also emphasized the societal value of mathematical work and questioned what will happen to the mathematical profession as AI advances.

**Tags**: `#mathematics`, `#AI`, `#research-culture`, `#philosophy`, `#academia`

---

<a id="item-4"></a>
## [Ubuntu leaves critical Linux kernel 0day RCE unpatched for nearly three weeks](https://freenode.net/article/ubuntu-lts-kernels-still-unfixed-for-critical-cve-2026-98432) ⭐️ 8.0/10

Ubuntu has not released a patch for CVE-2026-98432, a critical Linux kernel remote code execution vulnerability, for almost three weeks, despite the flaw being rated 9.8 on the CVSS scale by the kernel's CVE team. This delay affects many production environments running Ubuntu LTS, and the lack of a patch leaves systems exposed to a remotely exploitable flaw that could lead to full compromise. The vulnerability is a use-after-free in the Linux kernel's IPv4 networking subsystem, triggered by a race condition during TCP connection request processing; Red Hat has published a mitigation that it says reduces but does not fully prevent exposure.

hackernews · majorchord · Nov 2, 18:39 · [Discussion](https://news.ycombinator.com/item?id=50341462)

**Background**: CVE-2026-98432 is a critical Linux kernel vulnerability that allows a remote, unauthenticated attacker to execute arbitrary code. It was discovered with the help of Anthropic's AI research and affects multiple Linux distributions, including Ubuntu and Red Hat Enterprise Linux. Ubuntu LTS is a long-term support release widely used in servers and production systems.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/10/linux-kernel-tcp-flaw-with-98-cvss.html">Linux Kernel TCP Flaw With 9.8 CVSS Score Affects Ubuntu, Red ...</a></li>
<li><a href="https://access.redhat.com/security/vulnerabilities/RHSB-2026-016">RHSB-2026-016 Use-after-free - kernel IPv4 (CVE-2026-98432 ...</a></li>
<li><a href="https://securityboulevard.com/2026/11/linux-kernel-tcp-flaw-rated-9-8-gets-a-remote-root-exploit-from-an-ai-model/">Linux Kernel TCP Flaw Rated 9.8 Gets a Remote-Root Exploit ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration over Ubuntu's lack of communication and patch, with some suggesting iptables/nftables mitigations and others questioning why the delay occurred. Concerns were also raised about the broader issue of unpatched Linux kernels in consumer routers and the potential for AI-assisted exploitation.

**Tags**: `#linux`, `#security`, `#ubuntu`, `#cve`, `#kernel`

---

<a id="item-5"></a>
## [Anthropic warns it is very close to recursive self-improvement capability](https://techcrunch.com/2026/11/02/anthropic-warns-that-its-very-close-to-rsi-capability-aka-self-building-ai/) ⭐️ 8.0/10

Anthropic has issued a warning that it is very close to achieving recursive self-improvement (RSI), the point at which AI becomes so good at training itself that it triggers a dramatic acceleration in AI capabilities. The company framed this as a major safety concern, noting that RSI represents a potential point of no return. This warning from a leading AI lab signals that RSI—long discussed as a theoretical threshold—may be approaching in practice, with major implications for AI safety, governance, and existential risk. It could intensify calls for regulation and change how labs approach model development and deployment. The announcement provides few technical specifics, but RSI is defined as the point where AI systems can iteratively design more capable successors, potentially leading to an intelligence explosion. As of 2026, AI companies increasingly use AI for coding and research, though human work remains a bottleneck in some areas.

rss · TechCrunch · Nov 2, 22:14

**Background**: Recursive self-improvement (RSI) refers to a process where an AI system iteratively designs a more capable successor, potentially triggering an intelligence explosion and the creation of artificial superintelligence. AI doomers view RSI as a catastrophic risk from which there is no return, while recent research suggests RSI may take longer to arrive than some forecasts predict. Anthropic is an AI safety and research company that has publicly emphasized the importance of building reliable, interpretable, and steerable AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://www.anthropic.com/news/core-views-on-ai-safety">Anthropic's core views on AI safety</a></li>
<li><a href="https://www.technologyreview.com/2026/08/18/1142188/ai-recursive-self-improvement/">AI’s recursive self-improvement might not come so quickly ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#recursive self-improvement`, `#Anthropic`, `#AI capabilities`, `#existential risk`

---

<a id="item-6"></a>
## [Marvell to acquire Lumentum for $115B in tech mega-deal](https://techcrunch.com/2026/11/02/in-one-of-the-largest-deals-in-tech-history-marvell-buys-lumentum-for-115b/) ⭐️ 8.0/10

Marvell Technology has announced plans to acquire optical component maker Lumentum Holdings for $115 billion, one of the largest acquisitions in tech history. Both companies share Nvidia as a strategic investor, with Nvidia having previously invested $2 billion in Marvell to bolster its optical networking portfolio. The deal would create a semiconductor and optics powerhouse positioned to lead in AI connectivity, spanning chips to data centers, and could reshape the competitive landscape for AI infrastructure suppliers. It also deepens Nvidia's influence over the AI hardware supply chain through its shared stake in both companies. Lumentum is a leading supplier of advanced optical components, including 200G-per-lane electro-absorption modulated lasers (EMLs) used to shuttle massive amounts of data at high speeds. The $115 billion price tag makes this one of the largest tech acquisitions ever, though the deal likely faces regulatory scrutiny given the concentration of AI hardware assets.

rss · TechCrunch · Nov 2, 17:54

**Background**: Marvell is a semiconductor company that designs chips for data infrastructure, while Lumentum makes optical and photonic products such as lasers and optical components that enable high-speed data transmission. As AI workloads explode, demand has surged for optical interconnects that move data between chips and data centers. Nvidia, the dominant AI chip maker, has been investing in optical component suppliers like Lumentum, Coherent, and Marvell to secure control over the broader AI hardware ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/02/in-one-of-the-largest-deals-in-tech-history-marvell-buys-lumentum-for-115b/">In one of the largest deals in tech history, Marvell buys Lumentum for...</a></li>
<li><a href="https://au.investing.com/news/swot-analysis/lumentum-holdingss-swot-analysis-optical-stock-rides-ai-wave-93CH-4453832">Lumentum Holdings ’s SWOT analysis: optical stock rides AI wave By...</a></li>
<li><a href="https://www.fool.com/investing/2026/06/05/the-hidden-nvidia-trade-nobody-on-wall-street-is-t/">The Hidden Nvidia Trade Nobody on Wall Street Is... | The Motley Fool</a></li>

</ul>
</details>

**Tags**: `#acquisitions`, `#semiconductors`, `#Nvidia`, `#Marvell`, `#Lumentum`

---

<a id="item-7"></a>
## [Qwen Head Denies API-Only Rumors, Confirms Qwen 4.0 and 5.0 Will Stay Open Source](https://www.reddit.com/r/LocalLLaMA/comments/1xm28e6/official_statement_qwen_models_will_stick_to_open/) ⭐️ 8.0/10

Qwen Head Liu Dayi Heng officially stated that future Qwen 4.0 and Qwen 5.0 models will continue to be open source, directly refuting recent rumors that Qwen 4 would be the last open-weight series and that subsequent releases would be API-only. This commitment reassures developers and researchers who rely on Qwen's open-weight models for customization and local deployment, and it reinforces Qwen's position as a leading open-source AI provider amid industry uncertainty about open vs. closed strategies. Liu emphasized that AI's value should not belong to a few but should be a foundational capability accessible to users worldwide, and noted that Qwen has surpassed 3 billion cumulative global downloads, released over 460 open-source models, and spawned more than 300,000 derivative models, holding the top spot globally.

reddit · r/LocalLLaMA · /u/ResearchCrafty1804 · Nov 2, 16:42

**Background**: Qwen is Alibaba's family of large language models, which includes both open-weight models that can be downloaded and run locally, and proprietary models like Qwen 3-Max that are only available via API. Open-weight models publish the model weights but may not include training data or code, which is a key distinction from fully open-source AI. The rumor suggested a shift toward an API-only approach, which would limit community access and innovation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://bestllmfor.com/guides/open-weight-vs-open-source-llm/">Open - Weight vs Open - Source LLMs: What You Can Do | BestLLMfor</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#LLM`, `#Qwen`, `#AI policy`, `#model releases`

---

<a id="item-8"></a>
## [Open-source sparse attention enables 10M token context on Qwen](https://www.reddit.com/r/LocalLLaMA/comments/1xmbj0v/new_sparse_attention_method_for_ultralong_context/) ⭐️ 8.0/10

A research team released an open-source sparse attention method that sparsifies the attention of Qwen 3.8 27B without observed accuracy loss, extends context up to 10M tokens, and allows native sparse training on next-token prediction loss alone, achieving the same validation loss as full attention but faster. This work makes ultra-long context more affordable on local hardware by reducing the quadratic cost of attention, and its full open-source release (kernels, SGLang integration, paper) lowers the barrier for the community to adopt and build upon sparse attention for small open-weight models. While most tasks like NIAH remain fine at 10M tokens, accuracy degrades on some specific tasks; the team is focusing on H200/B300 GPUs and larger-scale systems, but the method is applicable to small open-weight models.

reddit · r/LocalLLaMA · /u/Immediate_Sky_6566 · Nov 2, 22:24

**Background**: Self-attention in Transformer-based large language models has quadratic time and memory complexity, which is a fundamental obstacle to efficient long-context modeling. Sparse attention is a class of efficient attention mechanisms that reduces this cost by having each token attend to only a subset of other tokens. Qwen 3.8 27B is a recent open-weight model from Alibaba's Qwen team, and NIAH (Needle in a Haystack) is a benchmark that tests long-context retrieval by hiding a 'needle' fact in a long 'haystack' of text.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2507.19595">Efficient Attention Mechanisms for Large Language Models: A ...</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://github.com/gkamradt/needle-in-a-haystack">GitHub - gkamradt/ needle - in - a - haystack : Doing simple retrieval from...</a></li>

</ul>
</details>

**Tags**: `#sparse-attention`, `#long-context`, `#LLM`, `#open-source`, `#Qwen`

---

<a id="item-9"></a>
## [ISTA Releases 763B DeepSeek Coder at ~1 Bit Per Parameter via GSQ and RCO](https://www.reddit.com/r/LocalLLaMA/comments/1xlys6k/release_ista_deepseekv41flash1017_gsqrco_coder_a/) ⭐️ 8.0/10

The ISTA Deep Algorithms and Systems Lab released a Coder build of DeepSeek-V4.1-Flash-1017 compressed with GSQ and RCO, pruning half of the routed experts (192 of 384 per layer) to achieve 72.1 GB of transformer weights, or about 1.05 bits per original parameter. The model retains 98.7% on LiveCodeBench v6 and 94.8% on SWE-bench Verified compared to the base model. This demonstrates that a 763B-parameter sparse MoE model can be compressed to roughly 1 bit per original parameter while maintaining strong coding performance, making large-model local inference far more feasible. It also showcases a novel combination of learned scalar quantization and constrained optimization for expert selection, which could influence future compression research. No individual weight is stored below 1 bit; the 280.1B kept parameters average 2.06 bits, and the removed experts count as zero bits. The shared Engram file (110.6 GB) and vision projector are identical to the unpruned release, and the GGUF runs in llama.cpp b11870 or newer and in Strata.

reddit · r/LocalLLaMA · /u/Loginhe · Nov 2, 14:33

**Background**: DeepSeek-V4.1-Flash-1017 is a sparse mixture-of-experts (MoE) model with 384 routed experts per layer, of which 6 are active per token, totaling 763.2B parameters. GSQ (Gumbel-Softmax Quantization) is a post-training scalar quantization method that jointly learns grid assignments and group scales, while RCO (Riemannian Constrained Optimization) enforces exact budgets via gradient descent on the task loss. Expert pruning removes low-importance experts to reduce memory and compute, and here RCO selects which experts to keep under a per-layer budget.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/IST-DASLab/GSQ">IST-DASLab/ GSQ : Gumbel - Softmax post - training quantization for...</a></li>
<li><a href="https://arxiv.org/html/2604.18556">GSQ : Highly-Accurate Low-Precision Scalar Quantization for LLMs...</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gsq-rco-quantization">What Are GSQ and RCO? Das Lab's New LLM Quantization Method</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#mixture-of-experts`, `#model-compression`, `#local-llm`, `#deepseek`

---

<a id="item-10"></a>
## [vLLM v0.33.0rc3: PyTorch 2.14, CUDA 13.0-only, and Many New Models](https://github.com/vllm-project/vllm/releases/tag/v0.33.0rc3) ⭐️ 7.0/10

vLLM released v0.33.0rc3, a large release candidate with 927 commits from 389 contributors, adding numerous new models such as Reflection Beam-1.0, Yandex AliceAI-Foundation-80B-A3B, and Step-5 Preview, while upgrading to PyTorch 2.14.0 and dropping CUDA 12.9 in favor of CUDA 13.0-only artifacts. As one of the most widely used open-source LLM inference engines, vLLM's move to PyTorch 2.14 and CUDA 13.0-only artifacts signals a broader ecosystem shift that will affect anyone deploying models on NVIDIA GPUs, while the many new model integrations expand out-of-the-box support for cutting-edge architectures. The release also introduces an AWS EFA image for multi-node serving, a shorter `vllm/vllm` image alias, speculative decoding improvements like the XPress refiner and FLy lossy verification, and ROCm 10.0 as the default AMD image; breaking changes include removal of Medusa and the MLP speculator, and requests during paused generation now return HTTP 503.

github · khluu · Nov 2, 10:10

**Background**: vLLM is a high-throughput, memory-efficient inference and serving engine for large language models, originally developed at UC Berkeley's Sky Computing Lab and now maintained by a large open-source community. It relies on PyTorch for tensor computation and CUDA for NVIDIA GPU acceleration, so major version bumps in these dependencies require coordinated releases. Release candidates like v0.33.0rc3 are pre-release builds meant for testing before a final stable version.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm-project/vllm: A high-throughput and memory ...</a></li>
<li><a href="https://vllm.ai/">vLLM — Fast, Memory-Efficient LLM Inference & Serving</a></li>
<li><a href="https://github.com/vllm-project/vllm/issues/26946">[RFC]: Enable libtorch - ABI - stable vLLM cuda wheels · Issue #26946...</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#llm-inference`, `#release`, `#pytorch`, `#cuda`

---

<a id="item-11"></a>
## [Show HN: Interactive Voxel Map of Warsaw Built from Open Data](https://p.migdal.pl/warsaw-vibe-voxel/) ⭐️ 7.0/10

A developer has released an open-source interactive 3D voxel map of central Warsaw, built from OpenStreetMap, Polish Geoportal LiDAR and aerial imagery, and the city's tree database. The map allows users to change date, time, and weather, and even click on pedestrians to control them. This project demonstrates how multiple open geospatial datasets can be combined into an engaging, game-like visualization, lowering the barrier for public exploration of urban data. It also highlights the potential of open data for creative applications and sparks discussion on data accuracy and performance. The map is built with voxel graphics inspired by Minecraft and MagicaVoxel, and works best on desktop but is usable on mobile. Initial load can be slow, and some areas like the Old Town are inaccurately represented due to data limitations.

hackernews · stared · Nov 2, 16:25 · [Discussion](https://news.ycombinator.com/item?id=50339221)

**Background**: Voxels are 3D pixels used in games and geographic information systems to represent volumetric data. OpenStreetMap provides crowd-sourced map data, while LiDAR (Light Detection and Ranging) uses laser pulses to measure building heights and terrain. Poland's Geoportal offers official spatial data, including LiDAR and aerial imagery, which the developer used to extrude buildings and color the scene.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voxel_graphics">Voxel graphics</a></li>
<li><a href="https://www.gov.pl/web/gugik-en/geoportal">Geoportal - Head Office of Geodesy and Cartography (GUGiK ...</a></li>
<li><a href="https://arxiv.org/html/2408.00967v1">Extracting Object Heights From LiDAR & Aerial Imagery</a></li>

</ul>
</details>

**Discussion**: Commenters praised the concept but reported performance issues, such as sub-1 FPS on Firefox/Linux and mobile reloads. Others criticized data accuracy, noting that landmarks like the Old Town and Plac Zamkowy are poorly represented, with wrong colors and exaggerated building heights.

**Tags**: `#3D visualization`, `#open data`, `#voxel graphics`, `#geospatial`, `#Show HN`

---

<a id="item-12"></a>
## [Cloudflare halves DNS build delay and cuts memory use by 85%](https://blog.cloudflare.com/dns-targeted-zone-builds/) ⭐️ 7.0/10

Cloudflare detailed a new approach called targeted DNS zone builds that reduced the time to build DNS zones by 50% and cut memory usage by 85% compared to the previous method. This optimization improves the efficiency and scalability of Cloudflare's authoritative DNS service, which handles a massive number of domains, and could inspire similar memory-saving techniques in other high-scale systems. The blog post explains that targeted builds avoid rebuilding entire zones by only updating the necessary records, but the community discussion raises questions about the actual throughput (e.g., 700 changes per second) and potential bugs introduced by the relational approach.

hackernews · wondersky · Nov 2, 14:47 · [Discussion](https://news.ycombinator.com/item?id=50337558)

**Background**: DNS zones are collections of DNS records for a domain, and building them involves compiling and loading these records into memory for serving queries. Cloudflare operates a large authoritative DNS service, so even small improvements in build time and memory usage can have significant operational benefits.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/improving-the-resiliency-of-our-infrastructure-dns-zone/">Improving the Resiliency of Our Infrastructure DNS ... | Cloudflare Blog</a></li>

</ul>
</details>

**Discussion**: Commenters praised Cloudflare's technical blog series but questioned whether 700 changes per second is low for their scale, and expressed curiosity about the ROI of memory optimization and potential bugs from the new approach.

**Tags**: `#DNS`, `#performance optimization`, `#memory efficiency`, `#Cloudflare`, `#systems engineering`

---

<a id="item-13"></a>
## [Oracle files to raise $20B in stock and bonds for AI buildout](https://www.cnbc.com/2026/11/02/oracle-files-to-sell-20-billion-in-new-stock-bonds-to-finance-ai-buildout.html) ⭐️ 7.0/10

Oracle has filed to sell $20 billion in new stock and bonds to finance its AI data center buildout, according to a CNBC report. The move is part of Oracle's broader effort to fund the compute infrastructure for a reported $300 billion, five-year OpenAI contract. This financing highlights the massive capital requirements of the AI infrastructure boom and raises concerns about debt risk, shareholder dilution, and the sustainability of AI capital expenditures. It could affect Oracle's balance sheet, its shareholders, and the broader AI supply chain. About half of the $20 billion is expected to be equity, implying roughly 2.5% dilution at the current market cap, while the stock has already fallen 8% on the news. Oracle is also reportedly cutting costs in its ERP business and has faced scrutiny over its use of force majeure on a data center lease.

hackernews · smartmic · Nov 2, 19:27 · [Discussion](https://news.ycombinator.com/item?id=50342284)

**Background**: Oracle is a legacy enterprise software and cloud company that has recently pivoted aggressively into AI infrastructure, building data centers to host GPUs for AI workloads. The AI buildout requires enormous upfront capital, often financed through debt or equity, and the rapid pace of GPU advancement means hardware can become economically obsolete before it is fully paid off. Investors are increasingly questioning whether the returns from AI compute will justify the soaring capital expenditures across the industry.

<details><summary>References</summary>
<ul>
<li><a href="https://toptechnews.net/articles/stargate-gpu-obsolescence-trap-oracle-openai-2026.html">The GPU Obsolescence Trap: How Nvidia's Annual Upgrade ...</a></li>
<li><a href="https://www.fitchratings.com/research/corporate-finance/weaker-ai-pricing-power-undermines-capex-sustainability-15-09-2026">Weaker AI Pricing Power Undermines Capex Sustainability</a></li>
<li><a href="https://abhs.in/blog/oracle-layoffs-30000-6am-cold-email-ai-data-center-debt-2026">Oracle Fires 30,000 at 6 AM to Pay for Its $156B AI Data Center ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism and concern, with some hoping Oracle defaults on its debt and others warning that Oracle provides commodity services to OpenAI with no proprietary IP, making it vulnerable to GPU obsolescence. Others noted the dilution impact and criticized the leadership's risk-taking, while some made sarcastic remarks about Larry Ellison's wealth.

**Tags**: `#AI infrastructure`, `#Oracle`, `#finance`, `#data centers`, `#AI capex`

---

<a id="item-14"></a>
## [NYT and publishers sue Brave over AI content scraping](https://techcrunch.com/2026/11/02/new-york-times-and-other-outlets-sue-web-browser-brave-over-alleged-content-scraping/) ⭐️ 7.0/10

The New York Times, New York Daily News, Chicago Tribune, and Orlando Sentinel have filed lawsuits against Brave Software, alleging the browser maker scraped their copyrighted content to build an index sold to AI companies including Anthropic, Perplexity, Mistral, xAI, and Cohere, while also helping users bypass paywalls. This case could set a precedent for whether browser makers and data brokers can profit from scraping publishers' content for AI training, potentially reshaping the legal and financial landscape for AI data acquisition and web publishing. The complaint alleges Brave provides paid access to its Brave Index and has given 'stolen copyrighted content' to many AI companies; Brave's privacy-focused model and paywall-bypassing features are central to the claims.

rss · TechCrunch · Nov 2, 19:19

**Background**: Brave is a privacy-focused web browser that blocks ads and trackers by default. It also operates a search index and has recently positioned itself as a source of data for AI companies. The lawsuit is part of a broader wave of copyright litigation by publishers against AI firms over the use of their content to train large language models.

<details><summary>References</summary>
<ul>
<li><a href="https://letsdatascience.com/news/new-york-times-and-publishers-sue-brave-over-ai-scraping-and-b4d8d347">New York Times and Publishers Sue Brave Over AI Scraping and ...</a></li>
<li><a href="https://aidailypost.com/news/nyt-other-publications-sue-brave">NYT Sues Brave Over AI Training Data Scraping</a></li>
<li><a href="https://www.techbuzz.ai/articles/new-york-times-sues-brave-browser-over-ai-scraping">New York Times Sues Brave Browser Over AI Scraping</a></li>

</ul>
</details>

**Tags**: `#copyright`, `#web-scraping`, `#AI-training-data`, `#legal`, `#Brave`

---

<a id="item-15"></a>
## [Amazon Allegedly Cancels GPU Orders and Closes Accounts, Including Tim Sweeney's](https://www.reddit.com/r/LocalLLaMA/comments/1xm8o8g/amazon_is_allegedly_canceling_gpu_orders_and_in/) ⭐️ 7.0/10

Amazon is reportedly canceling orders for compute hardware, including GPUs, and in rare cases closing customer accounts, with Epic Games CEO Tim Sweeney and AI educator Nick Saraev among those affected. Saraev's account was allegedly closed after his Nvidia GPU order was canceled. The allegations raise concerns about trust and transparency in cloud and hardware procurement, especially as AI-driven demand strains GPU supply. If verified, such practices could push developers and researchers toward alternative vendors or on-premises solutions to avoid vendor lock-in and sudden loss of compute access. The reports remain unverified allegations, and some coverage suggests the cancellations may reflect order verification issues rather than a confirmed Amazon policy change. The exact criteria for order cancellation or account closure have not been disclosed.

reddit · r/LocalLLaMA · /u/chemist_slime · Nov 2, 20:33

**Background**: Amazon Web Services (AWS) is a major cloud provider offering Elastic Compute Cloud (EC2) instances, and customers can purchase compute capacity through various options such as on-demand, reserved, and spot instances. Separately, Amazon sells hardware components, and reports of canceled GPU orders come amid broader anxiety over AI compute demand and supply shortages. Tim Sweeney is the CEO of Epic Games, known for Fortnite and the Epic Games Store.

<details><summary>References</summary>
<ul>
<li><a href="https://wccftech.com/amazon-allegedly-canceling-gpu-orders-closing-accounts-compute-hardware-tim-sweeney/">Amazon Is Allegedly Canceling GPU Orders And, In Rare Cases ...</a></li>
<li><a href="https://startupfortune.com/amazon-cancels-gpu-orders-and-locks-out-buyers-including-tim-sweeney/">Amazon cancels GPU orders and locks out buyers including Tim ...</a></li>
<li><a href="https://fyinternational.net/news/2026-11-02-amazon-gpu-order-verification/">Amazon GPU Cancellation Reports Put Order Verification in ...</a></li>

</ul>
</details>

**Tags**: `#cloud-computing`, `#gpu-hardware`, `#amazon-aws`, `#ai-infrastructure`, `#vendor-policy`

---

<a id="item-16"></a>
## [Local quants vs Claude benchmarked on 9 real C++/CUDA bugs](https://www.reddit.com/r/LocalLLaMA/comments/1xlwpqv/not_another_toks_post_local_quants_vs_claude_on_9/) ⭐️ 7.0/10

A LocalLLaMA author benchmarked local quantized models (Qwen3.8-Flash-Next and Qwen3.8-27B in NVFP4 and 3-bit) against Claude Opus 5.5, Sonnet 5.5, Haiku 5.5 and older Claude models on nine previously private C++/CUDA bug-fixing tasks from his own capy-flash inference engine. Claude Opus 5.5 scored highest at 0.74, while the best local model, Qwen3.8-Flash-Next NVFP4, reached 0.50, and the study found that 3-bit quantization hurt mainly through longer reasoning (40% more tokens) rather than lower scores. This benchmark moves beyond tokens-per-second metrics to measure whether local quantized models can actually find and fix real, non-public bugs, which is what matters for practical coding-agent use. It suggests that aggressive quantization may be nearly free in accuracy but costly in reasoning time, a trade-off that tok/s comparisons hide. The agent ran sandboxed on a Mac with no network or CUDA toolchain, so it had to reason from code alone with an 80-step limit and 3 runs per task; scoring combined an automatic hidden-key check with a blind Claude Opus 5.5 judge (r = 0.79), and confidence intervals are wide at about ±0.2, meaning models within ~0.1 are a coin flip. The 3-bit 27B decoded faster (153 vs 132 tok/s) but needed 18 minutes per task versus 13 for NVFP4, and non-compiling patches were capped at 0.25.

reddit · r/LocalLLaMA · /u/FeydRowan · Nov 2, 13:08

**Background**: Quantization reduces a model's numerical precision (e.g., to 4-bit or 3-bit) to shrink memory use and speed up inference on consumer hardware, but it can degrade quality. Mixture-of-Experts (MoE) models like Qwen3.8-Flash-Next activate only a subset of parameters per token, and 'expert skipping' techniques further reduce compute by deactivating less useful experts. The author's capy-flash is a custom two-GPU inference engine for running these Qwen models locally.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ValerioDolci/capy-flash">GitHub - ValerioDolci/ capy - flash : Qwen3.8-Flash-Next...</a></li>
<li><a href="https://localllm.in/blog/quantization-explained">The Complete Guide to LLM Quantization - localllm.in</a></li>
<li><a href="https://arxiv.org/abs/2609.05228">[2609.05228] ACE: Adaptive Calibration-Free Expert Skipping ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#quantization`, `#benchmarking`, `#code-generation`, `#cuda`

---

<a id="item-17"></a>
## [Unsloth benchmarks DeepSeek-V4.1 GGUFs at 512K context, claims 10-20% gain over GSQ-RCO](https://www.reddit.com/r/LocalLLaMA/comments/1xm102d/unsloth_vs_gsqrco_512k_context_deepseekv41_gguf/) ⭐️ 7.0/10

Unsloth released new benchmarks for its DeepSeek UD 3.1 GGUFs, running agentic tasks like DeepSWE, Terminal Bench, and Automation Bench at 512K context and general tasks at 128K, and claims its quantizations outperform GSQ-RCO by more than 10-20%. The team also increased benchmarking tokens from 1.3B to 35.1B (27x more data) and used improved graders including Math Verify and official Terminal Bench (Harbor) graders. This is a substantive, methodologically rigorous benchmark comparison from a well-known quantization team, and the claimed 10-20% advantage at long context could influence which GGUF quantization local LLM practitioners choose for running DeepSeek-V4.1 on their own hardware. It also directly challenges GSQ-RCO's advertised recovery rates with statistical tests, raising the bar for how quantization quality claims are validated. Unsloth reports that GSQ-RCO IQ1_M's claimed 98.7% recovery measured only 97.24% [96.23, 98.21] with p=0.0013, and IQ2_XXS's claimed 99.80% recovery measured 98.38% [97.52, 99.22] with p=0.0001, while IQ2_XS's 100% claim could not be rejected (p=0.21). For Terminal Bench 2.1, 7 of 89 tasks were excluded because they could not pass on Unsloth's infrastructure, and the results are vendor self-reported.

reddit · r/LocalLLaMA · /u/danielhanchen · Nov 2, 15:57

**Background**: GGUF is a file format for running quantized LLMs locally, and quantization compresses model weights to lower precision so large models fit on consumer hardware. Unsloth's Dynamic (UD) quants selectively allocate bits to sensitive layers, while GSQ-RCO is a newer method from ISTA's Das Lab that combines per-weight Gumbel-Softmax rounding (GSQ) with a global bit-budget allocator (RCO). Terminal Bench is an agentic benchmark that grades whether an AI agent leaves a live terminal environment in the correct final state, rather than just checking a single answer.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/basics/dynamic-3.0-ggufs">Unsloth Dynamic 3.0 GGUFs | Unsloth Documentation</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gsq-rco-quantization">What Are GSQ and RCO? Das Lab's New LLM Quantization Method</a></li>
<li><a href="https://www.tbench.ai/">TERMINAL - BENCH</a></li>

</ul>
</details>

**Tags**: `#llm-quantization`, `#gguf`, `#benchmarking`, `#local-llm`, `#deepseek`

---

<a id="item-18"></a>
## [Uncensored DeepSeek-V4.1-Flash-1017 runs on 12GB VRAM](https://www.reddit.com/r/LocalLLaMA/comments/1xm0uy0/running_uncensored_deepseekv41flash1017_on_a_12/) ⭐️ 7.0/10

A Reddit user (gladkos from the Atomic.Chat Local AI team) released abliterated GSQ-quantized shards of DeepSeek-V4.1-Flash-1017 that reduce refusals from ~85% to 0% on JailbreakBench while preserving benchmark performance. The modified files only touch 82 dense tensors per file and keep the 384 routed experts byte-for-byte identical to ISTA-DASLab's originals, allowing users to swap shards and keep using ISTA's Engram file. This enables uncensored local inference of a large MoE model on modest consumer hardware (12GB GPU plus 64GB RAM and SSD), which is valuable for the LocalLLaMA community interested in running unrestricted models locally. It also demonstrates a surgical abliteration approach that preserves quantized expert weights, potentially making refusal removal more accessible and less damaging to model capabilities. The release offers three quantization sizes (IQ1_M, IQ2_XXS, IQ2_XS) with refusals dropping to 0% for IQ1_M and IQ2_XXS, while IQ2_XS still refuses on 2 of 30 thinking prompts; MMLU-500 scores remain around 80-83% and KL divergence vs stock is 0.021-0.027. GPQA-Diamond and AIME25 on IQ2_XXS show no degradation (83.3% vs 83.3% and 80.0% vs 76.7%), but testing was limited to 8K context on a rented GPU and long-context/speed on a 12GB card is unverified.

reddit · r/LocalLLaMA · /u/gladkos · Nov 2, 15:52

**Background**: Abliteration is a technique that removes refusal behavior from aligned LLMs by projecting out a specific activation direction in weight space, without retraining. GSQ (Gumbel-Softmax quantization) is a post-training quantization method from ISTA-DASLab that produces mixed-precision GGUF files, and the Engram table is an auxiliary component used by the Strata inference engine to run large Mixture-of-Experts models by offloading parts to SSD. Strata is an open-source C++/CUDA engine that splits a model across GPU VRAM, host RAM, and NVMe storage, enabling models like DeepSeek-V4.1-Flash-1017 (197B parameters) to run on consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/abliteration">Abliteration in LLMs: Removing Refusal Behavior</a></li>
<li><a href="https://github.com/IST-DASLab/GSQ">IST- DASLab / GSQ : Gumbel-Softmax post-training quantization for...</a></li>
<li><a href="https://github.com/ro99/strata">GitHub - ro99/strata: C/C++ MoE inference engine for models ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#quantization`, `#abliteration`, `#deepseek`, `#model-modding`

---