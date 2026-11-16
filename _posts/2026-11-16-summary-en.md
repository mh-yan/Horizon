---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 35 items, 15 important content pieces were selected

---

1. [Microsoft 365 outage leads to chlorine gas poisoning of 15 hotel guests](#item-1) ⭐️ 8.0/10
2. [Paper applies recursive self-improvement to frontier pre-training, announces 30B-A3B base model](#item-2) ⭐️ 8.0/10
3. [Haru-4B: A Low-Latency Full-Duplex Spoken Dialogue Model](#item-3) ⭐️ 8.0/10
4. [Old Bitly Links Hijacked, Exposing URL Shortener Risks](#item-4) ⭐️ 7.0/10
5. [Protomaps: Self-hosting map tiles has gotten cheap and easy](#item-5) ⭐️ 7.0/10
6. [MacBook Pro OLED PWM Flicker Sparks Debate Over Display Comfort](#item-6) ⭐️ 7.0/10
7. [Turbo Pascal's Entire IDE Was Smaller Than Modern Single-Purpose Binaries](#item-7) ⭐️ 7.0/10
8. [Sebastian Raschka Explains Positional Embeddings in Modern LLMs](#item-8) ⭐️ 7.0/10
9. [Stripe closes small business account after $1,500 charge, citing unauthorized payment risk](#item-9) ⭐️ 7.0/10
10. [Blog argues all AI-generated code should be open source](#item-10) ⭐️ 7.0/10
11. [Voltage Glitch Unlocks 80GB VRAM and 126 SMs on NVIDIA CMP 170HX Mining Card](#item-11) ⭐️ 7.0/10
12. [Basalt 0.4.0 adds multi-model support and fast Qwen 27B NVFP4 quant](#item-12) ⭐️ 7.0/10
13. [EU's EUROPA open AI model targets nearly 1 trillion parameters](#item-13) ⭐️ 7.0/10
14. [inside-llm: Open-Source Tool Visualizes LLM Token Probabilities and Compares Quantizations](#item-14) ⭐️ 7.0/10
15. [audio.cpp 0.9.5 adds real-time local avatar chat with 850ms latency](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Microsoft 365 outage leads to chlorine gas poisoning of 15 hotel guests](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 8.0/10

A Microsoft 365 outage prevented a hotel from receiving email alerts from its cloud-connected chlorine dosing system, causing excess chlorine to be pumped into a pool and resulting in 15 guests suffering chlorine gas poisoning at the Phantasialand hotel in Germany. This incident highlights the risks of relying on cloud services for safety-critical systems, especially when alerts are sent via email without redundancy or fail-safes. It underscores the need for robust, independent safety mechanisms in infrastructure to prevent real-world harm. The hotel's automatic dosing system over-chlorinated the pool, and the maintenance safety system's email alert was not received due to the Microsoft 365 outage. The incident occurred at Phantasialand, a theme park resort in Germany, and injured 15 guests.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**Background**: Microsoft 365 is a cloud-based productivity suite that includes email and collaboration tools, widely used by businesses. Many organizations depend on it for critical communications, but outages can occur, as seen in the October 2025 Azure Front Door incident that disrupted Microsoft 365 services globally. Safety-critical systems, such as chlorine dosing in pools, require fail-safe designs with redundancy to prevent accidents when primary systems fail.

<details><summary>References</summary>
<ul>
<li><a href="https://windowsforum.com/threads/azure-front-door-outage-cloud-dependency-and-resilience-lessons.386927/">Azure Front Door Outage : Cloud Dependency and... | Windows Forum</a></li>
<li><a href="https://www.allaboutcircuits.com/industry-white-papers/designing-safety-critical-control-systems-architecture-redundancy-and-real-world-protection-strategies/">Designing Safety-Critical Control Systems: Architecture ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely blamed the hotel for poor safety design, emphasizing that safety-critical systems must not rely solely on cloud services or email alerts. Some noted that such systems often fail by over-dispensing chlorine, and proper safeguards and redundancy are essential. A Microsoft employee disclaimed that the outage was not Microsoft's fault, but acknowledged the need for resilient architecture.

**Tags**: `#cloud-reliability`, `#safety-critical-systems`, `#infrastructure`, `#outage`, `#IoT`

---

<a id="item-2"></a>
## [Paper applies recursive self-improvement to frontier pre-training, announces 30B-A3B base model](https://www.reddit.com/r/LocalLLaMA/comments/1xwt3ri/paper_no_second_run_does_rsi_stop_at_frontier/) ⭐️ 8.0/10

A new paper claims to be the first to apply recursive self-improvement (RSI) to an entire frontier pre-training run from scratch, decomposing the unrepeatable end-to-end process into smaller loops. The result is 801-30B-A3B-Base, a 30B-A3B Mixture-of-Experts model trained on 11.8T tokens in three months by a newly formed team, with the base model and lightweight SFT data open-sourced. Prior public RSI work has focused only on post-training, which starts from an existing base model and is relatively cheap and repeatable. Extending RSI to pre-training means improving the foundation that every later stage builds on, potentially accelerating the entire model development pipeline and affecting how frontier labs approach training. The paper argues that pre-training breaks three conditions that make post-training RSI feasible: runs cost hundreds of thousands of GPU-hours and cannot be repeated, the objective (post-training headroom) cannot be read from a single score, and the whole production system—not just the model—must improve. As a base model, 801-30B-A3B outperforms Qwen3-30B-A3B and Nemotron-3.5-Lightning-30B-A3B, trailing only the larger Qwen3.5-35B-A3B, and with lightweight SFT alone it achieves the highest average on four agentic benchmarks against fully post-trained models.

reddit · r/LocalLLaMA · /u/pmttyji · Nov 15, 11:21

**Background**: Recursive self-improvement (RSI) is a hypothetical process in which an AI system iteratively designs more capable successors, potentially leading to an intelligence explosion. As of 2026, various RSI-related projects are ongoing and AI companies increasingly use AI for coding and research, but human work is still needed. Pre-training is the initial, most expensive stage of building a large language model, where the model learns from massive amounts of text data before any task-specific fine-tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://www.anthropic.com/institute/recursive-self-improvement">Our progress toward recursive self - improvement , and its implications.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Training_of_large_language_models">Training of large language models - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#recursive self-improvement`, `#pre-training`, `#large language models`, `#AI research`, `#frontier models`

---

<a id="item-3"></a>
## [Haru-4B: A Low-Latency Full-Duplex Spoken Dialogue Model](https://www.reddit.com/r/LocalLLaMA/comments/1xww5o2/higurashiaiharu4b_hugging_face/) ⭐️ 8.0/10

Higurashi-ai released Haru-4B, a 4B-parameter pretrained full-duplex spoken dialogue foundation model that listens and speaks simultaneously at 7.5 Hz, producing one frame of audio and text every 133 ms. It generates continuous 64-dimensional audio latents in a single step via a small MLP head with MeanFlow sampling, eliminating discrete audio tokens and a separate audio transformer. This model advances real-time speech AI by enabling natural, simultaneous listening and speaking without turn-taking delays, which could improve voice assistants, call-center bots, and conversational agents. Its multilingual support across nine languages and efficient one-step audio generation make it a notable step toward more human-like spoken dialogue systems. User audio, model audio, and model text are summed into a single position of the language model, so listening and speaking never block each other. Character and voice control are achieved via a text card and a short reference clip, and the model supports English, Spanish, Portuguese, German, French, Chinese, Japanese, Russian, and Korean.

reddit · r/LocalLLaMA · /u/pmttyji · Nov 15, 13:58

**Background**: Full-duplex spoken dialogue models differ from traditional half-duplex systems that process one turn at a time; they can listen and speak concurrently, enabling more natural conversations with backchanneling and interruptions. Recent research has focused on benchmarks and taxonomies for these models, and continuous audio language models aim to avoid discrete tokens by predicting continuous latents, often using one-step generative methods like MeanFlow for efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2503.04721">Full-Duplex-Bench: A Benchmark to Evaluate Full-duplex Spoken ... A Survey of Full-Duplex Spoken Dialogue Systems ... GitHub - DanielLin94144/Full-Duplex-Bench: A Benchmark for ... Full-Duplex-Bench: A Benchmark for Full-duplex Spoken ... GitHub - Ruiqi-Yan/Awesome-Full-Duplex-SDM: A curated list of ... Full-Duplex Spoken Dialogue Model - emergentmind.com Beyond Turn-Based Interfaces: Synchronous LLMs as Full-Duplex ...</a></li>
<li><a href="https://arxiv.org/html/2509.06926v3">Continuous Audio Language Models - arXiv.org</a></li>
<li><a href="https://www.emergentmind.com/topics/meanflow">MeanFlow : One - Step Generative Modeling</a></li>

</ul>
</details>

**Tags**: `#speech`, `#dialogue`, `#full-duplex`, `#multilingual`, `#foundation-model`

---

<a id="item-4"></a>
## [Old Bitly Links Hijacked, Exposing URL Shortener Risks](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 7.0/10

A large-scale link-hijacking scheme has turned old Bitly links, including corporate social media archives such as a Burger King tweet, into bizarre and offensive redirects. The incident highlights how expired or abandoned short links can be repurposed by malicious actors. This incident affects many users and organizations that rely on URL shorteners for sharing links, as hijacked links can damage brand reputation and spread misinformation. It underscores the systemic risks of outsourcing link management and the need for long-term link integrity solutions. The hijacking exploits the fact that short link providers may recycle or release expired short codes, allowing attackers to claim them and redirect to malicious content. Bitly's Trust and Safety team exists to handle such abuse, but the incident shows that abandoned links remain a persistent vulnerability.

hackernews · hspeiser · Nov 15, 22:11 · [Discussion](https://news.ycombinator.com/item?id=50511395)

**Background**: URL shorteners like Bitly and TinyURL create compact links that redirect to longer web addresses, making them convenient for social media and messaging. However, these services introduce risks: link rot occurs when links stop working over time, and link hijacking happens when expired short codes are reused by attackers. The Hacker News discussion also touches on related issues like CNAME-based domain hijacking and the broader problem of abandoned URL ownership.

<details><summary>References</summary>
<ul>
<li><a href="https://nypost.com/2026/11/15/lifestyle/corporate-social-media-hacked-in-bizarre-bitly-link-hijacking-scheme/">Corporate social media hacked in bizarre Bitly link-hijacking ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Link_rot">Link rot - Wikipedia</a></li>
<li><a href="https://cutt.ly/resources/blog/url-shortener-security-brand-protection">URL Shortener Security: Protect Your Brand from Hijacking</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong opposition to outsourced link shorteners, arguing they create permanently broken links and are worse for the internet than in-house solutions. Some were surprised that a URL shortener has a Trust and Safety team, while others shared related experiences with spam using old CNAMEs from reputable organizations. Overall sentiment was critical of link shorteners and supportive of better link preservation practices.

**Tags**: `#security`, `#URL shorteners`, `#link rot`, `#internet infrastructure`, `#privacy`

---

<a id="item-5"></a>
## [Protomaps: Self-hosting map tiles has gotten cheap and easy](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

A blog post highlights that Protomaps offers a cheap and easy way to self-host map tiles, with community discussion on Hacker News adding comparisons to similar projects like OpenFreeMap and practical experiences using Cloudflare R2 and PMTiles. This matters because developers can now own their map infrastructure at low cost, avoiding expensive bills from commercial providers like Google Maps and reducing reliance on public tile services, which is especially valuable for privacy-sensitive or access-controlled applications. PMTiles is a single-file archive format for tiled data that can be hosted on commodity storage like S3, enabling serverless map applications; however, while basemaps are small enough to store cost-effectively, high-resolution satellite imagery can quickly become large and expensive at higher zoom levels.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**Background**: Protomaps is an open-source mapping project that provides a free, customizable map of the world deployable as a single static file on cloud storage. PMTiles, its underlying format, packages pyramids of map tiles into one archive, eliminating the need for a custom tile backend or third-party provider. This approach contrasts with traditional map services that charge per tile request and require API keys.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.protomaps.com/pmtiles/">PMTiles Concepts | Protomaps Docs</a></li>
<li><a href="https://github.com/protomaps/PMTiles">GitHub - protomaps/PMTiles: Pyramids of map tiles in a single ...</a></li>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>

</ul>
</details>

**Discussion**: Commenters shared positive experiences, with one noting they switched from Google Maps to Protomaps due to high bills and found it dirt cheap and easy to use. Others mentioned similar projects like OpenFreeMap and their own setups using Cloudflare R2, while cautioning that satellite imagery at high zoom levels can become prohibitively expensive to store and serve.

**Tags**: `#maps`, `#self-hosting`, `#PMTiles`, `#geospatial`, `#open-source`

---

<a id="item-6"></a>
## [MacBook Pro OLED PWM Flicker Sparks Debate Over Display Comfort](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

An analysis published on MacAnorak examines the MacBook Pro's OLED display and its use of PWM dimming, claiming a frequency of 240Hz that can cause flicker-related discomfort. The article has sparked a community debate, with commenters challenging the 240Hz figure based on their own oscilloscope measurements. This matters because PWM flicker is a real ergonomic and accessibility concern for a widely used professional device, affecting users with flicker sensitivity who may experience eye strain, headaches, or nausea. The debate highlights the need for better display standards and transparency from manufacturers like Apple. The article's 240Hz claim is contested; commenters suggest the tandem OLED design uses two panels PWM-ing at 480Hz and 180 degrees out of phase, yielding an effective 960Hz in most usable brightness ranges. Additionally, the discussion broadens to other display sensitivities such as low CRI on white LEDs and motion blur on LCDs.

hackernews · MacAnorak · Nov 15, 13:15 · [Discussion](https://news.ycombinator.com/item?id=50506719)

**Background**: PWM (pulse-width modulation) dimming is a technique used in displays to control brightness by rapidly turning the screen on and off. While this flicker is often imperceptible, low frequencies can cause discomfort for sensitive individuals. OLED displays commonly use PWM because their brightness is harder to control with simple voltage changes, and the frequency used varies by manufacturer and panel type.

<details><summary>References</summary>
<ul>
<li><a href="https://www.oled-info.com/pulse-width-modulation-pwm-oled-displays">Pulse-width modulation (PWM) in OLED displays - OLED-Info Monitor Flicker Test - Check PWM Flicker Online OLED Eye Strain and PWM Flicker: How to Test and Reduce ... PWM Flicker Test - Check Your Screen for PWM Dimming - XBitLabs PWM Flicker Test: Check If Your Monitor Uses PWM Dimming</a></li>
<li><a href="https://www.notebookcheck.net/Why-Pulse-Width-Modulation-PWM-is-such-a-headache.270240.0.html">Why Pulse-Width Modulation (PWM) is such a headache</a></li>
<li><a href="https://screenlab.nl/blog/pwm-sensitivity-test/">PWM Sensitivity: Why Some People Get Headaches from Monitors</a></li>

</ul>
</details>

**Discussion**: Commenters actively debated the actual PWM frequency, with some citing oscilloscope measurements suggesting an effective 960Hz due to out-of-phase tandem OLED panels. Others shared personal experiences with flicker sensitivity, including concussion-related screen intolerance, and called for broader awareness of display-related discomforts like low CRI and motion blur.

**Tags**: `#OLED`, `#PWM flicker`, `#display technology`, `#hardware ergonomics`, `#accessibility`

---

<a id="item-7"></a>
## [Turbo Pascal's Entire IDE Was Smaller Than Modern Single-Purpose Binaries](https://prog21.dadgum.com/116.html) ⭐️ 7.0/10

A 2011 blog post by James Hague resurfaced, pointing out that the complete Turbo Pascal integrated development environment and compiler fit in a binary smaller than many modern single-purpose command-line tools. The post sparked a renewed Hacker News discussion in 2024 with 191 points and 95 comments. The comparison highlights the dramatic growth in software size and complexity over decades, raising questions about whether modern software bloat is justified by developer productivity gains. It resonates with systems programmers and language designers concerned about efficiency and minimalism. Turbo Pascal, originally released by Borland in 1983, combined a compiler and IDE in a single executable that was remarkably small even by the standards of the time. The blog post specifically notes that the entire Turbo Pascal system was smaller than the modern `touch` command binary on some systems, which merely creates empty files or updates timestamps.

hackernews · ksec · Nov 15, 13:44 · [Discussion](https://news.ycombinator.com/item?id=50506894)

**Background**: Turbo Pascal was a highly influential programming environment for the Pascal language, known for its speed and low memory footprint on CP/M and MS-DOS. Software bloat refers to the ever-increasing complexity and size of software, often due to added features and layers of abstraction. The blog post uses binary size as a tangible metric to critique this trend.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turbo_Pascal">Turbo Pascal - Wikipedia</a></li>
<li><a href="https://www.computerlanguage.com/results.php?definition=software+bloat">software bloat - CLC Definition</a></li>

</ul>
</details>

**Discussion**: Commenters praised Anders Hejlsberg's career (Turbo Pascal, Delphi, C#, TypeScript) as exceptionally tasteful. Some expressed frustration with the comparison, arguing that bytes have different contexts and costs, while others lamented the inefficiency of modern tools like `touch` and questioned why Pascal faded despite its influence.

**Tags**: `#software-bloat`, `#turbo-pascal`, `#systems-programming`, `#programming-languages`, `#efficiency`

---

<a id="item-8"></a>
## [Sebastian Raschka Explains Positional Embeddings in Modern LLMs](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 7.0/10

Sebastian Raschka published a technical walkthrough on positional embeddings in large language models, covering classic methods like absolute positional embeddings and modern approaches such as Rotary Positional Embeddings (RoPE) and No Positional Embeddings (NoPE). The article includes visual examples, a small PyTorch implementation, and a survey of 2025 and 2026 open-weight architectures. Positional embeddings are crucial for transformers to understand token order, and this article provides practitioners with a clear, hands-on guide to implementing and choosing among modern techniques. It also highlights emerging trends like NoPE, which could simplify future LLM architectures. The article assumes familiarity with basic LLM architectures and attention internals, and it builds on Raschka's 'Build a Large Language Model (From Scratch)' material. It covers both theoretical foundations and practical implementation, including a PyTorch code snippet for RoPE.

hackernews · vismit2000 · Nov 15, 12:14 · [Discussion](https://news.ycombinator.com/item?id=50506376)

**Background**: Transformers lack an inherent mechanism to account for the order of tokens in a sequence, so positional embeddings are added to inject position information. Classic methods use fixed or learned absolute positions, while modern approaches like RoPE encode relative positions through rotation matrices, and NoPE relies on causal masking to implicitly preserve order.

<details><summary>References</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/understanding-positional-embeddings">Understanding Positional Embeddings in Modern LLMs</a></li>
<li><a href="https://cyrilzakka.github.io/llm-playbook/pos-embed.html">Positional Embeddings - The Large Language Model Playbook</a></li>
<li><a href="https://openreview.net/pdf?id=18f4nhMJ33">Positional Encodings as Group Representations: A Unified ...</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News appreciated the practical walkthrough but noted that a deeper theoretical understanding requires viewing positional embeddings as group representations. One commenter explained that RoPE corresponds to representations of the translation group, and such group-theoretic perspectives can guide the design of new, learnable positional encodings.

**Tags**: `#LLMs`, `#positional embeddings`, `#deep learning`, `#NLP`, `#machine learning`

---

<a id="item-9"></a>
## [Stripe closes small business account after $1,500 charge, citing unauthorized payment risk](https://news.ycombinator.com/item?id=50510042) ⭐️ 7.0/10

A small business owner reported on Hacker News that Stripe closed their account after they charged a saved card $1,500 for three completed appointments, following a $1 test payment weeks earlier. Stripe blocked the charge and closed the account, stating the payments 'don't appear to have been authorized by the customer,' and rejected the owner's appeal without requesting the recorded call or client messages as evidence. This case highlights the tension between automated fraud detection and legitimate small businesses, as Stripe's risk systems can shut down accounts without human review of available evidence. It affects many merchants who rely on saved payment methods for recurring or per-service billing and raises questions about payment processor accountability and transparency. The business used a $1 Stripe payment link to save the client's card, then charged $1,500 weeks later, a pattern that commenters noted resembles card-testing fraud. Stripe's Setup Intents with off-session usage is suggested as a more appropriate method for saving cards for future charges, and sending individual invoices via Stripe may also avoid triggering risk flags.

hackernews · snirgbs · Nov 15, 19:49

**Background**: Stripe is a payment processor that uses automated risk algorithms to detect fraud, and it may close accounts or block payments if it suspects unauthorized transactions. A common fraud pattern involves criminals making a small test charge (e.g., $1) to verify a stolen card, followed by a larger charge. Stripe's Setup Intents allow merchants to save payment methods for future off-session payments with proper authentication, reducing the risk of being flagged.

<details><summary>References</summary>
<ul>
<li><a href="https://support.stripe.com/questions/unexpected-1-charge-on-customers-bank-statement">Unexpected $1 charge on customer's bank statement - Stripe</a></li>
<li><a href="https://www.nextgenpayment.eu/articles/what-happens-if-stripe-closes-your-account-how-to-safeguard-your-business">What Happens If Stripe Closes Your Account – Risks ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed that the charge pattern (a $1 test followed by a $1,500 charge) closely resembles card-testing fraud, which likely triggered Stripe's risk system. They suggested using Setup Intents for off-session payments or sending individual invoices via Stripe to avoid such flags, while some shared frustrations about Stripe's lack of accountability and harsh account closures.

**Tags**: `#Stripe`, `#payments`, `#fraud-detection`, `#small-business`, `#risk-management`

---

<a id="item-10"></a>
## [Blog argues all AI-generated code should be open source](https://jakub.jankiewicz.org/blog/ai-code-open-source/) ⭐️ 7.0/10

A blog post by Jakub Jankiewicz argues that all AI-generated code should be open source, sparking a Hacker News discussion with 579 comments debating copyright, ownership, and software engineering. This debate is significant because AI coding tools are increasingly used in commercial software, and clarity on ownership and licensing will affect developers, companies, and the open-source ecosystem. The discussion highlights that current copyright law, such as US Copyright Office guidance, requires human authorship for protection, and that open-source licenses depend on copyright, so AI-generated code may not be licensable under terms like the GPL.

hackernews · jcubic · Nov 15, 14:46 · [Discussion](https://news.ycombinator.com/item?id=50507303)

**Background**: AI code generation tools like GitHub Copilot and Claude Code produce code based on models trained on vast amounts of public code, including open-source projects. This raises questions about whether the output is derivative of the training data, who owns it, and whether it can be copyrighted. Open-source licenses rely on copyright law to enforce sharing and attribution requirements, so if AI-generated code lacks copyright, those licenses may be ineffective.

<details><summary>References</summary>
<ul>
<li><a href="https://allthingsopen.org/articles/copyright-problem-ai-generated-code-open-source-licenses">The copyright problem with AI-generated code | We Love Open ...</a></li>
<li><a href="https://www.systemshardening.com/articles/cicd/ai-code-license-compliance/">AI-Generated Code and Open Source License Compliance: The ...</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue that AI is just a tool like a compiler and that human direction and engineering effort justify ownership, while others point out that AI models are trained on open-source code and should therefore produce open-source output. One AGPL author shared a story of a company cloning their system with an LLM after being caught violating the license, highlighting practical enforcement challenges.

**Tags**: `#AI`, `#open-source`, `#copyright`, `#software-engineering`, `#policy`

---

<a id="item-11"></a>
## [Voltage Glitch Unlocks 80GB VRAM and 126 SMs on NVIDIA CMP 170HX Mining Card](https://www.reddit.com/r/LocalLLaMA/comments/1xwxzgj/i_finally_succeed_the_cmp_170hx_voltage_glitch/) ⭐️ 7.0/10

A Reddit user (Yarukiless-cat) successfully performed a voltage glitch on an NVIDIA CMP 170HX mining card using a Raspberry Pi Pico, unlocking 80GB of VRAM and 126 SMs after about 15 hours of work. The user also plans to modify a second CMP card later. This hack turns a relatively cheap mining card into an A100-class accelerator with more memory and SMs than a real A100, offering a cost-effective path to high-VRAM GPUs for local LLM inference. It highlights a reproducible hardware vulnerability that could disrupt the second-hand GPU market. The method involves voltage fault injection on the GA100 die to blow locked fuses, rewriting the card's configuration; a Raspberry Pi Pico (or similar glitcher like PicoGlitcher) is used for the attack. The CMP 170HX typically costs around $2,500-$3,000, while a real A100 80GB PCIe can exceed $20,000, but success may vary by card and requires technical skill.

reddit · r/LocalLLaMA · /u/Yarukiless-cat · Nov 15, 15:16

**Background**: The NVIDIA CMP 170HX is a mining-specific graphics card based on the GA100 GPU, the same chip used in the A100 data center accelerator, but with severely limited memory (8GB or 10GB) and disabled SMs. Voltage glitching is a hardware attack that momentarily drops the voltage to cause faults in a chip's operation, allowing bypass of security checks or fuse locks. The Raspberry Pi Pico is a low-cost microcontroller often used to build affordable glitching tools like the PicoGlitcher.

<details><summary>References</summary>
<ul>
<li><a href="https://hwbusters.com/news/voltage-glitching-turns-nvidias-cmp-170hx-mining-card-into-an-80gb-a100-that-outruns-the-real-thing/">Voltage Glitching Turns NVIDIA 's CMP 170 HX Mining Card Into an...</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/techie-turns-usd2-500-cmp-170hx-8gb-mining-card-into-a-full-fat-a100-80gb-with-voltage-glitching-carefully-blowing-onboard-fuses-to-unlock-entire-vram-and-shader-modules">Techie uses voltage glitching hack to turn $2,500 Nvidia 8GB...</a></li>
<li><a href="https://www.hackster.io/news/matthias-kesenheimer-s-picoglitcher-turns-a-raspberry-pi-pico-into-a-python-powered-fault-injector-d1633e6a4b3a">Matthias Kesenheimer's PicoGlitcher Turns a Raspberry Pi Pico Into...</a></li>

</ul>
</details>

**Tags**: `#hardware-hacking`, `#voltage-glitching`, `#gpu`, `#local-llm`, `#nvidia`

---

<a id="item-12"></a>
## [Basalt 0.4.0 adds multi-model support and fast Qwen 27B NVFP4 quant](https://www.reddit.com/r/LocalLLaMA/comments/1xx1cu9/basalt_040_more_models_still_as_fast_qwen_27b_up/) ⭐️ 7.0/10

Basalt 0.4.0 introduces multi-model and router support, starting with DeepSeek V4.1 Flash, and debuts its first dense model, Qwen 3.8 27B NVFP4, which achieves up to 776 tok/s on structured output and 92.8% top-1 accuracy versus BF16 on an RTX 5090. This release shows Basalt expanding from a mixture-of-experts-only engine to a more general local inference platform, and the high-throughput, high-accuracy NVFP4 quant of Qwen 3.8 27B makes running a capable dense model on consumer Blackwell GPUs more practical. The Qwen 3.8 27B NVFP4 quant reaches 262 tok/s in conversation and 194 tok/s on prose in single-stream mode, with prefill of 12,000 tok/s at 4k context (slowing as context grows), and supports chat, tools, thinking, images, video, and up to 262K context; the 0.0262 KLD versus BF16 indicates low quantization error.

reddit · r/LocalLLaMA · /u/jesdga95 · Nov 15, 17:30

**Background**: Basalt is a local inference engine optimized for NVIDIA Blackwell GPUs (sm_120) that originally targeted mixture-of-experts models like Qwen3.8-Flash-Next and DeepSeek-V4.1-Flash, keeping experts that don't fit in VRAM in system RAM. NVFP4 is a 4-bit floating-point format with block scaling that reduces memory use and boosts throughput while aiming to preserve accuracy. Qwen 3.8 27B is a dense 27B vision-language model with configurable reasoning and a native 262K-token context window.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jesdga95/basalt">GitHub - jesdga95/basalt: Local inference engine optimized ...</a></li>
<li><a href="https://basalt.jgulfo.com/">Basalt: a fast local inference engine for NVIDIA Blackwell GPUs</a></li>
<li><a href="https://lmstudio.ai/models/qwen3.8">Qwen3.8 - lmstudio.ai</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#quantization`, `#inference`, `#qwen`, `#benchmarks`

---

<a id="item-13"></a>
## [EU's EUROPA open AI model targets nearly 1 trillion parameters](https://www.reddit.com/r/LocalLLaMA/comments/1xwr917/europa_the_eus_open_ai_model_is_aiming_for_nearly/) ⭐️ 7.0/10

The EU-backed open AI model EUROPA is reportedly aiming for nearly 1 trillion parameters, according to a discussion on r/LocalLLaMA. This signals a major public-sector push into frontier-scale open models. If realized, EUROPA would be one of the largest open models, potentially reshaping the open-source AI ecosystem and reducing reliance on closed models. It could also bolster EU digital sovereignty and multilingual AI capabilities. The model is expected to cover 24 EU languages and is positioned as a European common good, but technical details such as architecture, training data, and compute requirements remain scarce. Feasibility and compute demands are key concerns.

reddit · r/LocalLLaMA · /u/mawcopolow · Nov 15, 09:24

**Background**: EUROPA is a consortium-driven initiative to build a multilingual frontier open-source AI model, part of the EU's Apply AI Strategy announced in October 2025. Parameters are the internal weights of a large language model; more parameters generally mean greater capacity but also higher training and inference costs. Frontier-scale open models are those that compete with top closed models in performance.

<details><summary>References</summary>
<ul>
<li><a href="https://quoracast.com/the-european-open-source-ai-movement-is-gaining-momentum/">The European Open Source AI Movement Is Gaining... - quoracast.com</a></li>
<li><a href="https://www.linkedin.com/pulse/what-parameters-large-language-models-why-matter-olímpio-da-silva-ot7if">What Are Parameters in Large Language Models and Why They...</a></li>
<li><a href="https://huggingface.co/blog/state-of-open-models-summer-2026">State of Open Models: Summer 2026 Observations - Hugging Face</a></li>

</ul>
</details>

**Discussion**: The r/LocalLLaMA community expressed interest in the feasibility of training such a large model, the massive compute requirements, and the geopolitical implications of an EU-backed open model. Some are hopeful about a strong European open-source alternative, while others are skeptical about execution and cost.

**Tags**: `#open-source AI`, `#large language models`, `#EU policy`, `#AI research`, `#model scaling`

---

<a id="item-14"></a>
## [inside-llm: Open-Source Tool Visualizes LLM Token Probabilities and Compares Quantizations](https://www.reddit.com/r/LocalLLaMA/comments/1xx7qbf/i_have_created_a_tool_to_observe_what_happens/) ⭐️ 7.0/10

A developer released inside-llm, an open-source browser-based tool that loads one or two GGUF models via llama.cpp and visualizes token probabilities, sampler chain stages, and divergence metrics (Jensen-Shannon and KL) between two quantizations of the same model, token by token. It offers lockstep and free comparison modes, branching with exact KV-state snapshots, and a logit lens view, with self-contained packages for Linux and Windows supporting CUDA or Vulkan. This tool gives local LLM users and researchers a practical way to inspect how quantization changes model behavior at the token level, which is often opaque. By making sampler chains and distributional divergence visible, it can help diagnose quality differences between quants and support interpretability work in the llama.cpp ecosystem. The tool requires both models to share the same tokenizer and fit simultaneously in VRAM on a single GPU, falls back to slow CPU inference if no dedicated GPU is available, and supports only text models without split GGUFs or embedding models. It is MIT-licensed, listens only on 127.0.0.1 with no telemetry, and records sessions that can be replayed in a static page without the engine or GPU.

reddit · r/LocalLLaMA · /u/AlternativeEnough352 · Nov 15, 21:46

**Background**: GGUF is the unified model file format developed by the llama.cpp team, widely used for storing quantized local LLMs. llama.cpp is an open-source inference library that has become the de facto standard for local LLM tools like Ollama and LM Studio. Quantization reduces model precision to save memory and speed up inference, but different quantization levels can produce different outputs. Jensen-Shannon and Kullback-Leibler divergence are statistical measures of how different two probability distributions are, useful for comparing token-level predictions.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.mikihands.com/en/whitedec/2025/11/20/gguf-format-complete-guide-local-llm-new-standard/">Complete Guide to GGUF Format - The New Standard for Local LLMs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://en.wikipedia.org/wiki/Jensen–Shannon_divergence">Jensen–Shannon divergence - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#visualization`, `#llama.cpp`, `#interpretability`

---

<a id="item-15"></a>
## [audio.cpp 0.9.5 adds real-time local avatar chat with 850ms latency](https://www.reddit.com/r/LocalLLaMA/comments/1xx2vi0/audiocpp_soulxflashhead_lfm3audio_owsm_v4/) ⭐️ 7.0/10

audio.cpp 0.9.5 introduces a new avatar voice chat app in its WebUI that combines SoulX-FlashHead for talking-head generation, OWSM v4 for speech recognition, and LFM3-Audio for conversation and text-to-speech, achieving about 850ms end-to-end latency on an RTX 5090. This demonstrates a fully local, real-time speech-to-speech avatar pipeline that avoids cloud APIs, making private, low-latency interactive avatars feasible for enthusiasts and researchers with high-end consumer GPUs. The pipeline calls LFM3-Audio twice (once for the conversational response and once for TTS in a different voice), and the video generation stage remains GPU-intensive: SoulX requires an RTX 4090 or better, and cuDNN is mandatory for real-time performance, as without it inference is 2× slower and VRAM usage doubles.

reddit · r/LocalLLaMA · /u/Acceptable-Cycle4645 · Nov 15, 18:29

**Background**: SoulX-FlashHead is a 1.3B-parameter framework for high-fidelity, infinite-length, real-time streaming talking-head video generation, capable of 10.8 FPS on a single RTX 4090. OWSM v4 is an open speech recognition model from CMU that improves multilingual ASR and language identification over its predecessor. LFM3-Audio is Liquid AI's compact 2B-parameter audio model that runs locally and can take text or audio as input and respond with text, speech, or both.

<details><summary>References</summary>
<ul>
<li><a href="https://soul-ailab.github.io/soulx-flashhead/">SoulX - FlashHead : Oracle-guided Generation of Infinite Real-time...</a></li>
<li><a href="https://huggingface.co/espnet/owsm_v4_medium_1B">espnet/owsm_v4_medium_1B · Hugging Face</a></li>
<li><a href="https://docs.liquid.ai/lfm/models/lfm3-audio-2b">LFM3-Audio-2B - Liquid Docs</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#real-time-avatar`, `#speech-to-speech`, `#audio.cpp`, `#GPU-inference`

---