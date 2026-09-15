---
layout: default
title: "Horizon Summary: 2026-09-15 (EN)"
date: 2026-09-15
lang: en
---

> From 42 items, 20 important content pieces were selected

---

1. [TypeSafe AI Launches System One Models and Jev for Fast Typed Inference](#item-1) ⭐️ 8.0/10
2. [E-ink frame listens for birds and draws them as 1800s illustrations](#item-2) ⭐️ 8.0/10
3. [Internet Archive Fights Scraping Surge on Wayback Machine](#item-3) ⭐️ 8.0/10
4. [Google launches Gemini 3.8 Live and 3.8 Live Extended Thinking](#item-4) ⭐️ 8.0/10
5. [AI agent finds Baseten GitHub token, gains admin access in 25 minutes](#item-5) ⭐️ 8.0/10
6. [Developer Builds Linux GPU Driver for M4 Mac Mini in One Month Using LLMs](#item-6) ⭐️ 8.0/10
7. [US Confirms First Deployment of Space Weapons](#item-7) ⭐️ 8.0/10
8. [SpaceX to Attempt First Starship Orbital Flight on September 22](#item-8) ⭐️ 8.0/10
9. [Prior Labs releases TabPFN-3.5, new SOTA tabular foundation model](#item-9) ⭐️ 8.0/10
10. [Capsule bundles HTML apps and their data into a single SQLite file](#item-10) ⭐️ 7.0/10
11. [Norwegian Consumer Council argues for quality over disposable products](#item-11) ⭐️ 7.0/10
12. [Suspected sabotage disrupts Dutch rail network](#item-12) ⭐️ 7.0/10
13. [Modern CSS revives the CSS Zen Garden dream, sparking debate](#item-13) ⭐️ 7.0/10
14. [Hacker turns a $20 4G hotspot into a texting device](#item-14) ⭐️ 7.0/10
15. [IBM and Hugging Face Launch Framework for AI Agent Consistency](#item-15) ⭐️ 7.0/10
16. [AI data center boom meets Philadelphia's refinery-scarred neighborhood](#item-16) ⭐️ 7.0/10
17. [US Data Centers Could Outconsume Germany and Japan in Natural Gas by 2035](#item-17) ⭐️ 7.0/10
18. [OpenAI, Anthropic, Google DeepMind Hold Weeks of AI Safety Talks](#item-18) ⭐️ 7.0/10
19. [India to charge 0.4% merchant fee on larger UPI payments from October 15](#item-19) ⭐️ 7.0/10
20. [SHADOW-50M: A 44M Ternary LLM Running at 1,900 tok/s on CPU](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [TypeSafe AI Launches System One Models and Jev for Fast Typed Inference](https://typesafe.ai/blog/introducing-system-one-models-and-jev) ⭐️ 8.0/10

TypeSafe AI has released Jev, its first System One model, a new class of AI models designed to make fast, structured decisions that software can use directly. Jev evaluates a state and returns typed answers and probabilities, trading general-purpose text generation for speed and type safety. This launch could significantly impact AI/ML and software engineering by enabling fast, reliable structured outputs for tasks like classification and decision-making, potentially integrating with design-by-contract patterns to build more robust systems. The high engagement on Hacker News (565 points, 187 comments) indicates strong community interest in its capabilities and implications. Jev takes a state (structured text) and a question (as a Choice, Score, or Noul) with optional augmentations, then outputs answers such as choices, probabilities, and confidence scores. The largest performance claims remain internally tested, and the model is currently in early access.

hackernews · albelfio · Sep 15, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49717558)

**Background**: System One models are a new class of AI models built to make fast, structured decisions that software can use directly, as opposed to generative models that produce free-form text. Type inference refers to the ability of a compiler or system to automatically deduce the types of expressions, and design-by-contract is a software engineering pattern where components specify preconditions, postconditions, and invariants. TypeSafe AI's Jev is the first such model, aiming to provide typed inference for automation tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.typesafe.ai/concepts/system-one">System One - TypeSafe AI</a></li>
<li><a href="https://typesafe.ai/blog/introducing-system-one-models-and-jev">Introducing System One Models and Jev - TypeSafe AI Blog</a></li>
<li><a href="https://runtimewire.com/article/typesafe-jev-system-one-ai-model-early-access">TypeSafe opens Jev early access for fast, typed AI decisions</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the potential and call for open-sourcing, while others question the speed comparison to generative models and find the documentation confusing. There is excitement about combining Jev with design-by-contract patterns, but also skepticism about its limitations and marketing claims.

**Tags**: `#AI`, `#machine-learning`, `#typed-inference`, `#design-by-contract`, `#Hacker News`

---

<a id="item-2"></a>
## [E-ink frame listens for birds and draws them as 1800s illustrations](https://github.com/arnegiacomo/fugleramme) ⭐️ 8.0/10

A developer named Arne Munthe-Kaas (GitHub user arnegiacomo) published a Show HN project called 'fugleramme' — an e-ink frame that continuously listens for bird sounds, identifies the species using the BirdNET classifier, and then displays the detected bird as a vintage 1800s-style illustration on the e-ink screen. The project reached the front page of Hacker News with 1204 points and 167 comments. The project is a striking example of how cheap microcontrollers (ESP32) and machine-learning audio classifiers (BirdNET) can be combined with low-power e-ink displays to create ambient, 'magical' devices that blend nature observation with retro aesthetics. It highlights a growing wave of DIY bird-monitoring projects and shows how accessible bioacoustics has become for hobbyists. The system relies on BirdNET, a traditional convolutional neural network (not an LLM) developed for acoustic bird identification, and runs on an ESP32 microcontroller with Wi-Fi/Bluetooth. E-ink displays only consume power when refreshing, so such frames can run for months or years on a single battery charge, as noted by commenters comparing Wi-Fi versus BLE e-ink drivers.

hackernews · arnemunthekaas · Sep 15, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49711544)

**Background**: BirdNET is an AI-powered sound identification system developed at the Cornell Lab of Ornithology and Chemnitz University of Technology that lets anyone identify birds by their calls using a phone or embedded device. E Ink is an electronic paper display technology that mimics the look of printed paper and only uses power when the image changes, making it ideal for always-on, low-power devices. The ESP32 is a family of low-cost, low-power microcontrollers with integrated Wi-Fi and Bluetooth, widely used in IoT and hobbyist hardware projects.

<details><summary>References</summary>
<ul>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://en.wikipedia.org/wiki/E_Ink">E Ink - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were overwhelmingly enthusiastic, calling it 'the coolest thing on HN' and praising the blend of ideas that produces a 'magical' experience. One user pointed out that BirdNET is a traditional neural network rather than an LLM, another linked a related bird-monitoring project (birdnet-go), and several shared their own e-ink/ESP32 projects, noting that BLE e-ink drivers can last years on a single charge.

**Tags**: `#e-ink`, `#ESP32`, `#BirdNET`, `#hardware`, `#creative-coding`

---

<a id="item-3"></a>
## [Internet Archive Fights Scraping Surge on Wayback Machine](https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/) ⭐️ 8.0/10

The Internet Archive published an update stating that the Wayback Machine has been hit by waves of high-volume automated traffic, and that it has put protective measures in place to keep the service running. The Archive attributes the surge to scrapers trying to circumvent blocks on original sites by pulling content from archived copies instead. The Wayback Machine is a critical piece of free internet infrastructure used by journalists, researchers, and Wikipedia editors, so sustained scraping pressure threatens public access to the historical web. The incident also highlights how the AI-driven scraping arms race is imposing collateral costs on nonprofit archives and could push more sites to opt out of preservation. The Archive says the traffic is likely from scrapers working around blocks on original sites by hitting the Wayback Machine copy instead, and notes that some sites have already opted out of archiving as a result. Users have reported intermittent access problems, including 429 rate-limit errors, though the Archive says it has maintained open access without centralized gatekeepers.

hackernews · ChrisArchitect · Sep 15, 17:52 · [Discussion](https://news.ycombinator.com/item?id=49716176)

**Background**: The Internet Archive is a San Francisco-based nonprofit digital library founded in 1996 by Brewster Kahle, providing free access to archived websites, books, software, music, and audiovisual material. Its Wayback Machine, launched for public access in 2001, lets users view how websites looked in the past and now holds more than 1 trillion web captures and well over 99 petabytes of data. Web scraping refers to automated bots collecting data at mass scale, and in the mid-2020s scrapers used by LLM vendors became a major source of web traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wayback_Machine">Wayback Machine</a></li>
<li><a href="https://en.wikipedia.org/wiki/Internet_Archive">Internet Archive</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_scraping">Web scraping - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters strongly supported the Internet Archive, praising it as irreplaceable infrastructure and urging donations, while criticizing scrapers for abusing a free nonprofit resource. Some shared personal stories of recovering old content through the Wayback Machine, and others noted intermittent 429 errors, with one speculating the AI arms race is causing collateral damage to open resources.

**Tags**: `#internet-archive`, `#web-preservation`, `#scraping`, `#open-access`, `#infrastructure`

---

<a id="item-4"></a>
## [Google launches Gemini 3.8 Live and 3.8 Live Extended Thinking](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/) ⭐️ 8.0/10

Google announced Gemini 3.8 Live and Gemini 3.8 Live Extended Thinking, which it calls its most advanced live dialogue models yet, featuring major upgrades in intelligence and parallel reasoning for voice-driven tasks. The models are available through the Gemini Live experience, the Gemini API, and integrations such as Gmail. This release strengthens Google's position in the fast-growing voice AI and real-time conversational assistant market, where it competes directly with OpenAI's GPT Voice. Improvements in latency, multilingual support, and reasoning could make Gemini Live a more practical everyday tool for both consumers and developers building voice agents. Gemini 3.8 Live is positioned as the default option for low-latency voice agent experiences without reasoning-induced delays, supporting interleaved reasoning, asynchronous function calling, and built-in audio streaming. The Extended Thinking variant is designed to handle complex tasks in the background while the conversation continues, and the models are described as cost-efficient and optimized for high-volume, latency-sensitive dialogue.

hackernews · leumon · Sep 15, 17:38 · [Discussion](https://news.ycombinator.com/item?id=49715947)

**Background**: Gemini is Google's family of natively multimodal AI models, and the Live variants are specifically tuned for real-time spoken conversation rather than text-only chat. They follow earlier releases such as Gemini 3.1 Flash Live, and the Extended Thinking mode refers to a setting where the model spends extra compute on step-by-step reasoning before responding. Voice AI assistants like these aim to feel like natural human conversation while also being able to call tools and complete tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Gemini 3.8 Live & Gemini 3.8 Live Extended Thinking - The Keyword</a></li>
<li><a href="https://9to5google.com/2026/09/15/gemini-3-8-live-announced/">Gemini 3.8 Live Extended Thinking powers Gemini Live, Gmail</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models/gemini-3.8-live">Gemini 3 . 8 Live | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Discussion**: Community feedback is largely positive, with users praising voice quality, low latency, and strong multilingual performance, including one user who uses Gemini Live for Afrikaans conversation practice. Some users note Gemini Live feels more natural than GPT Voice, while others criticize Google for not yet rolling out Gemini 3.8 to Google AI Plus subscribers and question when Gemini will overtake competitors.

**Tags**: `#AI`, `#Gemini`, `#LLM`, `#Google`, `#Voice AI`

---

<a id="item-5"></a>
## [AI agent finds Baseten GitHub token, gains admin access in 25 minutes](https://www.strix.ai/blog/baseten-harbor-github-pat-takeover) ⭐️ 8.0/10

Security firm Strix used an AI agent to discover a live GitHub personal access token in Baseten's Docker build history, gaining admin access to Baseten's production repositories within 25 minutes. The token, belonging to the 'basetenbot' account, had admin and push access to Baseten's main product repo, GitOps repo, and Homebrew tap, plus read/write access to other private repositories. This incident highlights the growing risk of AI agent-driven penetration testing and the critical importance of securing CI/CD pipelines, as a single exposed credential can compromise an entire organization's supply chain. It also raises ethical and legal questions about security firms using real companies as marketing case studies without consent. The token was found in Docker build history, a common but dangerous practice where secrets passed as build arguments are permanently recorded in image layers and can be retrieved via 'docker history --no-trunc'. Baseten responded by making the Harbor project private and rotating the token, but the incident underscores that such tokens often have broad permissions and long lifetimes.

hackernews · bearsyankees · Sep 15, 18:11 · [Discussion](https://news.ycombinator.com/item?id=49716476)

**Background**: Baseten is a machine learning platform that helps companies deploy and manage AI models in production. GitHub personal access tokens (PATs) are alternative passwords for authenticating to GitHub, often used in CI/CD pipelines; if exposed, they can grant unauthorized access to repositories. Docker build history can leak secrets if they are passed as build arguments or environment variables during image creation, as these are stored in the image metadata.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baseten.co/">Inference Platform: Deploy AI models in production | Baseten</a></li>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://devblogs.microsoft.com/ise/hidden-risks-of-docker-build-time-arguments-and-how-to-secure-your-secrets/">The Hidden Risks of Docker Build Time Arguments and How to Secure Your Secrets - ISE Developer Blog</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise Strix's tool as effective marketing and plan to try it, while others question the legality and ethics of the disclosure, comparing it to breaking into a neighbor's house. Critics argue that naming the victim company is unnecessary and that the tone feels like shaming Baseten, though some acknowledge that Baseten handled the incident well by responding quickly.

**Tags**: `#security`, `#ai-agents`, `#supply-chain`, `#github`, `#penetration-testing`

---

<a id="item-6"></a>
## [Developer Builds Linux GPU Driver for M4 Mac Mini in One Month Using LLMs](https://codyho.dev/blog/gpu-driver/) ⭐️ 8.0/10

A developer named Cody Ho built a working Linux GPU driver for the M4 Mac Mini in just one month, relying heavily on large language models (LLMs) to assist with the development. The achievement was shared in a blog post that quickly gained traction, sparking debate about the role of AI in low-level driver development and ethical concerns surrounding the author's background. This demonstrates how LLMs can dramatically accelerate reverse-engineering and driver development for undocumented hardware, potentially upending the traditional multi-year effort required. It also highlights a growing tension between AI-assisted contributions and community policies, as the Asahi Linux project has a strict no-AI policy that would prevent this work from being upstreamed. The driver targets the M4 Mac Mini's GPU, which is part of Apple's ARM-based M4 system-on-chip featuring a 10-core GPU in the base model. The author, a former Apple engineer, was previously banned from the Asahi Linux community for concealing his extensive LLM use and his Apple connections during another contribution attempt.

hackernews · ADevWithAnIdea · Sep 15, 19:30 · [Discussion](https://news.ycombinator.com/item?id=49717638)

**Background**: Asahi Linux is a project dedicated to bringing Linux to Apple Silicon Macs, and its GPU drivers for M1 and M2 chips were developed through years of manual reverse engineering. Apple Silicon chips like the M4 integrate CPU, GPU, and other components, but Apple does not publicly document the GPU, making driver development extremely challenging. The Asahi Linux project has a strict no-AI policy for contributions, requiring that code be written without LLM assistance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M4">Apple M4 - Wikipedia</a></li>
<li><a href="https://support.apple.com/en-us/121555">Mac mini (2024) - Tech Specs - Apple Support</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed by the speed of development, with some calling it one of the best use cases for LLMs, but others raised ethical concerns about the author's concealed Apple background and the potential legal conflicts. Many noted that Asahi Linux's no-AI policy means this driver cannot be upstreamed, and predicted a rise of AI-assisted forks for newer hardware.

**Tags**: `#Linux`, `#GPU driver`, `#Apple Silicon`, `#LLM`, `#Asahi Linux`

---

<a id="item-7"></a>
## [US Confirms First Deployment of Space Weapons](https://www.bbc.com/news/articles/ck790xg41ygro) ⭐️ 8.0/10

The United States has officially confirmed for the first time that it has deployed weapons in space, marking a significant shift in its public stance on space militarization. This announcement ends decades of ambiguity about whether the US military has placed offensive or defensive systems in Earth's orbit. This confirmation could trigger a new arms race in space, as other nations may feel compelled to develop or deploy their own space weapons in response. It also raises serious concerns about the weaponization of low-earth orbit, which could threaten satellites essential for communication, navigation, and global security. The specific nature of the deployed weapons—whether they are kinetic, directed-energy, or electronic warfare systems—has not been disclosed, and it remains unclear whether they are intended for offensive or defensive purposes. The Outer Space Treaty of 1967 prohibits placing weapons of mass destruction in orbit, but does not ban conventional space weapons.

hackernews · harporoeder · Sep 15, 03:47 · [Discussion](https://news.ycombinator.com/item?id=49707473)

**Background**: Space militarization refers to the use of space for military purposes, such as surveillance and communication, while weaponization involves placing actual weapons in space. The Outer Space Treaty, signed in 1967, established that space should be used for peaceful purposes, but it left loopholes for non-nuclear weapons. The Kessler syndrome describes a scenario where collisions between space objects create a cascade of debris, potentially making low-earth orbit unusable for generations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kessler_syndrome">Kessler syndrome - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space_weapon">Space weapon - Wikipedia</a></li>
<li><a href="https://thepolitic.org/our-extraterrestrial-military-space-power/">Our Extraterrestrial Military Space Power - The Politic</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about the Kessler syndrome and the potential for space debris to deny future access to low-earth orbit, with some arguing space should be neutral like Antarctica. Others noted the historical context of US directed-energy programs and the irony of calls for the US to be 'unprepared for war,' while some referenced the militarization of space in popular culture.

**Tags**: `#space-weapons`, `#military-technology`, `#geopolitics`, `#space-policy`, `#kessler-syndrome`

---

<a id="item-8"></a>
## [SpaceX to Attempt First Starship Orbital Flight on September 22](https://techcrunch.com/2026/09/15/spacex-will-try-to-put-starship-in-orbit-for-the-first-time-on-september-22/) ⭐️ 8.0/10

SpaceX is scheduled to attempt the first orbital flight of its Starship rocket on September 22, 2026, and will also try to deploy the first operational V3 Starlink satellites during the mission. This marks the first time Starship would reach orbit rather than following a suborbital trajectory. If successful, Starship would become the first fully reusable orbital rocket with the highest payload capacity of any launch vehicle to date, potentially transforming satellite deployment and deep-space exploration. The mission also matters for Starlink, since V3 satellites could significantly boost the performance and capacity of SpaceX's orbital internet constellation. The ship is expected to carry around 20 operational V3 Starlink satellites for the first time, following a July test where earlier V3 satellites were deployed only to validate the deployment mechanism and burned up in Earth's atmosphere after roughly 20 minutes. This will be the second test flight of the Starship Version 3 configuration, pending regulatory clearance to fly.

rss · TechCrunch · Sep 15, 18:16

**Background**: Starship is SpaceX's next-generation launch system, consisting of the Super Heavy booster and the Starship upper stage, designed to be fully reusable and capable of carrying more payload than any previous rocket. Earlier flight tests focused on getting the vehicle through key milestones such as stage separation and controlled reentry, but none had yet placed Starship into a full orbit. Starlink is SpaceX's satellite internet network, and the V3 generation represents a larger, higher-capacity satellite design intended to expand coverage and bandwidth.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/15/spacex-will-try-to-put-starship-in-orbit-for-the-first-time-on-september-22/">SpaceX will try to put Starship in orbit for the first time on... | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship">SpaceX Starship - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/jean-pierre-palomba-marin-14508b162_spacex-launches-new-v3-starlink-satellites-activity-7487386203038613504-OPe2">SpaceX launches new V 3 Starlink satellites but suffers another...</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Starship`, `#Starlink`, `#Orbital Launch`, `#Aerospace`

---

<a id="item-9"></a>
## [Prior Labs releases TabPFN-3.5, new SOTA tabular foundation model](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 8.0/10

Prior Labs released TabPFN-3.5 today, a new tabular foundation model that tops both TabArena and BeyondArena and is state-of-the-art for datasets with up to 1M rows and 20k features. The release includes three variants: TabPFN-3.5-Fast (in alpha, 6x faster than the base model), TabPFN-3.5-Thinking (trades compute for accuracy via API), and TabPFN-3.5-Plus. TabPFN-3.5 sets a new state of the art on two widely used tabular benchmarks, with +250 Elo over the strongest previous baseline and +150 Elo ahead of the previous overall leader on BeyondArena, which could shift how practitioners approach tabular ML tasks. The availability of speed- and accuracy-oriented variants makes the model practical for real-world deployment rather than just leaderboard performance. On BeyondArena, TabPFN-3.5 leads specifically on text-rich, high-cardinality, and high-dimensional data, and TabPFN-3.5-Thinking adds +20 Elo over the base model on BeyondArena and +44 Elo on TabArena. The Fast variant is still in alpha, and the Thinking variant is only accessible through the API.

reddit · r/MachineLearning · /u/tuanacelik · Sep 15, 16:18

**Background**: TabPFN is a transformer-based tabular foundation model from Prior Labs that uses in-context learning to solve tabular prediction problems in a single forward pass, rather than requiring per-dataset training. TabArena is a living benchmark for tabular machine learning on small to medium-sized IID datasets, while BeyondArena extends evaluation to 142 tiny-to-large IID and non-IID tasks, including text-rich and high-cardinality settings. Elo ratings are used to compare models in a pairwise fashion, similar to chess rankings.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/ TabPFN : TabPFN : Foundation Model for Tabular ...</a></li>
<li><a href="https://github.com/autogluon/tabarena">GitHub - autogluon/tabarena: A Living Benchmark for Machine ...</a></li>
<li><a href="https://huggingface.co/datasets/TabArena/BeyondArena">TabArena/BeyondArena · Datasets at Hugging Face</a></li>

</ul>
</details>

**Tags**: `#tabular-data`, `#foundation-models`, `#machine-learning`, `#benchmarking`, `#SOTA`

---

<a id="item-10"></a>
## [Capsule bundles HTML apps and their data into a single SQLite file](https://withcapsule.app/) ⭐️ 7.0/10

Capsule is a new Rust and Tauri 2.0 tool that packs an HTML app, its assets, and its user data into a single portable SQLite file with a .capsule extension. It embeds the HTML and assets directly in the database, stores user data either as a localStorage-style key/value store or through a MongoDB-inspired collections API, and supports saving files like PDFs and images alongside the app. It offers a practical path for local-first, portable web apps that need no server hosting, which matters for sharing data-rich artifacts such as AI-generated visualizations that currently have no easy way to carry their data. The project has drawn strong interest on Hacker News (261 points, 113 comments), signaling real demand for self-contained app packaging. Capsule documents are sandboxed by default: they have no direct file system access and need explicit permission to reach the internet, and they can use local or remote AI models for document-specific features. Because multiple people editing the same file create divergent copies, every data entry carries a unique UUID and timestamp to support merging, and the author plans to open the file format specification for version 1.0.

hackernews · bashtian · Sep 15, 13:31 · [Discussion](https://news.ycombinator.com/item?id=49712278)

**Background**: Tauri 2.0 is an open-source Rust-based framework for building small, fast, cross-platform desktop and mobile apps using HTML, JS, and CSS frontends. SQLite is a self-contained, serverless, zero-configuration database engine whose entire database lives in one file that can be copied across machines and architectures. Local-first web applications store data primarily on the user's device rather than a server, giving instant, offline-capable operation.

<details><summary>References</summary>
<ul>
<li><a href="https://v2.tauri.app/">Tauri 2 . 0 | Tauri</a></li>
<li><a href="https://sqlite.org/onefile.html">SQLite: Single File Database</a></li>
<li><a href="https://www.aditjangid.com/blogs/local-first-web-apps">Local - First Web Application Architecture & Tools Guide</a></li>

</ul>
</details>

**Discussion**: Commenters were split: some praised the idea, especially for sharing AI-generated artifacts that embed data, while others questioned the need for a dedicated runtime when the File System Access API already lets webpages read and write local files. Several noted alternatives like Bun's single-file apps with built-in SQLite, and critics argued that apps whose state changes frequently are poorly suited to being passed around as bundled files.

**Tags**: `#local-first`, `#sqlite`, `#web-apps`, `#tauri`, `#rust`

---

<a id="item-11"></a>
## [Norwegian Consumer Council argues for quality over disposable products](https://www.forbrukerradet.no/short-life/) ⭐️ 7.0/10

The Norwegian Consumer Council (Forbrukerradet) published an article titled 'Let's make quality the norm again,' arguing that consumers should prioritize durable, high-quality products over cheap, disposable goods. The piece sparked a lively Hacker News discussion with 283 comments debating the causes and consequences of declining product quality. This article taps into growing consumer frustration with 'enshittification' and shrinkflation, where products and services degrade over time while prices remain high or increase. The discussion reflects broader concerns about market incentives, inflation, and the environmental impact of disposable goods, resonating with software engineers who worry about quality erosion in their own field. The article is hosted on the Norwegian Consumer Council's website and is part of their advocacy for consumer-friendly policies. The Hacker News discussion includes personal anecdotes about high-quality brands like Feetures socks, theories about quality decline as hidden inflation, and debates about consumer responsibility versus corporate incentives.

hackernews · ingve · Sep 15, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49710109)

**Background**: The Norwegian Consumer Council is a government-funded but independent agency established in 1953 to protect consumer interests. 'Enshittification' is a term coined by Cory Doctorow to describe how online platforms degrade over time to maximize profits, and it has since been applied more broadly to consumer products. Planned obsolescence refers to designing products with a limited lifespan to encourage repeat purchases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Enshittification">Enshittification - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Planned_obsolescence">Planned obsolescence - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Norwegian_Consumer_Council">Norwegian Consumer Council</a></li>

</ul>
</details>

**Discussion**: Commenters expressed a mix of frustration and resignation: some shared positive examples of quality brands like Feetures socks, while others argued that quality was never the norm and that consumers consistently choose cheapness over durability. A key concern was that even 'quality brands' are incentivized to sell out and cut costs, and that expecting consumers to research every purchase is unreasonable.

**Tags**: `#quality`, `#consumerism`, `#enshittification`, `#economics`, `#hacker-news`

---

<a id="item-12"></a>
## [Suspected sabotage disrupts Dutch rail network](https://www.bbc.com/news/articles/c8ly49w9g1edo) ⭐️ 7.0/10

On Tuesday morning, parts of the Netherlands including Amsterdam suffered major rail disruption after suspected sabotage to the tracks, according to ProRail, the country's rail infrastructure operator. The incident coincided with Prinsjesdag, the annual budget day when the monarch addresses parliament, and protests were expected in several locations. The event highlights a systemic vulnerability in rail networks: because signaling is deliberately designed to fail safe, a single well-placed act of sabotage can halt trains across a wide area without causing a crash. It also raises geopolitical questions, coming amid similar incidents in France and tensions with Russia in the Baltic region. Fail-safe rail design means signals and switches default to a safe state (typically stop) when a fault occurs, which prevents collisions but makes it easy to stop all trains in an area at scale. Experts note it is nearly impossible to cause two trains to collide without physically operating one, but trivial to trigger a network-wide halt.

hackernews · choult · Sep 15, 10:22 · [Discussion](https://news.ycombinator.com/item?id=49710253)

**Background**: Fail-safe is a design principle in which a system, upon failure, defaults to a state that does not endanger lives or property; in railways this means signals revert to red and trains stop. This is distinct from fail-secure, which protects data or access rather than physical safety. Rail signaling standards such as CENELEC EN 5012x codify these requirements, and the trade-off between safety and resilience has long been a topic in critical infrastructure security.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.co.uk/news/articles/c8ly49w9g1edo">Netherlands rail disruption due to suspected sabotage ... - BBC</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fail-safe">Fail - safe - Wikipedia</a></li>
<li><a href="https://www.intertechrail.com/fail-safe-rail-systems-standards">Fail-Safe Rail Systems & Standards</a></li>

</ul>
</details>

**Discussion**: Commenters with rail engineering experience confirmed that fail-safe design is an easy target at scale, noting that while collisions are hard to cause, stopping all trains in an area is trivial. Others linked the incident to a recent criminal derailment in France near a Renault factory that is preparing to make military drones with Ukrainian partners, to a Russian warship firing flares at a Danish helicopter in the Baltic, and to Dutch budget-day protests, suggesting possible motives ranging from protest to geopolitics.

**Tags**: `#infrastructure-security`, `#rail-systems`, `#sabotage`, `#fail-safe-design`, `#geopolitics`

---

<a id="item-13"></a>
## [Modern CSS revives the CSS Zen Garden dream, sparking debate](https://josprague.com/blog/the-css-zen-garden-dream-finally-shipped/) ⭐️ 7.0/10

A blog post by Jos Sprague argues that modern CSS features—such as Custom Properties, Flexbox, and Grid—finally make it possible to radically restyle the same HTML markup, fulfilling the original CSS Zen Garden vision. The post has sparked a 56-comment Hacker News discussion about separation of concerns, Tailwind, and the evolution of web styling. This matters because it challenges the long-held assumption that HTML/CSS separation of concerns is impractical, and it questions whether utility-first frameworks like Tailwind are truly necessary. The debate affects how developers think about structuring styles in modern web applications. The original CSS Zen Garden, launched in May 2003, used a single HTML file that never changed while hundreds of designers submitted radically different CSS stylesheets. Modern CSS features like Custom Properties, Flexbox, and Grid now enable similar flexibility without the rigid markup requirements of the past.

hackernews · yosito · Sep 15, 14:40 · [Discussion](https://news.ycombinator.com/item?id=49713262)

**Background**: CSS Zen Garden was a web development resource launched in 2003 to demonstrate the visual power of CSS-based design. It allowed designers to submit stylesheets that restyled a single, unchanging HTML file, proving that content and presentation could be fully separated. Tailwind CSS, by contrast, is a utility-first framework that embeds styling directly in HTML classes, and it has become popular as an alternative approach.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CSS_Zen_Garden">CSS Zen Garden</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tailwind_CSS">Tailwind CSS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Separation_of_concerns">Separation of concerns - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue the CSS Zen Garden model only worked because everyone used a single markup file and doesn't reflect real-world complexity, while others defend separation of concerns and call Tailwind a hack. A few note that the article's focus on maintaining a single stylesheet is not the same as the original Zen Garden's radical restyling goal.

**Tags**: `#CSS`, `#web development`, `#separation of concerns`, `#Tailwind`, `#CSS Zen Garden`

---

<a id="item-14"></a>
## [Hacker turns a $20 4G hotspot into a texting device](https://bkovac.github.io/modem-thing/) ⭐️ 7.0/10

A hacker known as bkovac repurposed a $20 MSM8916-based 4G wireless hotspot into a functional texting device by adding a Clicks Keyboard and a Sharp memory display, and documented the entire process on GitHub. The stock Android firmware was replaced with Linux via the OpenStick project, and the device can be reflashed through EDL mode accessible from ADB. This project demonstrates how cheap, mass-produced cellular hardware can be repurposed into a minimalist communication device, offering a practical alternative to smartphones for people wanting to reduce screen time or avoid doomscrolling. It also highlights the growing hobbyist ecosystem around OpenStick and MSM8916-based modems, which lowers the barrier for embedded hardware experimentation. The build combines an MSM8916-based 4G hotspot, a Clicks Keyboard, and a Sharp memory display; the original GC9107 display was discarded because of poor quality. The stock device runs Android with ADB accessible out of the box, allowing direct entry into EDL mode for reflashing, and Linux installation is described as trivial thanks to the OpenStick project.

hackernews · bobili1234 · Sep 15, 13:20 · [Discussion](https://news.ycombinator.com/item?id=49712102)

**Background**: MSM8916 is a Qualcomm system-on-chip commonly found in low-cost 4G modems and hotspots, and the OpenStick project provides tools to run mainline Linux on such devices. EDL (Emergency Download) mode is a low-level Qualcomm flashing mode that allows firmware replacement even when the normal operating system is inaccessible. The Clicks Keyboard is a physical keyboard accessory originally designed for smartphones, here repurposed for a DIY texting device.

<details><summary>References</summary>
<ul>
<li><a href="https://bkovac.github.io/modem-thing/">Converting a $20 4 G wireless hotspot into a texting device</a></li>
<li><a href="https://blog.adafruit.com/2026/09/15/converting-a-20-4g-wireless-hotspot-into-a-texting-device/">Converting a $20 4 G wireless hotspot into a texting device</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project as a clever, practical 'dumbphone' alternative and a mini cyberdeck, with one noting they often carry a hotspot instead of a phone but lack an easy way to view texts and OTPs. Suggestions included grafting a back-side battery holder for two 18650 cells in parallel to extend battery life to weeks, and running an agent system like Hermes Agent on the device if RAM and storage allow. Another commenter mentioned that some MSM8916-based dongles run an Android UI despite having no display.

**Tags**: `#hardware hacking`, `#4G hotspot`, `#embedded systems`, `#DIY electronics`, `#Show HN`

---

<a id="item-15"></a>
## [IBM and Hugging Face Launch Framework for AI Agent Consistency](https://huggingface.co/blog/ibm-research/altk-evolve-consistency) ⭐️ 7.0/10

IBM Research and Hugging Face published a new framework called ALTK-Evolve for evaluating whether AI agents can reliably repeat successful task completions across multiple runs. The work reframes agent reliability around consistency rather than single-run success, highlighting that an agent that succeeds once may not succeed again. As AI agents move from demos into production systems, consistency and reproducibility become critical for trust and deployment decisions. This framework gives developers a way to measure reliability beyond one-off benchmark scores, which could influence how agent products are evaluated and compared. The framework focuses on repeat-run evaluation, measuring whether an agent that aced a task once will do so again under the same conditions. It is presented as a technical deep-dive with practical implications, though it is not positioned as a groundbreaking paradigm shift.

rss · Hugging Face Blog · Sep 15, 16:00

**Background**: AI agents are systems that use large language models to autonomously perform multi-step tasks, such as browsing the web or manipulating files. Traditional evaluation often reports a single success rate, which can hide the fact that an agent succeeds inconsistently. IBM Research and Hugging Face collaborate on open AI tools, and this blog post continues that work by addressing reliability in agent evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://business20channel.tv/hugging-face-ai-agent-consistency-tool-targets-reliability-in-2026-15-09-2026">Hugging Face AI Agent Consistency Tool Targets Reliability in 2026</a></li>
<li><a href="https://snippora.com/tools/ibm-and-hugging-face-explore-agent-consistency-across-repeat-4162">IBM and Hugging Face explore agent consistency across... — Snippora</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#evaluation`, `#reliability`, `#consistency`, `#Hugging Face`

---

<a id="item-16"></a>
## [AI data center boom meets Philadelphia's refinery-scarred neighborhood](https://techcrunch.com/2026/09/15/the-ai-data-center-boom-is-colliding-with-cities-scarred-by-big-industry/) ⭐️ 7.0/10

National opposition to data center construction has now reached Philadelphia, where city officials proposed building an AI data center in a neighborhood already burdened by a now-defunct oil refinery. The proposal has drawn backlash from residents who have long dealt with industrial pollution. This case illustrates how the AI infrastructure buildout is increasingly colliding with communities that have already absorbed the environmental costs of heavy industry, potentially slowing data center expansion and reshaping energy and urban planning policy. It signals that community consent, not just capital and chips, may become a key constraint on AI scaling. The Philadelphia site sits in a neighborhood still recovering from the legacy of a refinery complex that operated in various forms from 1866 until 2019, including a major 2019 explosion. Data centers add new burdens such as heavy electricity and water consumption, plus air pollution and e-waste, compounding existing environmental justice concerns.

rss · TechCrunch · Sep 15, 21:47

**Background**: Data centers are large facilities that house servers powering cloud services and AI workloads, and they consume significant amounts of electricity and water for cooling. AI-focused data centers are larger and more power-hungry than traditional ones, driving a nationwide construction boom. Philadelphia's refinery history dates back to the 19th century, and the South Philadelphia refinery complex operated from 1866 to 2019, leaving a legacy of pollution and a deadly 2019 explosion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.consumerreports.org/data-centers/ai-data-centers-impact-on-electric-bills-water-and-more-a1040338678/">AI Data Centers Impact on Electric Bills, Water, and More ...</a></li>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>
<li><a href="https://en.wikipedia.org/wiki/2019_Philadelphia_refinery_explosion">2019 Philadelphia refinery explosion - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#community impact`, `#urban planning`, `#tech policy`

---

<a id="item-17"></a>
## [US Data Centers Could Outconsume Germany and Japan in Natural Gas by 2035](https://techcrunch.com/2026/09/15/us-data-centers-could-consume-more-natural-gas-than-germany-and-japan-combined-by-2035/) ⭐️ 7.0/10

A TechCrunch report published on September 15, 2026 warns that the AI-driven buildout of US data centers could make them one of the world's largest consumers of natural gas, potentially exceeding the combined consumption of Germany and Japan by 2035. Grid-connected data centers are projected to drive an additional 15 billion cubic feet per day of natural gas demand from the power sector by the middle of the next decade. This projection links the AI boom directly to energy systems and climate policy, showing that compute growth carries physical infrastructure and emissions consequences that extend far beyond the tech industry. Utilities, grid planners, regulators, and climate policymakers will all be affected as electricity and gas demand rises faster than many forecasts anticipated. The forecast centers on roughly 15 billion cubic feet per day of additional natural gas consumption by the power sector by the mid-2030s, a figure that would put US data centers in the same league as major industrial nations. The article itself is brief and lacks technical depth, and forecasts in this space remain in flux as data center efficiency, on-site generation, and grid expansion evolve.

rss · TechCrunch · Sep 15, 18:29

**Background**: Data centers that train and run AI models require enormous amounts of electricity, and in many US regions natural gas is the fastest fuel to build new power generation around. The International Energy Agency forecasts AI electricity demand rising from 460 terawatts in 2024 to 1,000 terawatts in 2030 and 1,300 terawatts by 2035, while other analysts project data center energy demand tripling by 2035. Because grid expansion often cannot keep pace with AI infrastructure deployment, gas turbines and even on-site fuel cells are increasingly used to fill the gap.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/15/us-data-centers-could-consume-more-natural-gas-than-germany-and-japan-combined-by-2035/">US data centers could consume more natural gas than Germany ...</a></li>
<li><a href="https://altiorem.org/research/ai-data-centers-and-electricity-demand-taming-the-energy-guzzlers/">AI data centers and electricity demand : Taming the energy ... - Altiorem</a></li>
<li><a href="https://introl.com/blog/data-center-energy-demand-106gw-2035-projection">Data Center Energy Demand to Triple by 2035 | Introl Blog</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#energy consumption`, `#natural gas`, `#climate impact`

---

<a id="item-18"></a>
## [OpenAI, Anthropic, Google DeepMind Hold Weeks of AI Safety Talks](https://techcrunch.com/2026/09/15/openai-anthropic-google-have-been-in-talks-on-ai-safety-for-weeks/) ⭐️ 7.0/10

OpenAI has confirmed that it held weeks of AI safety discussions with Anthropic and Google DeepMind, marking a rare instance of direct coordination among the three leading frontier AI labs. The talks are unfolding as the Trump administration dismisses safety concerns and emphasizes keeping pace with China in the AI race. If the three largest frontier labs can align on safety norms, they could shape de facto industry standards even as the new U.S. administration signals deregulation. This matters for policymakers, regulators, and anyone affected by how advanced AI systems are governed amid U.S.-China competition. The report is brief and does not disclose the specific technical topics, participants, or outcomes of the talks, nor whether any joint commitments were reached. It also remains unclear how these voluntary discussions would interact with formal government oversight or any future regulation.

rss · TechCrunch · Sep 15, 15:47

**Background**: AI safety is an interdisciplinary field focused on preventing accidents, misuse, or other harmful consequences from AI systems, including AI alignment, risk monitoring, and robustness. Interest surged in 2023 amid rapid generative AI progress, and the U.S. and U.K. each established AI safety institutes after the 2023 AI Safety Summit. Researchers have warned that safety measures are not keeping pace with the rapid development of AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_safety">AI safety</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_intelligence_safety_institute">Artificial intelligence safety institute - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_DeepMind">Google DeepMind</a></li>

</ul>
</details>

**Tags**: `#AI Safety`, `#AI Policy`, `#OpenAI`, `#Anthropic`, `#Google DeepMind`

---

<a id="item-19"></a>
## [India to charge 0.4% merchant fee on larger UPI payments from October 15](https://techcrunch.com/2026/09/15/india-ends-free-ride-for-larger-transactions-on-its-ubiquitous-digital-payments-network/) ⭐️ 7.0/10

India will impose a 0.4% merchant discount rate (MDR) on UPI person-to-merchant transactions above Rs 2,000 starting October 15, ending six years of zero-MDR on the country's dominant digital payments network. The fee is capped at Rs 300 for payments of Rs 75,000 and above, and small vendors remain exempt. UPI is one of the world's largest real-time payment systems, processing billions of transactions a month, so introducing fees changes the economics for merchants, banks, payment apps, and fintech companies that have built businesses on free UPI payments. It could also influence how other countries designing fast payment systems think about funding their infrastructure. The fee applies only to person-to-merchant (P2M) transactions above Rs 2,000, with the charge capped at Rs 300 for payments of Rs 75,000 or more, and small vendors are exempt. The National Payments Corporation of India (NPCI) released FAQs clarifying who pays, who is exempt, and why, while peer-to-peer transfers and smaller payments remain free.

rss · TechCrunch · Sep 15, 14:22

**Background**: UPI (Unified Payments Interface) is an instant payment system and protocol developed by the National Payments Corporation of India (NPCI) in 2016. It lets users link multiple bank accounts to a single mobile app for real-time peer-to-peer and person-to-merchant payments, and it has become ubiquitous across India for everything from grocery shopping to bill payments. Until now, UPI merchant transactions carried no MDR, making digital payments free for merchants and helping drive mass adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://yourstory.com/2026/09/govt-sets-04-fee-on-upi-merchant-payments-above-rs-2000-caps-charge-at-rs-300">Govt sets 0 . 4 % fee on UPI merchant payments above Rs... | YourStory</a></li>
<li><a href="https://www.financialexpress.com/money/explainer-the-new-upi-merchant-fee-what-changes-what-doesnt-4339883/">EXPLAINER | The new UPI merchant fee ... | The Financial Express</a></li>
<li><a href="https://en.wikipedia.org/wiki/Unified_Payments_Interface">Unified Payments Interface - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#UPI`, `#digital payments`, `#India`, `#fintech`, `#policy`

---

<a id="item-20"></a>
## [SHADOW-50M: A 44M Ternary LLM Running at 1,900 tok/s on CPU](https://www.reddit.com/r/MachineLearning/comments/1wgzpli/i_trained_a_44m_parameter_quantized_llm_from/) ⭐️ 7.0/10

A developer trained SHADOW-50M, a 44M parameter ternary-weight LLM, from scratch on 45B tokens, shipping as a 19.8 MB model that runs at roughly 1,900 tokens per second on a laptop CPU and about 500 tok/s in a WebAssembly browser tab. The model uses a 73,880-token vocabulary encoded as fixed 512-bit fingerprints instead of a trained embedding, plus a 159 KB compiled kernel and an integrated calculation circuit that handles arithmetic, dates, and other operations directly in the token stream. This demonstrates that extreme quantization combined with architectural tricks can push capable language model inference onto commodity CPUs and even browsers, which matters for offline, privacy-preserving, and edge deployments where GPUs are unavailable. It also shows a path toward tiny models that can reason over retrieved records and perform exact calculations without external tool calls. SHADOW-50M uses ternary {-1, 0, +1} weights, a 4.7 MB frozen fingerprint vocabulary table, and a 22-byte-per-token disk index that stores attention states at 1 bit (288 bytes/token) so records can be retrieved in about a microsecond without re-reading text. The author openly reports that a 51.8M parameter bf16 Llama-style baseline, Supra-50M-Reasoning, beats SHADOW on standard benchmarks like ARC-Easy (0.435 vs 0.307) and WikiText-2 perplexity (165 vs 186), while SHADOW outperforms on arithmetic, date, and retrieval tasks.

reddit · r/MachineLearning · /u/Final-Data-1410 · Sep 15, 12:59

**Background**: Ternary weight quantization compresses neural network weights to just three values (-1, 0, +1), drastically reducing model size and enabling fast integer arithmetic on CPUs, though it typically degrades quality compared to higher-precision formats. Most LLMs rely on trained embedding matrices to map tokens to vectors; SHADOW replaces this with fixed 512-bit fingerprints, a novel approach that avoids storing a large embedding table. Integrated calculation circuits are a way to give small models exact arithmetic ability by routing certain token patterns to a deterministic circuit rather than relying on learned computation.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2306.17442">Designing strong baselines for ternary neural network ...</a></li>
<li><a href="https://arxiv.org/html/2407.01235v2">A Fingerprint for Large Language Models - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#edge-computing`, `#CPU-inference`, `#model-compression`

---