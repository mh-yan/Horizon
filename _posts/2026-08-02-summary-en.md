---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 24 items, 9 important content pieces were selected

---

1. [Karpathy's Pelican Benchmark Sparks Debate on AI Physical Understanding](#item-1) ⭐️ 8.0/10
2. [Kakehashi: Run macOS Binaries on Linux ARM](#item-2) ⭐️ 8.0/10
3. [Open Letters Debate Open-Weight AI Models](#item-3) ⭐️ 8.0/10
4. [NIST Releases First Post-Quantum Encryption Standards to Protect Against Quantum Threats](#item-4) ⭐️ 8.0/10
5. [F*: A General-Purpose Proof-Oriented Programming Language Gains Attention](#item-5) ⭐️ 7.0/10
6. [How Essential English Vocabulary for Learners Has Shifted Since 1953](#item-6) ⭐️ 7.0/10
7. [Bor: Open-Source Policy Management for Linux Desktops](#item-7) ⭐️ 7.0/10
8. [Universal Computing with echo, ed, test, and exec](#item-8) ⭐️ 7.0/10
9. [Building Raft Leader Election from Scratch: A Hands-On Tutorial](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Karpathy's Pelican Benchmark Sparks Debate on AI Physical Understanding](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

Andrej Karpathy highlighted the 'pelican on a bicycle' prompt as a new benchmark for AI models' understanding of the physical world, sparking a debate about evaluation methods and quality standards. The discussion, with 304 points and 238 comments, centers on whether such informal benchmarks are valid and whether AI progress is being overstated. This matters because it highlights a shift in how AI models are evaluated, moving beyond simple image generation to more complex tasks that test physical world understanding. The debate influences how the AI community measures progress and sets quality expectations, potentially shaping future benchmark development and model training priorities. The benchmark originates from a prompt by Simon Willison in late 2024: 'Generate an SVG of a pelican riding a bicycle.' It has been used to test models like GPT-4 and Claude, with some evidence suggesting labs may be 'pelicanmaxxing'—training specifically on this benchmark—though a July 2026 study found no significant effect.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: The 'pelican on a bicycle' benchmark is an informal test for large language models (LLMs) that evaluates their ability to generate code (SVG) that accurately depicts a complex scene, requiring understanding of object relationships and physical plausibility. It gained traction as a way to compare model capabilities beyond simple text generation, and has been featured in tools like Hugging Face spaces and GitHub galleries.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://dylancastillo.co/posts/pelicanmaxxing.html">Are AI labs pelicanmaxxing? – Dylan Castillo</a></li>
<li><a href="https://huggingface.co/spaces/victor/pelican-benchmark">Pelican Benchmark - a Hugging Face Space by victor</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some argued the benchmark is useful for measuring progress, while others criticized it for being subjective and potentially overhyped. Concerns were raised about AI content raising expectations for speed and volume but lowering quality standards, and some noted that models may be specifically trained on three.js code, making animations less indicative of general understanding.

**Tags**: `#AI`, `#benchmarking`, `#Karpathy`, `#physical understanding`, `#model evaluation`

---

<a id="item-2"></a>
## [Kakehashi: Run macOS Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi is an experimental userspace translation layer that enables macOS ARM64 binaries to run natively on Linux aarch64, with working prototypes for 7-Zip, curl, and Xcode's Git. It loads Darwin Mach-O binaries, maps a freestanding libSystem, and translates BSD syscalls without using a JIT. This project addresses a significant technical challenge in cross-OS binary compatibility, potentially enabling macOS command-line tools to run on Linux ARM hardware like Apple Silicon Macs running Asahi Linux. It could foster a broader ecosystem where macOS software becomes accessible on Linux, similar to how Wine/Proton did for Windows applications. The project is CLI-first and does not use JIT compilation; it translates BSD syscalls and maps a freestanding libSystem. Current performance shows 7-Zip is about 5.2x slower than native Linux execution, but the author has an optimization plan to reduce this gap.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Background**: Running macOS binaries on non-Apple hardware has been a long-standing challenge. Darling is a similar project that aims to provide a compatibility layer for macOS on Linux, but it has an open PR for ARM64 support. Asahi Linux is a project that ports Linux to Apple Silicon Macs, which could benefit from such a translation layer.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">wie-project/kakehashi: Userspace macOS translation layer for Linux ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49145937">Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asahi_Linux">Asahi Linux - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community shows strong interest, with comments referencing the Darling project and suggesting potential collaboration. Some express cautious optimism, noting the project is still early, while others see potential for applications like yabridge to run AU binaries on Linux.

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#binary compatibility`, `#reverse engineering`

---

<a id="item-3"></a>
## [Open Letters Debate Open-Weight AI Models](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

In late July 2026, Microsoft spearheaded an open letter signed by 235 AI companies, including NVIDIA and OpenAI, advocating for open-weight AI models. Anthropic and a group of 1,324 frontier AI employees published separate responses, with the latter calling for international efforts to pace AI development. This debate highlights a growing policy rift over AI governance, with major industry players publicly clashing on open-weight models' safety and innovation trade-offs. The outcome could shape future US regulations and global AI competition, affecting developers, researchers, and national security. Microsoft's letter explicitly supports distillation, a technique where models train on other models' outputs, countering potential misappropriation concerns. Anthropic notably did not sign and instead published its own position, warning of risks from authoritarian governments and calling for a crackdown on industrial-scale distillation, while denying advocacy for a ban.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open-weight models are AI models whose core components, including trained weights, are publicly released, allowing anyone to download and use them. This contrasts with closed models, which are kept proprietary. The debate centers on balancing innovation and transparency against potential misuse and national security risks, especially as AI capabilities advance rapidly.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.anthropic.com/news/position-open-weights-models">Our position on open-weights models \ Anthropic</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#policy`, `#industry`, `#governance`

---

<a id="item-4"></a>
## [NIST Releases First Post-Quantum Encryption Standards to Protect Against Quantum Threats](https://www.reddit.com/r/programming/comments/1vd7jnr/quantum_computers_may_put_internet_traffic_at/) ⭐️ 8.0/10

NIST has released the first three finalized post-quantum encryption standards, which are now ready for immediate use. These standards are designed to protect internet traffic from the future threat of quantum computers. This is a significant milestone in cybersecurity, as current encryption methods like RSA and ECC are vulnerable to quantum attacks. The new standards will help organizations and governments migrate to quantum-resistant cryptography, ensuring long-term data security. The three standards include algorithms for encryption and digital signatures, such as ML-KEM (based on lattice cryptography) and ML-DSA. They are specified in Federal Information Processing Standards (FIPS), which are mandatory for U.S. federal systems and widely adopted globally.

reddit · r/programming · /u/donutloop · Aug 2, 03:53

**Background**: Post-quantum cryptography (PQC) refers to cryptographic algorithms believed to be secure against quantum computer attacks. Current public-key algorithms rely on mathematical problems that quantum computers could solve efficiently using Shor's algorithm. NIST's standardization process began in 2016, and these first standards are the result of a multi-year competition and evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://www.nist.gov/news-events/news/2024/08/nist-releases-first-3-finalized-post-quantum-encryption-standards">NIST Releases First 3 Finalized Post-Quantum Encryption Standards | NIST</a></li>
<li><a href="https://csrc.nist.gov/projects/post-quantum-cryptography">Post-Quantum Cryptography | CSRC | CSRC</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#cryptography`, `#NIST`, `#internet security`, `#post-quantum`

---

<a id="item-5"></a>
## [F*: A General-Purpose Proof-Oriented Programming Language Gains Attention](https://fstar-lang.org/) ⭐️ 7.0/10

F*, a general-purpose proof-oriented programming language for verifying software, has recently gained traction in online communities, with discussions highlighting its syntax, industrial use, and potential for formal verification. The language supports both purely functional and effectful programming, enabling developers to write and verify code within a single framework. F* is significant because it bridges the gap between programming and formal verification, allowing developers to prove properties of their code at compile time, which can greatly enhance software reliability and security. Its adoption in industry and academia could lead to more verified systems, especially in critical domains like cryptography and protocol implementation. F* is developed by Microsoft Research and Inria, and it integrates SMT-based automated reasoning with dependent types, allowing for both automated and interactive proofs. It has been used in real-world projects like the Everest project, which aims to produce verified HTTPS stack components, and it supports extraction to OCaml, F#, C, and WebAssembly.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Proof-oriented programming languages like F* allow developers to write specifications alongside code and use automated theorem provers to verify correctness. This is part of the broader field of formal verification, which uses mathematical methods to ensure software behaves as intended. F* is particularly notable for its ability to handle effectful programs and its integration with existing languages, making it practical for incremental adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language) - Wikipedia</a></li>
<li><a href="https://fstar-lang.org/">F*: A Proof-Oriented Programming Language</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/1hmeqec/f_a_generalpurpose_prooforiented_programming/">r/programming on Reddit: F* : A general-purpose proof-oriented programming language</a></li>

</ul>
</details>

**Discussion**: The community discussion shows a mix of interest and critique. Some users praised F* for its ability to express external library calls and incremental migration from C, while others criticized the lack of code examples on the homepage, making it hard to quickly grasp the syntax. There were also questions about its industrial usage and comparisons to Haskell, indicating both curiosity and a desire for more accessible documentation.

**Tags**: `#proof-oriented`, `#formal verification`, `#programming language`, `#functional programming`, `#security`

---

<a id="item-6"></a>
## [How Essential English Vocabulary for Learners Has Shifted Since 1953](https://pudding.cool/2026/07/essential-words/) ⭐️ 7.0/10

The Pudding published a data-driven analysis showing how the essential vocabulary taught to English language learners has changed from 1953 to 2023, revealing a shift from personal virtues like 'humble' and 'loyalty' to broader social identities like 'community' and 'gender'. This analysis highlights how language education reflects and shapes cultural values, offering insights for educators, linguists, and policymakers. It also sparks discussion about inequality and the evolving nature of social belonging in a globalized world. The 'Social-Communicative' level of vocabulary barely changed in size, but nearly a quarter of the 1953 words are gone, and 39% of the 2023 words are new. The shift includes words like 'humble', 'loyalty', 'fellowship', 'generous', 'polite', and 'companionship' being replaced by 'community', 'identity', 'organization', 'ethnic', 'gender', and 'narrative'.

hackernews · c-oreills · Aug 2, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49145590)

**Background**: English language teaching often relies on curated vocabulary lists to guide learners. This analysis compares lists from 1953 and 2023 to track cultural shifts. The change from personal virtues to social identities may reflect broader societal trends toward individualism and group affiliation.

**Discussion**: Commenters discussed the difficulty of creating universal vocabulary lists, noting that the purpose of learning (travel, TV, newspapers) greatly affects word choice. Some linked the shift to inequality and 'tribalization', while others debated language change and the challenges of building such lists.

**Tags**: `#linguistics`, `#education`, `#language learning`, `#cultural change`, `#data analysis`

---

<a id="item-7"></a>
## [Bor: Open-Source Policy Management for Linux Desktops](https://getbor.dev/blog/2026-08-02-bor-v080-release/) ⭐️ 7.0/10

Bor, an open-source centralized policy management system for Linux desktops, released version 0.8, adding support for Thunderbird, Microsoft Edge for Business, and FirewallD zones, along with various improvements and fixes. This release expands Bor's coverage to more applications and system components, making it a more viable solution for organizations managing Linux workstations. It addresses a gap in Linux desktop management, offering a modern, real-time alternative to manual configuration or legacy tools. Bor uses a lightweight Go agent and a central server, streaming policies over mTLS/gRPC in real time without polling. Version 0.8 introduces new policy types for Thunderbird, Microsoft Edge for Business, and FirewallD zones, and the project is open-source with active community engagement.

hackernews · eniac111 · Aug 2, 09:06 · [Discussion](https://news.ycombinator.com/item?id=49142569)

**Background**: Policy management for Linux desktops typically involves manual configuration or tools like Ansible, which lack real-time enforcement. Bor aims to provide a centralized, real-time policy distribution system similar to Microsoft Intune or Group Policy for Windows, but tailored for Linux. It supports various desktop environments and system components, including Firefox, Chrome, KDE, dconf, polkit, and package management.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/neibla/streaming-grpc-with-mtls">GitHub - neibla/ streaming - grpc -with- mtls : Demo Golang project with...</a></li>
<li><a href="https://asoasis.tech/articles/2026-03-20-0254-grpc-streaming-api-tutorial/">gRPC Streaming API Tutorial: Server... | ASOasis - All about Tech</a></li>
<li><a href="https://firewalld.org/documentation/zone/">Documentation - Zone | firewalld</a></li>

</ul>
</details>

**Discussion**: Community members expressed interest in Bor for managing Linux laptops, especially for non-profits, and asked about custom script execution, user mapping with identity providers like Authentik, and comparisons to existing solutions. Some questioned the choice of mTLS over SSH, and others asked about configuration drift handling without polling.

**Tags**: `#Linux`, `#desktop management`, `#open-source`, `#policy management`, `#gRPC`

---

<a id="item-8"></a>
## [Universal Computing with echo, ed, test, and exec](https://www.reddit.com/r/programming/comments/1vdiryk/an_unexpected_computer_universal_computing_with/) ⭐️ 7.0/10

A paper published in PagedOut #9 demonstrates that universal computation can be achieved using only the Unix commands echo, ed, test, and exec. This is a novel and clever exploration of the computational power of basic Unix utilities. This finding is significant because it shows that even the most basic Unix tools can be combined to form a Turing-complete system, highlighting the inherent computational power of Unix-like environments. It is likely to appeal to systems programmers and enthusiasts of esoteric programming and computational theory. The paper is part of PagedOut #9, a free experimental magazine that features one-article-per-page technical content. The specific techniques used to achieve universality are not detailed in the provided content, but the combination of these four commands is sufficient to simulate any Turing machine.

reddit · r/programming · /u/Dull_Replacement8890 · Aug 2, 13:57

**Background**: Universal computation, or Turing completeness, refers to a system's ability to simulate any Turing machine, which is a theoretical model of computation. In practice, many programming languages and instruction sets are Turing-complete, but demonstrating this for a minimal set of Unix commands is a non-trivial and interesting exercise. Unix commands like echo, ed, test, and exec are typically used for simple file operations, text editing, condition testing, and process execution, respectively, but their combination can yield surprising computational power.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turing_completeness">Turing completeness - Wikipedia</a></li>
<li><a href="https://pagedout.institute/">Paged Out !</a></li>

</ul>
</details>

**Tags**: `#unix`, `#computing theory`, `#esoteric programming`, `#systems programming`

---

<a id="item-9"></a>
## [Building Raft Leader Election from Scratch: A Hands-On Tutorial](https://www.reddit.com/r/programming/comments/1vd9q70/understanding_raft_leader_election_by_building/) ⭐️ 7.0/10

A Reddit post shares a hands-on tutorial that guides readers through implementing Raft leader election from scratch, offering a practical deep-dive into the core consensus mechanism. This tutorial helps developers and students understand Raft's leader election, a fundamental concept in distributed systems, by building it themselves. It addresses the common difficulty of grasping consensus algorithms and provides a valuable learning resource for the community. The tutorial likely covers key Raft concepts such as terms, election timeouts, and RequestVote RPCs, and may include code examples in a specific language. It emphasizes practical implementation over theoretical explanation, making it suitable for hands-on learners.

reddit · r/programming · /u/Sushant098123 · Aug 2, 05:47

**Background**: Raft is a consensus algorithm designed to be more understandable than Paxos, decomposing consensus into leader election, log replication, and safety. In leader election, nodes start as followers, and if they don't receive heartbeats from a leader within a timeout, they become candidates and request votes from other nodes. A candidate wins if it receives votes from a majority of nodes, ensuring a single leader per term.

<details><summary>References</summary>
<ul>
<li><a href="https://prateek-gupta.medium.com/raft-consensus-algorithm-fc2de6852d9">Raft Consensus algorithm . Raft is the way to achieve... | Medium</a></li>
<li><a href="https://codefarm.in/guides/system-design/04-core-algorithms/raft-consensus">Raft Consensus Algorithm : Leader Election , Log... — codefarm</a></li>
<li><a href="https://medium.com/@mohllal/implementing-raft-part-2-leader-election-655b7a244847">Implementing Raft, Part 2: Leader Election | by Kareem Mohllal | Medium</a></li>

</ul>
</details>

**Tags**: `#distributed systems`, `#Raft`, `#consensus`, `#tutorial`

---