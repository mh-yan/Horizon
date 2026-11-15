---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 35 items, 14 important content pieces were selected

---

1. [SpaceX catches Starship booster for first time on Flight 15](#item-1) ⭐️ 9.0/10
2. [Lovable apps leak passport data and 200K messages due to missing RLS](#item-2) ⭐️ 8.0/10
3. [EFF Warns Tech Companies Are Redefining Privacy Again](#item-3) ⭐️ 8.0/10
4. [Asian Governments React to Nvidia CEO Jensen Huang's Exit](#item-4) ⭐️ 8.0/10
5. [tandem.cpp update runs DeepSeek-V4.1 on 64GB PC with 16GB GPU, adds AMD ROCm support](#item-5) ⭐️ 8.0/10
6. [Rust+CUDA Leech lattice quantization compresses Qwen3 models to 2.7 bits per weight](#item-6) ⭐️ 8.0/10
7. [PyPI launches redesigned project pages with clearer security signals](#item-7) ⭐️ 7.0/10
8. [DeepSeek V3 Reimplemented in ~200 Lines of Pure JAX](#item-8) ⭐️ 7.0/10
9. [Google Project Zero to Disclose Vulnerabilities 90 Days After Reporting](#item-9) ⭐️ 7.0/10
10. [Practitioner argues frontier LLM gains come from harnesses, not raw intelligence](#item-10) ⭐️ 7.0/10
11. [tiny-voca: a fully open 4.5M-parameter TTS that runs 70x real-time on CPU](#item-11) ⭐️ 7.0/10
12. [IBM trains two small open models to ignore orders hidden in documents](#item-12) ⭐️ 7.0/10
13. [Nex-AGI Releases Nex-N2.6, a 321B FP8 Multimodal Agentic Model](#item-13) ⭐️ 7.0/10
14. [SenseNova-Loop-9B-Preview: 9B model reportedly matches Qwen 3.5 27B](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [SpaceX catches Starship booster for first time on Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 9.0/10

On November 13, 2026, SpaceX launched Starship Flight 15 from Starbase and successfully caught the Super Heavy booster with the launch tower's chopstick arms, while the upper stage achieved the first successful upright landing after reaching orbit. This milestone demonstrates full reusability of both stages, a paradigm shift that could dramatically lower launch costs and increase flight frequency, impacting the entire space industry and NASA's Artemis lunar plans. The mission used the Block 3 Starship and was the second operational flight; the booster catch was performed by the Pad 2 tower arms, and the upper stage landing marks the first time a Starship upper stage has landed upright after orbital flight.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**Background**: Starship is SpaceX's fully reusable super-heavy-lift rocket, consisting of the Super Heavy booster and the Starship upper stage. The company aims to achieve rapid reusability by catching both stages with the launch tower's arms, similar to the approach first demonstrated with the Falcon 9 booster landings. Flight 15 follows a series of tests, including Flight 14 which deployed Starlink satellites, and represents a key step toward operational reusability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starship_flight_15">Starship flight 15 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship_flight_tests">SpaceX Starship flight tests</a></li>
<li><a href="https://www.nytimes.com/2026/11/13/science/spacex-launch-starship-rocket-catch.html">SpaceX’s Latest Starship Launch Skips Attempt to Catch the Booster</a></li>

</ul>
</details>

**Discussion**: Commenters celebrated the achievement as a historic milestone, with comparisons to the Space Shuttle highlighting Starship's safer design and assembly-line production. Some noted that full reusability could make spaceflight significantly cheaper, while others discussed technical details like mass fraction and the potential for catching both stages in future flights.

**Tags**: `#SpaceX`, `#Starship`, `#reusable rockets`, `#aerospace engineering`, `#spaceflight`

---

<a id="item-2"></a>
## [Lovable apps leak passport data and 200K messages due to missing RLS](https://www.crissyfield.de/research/lovable-en/) ⭐️ 8.0/10

Security research published by Crissy Field reveals that apps built with Lovable, an AI app builder, exposed passport details and over 200,000 private messages because Row-Level Security (RLS) was not enabled on their Supabase databases. The researcher found that these leaks could be discovered by simply inspecting network calls in the browser, requiring no sophisticated hacking. This incident highlights a systemic risk in AI-generated code: platforms can produce full-stack apps quickly, but insecure defaults can leave sensitive data publicly accessible to anyone. As AI app builders proliferate, the burden shifts to platforms to enforce secure defaults and to users to understand the security posture of what they deploy. The root cause was insufficient Row-Level Security, which Lovable's Head of Security says their automated scanning is designed to catch; Lovable scans every app before publish and offers a deeper SAST scan for free, with options to auto-fix or block publishing. However, Supabase's default behavior—where tables without RLS enabled are accessible to all authenticated users—has been a known tradeoff for easier onboarding, and reports suggest the fix may not apply to existing projects.

hackernews · armcat · Nov 14, 17:43 · [Discussion](https://news.ycombinator.com/item?id=50499017)

**Background**: Lovable is an AI-powered app builder that generates full-stack applications from natural language descriptions, often using Supabase as the backend database. Supabase is an open-source Firebase alternative built on PostgreSQL, where Row-Level Security (RLS) is a feature that restricts which rows users can access; without RLS, any authenticated user can read or write all data via the Supabase JavaScript SDK. This case illustrates how AI-generated code can inherit insecure defaults from backend platforms, leading to real-world data exposure.

<details><summary>References</summary>
<ul>
<li><a href="https://supabase.com/docs/guides/database/postgres/row-level-security">Row Level Security - Supabase Docs</a></li>
<li><a href="https://engineersuniverse.com/studios/software-engineering/row-level-security-supabase-guide">Row Level Security in Supabase: The Complete Guide to Multi ...</a></li>
<li><a href="https://lovable.dev/security">Security at Lovable | Build Apps Faster</a></li>

</ul>
</details>

**Discussion**: The discussion acknowledges Lovable's response but also points to Supabase's culpability: commenters note that Supabase deliberately chose insecure defaults years ago to ease onboarding, and a fix from October 30 may not apply to existing projects. Others emphasize that AI-generated apps are easy targets for unsophisticated attacks and that platforms need deny-by-default databases, least-privilege APIs, and automated auth tests to make insecure deployments difficult.

**Tags**: `#security`, `#AI-generated-code`, `#Supabase`, `#Row-Level-Security`, `#data-privacy`

---

<a id="item-3"></a>
## [EFF Warns Tech Companies Are Redefining Privacy Again](https://www.eff.org/deeplinks/2026/11/tech-companies-are-trying-shift-entire-concept-privacy-again) ⭐️ 8.0/10

The Electronic Frontier Foundation (EFF) published an analysis arguing that tech companies are once again attempting to shift the entire concept of privacy, likely to justify expanded data collection and AI-driven features. The piece sparked a substantial Hacker News discussion with 441 points and 167 comments. This matters because how privacy is defined shapes laws, product design, and user expectations; if companies succeed in narrowing the definition, individuals could lose control over personal data in workplaces and public spaces. The debate affects anyone using AI transcription tools, smart glasses, or workplace communication platforms. The EFF analysis is commentary rather than a technical breakthrough, and the community discussion highlights tradeoffs: accessibility benefits of live transcription for deaf and hard-of-hearing users versus the risk of always-on recording and retention. Commenters also noted the difficulty of opting out of AI notetakers in professional meetings and referenced UN Human Rights Article 12 on arbitrary interference with privacy.

hackernews · gslin · Nov 14, 12:45 · [Discussion](https://news.ycombinator.com/item?id=50496602)

**Background**: The EFF is a leading nonprofit founded in 1990 that defends civil liberties in the digital world through litigation, policy analysis, and activism. AI transcription tools, including AI notetakers in meetings and live-transcribing glasses, are increasingly common but raise privacy concerns because they can record and retain conversations. The debate often centers on whether privacy should be redefined to accommodate such technologies or whether existing rights should be preserved.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eff.org/about">About EFF | Electronic Frontier Foundation</a></li>
<li><a href="https://www.eff.org/issues/privacy">Privacy | Electronic Frontier Foundation</a></li>
<li><a href="https://basilai.app/articles/2026-03-31-ai-meeting-transcription-employee-surveillance-workplace-privacy-on-device.html">AI Meeting Transcription as Employee Surveillance: Where ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about the ubiquity of AI recording in professional meetings, with one asking how to minimize exposure when opting out is impossible without risking employment. Others highlighted the transformative potential of live transcription for accessibility and questioned whether banning such devices would also ban open-source prosthetics, while another invoked UN Human Rights Article 12 to argue that tech companies have no right to private data.

**Tags**: `#privacy`, `#surveillance`, `#AI ethics`, `#policy`, `#accessibility`

---

<a id="item-4"></a>
## [Asian Governments React to Nvidia CEO Jensen Huang's Exit](https://techcrunch.com/2026/11/14/asian-governments-react-to-nvidia-ceo-jensen-huangs-exit/) ⭐️ 8.0/10

Following Nvidia CEO Jensen Huang's resignation amid reports of extramarital affairs, Asian governments have begun responding by confirming chip supply commitments and monitoring the impact on local projects and ongoing investigations. Huang's departure from Nvidia, a linchpin in the global AI hardware supply chain, could disrupt semiconductor supply and shift competitive dynamics, affecting governments and companies across Asia that rely on Nvidia's chips for AI infrastructure. Nvidia's Asian supply chain, spanning South Korea's memory chip makers and Taiwan's advanced chipmaking hubs, is already redrawing plans in case Huang departs, while Nvidia's board met to decide on his future after reports of two extramarital affairs.

rss · TechCrunch · Nov 14, 16:34

**Background**: Nvidia is a leading designer of AI accelerators such as the H100 GPU, which powers large language models and is central to the global AI buildout. Jensen Huang co-founded the company and has been its public face, making his exit a major leadership change. Asian economies, particularly South Korea and Taiwan, are key partners in Nvidia's supply chain, so his departure raises concerns about continuity and government relations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/media-telecom/nvidias-asian-supply-chain-prepares-life-after-huang-2026-11-12/">Nvidia's Asian supply chain prepares for life after Huang</a></li>
<li><a href="https://www.nytimes.com/2026/11/12/technology/nvidia-jensen-huang.html">Jensen Huang Resigns From Nvidia After Affairs - The New York Times</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/nvidia-jensen-huang-affairs-amd-broadcom-tsmc.html">Nvidia ’s turmoil is prompting a rotation across chip stocks.</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#semiconductors`, `#AI hardware`, `#Asia`, `#tech leadership`

---

<a id="item-5"></a>
## [tandem.cpp update runs DeepSeek-V4.1 on 64GB PC with 16GB GPU, adds AMD ROCm support](https://www.reddit.com/r/LocalLLaMA/comments/1xwan2j/update_tandemcpp_deepseekv41_on_a_64_gb_pc_with_a/) ⭐️ 8.0/10

tandem.cpp, a patch set for llama.cpp that accelerates large MoE models by keeping hot experts on GPU and offloading the rest to CPU/SSD, now supports AMD GPUs via HIP/ROCm. Benchmarks show up to 2x speedup over llama.cpp on consumer hardware, e.g., 14.2 tok/s vs 7.4 tok/s on an RTX 5070 Ti with 64GB RAM. This update significantly lowers the hardware barrier for running massive MoE models like DeepSeek-V4.1-Flash (763B parameters) on consumer PCs, making local inference more accessible. The addition of AMD ROCm support broadens accessibility beyond NVIDIA, benefiting users with AMD GPUs. tandem.cpp excels when the model is much larger than VRAM+RAM combined, such as a 16GB card with 32GB RAM, achieving 34.3 tok/s vs 14.9 tok/s on llama.cpp for Qwen3.8-Flash-Next. However, Vulkan is not yet supported, and on an old 6-core CPU, AMD-specific engines like Strata and Avalon still outperform tandem.cpp.

reddit · r/LocalLLaMA · /u/smflx · Nov 14, 19:12

**Background**: Mixture-of-Experts (MoE) models like DeepSeek-V4.1-Flash have many parameters but only activate a subset (experts) per token, making them suitable for offloading. llama.cpp is a popular open-source inference engine for local LLMs, and tandem.cpp is a patch set that improves MoE offloading by dynamically keeping frequently used experts on GPU. ISTA GSQ-RCO is a quantization method from Das Lab at ISTA that reduces model size with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/Doctor-Shotgun/llamacpp-moe-offload-guide">Performant local mixture-of- experts CPU inference with GPU...</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gsq-rco-quantization">What Are GSQ and RCO ? Das Lab's New LLM Quantization Method</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4.1-Flash">deepseek-ai/DeepSeek-V4.1-Flash · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#MoE`, `#local-llm`, `#ROCm`, `#performance`

---

<a id="item-6"></a>
## [Rust+CUDA Leech lattice quantization compresses Qwen3 models to 2.7 bits per weight](https://www.reddit.com/r/LocalLLaMA/comments/1xwerbo/qwen3_4b_8b_14b_at_27_bits_per_weight_with_leech/) ⭐️ 8.0/10

An independent open-source Rust implementation of Leech Lattice Vector Quantization (LLVQ), with custom CUDA kernels, has been released for Qwen3 4B, 8B, and 14B models, achieving ~2.7 bits per parameter. The quantized models outperform llama.cpp's IQ2_S at the same bit rate on MMLU and GSM8K benchmarks, but run slower. This demonstrates that advanced lattice-based quantization can be practically implemented outside major frameworks, offering better quality at extremely low bit rates for local LLM inference. It provides an alternative for fitting larger models into limited VRAM, though speed remains a trade-off. The method encodes blocks of 24 weights into 48-bit codes using the Leech lattice, with GPTQ-style offline calibration. Quality gains over IQ2_S diminish with model size (e.g., +9.1 MMLU at 4B vs +2.9 at 14B), and decoding is significantly slower than llama.cpp (60, 64, and 34 tok/s slower for 4B, 8B, and 14B respectively).

reddit · r/LocalLLaMA · /u/Fuzzy-Layer9967 · Nov 14, 22:10

**Background**: Quantization reduces the precision of model weights to shrink memory usage and speed up inference, but lower bit rates typically degrade quality. Leech lattice quantization is a technique from a Qualcomm paper (arXiv:2603.11021) that uses a dense 24-dimensional lattice to achieve near-optimal compression. IQ2_S is a 2-bit quantization method in llama.cpp, a popular inference framework for local LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2603.11021">Leech Lattice Vector Quantization for Efficient LLM Compression</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/tools/quantize/README.md">llama.cpp/tools/quantize/README.md at master · ggml ... - GitHub</a></li>
<li><a href="https://huggingface.co/collections/Qwen/qwen3">Qwen 3 - a Qwen Collection</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#LLM inference`, `#Rust`, `#CUDA`, `#local LLMs`

---

<a id="item-7"></a>
## [PyPI launches redesigned project pages with clearer security signals](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI has completed a redesign of its project pages, now displaying security signals such as provenance attestations and trusted publishing status more prominently. The update aims to make it easier for users to verify how packages were built and published. This matters because supply chain attacks on package repositories are a growing threat, and clearer provenance signals help developers make informed trust decisions. It also pushes the ecosystem toward wider adoption of keyless signing and automated, verifiable publishing workflows. Provenance attestations are currently generated through trusted publishing on platforms like GitHub Actions, and the community notes that provenance detects compromised accounts but not malicious projects. Additionally, trusted publishing does not yet support reusable workflows, which limits some CI/CD setups.

hackernews · rbanffy · Nov 14, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50497892)

**Background**: PyPI is the official package index for Python, hosting hundreds of thousands of projects. Trusted publishing lets maintainers publish packages via short-lived OIDC tokens from CI/CD systems instead of long-lived API tokens, reducing credential leakage. Provenance attestations, often built on Sigstore-style keyless signing, cryptographically record which workflow built a package, providing transparency into the supply chain.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.pypi.org/trusted-publishers/using-a-publisher/">Publishing with a Trusted Publisher - PyPI Docs</a></li>
<li><a href="https://docs.sigstore.dev/cosign/signing/overview/">Overview - Sigstore</a></li>
<li><a href="https://www.securityscientist.net/blog/12-questions-and-answers-about-software-provenance/">12 Questions and Answers About software provenance</a></li>

</ul>
</details>

**Discussion**: Commenters welcomed the security improvements but raised concerns about centralization and lock-in to big cloud CI providers, and debated the limits of provenance—it detects compromised accounts, not malicious projects. Others expressed enthusiasm for Sigstore-style keyless signing and called for broader support, including reusable workflows in trusted publishing.

**Tags**: `#pypi`, `#supply-chain-security`, `#sigstore`, `#python`, `#provenance`

---

<a id="item-8"></a>
## [DeepSeek V3 Reimplemented in ~200 Lines of Pure JAX](https://github.com/Vaibhaav-Tiwari/deepseek-v3-jax) ⭐️ 7.0/10

A developer released a concise implementation of the DeepSeek V3 language model in approximately 200 lines of pure JAX code on GitHub. The project, shared as a Show HN, aims to provide an educational and practical resource for understanding and running the model. This project lowers the barrier to understanding and experimenting with a state-of-the-art Mixture-of-Experts model by offering a minimal, readable codebase. It also enables practical use on non-NVIDIA hardware, as evidenced by a user successfully running it on an AMD GPU via ROCm. The implementation focuses on inference and is written in pure JAX, leveraging its automatic differentiation and JIT compilation capabilities. A user reported that it ran end-to-end on an AMD RX 7600 XT 16GB GPU with ROCm, requiring specific environment variables like HSA_OVERRIDE_GFX_VERSION=11.0.0.

hackernews · VaibhaavTiwari · Nov 14, 15:04 · [Discussion](https://news.ycombinator.com/item?id=50497589)

**Background**: DeepSeek V3 is a large language model with 671 billion total parameters, using a Mixture-of-Experts architecture that activates only 37 billion parameters per token. It employs Multi-head Latent Attention (MLA) and DeepSeekMoE for efficient inference and training. JAX is a Python library for high-performance numerical computing and machine learning, known for its composable transformations and support for accelerators like GPUs and TPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JAX_(software)">JAX (software) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2412.19437">[2412.19437] DeepSeek-V3 Technical Report - arXiv.org GitHub - deepseek-ai/DeepSeek-V3 · GitHub Model Architecture Overview | deepseek-ai/DeepSeek-V3 | DeepWiki DeepSeek V3 Complete Guide: Deploy and Optimize ... - SitePoint DeepSeek-V3/inference/model.py at main - GitHub</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V3-Base">deepseek -ai/ DeepSeek - V 3 -Base · Hugging Face</a></li>

</ul>
</details>

**Discussion**: The discussion is overwhelmingly positive, with commenters praising the educational value of rebuilding a model from first principles. One user shared a practical success story of running the code on an AMD GPU with ROCm, while another asked for a roadmap to build intuition about inference for developers familiar with Java and Python.

**Tags**: `#JAX`, `#DeepSeek`, `#LLM`, `#inference`, `#Show HN`

---

<a id="item-9"></a>
## [Google Project Zero to Disclose Vulnerabilities 90 Days After Reporting](https://projectzero.google/2026/11/disclosure-policy.html) ⭐️ 7.0/10

Google Project Zero announced a new vulnerability disclosure policy starting with a 90-day deadline, which will be reduced to 60 days on February 2, 2027, and to 30 days on January 3, 2028. This policy shift significantly accelerates the timeline for public disclosure of zero-day vulnerabilities, pressuring vendors to patch faster and potentially reshaping industry norms for coordinated disclosure. The policy applies to vulnerabilities reported by Project Zero to vendors, with the 90-day deadline starting immediately and the 60-day and 30-day deadlines taking effect on specific dates in 2027 and 2028.

hackernews · hacb · Nov 14, 11:13 · [Discussion](https://news.ycombinator.com/item?id=50496051)

**Background**: Project Zero is a team of security analysts at Google that finds zero-day vulnerabilities in widely used software. Since its founding in 2014, it has used a 90-day disclosure deadline to encourage vendors to fix flaws promptly. Vulnerability disclosure policies define how and when security researchers publicly reveal bugs after notifying vendors, balancing the need for fixes with transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Zero">Project Zero - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Responsible_disclosure">Responsible disclosure</a></li>
<li><a href="https://projectzero.google/">Google Project Zero</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some argued for immediate disclosure to pressure vendors, while others noted that certain vendors like Ubuntu would need more time. One commenter raised concerns about companies using vulnerability discovery as leverage to promote their own LLM products.

**Tags**: `#security`, `#vulnerability-disclosure`, `#google`, `#project-zero`, `#policy`

---

<a id="item-10"></a>
## [Practitioner argues frontier LLM gains come from harnesses, not raw intelligence](https://www.reddit.com/r/LocalLLaMA/comments/1xwegdi/hot_take_frontier_models_havent_actually_become/) ⭐️ 7.0/10

A Reddit user on r/LocalLLaMA posted a detailed argument that frontier LLMs have become more useful mainly because of better harnesses—context retrieval, prompts, and custom tools—rather than significant improvements in raw intelligence. Drawing on experience building production AI systems, software engineering, and local models, the author claims that switching to newer frontier models rarely improved results once a harness worked well, and that smaller local models now perform surprisingly well on efficient problem solving. This perspective challenges the prevailing narrative of rapid, exponential intelligence gains and the accompanying hype and doom about superintelligence, suggesting that much of the recent progress is cumulative engineering rather than a fundamental leap. It matters for practitioners deciding whether to invest in newer models or in better context engineering and tooling, and for how the industry evaluates and markets model capabilities. The author defines 'raw intelligence' as efficiently using given information, tools, and time to solve problems, and notes that while newer models sometimes found creative workarounds, these were often too slow or unreliable for production. The post acknowledges real improvements in tool calling, reduced hallucinations, and longer context windows, but questions whether efficient problem solving truly requires many parameters.

reddit · r/LocalLLaMA · /u/Reasonable_Goat · Nov 14, 21:57

**Background**: An agent harness (also called agent scaffolding) is the software infrastructure around an LLM that lets it act as an agent—managing context, calling tools, and interacting with the environment. Context engineering involves designing prompts, retrieval, and memory to supply the model with relevant information. The debate over whether scaling parameters or improving harnesses drives performance is central to how the AI community assesses frontier progress.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://github.com/aglio-lab/context-engineering-tools">GitHub - aglio-lab/context-engineering-tools: The ...</a></li>
<li><a href="https://www.kamiljozwik.com/posts/agentic-capabilities">Agentic Capabilities of LLMs</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#AI evaluation`, `#model capabilities`, `#production AI`, `#community discussion`

---

<a id="item-11"></a>
## [tiny-voca: a fully open 4.5M-parameter TTS that runs 70x real-time on CPU](https://www.reddit.com/r/LocalLLaMA/comments/1xw7zrg/tinyvoca_a_fully_open_45mparameter_tts_code/) ⭐️ 7.0/10

A developer released tiny-voca, a 4.5M-parameter English text-to-speech model with code, weights, dataset, and training recipe all open. It runs 70x faster than real time on 4 CPU threads and in the browser, using a custom phonemizer and a source-filter synthesizer instead of a neural vocoder. This project demonstrates that practical, fully open TTS can run efficiently on edge devices without a neural vocoder, lowering the barrier for on-device and browser-based speech applications. Its complete openness—including the synthetic training dataset—provides a reproducible baseline for the local AI community. The model is 18 MB, supports two voices (one female, one male) at 24 kHz, and was trained from scratch in 7.7 hours on a single RTX 4090. Limitations include English-only support, no voice cloning, occasional mispronunciation of foreign names, and a somewhat synthetic sound due to synthetic training data generated with Qwen3-TTS.

reddit · r/LocalLLaMA · /u/nato_nob · Nov 14, 17:26

**Background**: Text-to-speech (TTS) systems typically convert text to phonemes and then use a neural vocoder to generate waveforms, which can be computationally heavy. Source-filter synthesis is a classic alternative that models speech as a glottal source filtered by the vocal tract, and it is much lighter computationally. A phonemizer is a tool that transcribes text into phonemes, which is essential for TTS pronunciation.

<details><summary>References</summary>
<ul>
<li><a href="https://praat.org/manual/Source-filter_synthesis.html">Source - filter synthesis</a></li>
<li><a href="https://bootphon.github.io/phonemizer/">Welcome to Phonemizer ’s documentation! — Phonemizer ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deep_learning_speech_synthesis">Deep learning speech synthesis - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#text-to-speech`, `#open-source`, `#edge-ai`, `#on-device-ml`, `#model-release`

---

<a id="item-12"></a>
## [IBM trains two small open models to ignore orders hidden in documents](https://www.reddit.com/r/LocalLLaMA/comments/1xw09tu/ibm_trains_two_small_open_models_to_ignore_orders/) ⭐️ 7.0/10

IBM has trained two small open language models specifically designed to resist prompt injection attacks, where malicious instructions are hidden inside documents. The release was shared on r/LocalLLaMA, where it received positive community interest. Prompt injection is a major security risk for LLM-powered applications, and small models are often more vulnerable. IBM's release provides practitioners with open, hardened models that can be deployed in document-processing pipelines, potentially reducing attack surface and increasing trust in AI systems. The models are small and open, making them suitable for local deployment and customization. However, the post itself is brief and lacks technical details such as model size, architecture, or evaluation benchmarks, so the extent of their robustness remains to be independently verified.

reddit · r/LocalLLaMA · /u/mawcopolow · Nov 14, 11:33

**Background**: Prompt injection is a technique where an attacker inserts hidden instructions into text (e.g., a document or webpage) that an LLM processes, causing the model to follow the attacker's commands instead of the user's original request. This is especially dangerous in applications like document summarization or web browsing, where the model may inadvertently execute malicious actions. Small language models (SLMs) are compact versions of LLMs, often used for cost-effective and on-device tasks, but they may have weaker defenses due to fewer parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/prompt-injection">What Is a Prompt Injection Attack ? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Small_language_model">Small language model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/small-language-models">What are Small Language Models (SLM)? | IBM</a></li>

</ul>
</details>

**Discussion**: The r/LocalLLaMA community reacted positively, with users appreciating IBM's effort to address prompt injection in small models. Some noted that prompt injection is a significant issue for small models, and the release is seen as a valuable step forward.

**Tags**: `#prompt-injection`, `#LLM-security`, `#open-models`, `#IBM`, `#small-language-models`

---

<a id="item-13"></a>
## [Nex-AGI Releases Nex-N2.6, a 321B FP8 Multimodal Agentic Model](https://www.reddit.com/r/LocalLLaMA/comments/1xw9mpa/nexaginexn26_hugging_face/) ⭐️ 7.0/10

Nex-AGI released Nex-N2.6, an approximately 321B-parameter FP8-quantized multimodal agentic model built on GLM-5.3-Flash, with weights published on Hugging Face. The release follows Nex-N2.5-Pro and focuses on reducing repetitive reasoning and improving adherence to the tools available in the current environment. This is a substantial open-weight release aimed at computer use, coding, and long-horizon tool tasks, giving the local LLM community a large multimodal agentic option. It also shows the trend of building specialized agentic models on top of strong open base models like GLM-5.3-Flash. The repository contains FP8-quantized weights of roughly 321B parameters, which halves memory versus FP16 but still requires substantial GPU resources to run locally. It is an incremental follow-up to Nex-N2.5-Pro rather than a paradigm shift, and the base GLM-5.3-Flash is a 320B-parameter Mixture-of-Experts model with only about 18B active parameters.

reddit · r/LocalLLaMA · /u/TheRealMasonMac · Nov 14, 18:31

**Background**: Agentic models are LLMs designed to autonomously plan and execute multi-step tasks, calling external tools and interacting with software over long horizons. FP8 is an 8-bit floating-point format that roughly halves model memory versus FP16 with minimal accuracy loss, making very large models more practical to serve. GLM-5.3-Flash is Z.ai's natively multimodal model in the GLM-5 series, and Nex-AGI built Nex-N2.6 on top of it for computer use and coding.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.3-Flash">zai-org/GLM-5.3-Flash · Hugging Face</a></li>
<li><a href="https://www.together.ai/models/glm-5-3-flash">GLM-5.3-Flash API: Pricing, Benchmarks & Docs | Together AI</a></li>
<li><a href="https://docs.vllm.ai/en/v0.5.4/quantization/fp8.html">FP8 — vLLM</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#multimodal`, `#agentic-models`, `#model-release`, `#hugging-face`

---

<a id="item-14"></a>
## [SenseNova-Loop-9B-Preview: 9B model reportedly matches Qwen 3.5 27B](https://www.reddit.com/r/LocalLLaMA/comments/1xvysss/sensenovasensenovaloop9bpreview_hugging_face/) ⭐️ 7.0/10

A Reddit post on r/LocalLLaMA highlights SenseNova-Loop-9B-Preview, a new small model from SenseTime that reportedly matches the overall performance of Qwen 3.5 27B despite having only 9B parameters. The poster notes the model appears not yet fully finished and has not personally tested it. If the claim holds, a 9B model matching a 27B one would significantly lower hardware requirements for local LLM deployment, making strong performance accessible on consumer GPUs. This reflects a broader industry trend toward parameter-efficient architectures that trade raw size for smarter computation. The model uses a looped decoder with shared weights and two-stream manifold-constrained hyper-connections (mHC), executing 56 layer passes with a 262K-token training context. The poster notes that effective inference parameters are around 15B and that the model includes multi-token prediction (MTP), so actual speed versus Qwen remains uncertain.

reddit · r/LocalLLaMA · /u/barbear22 · Nov 14, 10:02

**Background**: SenseNova-Loop-9B-Preview is a multimodal image-text-to-text model from SenseTime, designed for long-context and agentic workflows such as document understanding, coding, and tool use. Its looped decoder reuses the same layers multiple times rather than stacking unique ones, which keeps parameter count low while increasing effective depth. Multi-token prediction (MTP) is a technique that lets a model draft several tokens at once to speed up generation, and it has recently been integrated into llama.cpp for local inference.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/OpenSenseNova/SenseNova-Loop">GitHub - OpenSenseNova/SenseNova-Loop</a></li>
<li><a href="https://aicybr.com/blog/sensenova-loop-9b-preview-local-inference-architecture-guide">SenseNova-Loop-9B Preview: Architecture, Local GPU ...</a></li>
<li><a href="https://www.banandre.com/blog/multi-token-prediction-lands-in-llamacpp-nearly-2x-faster-generation-but-prompt-processing-is-paying-the-price">Multi - Token Prediction Lands in llama.cpp: Nearly... - Banandre</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#model-architecture`, `#local-llm`, `#efficient-inference`, `#hugging-face`

---