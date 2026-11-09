---
layout: default
title: "Horizon Summary: 2026-11-09 (EN)"
date: 2026-11-09
lang: en
---

> From 31 items, 8 important content pieces were selected

---

1. [Goldman Sachs Pulls Claude Code from Bankers and Traders](#item-1) ⭐️ 8.0/10
2. [Outlook.com Reportedly Rejects Email from Domains Without DMARC](#item-2) ⭐️ 7.0/10
3. [llama-modchip runs 284B DeepSeek on 64GB RAM without GPU](#item-3) ⭐️ 7.0/10
4. [Essay Argues Writing Is a Core Thinking Tool, Not Just a Record](#item-4) ⭐️ 7.0/10
5. [Nvidia Board Investigates Foreign Spy Targeting CEO Jensen Huang](#item-5) ⭐️ 7.0/10
6. [C64 Demo Effect Explained: Bumpmapped Rain in Lunatico](#item-6) ⭐️ 7.0/10
7. [Sem86: Full-System Emulator Without Hardcoded Semantics](#item-7) ⭐️ 7.0/10
8. [Stroustrup Advocates C++ Profiles for Safety and Simplicity](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Goldman Sachs Pulls Claude Code from Bankers and Traders](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 8.0/10

Goldman Sachs is removing Anthropic's Claude Code AI coding agent from its bankers and traders, according to a report that sparked a 328-comment Hacker News discussion. The move comes just weeks before Anthropic's IPO, which Goldman Sachs is reportedly leading. This is a high-profile example of the security, billing, and compliance hurdles that enterprises face when deploying AI coding agents, especially in regulated industries like finance. It signals that even advanced AI tools may be restricted from roles with access to sensitive data and trading systems. Claude Code is an agentic coding tool that can edit files and run commands, and its semi-unattended operation on workstations with access to client, trade, and email data creates a 'lethal trifecta' of risk. Community members also note that consumption-based billing overages and lack of normalized rates are driving some firms to alternatives like Gemini.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**Background**: Claude Code is Anthropic's agentic coding assistant that runs in the terminal or IDE, allowing developers to delegate coding tasks to an AI agent. In enterprise settings, such agents must comply with strict security and data governance policies, particularly in financial services where access to trading systems and client data is tightly controlled. The 'lethal trifecta' refers to the combination of access to private data, untrusted content, and external communication, which can enable data exfiltration.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI coding agent and assistant</a></li>
<li><a href="https://www.docker.com/blog/ai-coding-agent-horror-stories-security-risks/">AI Coding Agent Horror Stories: Security Risks Explained | Docker</a></li>
<li><a href="https://claude.com/solutions/enterprise">Claude Enterprise plan | Claude by Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that operating coding agents on finance professionals' primary machines creates unacceptable security risks, with one calling it the 'lethal trifecta.' Others highlight chronic billing overages and the appeal of flat-rate alternatives like Gemini, while some speculate that Goldman's move may be motivated by an operational loss or timing related to Anthropic's IPO.

**Tags**: `#AI`, `#enterprise`, `#security`, `#finance`, `#Claude Code`

---

<a id="item-2"></a>
## [Outlook.com Reportedly Rejects Email from Domains Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Outlook.com is reportedly rejecting email from domains that lack a DMARC record, according to a Mailroute blog post that sparked a 205-point Hacker News discussion with 165 comments. The change appears to be an operational enforcement step by Microsoft, though no official announcement has been cited. This affects anyone who sends email to Outlook.com addresses, especially self-hosters and small senders who have not yet deployed DMARC, and it signals that major mailbox providers are moving from passive filtering to active rejection of unauthenticated domains. It could accelerate DMARC adoption across the long tail of domains that have delayed implementation. Community members note that Outlook.com has long silently dropped or filtered email from certain domains and IPs even when SPF, DKIM, and DMARC were correctly configured, and that its blocklists are opaque and hard to appeal. One commenter disputes the 'quiet' framing, saying Outlook.com returns 5xx permanent delivery failures rather than silently discarding messages.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**Background**: DMARC (Domain-based Message Authentication, Reporting, and Conformance) is an email authentication protocol that builds on SPF and DKIM and tells receiving servers how to handle mail that fails authentication. SPF verifies the sending IP against DNS records, DKIM cryptographically signs messages, and DMARC requires alignment between these checks and the visible From domain. Major providers like Google and Yahoo have increasingly required DMARC for bulk senders, and Microsoft's reported enforcement extends that trend to Outlook.com.

<details><summary>References</summary>
<ul>
<li><a href="https://linuxize.com/post/email-authentication-spf-dkim-dmarc/">Email Authentication Explained: SPF, DKIM, and DMARC</a></li>
<li><a href="https://noc.org/learn/what-is-dmarc">DMARC Email Authentication Explained | NOC.org</a></li>
<li><a href="https://docs.ankiweb.net/faqs/outlook-silently-discards-email">Outlook . com silently discards email - Anki Docs</a></li>

</ul>
</details>

**Discussion**: Commenters broadly support requiring DMARC but criticize Outlook.com's opaque blocklists and silent filtering, with one self-hoster calling Outlook 'the bane of my existence' and another noting they set up DMARC over a decade ago and are surprised enforcement came so late. A minority view argues the change is overdue and that late adopters have only themselves to blame.

**Tags**: `#email`, `#dmarc`, `#deliverability`, `#self-hosting`, `#infrastructure`

---

<a id="item-3"></a>
## [llama-modchip runs 284B DeepSeek on 64GB RAM without GPU](https://github.com/synchopate/llama-modchip) ⭐️ 7.0/10

A GitHub project called llama-modchip demonstrates running a 284B-parameter DeepSeek model on a machine with 64GB of RAM and no GPU, using aggressive quantization and CPU-based inference. The project has sparked discussion on Hacker News about the feasibility of local AI on consumer hardware. This achievement pushes the boundary of what consumer hardware can run, potentially making large language models more accessible to individuals and organizations without expensive GPUs. It highlights the growing importance of quantization techniques in democratizing AI inference. The DeepSeek model is a Mixture-of-Experts (MoE) architecture with 284B total parameters but only 13B active per token, which reduces computational load. The project relies on extreme quantization (likely 1-2 bits per weight) to fit the model into 64GB of RAM, but such aggressive quantization may significantly degrade output quality.

hackernews · joshcsimmons · Nov 8, 10:22 · [Discussion](https://news.ycombinator.com/item?id=50411961)

**Background**: Quantization is a technique that reduces the precision of model weights, typically from 16-bit floating point to 8-bit or lower integers, to shrink memory usage and speed up inference. Mixture-of-Experts models activate only a subset of parameters per token, making them more efficient for inference. Running large models on CPUs with limited RAM often requires aggressive quantization and optimized runtimes like llama.cpp.

<details><summary>References</summary>
<ul>
<li><a href="https://canitrun.dev/models/deepseek-v4-flash/">DeepSeek V4 Flash 284 B VRAM Requirements: Runs on... | CanItRun</a></li>
<li><a href="https://www.ibm.com/think/topics/quantization">What is Quantization ? | IBM</a></li>
<li><a href="https://aiindigo.com/blog/running-massive-models-on-tiny-hardware-a-guide-to-local-llm-optimization">Running Massive Models on Tiny Hardware: A Guide to Local LLM…</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the project's novelty, with one noting it performs similarly to plain llama.cpp on CPU except for faster prefill. Others highlighted that quantization beyond 4-bit often leads to significant performance drops, and some criticized the project's documentation for not clearly explaining the quantization approach.

**Tags**: `#local-llm`, `#quantization`, `#deepseek`, `#consumer-hardware`, `#ai-inference`

---

<a id="item-4"></a>
## [Essay Argues Writing Is a Core Thinking Tool, Not Just a Record](http://muratbuffalo.blogspot.com/2026/11/writing-as-thinking-tool.html) ⭐️ 7.0/10

A blog post by Murat Buffalo argues that writing is not merely a way to record results but a fundamental cognitive tool that shapes and clarifies thinking. The essay sparked a Hacker News discussion with 259 points and 79 comments, where readers extended the idea to design, programming, and systems diagramming. This perspective challenges the common view that writing is just a final step in knowledge work, suggesting instead that the act of writing is integral to discovery and problem-solving. It has implications for how professionals in software engineering, design, and research approach their creative and analytical processes. The essay emphasizes that clarity of thought emerges through multiple drafts and the effort to convey ideas to others, a point echoed by commenters who note that manual coding and sketching serve similar cognitive functions. The discussion highlights that while AI tools can generate outputs, the tight loop between thinking and creating remains critical for developing insights.

hackernews · jruohonen · Nov 8, 10:41 · [Discussion](https://news.ycombinator.com/item?id=50412067)

**Background**: The idea that writing is a thinking tool is rooted in cognitive science and education theory, which hold that externalizing thoughts through language forces deeper processing and reveals gaps in understanding. In knowledge work, this concept is often applied to programming (where writing code clarifies requirements) and design (where prototyping externalizes ideas). The Hacker News discussion reflects a growing interest in how manual, craft-based activities complement or resist automation.

**Discussion**: Commenters broadly agreed with the essay, sharing personal experiences from PhD research, UX design, programming, and system diagramming to show that the act of creating—whether writing, coding, or sketching—is where insights develop. Several noted that AI prompting does not replicate the same tight loop between thinking and making, and that externalizing thoughts on paper helps clarify problems and improve recall.

**Tags**: `#writing`, `#productivity`, `#cognition`, `#software-engineering`, `#design`

---

<a id="item-5"></a>
## [Nvidia Board Investigates Foreign Spy Targeting CEO Jensen Huang](https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors) ⭐️ 7.0/10

Nvidia's board of directors announced on Sunday that it has launched an independent investigation after reports that CEO Jensen Huang was the target of a foreign intelligence operation, specifically involving his relationship with a businesswoman alleged to be a Chinese spy. The investigation raises serious questions about corporate security and export control compliance for one of the world's most valuable companies, and could have significant geopolitical and legal implications for Nvidia and the broader tech industry. The board's statement says the investigation is in light of recent reporting that Huang was the target of a foreign intelligence effort; Bloomberg reported the probe follows Huang admitting infidelity, and the case may touch on whether Nvidia's due diligence on export controls to China was compromised.

hackernews · vincentchau · Nov 8, 20:26 · [Discussion](https://news.ycombinator.com/item?id=50416801)

**Background**: Corporate espionage, also known as economic espionage, refers to the systematic and unauthorized acquisition of sensitive business information, often by state-backed actors. As CEOs of major tech companies influence decisions worth billions and shape national interests, they can become targets of foreign intelligence services seeking leverage through personal relationships.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/08/nvidia-jensen-huang-investigation-china-spy.html">Nvidia investigates CEO Jensen Huang's relationship with alleged...</a></li>
<li><a href="https://www.bbc.com/news/articles/c3dxw10rjn9no">Nvidia launches investigation into CEO's affair with suspected...</a></li>
<li><a href="https://techcrunch.com/2026/11/08/nvidia-says-its-investigating-ceo-jensen-huangs-relationship-with-possible-chinese-spy/">Nvidia will investigate CEO Jensen Huang’s relationship... | TechCrunch</a></li>

</ul>
</details>

**Discussion**: Commenters widely criticized the misleading title, clarifying that Nvidia is investigating an intelligence operation targeting Huang, not Huang himself. Many discussed the geopolitical reality that powerful CEOs are natural targets for espionage, while others raised concerns about potential export control violations and the legal risks if Huang knew the woman was a Chinese operative.

**Tags**: `#Nvidia`, `#Jensen Huang`, `#espionage`, `#corporate governance`, `#geopolitics`

---

<a id="item-6"></a>
## [C64 Demo Effect Explained: Bumpmapped Rain in Lunatico](https://www.reddit.com/r/programming/comments/1xrbciy/c64_demo_effect_explained_the_bumpmapped_rain_in/) ⭐️ 7.0/10

A technical explanation has been published detailing how the bumpmapped rain effect in the Commodore 64 demo 'Lunatico' was implemented. The breakdown highlights clever programming tricks used to achieve the effect on severely constrained hardware. This deep-dive is significant for the demoscene and retrocomputing communities, as it reveals how modern-looking effects like bumpmapping can be realized on 1980s hardware with only 64 KB of RAM and a 1 MHz CPU. It provides insight into low-level optimization techniques that continue to inspire programmers today. The effect likely relies on precomputed lookup tables, raster interrupts, and careful cycle-timing to simulate bumpmapping within the C64's limited color palette and character-based graphics. Such techniques often involve trading off resolution or color depth to maintain real-time performance.

reddit · r/programming · /u/jailbird · Nov 8, 22:43

**Background**: The Commodore 64, released in 1982, has a MOS 6510 CPU at ~1 MHz, 64 KB RAM, and a VIC-II graphics chip with a 16-color palette. Bumpmapping is a graphics technique that simulates surface relief by perturbing normals and modulating lighting, typically requiring per-pixel calculations. Demoscene programmers are known for pushing such hardware beyond its intended limits through tricks like cycle-exact coding and self-modifying code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Commodore_64_demos">Commodore 64 demos - Wikipedia</a></li>
<li><a href="https://codebase.c64.org/doku.php?id=vic:demo_programming">vic:demo_programming [Codebase64 wiki]</a></li>
<li><a href="https://demozoo.org/parties/3020/">X 2016 - Demozoo</a></li>

</ul>
</details>

**Tags**: `#demoscene`, `#Commodore 64`, `#graphics programming`, `#retrocomputing`, `#bumpmapping`

---

<a id="item-7"></a>
## [Sem86: Full-System Emulator Without Hardcoded Semantics](https://www.reddit.com/r/programming/comments/1xr4v4f/sem86_a_fullsystem_emulator_without_hardcoded/) ⭐️ 7.0/10

Sem86 is an x86 full-system emulator that loads instruction semantics at runtime from an input file, eliminating the need for hardcoded semantics in the emulator's source code. This approach, presented by the libLISA project, allows the emulator to derive instruction behavior dynamically rather than relying on manually coded logic. This novel approach could simplify the development and maintenance of emulators, making it easier to support new instruction sets or update semantics without rewriting code. It may also improve accuracy by deriving semantics from formal specifications or runtime data, impacting systems researchers and emulator developers. Sem86 is specifically an x86 emulator, and it loads semantics from an input file at runtime, which means the semantics are not hardcoded but provided as data. This design likely facilitates easier updates and customization of instruction semantics, though it may introduce performance overhead compared to hardcoded emulators.

reddit · r/programming · /u/mttd · Nov 8, 18:09

**Background**: Full-system emulators like QEMU simulate entire computer systems, allowing software designed for one architecture to run on another. Traditionally, emulators hardcode the semantics of each instruction, which is labor-intensive and error-prone. Sem86 introduces a data-driven approach where semantics are loaded at runtime, similar to how Sail provides a language for formal ISA semantics.

<details><summary>References</summary>
<ul>
<li><a href="https://liblisa.nl/publications/">Publications - libLISA</a></li>
<li><a href="https://www.qemu.org/docs/master/system/index.html">System Emulation — QEMU documentation</a></li>
<li><a href="https://www.cl.cam.ac.uk/~pes20/sail/manual.pdf">The Sail instruction -set semantics specication language</a></li>

</ul>
</details>

**Tags**: `#emulation`, `#systems`, `#formal-methods`, `#computer-architecture`, `#virtualization`

---

<a id="item-8"></a>
## [Stroustrup Advocates C++ Profiles for Safety and Simplicity](https://www.reddit.com/r/programming/comments/1xqs5vb/profiles_for_simplicity_and_guarantees_bjarne/) ⭐️ 7.0/10

Bjarne Stroustrup, the creator of C++, has presented a proposal to use profiles as a mechanism to enforce safety guarantees and improve simplicity in the language. The talk outlines how profiles can ban unsafe features and provide guarantees such as type safety, bounds safety, and lifetime safety. This matters because C++ faces increasing pressure to improve memory safety, and Stroustrup's proposal could shape the direction of C++26 and future standards. It affects all C++ developers and organizations concerned with writing safe and reliable code. Profiles are sets of rules that, when enabled, enforce specific guarantees like type safety, bounds safety, initialization safety, and lifetime safety. The proposal, detailed in papers such as P3081 and P3704, aims to define standard enforced profiles that conforming implementations must support, while allowing user-defined profiles.

reddit · r/programming · /u/_telesis · Nov 8, 06:53

**Background**: C++ is a widely used programming language known for performance and flexibility, but it also allows unsafe operations that can lead to memory errors. The C++ Core Guidelines, a collaborative effort to promote best practices, introduced the concept of profiles as a way to enforce safety rules. Profiles are designed to eliminate classes of errors by restricting or banning certain language features.

<details><summary>References</summary>
<ul>
<li><a href="https://www.infoworld.com/article/3839386/c-plus-plus-founder-champions-profiles-for-memory-safety.html">C++ founder champions profiles for memory safety | InfoWorld</a></li>
<li><a href="https://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines">C++ Core Guidelines - GitHub Pages</a></li>
<li><a href="https://isocpp.org/files/papers/P3081R2.pdf">Core safety profiles for C++26 - isocpp.org</a></li>

</ul>
</details>

**Tags**: `#C++`, `#programming languages`, `#software safety`, `#language design`, `#Bjarne Stroustrup`

---