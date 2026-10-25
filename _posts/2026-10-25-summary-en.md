---
layout: default
title: "Horizon Summary: 2026-10-25 (EN)"
date: 2026-10-25
lang: en
---

> From 28 items, 8 important content pieces were selected

---

1. [Moderna and Merck's mRNA cancer vaccine cuts melanoma death and recurrence by 42%](#item-1) ⭐️ 9.0/10
2. [10-year-old Inception v3 CNN beats frontier LLMs in skin cancer diagnosis](#item-2) ⭐️ 7.0/10
3. [Oregon Police Quote $2.5M for Records on One Officer](#item-3) ⭐️ 7.0/10
4. [UC Berkeley math professor questions homework grading amid AI use](#item-4) ⭐️ 7.0/10
5. [Cerebras Deploys Trillion-Parameter AI Models on Wafer-Scale Hardware](#item-5) ⭐️ 7.0/10
6. [OpenAI and Anthropic Block Reverse Engineering of Smart TVs](#item-6) ⭐️ 7.0/10
7. [RTX 3080 20GB mod unlocks P2P and ReBAR, boosting vLLM prompt processing by up to 115%](#item-7) ⭐️ 7.0/10
8. [Lean-QwenFlash runs 125B Qwen3.8-Flash-Next at 20 tok/s on 16GB VRAM and 8GB RAM via NVMe SSD offloading](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Moderna and Merck's mRNA cancer vaccine cuts melanoma death and recurrence by 42%](https://arstechnica.com/health/2026/10/personalized-mrna-cancer-vaccine-cut-melanoma-death-recurrence-by-42/) ⭐️ 9.0/10

Moderna and Merck reported that their personalized mRNA cancer vaccine reduced the risk of death or recurrence by 42% in a Phase 2 trial involving patients with melanoma. This is a major medical breakthrough that validates the personalized mRNA cancer vaccine approach and could reshape cancer treatment, while also boosting Moderna's platform strategy beyond COVID-19. The trial measured recurrence-free survival in melanoma patients, but the data is from a Phase 2 trial and larger Phase 3 trials are needed to confirm efficacy and safety.

hackernews · _Microft · Oct 25, 19:29 · [Discussion](https://news.ycombinator.com/item?id=50235217)

**Background**: Personalized mRNA cancer vaccines work by analyzing a patient's tumor mutations and encoding those neoantigens into mRNA, which is delivered to prompt the immune system to attack cancer cells. This approach builds on the mRNA platform technology used in COVID-19 vaccines, but is customized for each patient.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Personalized_mRNA_cancer_vaccine_therapy">Personalized mRNA cancer vaccine therapy - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11908549/">Challenges and opportunities of predicting overall survival ...</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted Moderna's on-demand vaccine platform business model, noted that the stock dropped despite good data due to inflated expectations, and raised concerns about political opposition to mRNA vaccines from the Trump administration and RFK Jr.

**Tags**: `#mRNA`, `#cancer-vaccine`, `#biotech`, `#Moderna`, `#healthcare`

---

<a id="item-2"></a>
## [10-year-old Inception v3 CNN beats frontier LLMs in skin cancer diagnosis](https://lynchlab.net/llm-skin-cancer) ⭐️ 7.0/10

A blog post by lynchlab.net reports that a 10-year-old Inception v3 convolutional neural network, fine-tuned on 68,011 dermoscopic and clinical images from the ISIC Archive, outperformed two frontier large language models (LLMs) in diagnosing skin cancer on a test set of 200 lesions. The model was trained on a single H100 GPU and had never seen the test lesions or any images of the same patient during training. This finding challenges the assumption that general-purpose LLMs are always the best tool for specialized tasks, highlighting that small, task-specific models can achieve superior accuracy in narrow domains like medical imaging. It has sparked debate about the value of specialized architectures versus LLMs and the role of benchmarking in model evaluation. The CNN used Inception v3 pretrained on everyday photographs and fine-tuned all layers on the ISIC Archive dataset; the test set was carefully curated to exclude any images of the same lesion or patient from training. However, critics argue this is an example of 'benchmaxxing'—optimizing specifically for the benchmark—and that the comparison may not reflect real-world clinical performance.

hackernews · sungam · Oct 25, 17:15 · [Discussion](https://news.ycombinator.com/item?id=50233779)

**Background**: Inception v3 is a convolutional neural network architecture released in 2016 by Google, known for its efficiency and use of factorized convolutions. Fine-tuning involves taking a pretrained model and further training it on a specific dataset to adapt it to a new task. LLMs are large language models trained on vast text data, capable of general-purpose reasoning but not inherently specialized for image classification. The ISIC Archive is a large public collection of skin lesion images used for dermatology research.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Inception_(deep_learning_architecture)">Inception (deep learning architecture) - Wikipedia</a></li>
<li><a href="https://huggingface.co/docs/timm/main/models/inception-v3">Inception v3 - Hugging Face</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC7969634/">Convolutional Neural Network for Skin Lesion Classification ...</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News debated the implications: some argued that for scaled applications, dedicated classifiers are more accurate and LLMs can help build them cheaply, while others pointed out that the comparison is unfair because the CNN was specifically optimized for this benchmark ('benchmaxxing'). Some noted that specialized models like KataGo outperform LLMs in narrow tasks, and others welcomed the renewed appreciation for diverse machine learning techniques.

**Tags**: `#machine-learning`, `#LLMs`, `#medical-imaging`, `#model-architecture`, `#benchmarking`

---

<a id="item-3"></a>
## [Oregon Police Quote $2.5M for Records on One Officer](https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/) ⭐️ 7.0/10

The Intercept reports that the Eugene Police Department in Oregon estimated it would take 44,816 staff hours and cost approximately $2,484,599.04 to fulfill a public records request from a local news outlet concerning a single police officer. This case illustrates how prohibitive fee estimates can be used to obstruct access to public records, undermining government transparency and accountability. It has sparked broader discussion about FOIA practices and the need for reforms to prevent such abuses. The estimate of 44,816 hours is equivalent to about 21 years of full-time work for one person, and the quoted fee exceeds $2.4 million. Under Oregon's public records law, agencies must provide a written estimate of fees and time before fulfilling a request, which can be used to deter requesters.

hackernews · tdeck · Oct 25, 18:04 · [Discussion](https://news.ycombinator.com/item?id=50234232)

**Background**: The Freedom of Information Act (FOIA) and state-level public records laws are designed to ensure public access to government records, promoting transparency and accountability. However, agencies can impose fees for searching, reviewing, and duplicating records, and excessively high estimates can effectively block requests. Oregon's public records law (ORS 192.410 to 192.505) requires agencies to acknowledge requests within five business days and provide estimates for fees, but does not cap the fees, allowing agencies to quote prohibitive amounts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.searchsystems.net/us/or/public-records-law">Oregon Public Records Law - Oregon Public ... | SearchSystems.net</a></li>
<li><a href="https://cdnsm5-hosted.civiclive.com/UserFiles/Servers/Server_3585797/File/Government/Public+Records+and+Regulations/Public+Records+Law/OregonPublicRecordLaw.pdf">A Quick Reference Guide to Oregon 's Public Records Law</a></li>
<li><a href="https://covenantforwarriors.org/advocacy-stories/what-they-dont-want-you-to-know/how-government-agencies-dodge-transparency-laws/">How U.S. Government Agencies dodge transparency laws | Covenant...</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News expressed outrage at the absurdity of the estimate, with one noting it equates to 21 years of work. Others shared similar experiences of agencies using slow-walking tactics, and compared the U.S. system unfavorably to the UK's FOIA, which mandates responses within 30 days, and Germany's ongoing battle over FOIA fees. Some pointed out even larger fee estimates from the Department of Defense, highlighting a pattern of obstruction.

**Tags**: `#public-records`, `#foia`, `#government-transparency`, `#police-accountability`, `#journalism`

---

<a id="item-4"></a>
## [UC Berkeley math professor questions homework grading amid AI use](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 7.0/10

UC Berkeley mathematician Richard Borcherds, a Fields Medalist, publicly questioned the value of grading homework given the prevalence of AI tools that can complete assignments, sparking a large discussion on Hacker News. This highlights how AI is forcing educators to rethink traditional assessment methods, potentially reshaping how students are evaluated and what skills are valued in higher education. Borcherds is a Fields Medalist known for proving the Monstrous Moonshine conjecture, and the discussion revealed that he likely delegates grading to teaching assistants, raising questions about the purpose of homework and the role of AI in learning.

hackernews · romanhn · Oct 25, 16:28 · [Discussion](https://news.ycombinator.com/item?id=50233304)

**Background**: Large language models (LLMs) like ChatGPT can generate human-like text and solve problems, making it easy for students to use AI for homework. This has led to debates about academic integrity and the effectiveness of homework as a learning tool. Richard Borcherds is a prominent mathematician at UC Berkeley, awarded the Fields Medal in 1998 for his work in lattices, group theory, and infinite-dimensional algebras.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Richard_Borcherds">Richard Borcherds - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models ( LLMs )? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters noted the irony that Borcherds likely hasn't graded homework himself in years, and debated whether homework's purpose is to learn or to assess. Some argued that AI removes the forcing function that made students engage with material, while others questioned the value of grading homework for college students at all.

**Tags**: `#AI`, `#education`, `#LLMs`, `#academia`, `#assessment`

---

<a id="item-5"></a>
## [Cerebras Deploys Trillion-Parameter AI Models on Wafer-Scale Hardware](https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras) ⭐️ 7.0/10

Cerebras published a blog post detailing how it deploys trillion-parameter frontier AI models on its wafer-scale hardware, achieving inference speeds of 1,000–2,000+ tokens per second. The post explains how models are mapped across WSE-3T wafers to deliver scalable inference. This demonstrates that wafer-scale hardware can handle the largest AI models at high throughput, offering an alternative to GPU clusters for inference. It could impact how enterprises deploy frontier models, especially where speed and cost-efficiency are critical. Cerebras claims inference speeds of 1,000–2,000+ tokens per second, but community members note that the models available on Cerebras are often outdated compared to frontier models. The hardware requires significant resources, and scaling to meet demand remains a challenge.

hackernews · gmays · Oct 25, 01:33 · [Discussion](https://news.ycombinator.com/item?id=50227356)

**Background**: Cerebras Systems is known for its Wafer-Scale Engine (WSE), a chip the size of a silicon wafer that integrates hundreds of thousands of AI-optimized cores. The WSE-3, introduced in March 2024, features 4 trillion transistors and 900,000 cores, powering the CS-3 supercomputer. Trillion-parameter models are the largest language models, requiring immense compute and memory for inference.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Cerebras WSE-3 Turbo | Wafer-Scale AI Chip</a></li>
<li><a href="https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras">How Cerebras Deploys Trillion-Parameter AI Models</a></li>

</ul>
</details>

**Discussion**: Commenters debated Cerebras's ability to keep up with demand, with some noting that the company lacks the financial resources of OpenAI and struggles to manufacture enough wafer-scale nodes. Others criticized the service for offering outdated models, though some expect Cerebras to soon release better models at lower cost and higher speed. A few questioned the technical details of how data flows across the wafer's processing elements.

**Tags**: `#AI hardware`, `#large language models`, `#Cerebras`, `#wafer-scale`, `#inference`

---

<a id="item-6"></a>
## [OpenAI and Anthropic Block Reverse Engineering of Smart TVs](https://www.reddit.com/r/LocalLLaMA/comments/1xer30z/openai_and_anthropic_blocked_the_reverse/) ⭐️ 7.0/10

A Reddit post in r/LocalLLaMA highlights that OpenAI and Anthropic blocked a reverse-engineering effort (REA) aimed at investigating smart TVs that spy on users, with Claude reportedly blocking the tool one day later. This raises concerns about frontier model providers refusing legitimate security research use cases, which could hinder privacy investigations and fuel the debate over open-weight models as an alternative for such work. The post is thin, consisting of a link to an X post and a brief comment, and the blocking appears to be due to safety guardrails rather than a specific policy change; the REA tool (Reverse Engineer Anything) was reportedly interrupted during detailed binary and firmware analysis.

reddit · r/LocalLLaMA · /u/kroggens · Oct 25, 02:51

**Background**: Reverse engineering smart TVs involves analyzing firmware and binaries to uncover hidden data collection practices, such as always-on microphones or tracking. Recent investigations into LG and Samsung TVs have exposed extensive data sharing, prompting researchers to use AI tools like REA. OpenAI and Anthropic have safety policies that restrict certain reverse-engineering requests, which can inadvertently block legitimate security research.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=8eyy-Dri9dU">The LG Smart TV Spying Scandal: How Researchers Actually ... LG Smart TV Spying Exposed: 216M TVs, Full Breakdown | The ... Researcher says Samsung TV software tracks viewing and may ... LG Smart TVs Accused of Audio and Wi-Fi Data Collection Samsung TV Privacy Claims Raise Fresh Questions About AI ... Anthropic Limits Claude's Help with Reverse-Engineering T... People are now vibe-coding their smart TVs to strip them of ...</a></li>
<li><a href="https://ai-tldr.dev/learn/evaluation-safety/alignment-safety/why-llms-refuse/">Why Do LLMs Refuse? Over-Refusals Explained | AI/TLDR</a></li>

</ul>
</details>

**Discussion**: The r/LocalLLaMA community expresses frustration over model refusals for legitimate security research, with commenters arguing that such over-refusals strengthen the case for open-weight models that users can control and run locally.

**Tags**: `#AI safety policy`, `#open weights`, `#reverse engineering`, `#LLM refusals`, `#privacy`

---

<a id="item-7"></a>
## [RTX 3080 20GB mod unlocks P2P and ReBAR, boosting vLLM prompt processing by up to 115%](https://www.reddit.com/r/LocalLLaMA/comments/1xf9kmd/rtx_3080_20gb_got_rebar_and_p2p_unlock_70_prompt/) ⭐️ 7.0/10

A community member (u/nathannguyennng) has unlocked PCIe peer-to-peer (P2P) and Resizable BAR (ReBAR) support on modded RTX 3080 20GB cards, and another user shared benchmark results showing up to 115% faster prompt processing in tensor-parallel vLLM inference compared to stock. The tests used dual RTX 3080 20GB GPUs in a Proxmox VM with vLLM 0.32.0 serving a 27B AWQ-INT4 model. This is a significant win for the local LLM community, as it demonstrates that older, modded GPUs can achieve substantial prompt-processing speedups in multi-GPU setups through firmware/driver-level unlocks, potentially extending the useful life of affordable hardware for self-hosted inference. It also highlights how P2P and ReBAR, features typically reserved for newer or professional GPUs, can be enabled on consumer cards to improve tensor-parallel workloads. The benchmarks show prompt processing gains ranging from 70% to 115% over stock when both GPU unlock and P2P are enabled, with P2P alone contributing up to 70% improvement over GPU unlock alone. However, token generation (decode) performance showed no consistent improvement, remaining within noise except for a slight gain at very long prompts (261k tokens). The test system used PCIe 3.0 x16 slots and limited both GPUs to 240W.

reddit · r/LocalLLaMA · /u/No-Refrigerator-1672 · Oct 25, 18:16

**Background**: P2P (peer-to-peer) allows GPUs to directly access each other's memory over the PCIe bus, bypassing the CPU and system RAM, which reduces latency and increases bandwidth for multi-GPU communication. ReBAR (Resizable BAR) is a PCIe feature that lets the CPU access the full GPU memory instead of a limited 256MB window, improving data transfer efficiency. vLLM is a popular open-source inference engine that supports tensor parallelism, splitting a model across multiple GPUs to fit larger models and accelerate processing. The RTX 3080 20GB is a modified version of the original 10GB card, likely with doubled VRAM, and these unlocks enable features not officially supported by NVIDIA on consumer Ampere GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.nvidia.com/ai-enterprise/release-8/latest/infra-software/vgpu/features/p2p.html">Peer-To-Peer (P2P) CUDA Transfers — NVIDIA AI Enterprise</a></li>
<li><a href="https://www.intel.com/content/www/us/en/support/articles/000090831/graphics.html">What Is Resizable BAR and How Do I Enable It? - Intel</a></li>
<li><a href="https://docs.vllm.ai/en/latest/serving/parallelism_scaling/">Parallelism and Scaling - vLLM</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#gpu-inference`, `#vllm`, `#tensor-parallelism`, `#hardware-modding`

---

<a id="item-8"></a>
## [Lean-QwenFlash runs 125B Qwen3.8-Flash-Next at 20 tok/s on 16GB VRAM and 8GB RAM via NVMe SSD offloading](https://www.reddit.com/r/LocalLLaMA/comments/1xev6bo/leanqwenflash_qwen38flashnext_125b_running_at_20/) ⭐️ 7.0/10

A Reddit user adapted the SSD-offloading design from sybil-solutions/glm-flash-lite to run Qwen3.8-Flash-Next (125B) on consumer hardware with only 16GB VRAM and 8GB system RAM, achieving ~20 tok/s decode at 262k context. Benchmarks show 28–33 tok/s for prose and 19–22 tok/s for code at 8k context, with prefill speeds of ~1,080 tok/s on an RTX 4090. This demonstrates that large MoE models can run on modest consumer laptops by offloading experts to NVMe SSDs instead of keeping them in RAM, significantly lowering the memory barrier for local LLM deployment. It could enable more users to experiment with 100B+ parameter models without high-end workstations. The benchmarks use a 3.05bpw_h5_ng5 quantization with Q4 KV cache; on an RTX 3080 Laptop (16GB VRAM, 32GB RAM), 100k context yields ~18–21 tok/s decode and ~650–700 tok/s prefill with peak VRAM of 15.5GB. Setup instructions, model downloaders, and packing scripts are available on GitHub.

reddit · r/LocalLLaMA · /u/MaxDev0 · Oct 25, 06:41

**Background**: Mixture of Experts (MoE) models like Qwen3.8-Flash-Next contain many specialized sub-networks (experts), but only a subset is activated per token, reducing compute. However, all experts must be stored somewhere; typically they are kept in system RAM, requiring 48–64GB for a 125B model. SSD offloading moves inactive experts to fast NVMe storage, trading some latency for drastically lower memory requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://arxiv.org/pdf/2408.10013">SSDTrain: An Activation Offloading Framework to SSDs for ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#model-offloading`, `#moe`, `#qwen`, `#nvme-ssd`

---