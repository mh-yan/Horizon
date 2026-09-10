---
layout: default
title: "Horizon Summary: 2026-09-10 (EN)"
date: 2026-09-10
lang: en
---

> From 49 items, 19 important content pieces were selected

---

1. [Microsoft Designates Rust as Tier-1 Language](#item-1) ⭐️ 9.0/10
2. [Calif Research Unveils WeWorm, First Zero-Click WeChat Call Worm](#item-2) ⭐️ 9.0/10
3. [Researchers Question Whether They Can Trust OpenAI with Unpublished Math](#item-3) ⭐️ 8.0/10
4. [Forgejo 16.0.4 Fixes Critical RCE in Template Expansion](#item-4) ⭐️ 8.0/10
5. [Shopify moves back to native from React Native](#item-5) ⭐️ 8.0/10
6. [Sony faces lawsuit over digital game ownership claims](#item-6) ⭐️ 8.0/10
7. [Anthropic Alleges Distillation Attacks by Alibaba, Moonshot AI, DeepSeek](#item-7) ⭐️ 8.0/10
8. [IDScan confirms breach exposing 150 million driver's licenses](#item-8) ⭐️ 8.0/10
9. [Cognition launches SWE-2 coding model, claiming frontier parity at lower cost](#item-9) ⭐️ 7.0/10
10. [NASA Mars Color Trick Now Reveals Hidden Rock Art on Earth](#item-10) ⭐️ 7.0/10
11. [Brown Report: Silicon Valley Reshapes the Military-Industrial Complex](#item-11) ⭐️ 7.0/10
12. [Raymond Chen Reveals Windows XP's Initial User Picture Algorithm](#item-12) ⭐️ 7.0/10
13. [OpenAI Pauses Pro Subscriptions as Astra Demand Strains Systems](#item-13) ⭐️ 7.0/10
14. [Meta's AI agent Muse becomes No. 2 US app](#item-14) ⭐️ 7.0/10
15. [Proxima Fusion to build €140M factory for fusion-grade HTS tape](#item-15) ⭐️ 7.0/10
16. [Pocket FM doubles revenue run rate to $500M as AI produces 99% of new audio content](#item-16) ⭐️ 7.0/10
17. [Bending Spoons to acquire Miro for $1.36B, 90% below 2021 valuation](#item-17) ⭐️ 7.0/10
18. [Animated Explainer Scales Database Writes from 300 to 1M TPS](#item-18) ⭐️ 7.0/10
19. [Decoding the NEC V20 Microcode](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Microsoft Designates Rust as Tier-1 Language](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 9.0/10

Microsoft has officially designated Rust as a tier-1 language, placing it alongside C++ and C# in its supported language portfolio. The announcement, published as a guest post on the Rust Foundation blog, also confirms that Microsoft has replaced LLVM with MSVC's backend for Rust code generation. This is a major strategic shift for one of the world's largest software vendors, signaling that memory-safe systems programming is now a first-class priority. It could accelerate Rust adoption across the industry, influence how other OS vendors diversify their language choices, and reduce the volume of memory-safety CVEs in widely used products. Microsoft's stated goal is to convert 1 billion lines of code to Rust by 2030 using automated tooling, targeting a productivity rate of '1 engineer, 1 month, 1 million lines of code.' DARPA is also funding research with six different teams exploring automated C-to-Rust conversion, though C++ still dominates Microsoft's existing codebase after decades of development.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**Background**: Memory safety refers to a property of programming languages that prevents bugs such as use-after-free, buffer overflows, and null pointer dereferences, which are common sources of security vulnerabilities. C and C++ are not memory-safe, and Microsoft has reported that roughly 70% of its CVEs stem from memory-safety issues. Rust enforces memory safety at compile time without a garbage collector, making it an attractive alternative for systems programming.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://www.memorysafety.org/docs/memory-safety/">What is memory safety and why does it matter? - Prossimo</a></li>
<li><a href="https://blog.jetbrains.com/rust/2025/12/16/rust-vs-cpp-comparison-for-2026/">Rust VS C++ Comparison for 2026 | The RustRover Blog</a></li>

</ul>
</details>

**Discussion**: Commenters largely view this as validation of Rust's maturity, with some noting it is no longer a 'fledgling' language and now competes seriously with C++ and C#. Others highlight the strategic logic of reducing memory-safety CVEs and the significance of replacing LLVM with MSVC's backend, while pointing to Microsoft's 1-billion-line conversion goal and DARPA-funded C-to-Rust research as key context.

**Tags**: `#Rust`, `#Microsoft`, `#Systems Programming`, `#Memory Safety`, `#Language Adoption`

---

<a id="item-2"></a>
## [Calif Research Unveils WeWorm, First Zero-Click WeChat Call Worm](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research released a demo of WeWorm, the first zero-click worm that spreads through WeChat calls on both iOS and Android, hijacking accounts without any user interaction. The team used AI to find the memory-corruption bug and write a remote code execution (RCE) exploit in about two days, then built the worm in one more week. This marks a paradigm shift in AI-assisted vulnerability discovery and exploit development, showing that a small team can now build a large-scale worm in days rather than months. It raises urgent questions for mobile security, WeChat's billions of users, and AI safety, as offensive capabilities become dramatically faster and cheaper to produce. The victim does not need to answer the call or interact with the phone at all, and even if they answer, they hear nothing while the exploit still succeeds. Calif Research says it privately reported the critical vulnerability to Tencent, and the exploit targets a memory-corruption flaw in WeChat's call stack.

rss · Simon Willison · Sep 10, 00:56

**Background**: A zero-click worm spreads automatically without any action from the victim, unlike traditional malware that requires a click or download. Remote code execution (RCE) is a class of vulnerability that lets an attacker run arbitrary code on a target device, often over a network, making it one of the most severe bug categories. WeChat is a massively popular messaging and calling app in China and beyond, so a worm spreading through its call feature could reach an enormous number of users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">"Zero-click" WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://www.martincid.com/technology-sv/wechat-weworm-zero-click-worm-account-hijack/">A missed WeChat call hijacks your account — AI wrote the exploit in two days</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arbitrary_code_execution">Arbitrary code execution - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#ai`, `#mobile`, `#exploit`, `#worm`

---

<a id="item-3"></a>
## [Researchers Question Whether They Can Trust OpenAI with Unpublished Math](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

A Mathstodon post by @andreasthom sparked a debate, cross-posted to Hacker News with 544 comments, about whether mathematicians can safely share unpublished work with OpenAI after the company reportedly used insights from researcher collaborations without clear attribution. Commenters compared OpenAI to a human collaborator who takes ideas and publishes without credit, and OpenAI has admitted it cannot rule out that de-identified data derived from user interactions helped improve its models. This touches on research integrity and AI ethics: if a trillion-dollar company can absorb unpublished ideas from collaborators and publish results without credit, it could deter mathematicians from using frontier models and erode trust in industry-academia collaboration. The debate also raises broader questions about data rights, attribution norms, and whether AI-driven mathematical discovery is genuinely superhuman or partly built on researchers' fresh, unpublished insights. OpenAI reportedly gave at least 100,000 researchers free access to its models, and internal models are said to solve open problems at a surprisingly fast rate; critics note that researchers working on open problems with tools like Codex may be feeding fresh training data back to OpenAI. OpenAI has stated it "cannot rule out that de-identified data derived from their usage of our products helped improve our models," while defenders argue that large-scale reinforcement learning on verifiable math could independently discover techniques unrelated to any specific chat.

hackernews · pred_ · Sep 10, 06:49 · [Discussion](https://news.ycombinator.com/item?id=49639408)

**Background**: Mathstodon is a Mastodon instance for mathematicians, a decentralized social network where this discussion originated. OpenAI is the company behind models such as GPT and Codex, which researchers increasingly use as tools for mathematical work. Attribution is a core norm in academia: collaborators who contribute ideas are normally credited as co-authors, so applying that norm to an AI company raises novel ethical questions about data usage and credit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.banandre.com/blog/openai-navier-stokes-millennium-problem-ai-proof-controversy">OpenAI Cracked a 90-Year-Old Math Problem in 88 Hours. - Banandre</a></li>
<li><a href="https://mathstodon.xyz/">About - Mathstodon</a></li>
<li><a href="https://www.youtube.com/watch?v=2n9yfT6jvqw">AI model trained on YOUR data ? OpenAI stole credit from... - YouTube</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed the situation would be clearly unethical if OpenAI were a human collaborator, with nezi noting that giving ideas and receiving useful replies, then publishing without attribution, would be unacceptable for a person. sashank_1509 argued both things can be true: chats may improve the model's latent intuition, while RL on verifiable math may independently discover superhuman techniques. bertonvv questioned whether AI is truly racing ahead on open problems or whether researchers are inadvertently feeding it fresh training data, and nautikos2 framed the issue as part of a broader erosion of digital rights in a society where trillion-dollar companies can aggregate vast personal data.

**Tags**: `#AI ethics`, `#OpenAI`, `#research integrity`, `#mathematics`, `#attribution`

---

<a id="item-4"></a>
## [Forgejo 16.0.4 Fixes Critical RCE in Template Expansion](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo versions up to and including 16.0.3 contain a critical remote code execution vulnerability (CVE-2026-89094) related to template expansion during repository initialization, and the project released fixes in 16.0.4 (and backported to 15.0.8). The flaw allows an attacker to craft a malicious template repository whose files under .forgejo/template are processed with variable template expansion, leading to code injection. Forgejo is a widely used self-hosted Git service, so this critical RCE could let attackers execute arbitrary code on instances that process untrusted template repositories, potentially compromising the entire server. Administrators are urged to upgrade immediately to 16.0.4 or 15.0.8 to mitigate the risk. The vulnerability is tracked as CVE-2026-89094 and is rated critical; it occurs because Forgejo clones a template repository, removes the .git folder, performs variable template expansion on files listed in .forgejo/template, and then initializes a new git repository, with the expansion step mishandled. The fix is included in Forgejo 16.0.4 and backported to 15.0.8, and users should review the release notes for upgrade steps.

hackernews · weierstass · Sep 10, 15:57 · [Discussion](https://news.ycombinator.com/item?id=49645907)

**Background**: Forgejo is a community-driven fork of Gitea, a lightweight self-hosted Git service similar to GitHub. Template repositories let users create new repositories pre-populated with files and configuration, and Forgejo supports variable expansion in files under .forgejo/template to customize the generated content. A remote code execution (RCE) vulnerability means an attacker can run arbitrary commands on the server, often the most severe class of security flaw.

<details><summary>References</summary>
<ul>
<li><a href="https://vuldb.com/vuln/402227">CVE-2026-89094 Forgejo Template Expansion code injection</a></li>
<li><a href="https://cvefeed.io/vuln/detail/CVE-2026-89094">CVE-2026-89094 - Forgejo Remote Code Execution Vulnerability</a></li>
<li><a href="https://lwn.net/Articles/1093671/">Forgejo 16.0.4 and 15.0.8 address critical security vulnerability [LWN.net]</a></li>

</ul>
</details>

**Discussion**: Commenters shared the specific pull request and release notes, with one noting that Codeberg rate limits made the release notes hard to read. A Gitea project leader stated that Gitea is protected against both issues and cautioned against shaming reporters, while another commenter argued that Forgejo's ban on LLM contributions may put it at a disadvantage since attackers will use AI to find vulnerabilities.

**Tags**: `#security`, `#vulnerability`, `#forgejo`, `#git`, `#rce`

---

<a id="item-5"></a>
## [Shopify moves back to native from React Native](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify published an engineering post explaining why it moved its mobile app from React Native back to fully native iOS and Android development. The decision, shared on Shopify's engineering blog, reverses an earlier cross-platform strategy and has sparked a large debate among developers. Shopify is a major, high-profile company, so its reversal adds weight to the long-running native-versus-cross-platform debate and may influence how other engineering teams weigh framework choices. It also highlights how AI code generation is changing the economics of writing platform-specific code. The discussion around the post points to AI-assisted migration as a key factor: some developers report using tools like Codex to inventory screens from the React Native codebase and generate native iOS and Android versions in a single overnight session. The tradeoff remains that native development requires separate codebases per platform, increasing maintenance costs.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**Background**: React Native is an open-source framework, originally created by Facebook, that lets developers build Android and iOS apps using JavaScript and React, sharing much of the code across platforms. Cross-platform frameworks like React Native and Electron are often chosen to reduce headcount and reuse web developers, while native development targets a specific operating system and typically yields better platform-specific performance and polish. The native-versus-cross-platform tradeoff has been debated for nearly two decades.

<details><summary>References</summary>
<ul>
<li><a href="https://reactnative.dev/">React Native · Learn once, write anywhere</a></li>
<li><a href="https://circleci.com/blog/native-vs-cross-platform-mobile-dev/">Native vs cross-platform mobile app development - CircleCI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely frame the choice as a normal engineering tradeoff rather than a universal verdict, with one noting that companies differ in problems and resources. Several developers say AI code generation has weakened React Native's main advantage of reusing web developers, and some report migrating apps to native in a single overnight AI-assisted session. A veteran commenter warns that cross-platform teams often end up with lowest-common-denominator apps without actually saving on headcount.

**Tags**: `#react-native`, `#mobile-development`, `#native-apps`, `#engineering-decisions`, `#cross-platform`

---

<a id="item-6"></a>
## [Sony faces lawsuit over digital game ownership claims](https://consumerrights.wiki/w/Sony_PlayStation_digital_game_ownership_lawsuit) ⭐️ 8.0/10

A wiki page compiling references to Sony's claims about players "owning" their digital games has sparked a Hacker News discussion with 338 upvotes and 112 comments. The page documents Sony's legal defense in a class action lawsuit, where Sony argues that reasonable PlayStation buyers understand digital purchases are licenses, not ownership. This lawsuit could set a precedent for how digital goods are sold and represented across the gaming and media industries, affecting millions of consumers who believe they own their digital purchases. It highlights the growing tension between consumer expectations and the legal reality of digital licensing. Sony's defense cites its Terms of Service, which include a binding arbitration agreement and a class action waiver in Section 14, requiring users to opt out in writing within 30 days. The lawsuit, filed on September 10, 2026, centers on whether Sony's use of terms like "buy" and "own" misleads consumers.

hackernews · haunter · Sep 10, 12:18 · [Discussion](https://news.ycombinator.com/item?id=49642531)

**Background**: Digital storefronts like the PlayStation Store typically sell licenses to access content rather than transferring ownership of a copy. This distinction means that companies can revoke access to digital purchases, as seen in cases like McTyere v. Apple, where consumers sued over the removal of purchased content. The legal concept of ownership involves a bundle of rights, including the ability to resell or transfer, which digital licenses often do not include.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibtimes.com.au/sony-legal-battle-digital-game-ownership-disclosure-1874952">Sony Tells Court Reasonable PlayStation Buyers Know Digital Games ...</a></li>
<li><a href="https://law.vanderbilt.edu/gone-but-not-forgotten/">Gone but Not Forgotten: The Digital Ownership Dilemma and the Rise of Lost Media - Vanderbilt Law School | Vanderbilt Law School | Vanderbilt University</a></li>
<li><a href="https://news.ycombinator.com/item?id=49642531">List of references on Sony websites to players "owning" their digital games | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters debated the implications of Sony's defense, with some arguing that binding arbitration clauses unfairly strip consumers of their rights, while others compared digital purchases to physical books, noting that owning a copy does not mean owning the same copy as someone else. Some expressed ambivalence toward Sony, citing past missteps like the rootkit scandal, and questioned whether Sony's defense could backfire by undermining its own licensing model.

**Tags**: `#digital ownership`, `#consumer rights`, `#legal`, `#gaming`, `#Sony`

---

<a id="item-7"></a>
## [Anthropic Alleges Distillation Attacks by Alibaba, Moonshot AI, DeepSeek](https://techcrunch.com/2026/09/10/anthropic-details-distillation-campaigns-from-alibaba-moonshot-ai-and-deepseek/) ⭐️ 8.0/10

Anthropic released a report on Thursday alleging that China-based AI companies Alibaba, Moonshot AI, and DeepSeek have conducted persistent distillation attacks against its Claude models, with the activity escalating in recent months as competition in the AI space intensifies. The allegation escalates the debate over intellectual property protection and export controls in AI, potentially fueling regulatory scrutiny and geopolitical tensions between the U.S. and China while shaping how frontier labs defend their models. Distillation attacks involve systematically querying a proprietary model's API at scale and using the responses as training data to build a competing model, and Anthropic has previously argued such attacks reinforce the rationale for chip export controls.

rss · TechCrunch · Sep 10, 20:57

**Background**: Knowledge distillation is a standard machine learning technique that transfers knowledge from a large 'teacher' model to a smaller 'student' model, often for cheaper deployment. A distillation attack, by contrast, is when someone abuses a commercial API to extract a frontier model's capabilities without paying for the original training. Anthropic has previously accused Chinese firms such as DeepSeek and Alibaba's Qwen of distilling its Claude models, and Google DeepMind has reported similar model extraction attempts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>
<li><a href="https://blog.bibabo.ai/blog/anthropic-claude-distillation-attack-deepseek-moonshot-minimax-2026">Anthropic Exposes AI Model Distillation Attacks by DeepSeek (2026)</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#model distillation`, `#Anthropic`, `#China AI`, `#industry news`

---

<a id="item-8"></a>
## [IDScan confirms breach exposing 150 million driver's licenses](https://techcrunch.com/2026/09/10/id-verification-giant-idscan-confirms-data-breach-with-more-than-150-million-drivers-licenses-stolen/) ⭐️ 8.0/10

IDScan, a major identity verification provider, confirmed that a data breach exposed more than 150 million driver's licenses and other government-issued identity documents, including people's full names. The confirmation came about a week after an initial report alleged the company had been breached during a year-long hack. The scale and sensitivity of the leaked government-issued identity documents make this one of the largest identity-verification breaches on record, with serious implications for identity theft, fraud, and regulatory scrutiny. It also undermines trust in the third-party identity verification infrastructure that many banks, retailers, and online services rely on. The stolen data includes full names and driver's licenses as well as other government-issued identity documents, according to the company's confirmation. The breach reportedly occurred during a year-long hack, though the exact number of affected individuals and the full scope of the exposed records may still be under investigation.

rss · TechCrunch · Sep 10, 13:21

**Background**: IDScan is an identity verification company that checks government-issued documents such as driver's licenses and passports on behalf of businesses, using AI-driven authentication and biometric technologies. Identity verification providers sit in a sensitive position because they aggregate large volumes of personal identity documents, making them attractive targets for attackers. Government-issued identity documents like driver's licenses are considered primary identification documents and are widely used to prove identity for banking, travel, and online services.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/10/id-verification-giant-idscan-confirms-data-breach-with-more-than-150-million-drivers-licenses-stolen/">ID verification giant IDScan confirms data breach with... | TechCrunch</a></li>
<li><a href="https://idscan.net/about-us/">About us - IDScan .net</a></li>
<li><a href="https://en.wikipedia.org/wiki/Identity_document">Identity document - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#data-breach`, `#privacy`, `#identity-verification`, `#cybersecurity`

---

<a id="item-9"></a>
## [Cognition launches SWE-2 coding model, claiming frontier parity at lower cost](https://cognition.com/blog/swe-2) ⭐️ 7.0/10

Cognition released SWE-2, a coding model it says scores 50.0% on FrontierCode 1.1 Main, within one point of Fable 5.1 while costing up to 64-70% less, and is post-trained from Kimi K3 using RL scaled to the multi-trillion-parameter regime. The release intensifies competition among coding-model providers by pushing the capability-versus-cost Pareto frontier, but it also fuels debate over whether closed-weight models built on third-party bases can sustain an advantage as open-weight alternatives like DeepSeek improve. SWE-2 builds on Cognition's SWE-1.7 training infrastructure and recipe, with the key addition being reinforcement learning at multi-trillion-parameter scale; however, the model is closed-weight and shows a large gap between Terminal Bench 2.1 (92.8%) and the newer Terminal Bench 4 (27.3%), raising generalization concerns.

hackernews · seelos · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645443)

**Background**: Cognition is the startup behind Devin, an autonomous AI coding agent. SWE-2 is a post-trained model, meaning it starts from an existing base model (here Kimi K3) and is further trained with techniques like reinforcement learning to specialize it for coding tasks. FrontierCode and Terminal Bench are benchmarks used to compare coding models, while Fable 5.1 and GPT-Astra are recent frontier models from Anthropic and OpenAI respectively.

<details><summary>References</summary>
<ul>
<li><a href="https://cognition.com/blog/swe-2">Introducing SWE-2: Pushing the Pareto Frontier | Cognition</a></li>
<li><a href="https://officechai.com/ai/cognition-releases-swe-2-says-it-performs-close-to-frontier-at-70-lower-cost/">Cognition Releases SWE-2, Says It Performs Close To Frontier ...</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters are broadly skeptical: one highlights the huge Terminal Bench 2.1 versus 4 gap as evidence of benchmark overfitting, another recalls Cognition's past demo that went off the rails, and others question why they would choose a closed-weight model over open alternatives like DeepSeek Flash 4.1, though some note that an RL-tuned Kimi K3 reaching Fable 5-level capability is encouraging.

**Tags**: `#AI`, `#coding-models`, `#benchmarks`, `#model-release`, `#community-discussion`

---

<a id="item-10"></a>
## [NASA Mars Color Trick Now Reveals Hidden Rock Art on Earth](https://gizmodo.com/this-nasa-color-trick-was-meant-for-mars-now-its-unveiling-rock-art-on-earth-2000809844) ⭐️ 7.0/10

A NASA color-enhancement technique originally developed for analyzing Mars satellite imagery is now being applied to reveal hidden rock art on Earth. The method, detailed in a NASA Spinoff article, uses false-color composite imaging to make faint archaeological markings visible to researchers. This demonstrates how space technology can be repurposed for terrestrial archaeology, potentially uncovering previously invisible rock art and archaeological features worldwide. It highlights the broader value of NASA spinoffs and remote sensing techniques beyond their original planetary science goals. The technique involves manipulating satellite photos by enhancing color channels to detect subtle differences in vegetation or surface materials that indicate buried or faint archaeological features. Community members noted that similar results can be achieved in GIMP using LAB color decomposition and level adjustments.

hackernews · gumby · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645437)

**Background**: False-color composite imaging is a remote sensing technique where different wavelengths of light (including infrared) are assigned visible colors to highlight features not obvious to the naked eye. NASA has long used this for planetary exploration, such as mapping Mars' surface. In archaeology, it helps detect subtle ground anomalies that may indicate ancient structures or art.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sflorg.com/2022/06/arch06282201.html">Rock art detection via machine learning model a breakthrough</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences with false-color composites in GIS and remote sensing, with one calling it a 'Eureka!' moment for understanding signal processing. Others provided a GIMP method for similar enhancement and discussed the challenges of field applications, such as at Angkor Wat.

**Tags**: `#remote sensing`, `#image processing`, `#NASA spinoff`, `#archaeology`, `#false color`

---

<a id="item-11"></a>
## [Brown Report: Silicon Valley Reshapes the Military-Industrial Complex](https://costsofwar.watson.brown.edu/paper/how-big-tech-and-silicon-valley-are-transforming-military-industrial-complex) ⭐️ 7.0/10

A Brown University Costs of War report examines how big tech and Silicon Valley have become deeply intertwined with the U.S. military and intelligence apparatus, tracing the relationship from early semiconductor funding to today's AI and cloud defense contracts. The paper, which details cases like the CIA-backed seed funding of Keyhole (later Google Earth), sparked a 255-comment Hacker News debate on the ethics and history of defense work in tech. The report reframes the debate over tech's role in warfare by showing that Silicon Valley's ties to the Pentagon are not a recent development but a founding feature of the region's economy. This matters because it challenges the common narrative that big tech only recently 'sold out' to defense, and it puts pressure on engineers and companies to reckon with the historical and ethical dimensions of their work. The report highlights that Keyhole, a San Francisco startup building 3D earth models, received seed funding in 2003 from In-Q-Tel, a CIA-backed venture firm, and within two weeks its software was reportedly used by military and intelligence agencies in the Iraq war; Google acquired it the next year and renamed it Google Earth. The paper frames this as part of a century-long triad of research universities, tech companies, and the U.S. military that shaped Silicon Valley's economy and culture.

hackernews · paimapi · Sep 10, 15:47 · [Discussion](https://news.ycombinator.com/item?id=49645754)

**Background**: The term 'military-industrial complex' was popularized by President Dwight D. Eisenhower in his 1961 farewell address, warning against the unwarranted influence of the defense industry and military on public policy. Silicon Valley's origins are closely tied to defense funding: Fairchild Semiconductor, founded in Mountain View in the 1950s, sold integrated circuits to the military for missile systems, and much of the region's early growth depended on Pentagon and intelligence contracts.

<details><summary>References</summary>
<ul>
<li><a href="https://costsofwar.watson.brown.edu/sites/default/files/papers/Silicon-Valley-MIC.pdf">How Big Tech and Silicon Valley are Transforming the...</a></li>
<li><a href="https://www.britannica.com/topic/military-industrial-complex">Military - industrial complex | Definition , Elements... | Britannica</a></li>
<li><a href="https://en.wikipedia.org/wiki/Military–industrial_complex">Military – industrial complex - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were sharply divided: some argued that Silicon Valley has been Pentagon-funded from the start and that the report's framing of 'transformation' is misleading, while others insisted tech workers have a moral duty to refuse defense contracts, with one user describing quitting Microsoft over its involvement with Israeli military operations. A recurring question was whether the same technologies would have emerged under purely civilian funding, and whether it is fair to single out U.S. companies for ethical criticism.

**Tags**: `#military-industrial complex`, `#Silicon Valley`, `#ethics`, `#defense contracts`, `#tech industry`

---

<a id="item-12"></a>
## [Raymond Chen Reveals Windows XP's Initial User Picture Algorithm](https://devblogs.microsoft.com/oldnewthing/20260909-00/?p=112683) ⭐️ 7.0/10

Raymond Chen published a blog post explaining the exact algorithm Windows XP used to pick a default user picture when a new account was created, revealing that it relied on the RtlRandomEx pseudo-random number generator seeded with GetTickCount(). The post also notes that the function used a one-pass random selection algorithm, and community members quickly linked to the actual leaked Windows XP source code implementing it. This deep-dive offers a rare, authoritative look into Windows XP internals from a longtime Microsoft engineer, satisfying ongoing curiosity about how everyday OS behaviors were implemented. It also illustrates a broader lesson in software design: true randomness is hard for computers, so developers rely on deterministic pseudo-random generators seeded by system state. The algorithm used RtlRandomEx with the current GetTickCount() value as its initial seed, and Chen highlights that the one-pass selection approach has at least two benefits, though the post does not enumerate all of them. Because GetTickCount() is based on system uptime, the seed is predictable, meaning the chosen picture is not truly random.

hackernews · soheilpro · Sep 10, 09:04 · [Discussion](https://news.ycombinator.com/item?id=49640646)

**Background**: Windows XP introduced a welcome screen where each user account could display a small picture, and new accounts were automatically assigned one from a built-in set. RtlRandomEx is a Windows runtime library function that generates pseudo-random numbers, while GetTickCount() returns the number of milliseconds since the system started. Pseudo-random generators are deterministic algorithms that produce repeatable sequences from a seed, which is why they are not suitable for security-sensitive randomness.

<details><summary>References</summary>
<ul>
<li><a href="https://devblogs.microsoft.com/oldnewthing/20260909-00/?p=112683">What algorithm did Windows XP use to choose your initial user ...</a></li>
<li><a href="https://saw-tools.me/en/computing-randomness-guide.html">Randomness in computing : PRNG, CSPRNG — SAW TOOLS</a></li>

</ul>
</details>

**Discussion**: Commenters expressed appreciation for Chen's Windows internals posts, with one calling each one 'a little Xmas,' and another sharing a link to the actual leaked source code. A recurring theme was the cognitive gap between human and computer randomness: humans can casually grab one item from a pile, but computers must count and select algorithmically. Some also noted that in day-to-day work, developers often lack the awareness or discipline to consider such subtle implications.

**Tags**: `#Windows XP`, `#algorithms`, `#software history`, `#Raymond Chen`, `#randomness`

---

<a id="item-13"></a>
## [OpenAI Pauses Pro Subscriptions as Astra Demand Strains Systems](https://techcrunch.com/2026/09/10/openai-puts-pro-subscriptions-on-hold-due-to-astra-demand/) ⭐️ 7.0/10

OpenAI has paused new sign-ups for its Pro subscription tier, saying Pro puts the most strain on its systems, and will resume sales only after adding more capacity. The pause comes amid surging demand tied to its new Astra model, which the company has been rolling out to users. This signals unusually strong market traction for Astra and shows that even a leading AI lab can be constrained by compute and serving capacity. The pause could limit access for power users and researchers, and it highlights how infrastructure, not just model quality, shapes competition in the AI industry. OpenAI specifically identified the Pro tier as the heaviest load on its systems, implying that higher-usage power-user plans consume disproportionate compute. The company did not give a timeline for resuming sign-ups, only saying it is adding capacity first.

rss · TechCrunch · Sep 10, 20:59

**Background**: OpenAI's Pro subscription is positioned for power users such as researchers, domain experts, and professionals working on large projects, and it typically offers higher usage limits than standard plans. Astra is OpenAI's newly introduced frontier model, described as its most intelligent and aligned model yet, with strong capabilities in coding, computer use, cybersecurity, and science. Reports also note that an unreleased version of Astra solved ten long-open math problems, further fueling interest.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT-6 Astra : A new generation of intelligence | OpenAI</a></li>
<li><a href="https://medium.com/@SPX701/is-the-openai-pro-subscription-worth-the-price-86a0b1fc9f91">Is the OpenAI Pro Subscription worth the price? | by SPX | Medium</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lwMWZQZEVSRndyd19YMUxTMHRTZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Google News - OpenAI Astra model solves ten unsolved math...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Astra`, `#AI industry`, `#subscriptions`, `#infrastructure`

---

<a id="item-14"></a>
## [Meta's AI agent Muse becomes No. 2 US app](https://techcrunch.com/2026/09/10/metas-ai-agent-muse-is-now-the-no-2-app-in-the-us/) ⭐️ 7.0/10

Meta's new personal AI agent app Muse has climbed to the No. 2 spot in the US app rankings, though its early growth is slower than Meta's previous launches such as Meta AI and Threads. Muse rolled out in September 2026 for iOS and Android users via a dedicated app and the Muse.ai website. A major tech company's AI agent app reaching the No. 2 spot in the US signals that AI agents are moving into mainstream consumer adoption, which could reshape competitive dynamics and product strategy across the AI assistant market. It also puts pressure on rivals like OpenAI and Google to accelerate their own agent offerings. Muse is described as a personal AI agent that does the work rather than just answering questions, connecting to Facebook, Instagram, and third-party apps such as Spotify and OpenTable. Meta is positioning it as the first AI agent covered by Link's purchase protections for agents, which guarantees no-fee returns, and is emphasizing security and privacy features to differentiate itself despite being late to the personal agent market.

rss · TechCrunch · Sep 10, 19:50

**Background**: An AI agent is a system that can autonomously carry out multi-step tasks on a user's behalf, such as sending emails or making bookings, rather than only generating text responses. Meta previously launched Meta AI, its general assistant, and Threads, its text-based social network, both of which grew quickly after launch. Muse represents Meta's entry into the more competitive personal agent space, where it is trying to catch up with earlier movers.

<details><summary>References</summary>
<ul>
<li><a href="https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/">Introducing Muse : The World’s First Personal AI Agent Built for...</a></li>
<li><a href="https://9to5mac.com/2026/09/08/meta-ai-launches-muse-personal-agent-including-a-new-mobile-app-for-iphone/">Meta AI launches Muse personal agent , including a new mobile app ...</a></li>
<li><a href="https://www.wired.com/story/meta-releases-muse-a-personal-ai-agent-with-privacy-built-into-it/">Muse , Meta ’s New Personal AI Agent , Needs You to Trust It | WIRED</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Meta`, `#consumer apps`, `#product adoption`, `#tech industry`

---

<a id="item-15"></a>
## [Proxima Fusion to build €140M factory for fusion-grade HTS tape](https://techcrunch.com/2026/09/10/proxima-fusion-bets-e140m-on-a-critical-fusion-ingredient-dominated-by-asian-suppliers/) ⭐️ 7.0/10

Proxima Fusion announced on Wednesday that it plans to build a €140 million ($162.6 million) factory to produce fusion-grade high-temperature superconducting (HTS) tape, a key component for its stellarator reactor design. The facility is intended to secure the startup's supply of HTS tape, which is currently dominated by Asian suppliers. This investment could reduce Europe's reliance on Asian suppliers for a critical fusion component and help localize the HTS tape supply chain, which is essential for commercializing fusion energy. It also signals growing confidence in stellarator designs and could accelerate timelines for fusion startups aiming to demonstrate net energy gain. HTS tape allows fusion magnets to operate at higher temperatures, greatly reducing cooling requirements, and a single reactor like SPARC may need up to 10,000 kilometers of tape. Proxima Fusion aims to build its demonstration stellarator, Alpha, by 2031, with the new factory intended to supply the tape needed for that reactor.

rss · TechCrunch · Sep 10, 18:38

**Background**: High-temperature superconducting tape is a key enabling technology for compact fusion reactors because it can carry large currents and generate strong magnetic fields at higher temperatures than conventional superconductors. Proxima Fusion is a German startup developing a stellarator, a twisted magnetic confinement design that differs from the more common tokamak. The company is targeting a demonstration stellarator called Alpha by 2031 to show net fusion energy in continuous operation.

<details><summary>References</summary>
<ul>
<li><a href="https://energy.mit.edu/news/pushing-the-envelope-with-fusion-magnets/">Pushing the envelope with fusion magnets | MIT Energy Initiative</a></li>
<li><a href="https://www.nucnet.org/news/german-startup-unveils-design-for-world-s-most-viable-commercial-nuclear-fusion-plant-2-4-2025">Proxima Fusion on track to build demonstration stellarator by 2031</a></li>
<li><a href="https://www.world-nuclear-news.org/articles/german-stellarator-fusion-design-concept-unveiled">German stellarator fusion design concept... - World Nuclear News</a></li>

</ul>
</details>

**Tags**: `#fusion energy`, `#superconductors`, `#supply chain`, `#clean tech`, `#manufacturing`

---

<a id="item-16"></a>
## [Pocket FM doubles revenue run rate to $500M as AI produces 99% of new audio content](https://techcrunch.com/2026/09/10/indias-pocket-fm-doubles-revenue-run-rate-to-500m-as-ai-powers-93-of-audio-content/) ⭐️ 7.0/10

Pocket FM, the Indian serialized audio storytelling platform launched in 2018, has doubled its annualized revenue run rate to $500 million, with AI now generating 93% of its content catalog and 99% of all new material. The company says AI has cut content production costs by roughly 80 times, while human creators still supply the underlying ideas and storytelling. This is one of the largest-scale commercial validations yet of generative AI in media, showing that AI-driven production can roughly double revenue while slashing costs at a company with a global audio audience. It signals that AI cost curves may reshape the economics of entertainment content, pressuring traditional studios and other audio platforms to adopt similar pipelines. The 93% figure refers to the share of Pocket FM's existing catalog produced with AI, while 99% applies to newly created content; the roughly 80x cost reduction is the company's own claim and has not been independently audited. Pocket FM still relies on human creators for ideas and storytelling, using AI mainly to convert scripts into finished audio at scale, reportedly in partnership with voice AI provider ElevenLabs.

rss · TechCrunch · Sep 10, 17:45

**Background**: Pocket FM is an Indian audio entertainment app that publishes serialized fiction in an episodic, "audio series" format, similar to podcasts but scripted and dramatized. Revenue run rate is a metric that annualizes a company's most recent monthly or quarterly revenue to estimate full-year performance, assuming current trends continue; it can be inflated by one-time revenue and is not the same as audited annual revenue. Generative AI audio tools can now synthesize realistic speech, sound effects, and music, allowing media companies to produce content far faster and cheaper than traditional recording workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/10/indias-pocket-fm-doubles-revenue-run-rate-to-500m-as-ai-powers-93-of-audio-content/">India's Pocket FM doubles revenue run rate to $500M as AI powers 93...</a></li>
<li><a href="https://chang.aevumnews.com/en/pocket-fm-ai-powered-audio-storytelling-reaches-500m-revenue-milestone">Pocket FM : AI -Powered Audio Storytelling Reaches $500M Revenue...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#generative-ai`, `#audio-content`, `#media-tech`, `#business`

---

<a id="item-17"></a>
## [Bending Spoons to acquire Miro for $1.36B, 90% below 2021 valuation](https://techcrunch.com/2026/09/10/bending-spoons-to-buy-collaboration-tools-maker-miro-for-1-36b-90-less-than-its-2022-valuation/) ⭐️ 7.0/10

Bending Spoons has agreed to acquire workplace collaboration platform Miro for $1.36 billion, a roughly 90% decline from Miro's late-2021 valuation of $17.5 billion. The deal marks one of the steepest valuation markdowns for a well-known SaaS startup of the pandemic-era boom. The deal underscores how far once-high-flying SaaS valuations have fallen and signals that consolidation is accelerating as acquirers like Bending Spoons snap up established products at steep discounts. It affects Miro's 90 million-plus users, its investors, and founders tracking exit expectations in the collaboration software market. Miro's platform serves over 90 million users and more than 250,000 organizations as of 2025, and Bending Spoons plans to manage it for long-term ownership rather than flip it. The buyer, an Italian technology conglomerate, has already acquired Airtable, AOL, Eventbrite, Vimeo, Evernote, Meetup, Remini, Splice, and WeTransfer, and filed for a U.S. IPO in June 2026.

rss · TechCrunch · Sep 10, 14:34

**Background**: Miro is an AI-powered visual collaboration platform that functions as an online whiteboard, used by distributed teams for brainstorming, agile planning, customer journey mapping, product design, and remote workshops. Bending Spoons, founded in Milan in 2013, is a technology conglomerate that buys apps with existing product-market fit and manages them for long-term ownership, often increasing revenue and lowering expenses. Miro's $17.5 billion valuation came during the 2021 venture funding peak, before a broad startup valuation downturn that began in 2022.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bending_Spoons">Bending Spoons - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Miro_(collaboration_platform)">Miro (collaboration platform)</a></li>
<li><a href="https://fortune.com/2026/06/08/bending-spoons-italian-aol-evernote-wetransfer-files-us-ipo/">Bending Spoons, the Italian app acquirer behind AOL, Evernote, Vimeo, and WeTransfer, files for a U.S. IPO | Fortune</a></li>

</ul>
</details>

**Tags**: `#acquisitions`, `#saas`, `#startups`, `#tech-industry`, `#valuation`

---

<a id="item-18"></a>
## [Animated Explainer Scales Database Writes from 300 to 1M TPS](https://www.reddit.com/r/programming/comments/1wch6vw/the_physics_of_database_speed_from_300_to_1m/) ⭐️ 7.0/10

A 19-minute animated explainer video, submitted to r/programming by /u/tanayvk, walks through low-level database concepts, identifies performance bottlenecks, runs benchmarks, and demonstrates optimization techniques that scale write throughput from 300 to 1 million transactions per second. Write throughput is a critical constraint for modern write-heavy workloads such as telemetry pipelines and real-time analytics, so a clear, visual walkthrough of how to reach 1M TPS helps engineers understand where bottlenecks actually live and how to address them systematically. The video focuses specifically on write throughput optimization and uses benchmarks to demonstrate each step, though the summary does not specify which database engine, hardware, or benchmark tool was used, so the 1M TPS figure should be interpreted in the context of the presenter's setup.

reddit · r/programming · /u/tanayvk · Sep 10, 12:01

**Background**: Databases process transactions, and throughput is measured in transactions per second (TPS). Traditional B-tree storage engines can struggle under write-intensive workloads because each insert may trigger costly random disk writes, which is why techniques like log-structured merge (LSM) trees and careful indexing are often discussed when optimizing write-heavy systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/martinuke0_optimizing-write-throughput-with-log-structured-activity-7460343598882979840-B1q0">Optimizing Write Throughput with Log-Structured Merge... | LinkedIn</a></li>
<li><a href="https://milvus.io/ai-quick-reference/what-are-the-key-metrics-for-benchmarking-databases">What are the key metrics for benchmarking databases ?</a></li>

</ul>
</details>

**Tags**: `#databases`, `#performance`, `#benchmarking`, `#optimization`, `#systems`

---

<a id="item-19"></a>
## [Decoding the NEC V20 Microcode](https://www.reddit.com/r/programming/comments/1wc3hjq/decoding_the_nec_v20_microcode/) ⭐️ 7.0/10

A new technical deep-dive explores the microcode inside the NEC V20 processor, detailing how it was decoded and what it reveals about this classic x86-compatible chip. The analysis focuses on reverse-engineering the internal microcode that drives the V20's instruction execution. This work is significant for retrocomputing and systems enthusiasts because the NEC V20 was a historically important chip that helped establish Japan's semiconductor industry through reverse-engineering rather than licensing. Understanding its microcode provides insight into early x86-compatible design and low-level hardware analysis techniques. The NEC V20 is pin-compatible and object-code compatible with the Intel 8088, featuring an instruction set architecture similar to the Intel 80188 with some extensions. The decoding effort likely involved extracting and analyzing the microcode ROM to understand how instructions are translated into internal operations.

reddit · r/programming · /u/self · Sep 10, 00:30

**Background**: The NEC V20 is a 16-bit CMOS microprocessor with an 8-bit external data bus, designed by NEC as their first venture into reverse-engineering an Intel microprocessor instead of licensing the design. It was object-code and pin-compatible with the Intel 8088, meaning it could run the same software and fit into the same sockets. Microcode is the low-level layer of instructions inside a CPU that implements the higher-level machine instructions, and reverse-engineering it reveals how the processor actually works internally.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NEC_V20">NEC V20 - Wikipedia</a></li>
<li><a href="https://micro.magnet.fsu.edu/optics/olympusmicd/galleries/chips/necv20low.html">Molecular Expressions: Science, Optics & You - Olympus MIC-D: Integrated Circuit Gallery - NEC V20 Microprocessor</a></li>
<li><a href="https://www.cpu-world.com/CPUs/V20/index.html">NEC V20 processor family</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#microcode`, `#NEC V20`, `#retrocomputing`, `#hardware`

---