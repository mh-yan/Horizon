---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 36 items, 15 important content pieces were selected

---

1. [Scott Aaronson Sounds Alarm on AI's Mathematical Breakthroughs](#item-1) ⭐️ 9.0/10
2. [1Password Discloses Incident: Compromised Laptop Led to Malicious Code Push](#item-2) ⭐️ 8.0/10
3. [Lean verification of GRH shrinks from 17M to 76k lines](#item-3) ⭐️ 8.0/10
4. [Polynomial Hirsch Conjecture Disproved by New Preprint](#item-4) ⭐️ 8.0/10
5. [Google Research Releases Cogentic Papers on Integer Factorization and Discrete Logs](#item-5) ⭐️ 8.0/10
6. [Essay argues conscientious engineers should embrace LLM tools, sparking debate](#item-6) ⭐️ 8.0/10
7. [FCC Approves SpaceX Plan for Orbital AI Data Centers](#item-7) ⭐️ 8.0/10
8. [Security researcher criticizes Ubuntu's slow patch response](#item-8) ⭐️ 7.0/10
9. [NYT Warns Photographers Against Updating Photoshop Over AI Features](#item-9) ⭐️ 7.0/10
10. [Blog claims Jev is likely Qwen3.5-35B-A3B based on latency](#item-10) ⭐️ 7.0/10
11. [Developer reverse-engineers Windows Loudness Equalization for PipeWire](#item-11) ⭐️ 7.0/10
12. [Author uses Lean to audit Clojure core, finds unreported bugs](#item-12) ⭐️ 7.0/10
13. [Scientists Define Boundaries for AI Agents in Research](#item-13) ⭐️ 7.0/10
14. [New York Bans AI Chatbot Toys for Five Years](#item-14) ⭐️ 7.0/10
15. [State AGs Challenge Character.AI's Plan to Auction User Chats in Bankruptcy](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Scott Aaronson Sounds Alarm on AI's Mathematical Breakthroughs](https://scottaaronson.blog/?p=10379) ⭐️ 9.0/10

Scott Aaronson published a blog post reacting to a major AI-driven mathematical breakthrough, linking to an OpenAI preprint claiming the matrix multiplication exponent is exactly 9/4. The post sparked a massive Hacker News discussion with over 1,000 points and 847 comments. The claim that the matrix multiplication exponent is exactly 9/4 would be the biggest shift in this fundamental complexity bound since 1979, with wide implications for algorithm design. More broadly, AI systems solving long-standing open math problems signals a potential paradigm shift in how mathematical research is conducted. The OpenAI preprint claims a lower bound matching the known upper bound for the matrix multiplication exponent ω, meaning no algorithm could achieve a smaller exponent. However, community members question how one can verify that AI-generated Lean proofs actually prove the intended statement rather than some other compilable code.

hackernews · Kotlopou · Nov 25, 19:11 · [Discussion](https://news.ycombinator.com/item?id=50646108)

**Background**: The matrix multiplication exponent ω describes the asymptotic complexity of multiplying two n×n matrices; the naive algorithm gives ω=3, while the best known upper bound has been around 2.37 since 1986. Scott Aaronson is a theoretical computer scientist at UT Austin known for his blog Shtetl-Optimized, where he has chronicled OpenAI's recent flood of AI-generated mathematical results. In 2026, OpenAI released numerous AI-discovered proofs of open problems, prompting debate about trust, verification, and the future of mathematical research.

<details><summary>References</summary>
<ul>
<li><a href="https://xenospectrum.com/en/matrix-multiplication-nine-fourths-lower-bound/">OpenAI Preprint Claims the Matrix Multiplication Exponent Is ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_bulk_release_of_mathematical_papers">OpenAI bulk release of mathematical papers - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_mathematical_discoveries_made_with_artificial_intelligence">List of mathematical discoveries made with artificial ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed awe at the pace of AI progress, with some arguing humans are biologically incapable of appreciating the magnitude of change. Others pushed back, noting that success in axiomatic math does not imply AI will solve all fields or pose existential risks, and raised concerns about verification of Lean proofs.

**Tags**: `#AI`, `#mathematics`, `#research breakthrough`, `#philosophy of science`, `#community discussion`

---

<a id="item-2"></a>
## [1Password Discloses Incident: Compromised Laptop Led to Malicious Code Push](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password disclosed a security incident in which an attacker gained access to an employee's corporate GitHub account and used it to push malicious code to backend services, which downloaded administrative data pertaining to customers. The company confirmed that customer vaults were not accessed and remain secure. This incident highlights a critical SaaS supply-chain risk: a single compromised employee laptop can lead to code being pushed to production, potentially exposing sensitive customer data. Given 1Password's role as a widely-used password manager, the event underscores the need for robust branch protection and endpoint security across SaaS providers. The attacker used the compromised GitHub account to access source code and push malicious code to backend services, which then downloaded administrative data about customers. 1Password has not yet detailed whether branch protection rules were missing or bypassed, a point raised by commenters.

hackernews · lxhrstn · Nov 25, 17:18 · [Discussion](https://news.ycombinator.com/item?id=50644817)

**Background**: 1Password is a popular password manager that stores user credentials in encrypted vaults. In a typical SaaS supply-chain attack, attackers compromise an employee's device to gain access to code repositories and inject malicious code into production systems. This incident follows a pattern seen in other breaches, such as the 2026 GitHub breach via a compromised employee device.

<details><summary>References</summary>
<ul>
<li><a href="https://1password.com/blog/update-on-nov-2026-security-incident">Update on a security incident involving 1Password’s backend ...</a></li>
<li><a href="https://www.1password.community/announcements-52/update-on-a-security-incident-involving-1password-s-backend-systems-customer-vaults-were-not-affected-and-all-vault-contents-remain-secure-26259">Update on a security incident involving 1Password’s backend ...</a></li>
<li><a href="https://www.pcmag.com/news/hackers-infiltrate-github-by-compromising-employee-device">Hackers Infiltrate GitHub by Compromising Employee Device</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that compromised employee laptops are the most important attack vector for SaaS companies, with the likelihood approaching 1 as employee count grows. Some expressed concern that pushing malicious code to backend services indicates missing branch protection, and others worried about the security of online vaults versus local-only vaults. A few noted that passkey implementations often lack a second factor, potentially weakening security.

**Tags**: `#security`, `#SaaS`, `#supply-chain`, `#1Password`, `#incident-response`

---

<a id="item-3"></a>
## [Lean verification of GRH shrinks from 17M to 76k lines](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

A new GitHub repository by lsernau presents a much shorter, more readable Lean verification of the Generalized Riemann Hypothesis, reduced from approximately 17 million lines to about 76,000 lines—a 99.56% reduction. The project includes clear documentation and explicitly separates known mathematics from new mathematics. This dramatic reduction makes the formal proof far more accessible for mathematicians to review and understand, potentially addressing concerns that huge formal proofs lack insight. It also highlights the growing role of AI-assisted proof golfing in making formal verification more practical. The reduction was achieved through proof golfing, likely with LLM assistance, and the repository includes human-readable documentation throughout. A related tool, slim, can be used to navigate the Lean source without setting up Lean or building the project.

hackernews · nb-t · Nov 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=50648050)

**Background**: The Generalized Riemann Hypothesis (GRH) is a major unsolved conjecture in number theory that extends the Riemann Hypothesis to Dirichlet L-functions and other global L-functions. Lean is a proof assistant and functional programming language used to formally verify mathematical proofs. In November 2026, mathematician Levent Alpöge proposed an AI-assisted proof of GRH, which was verified by the Lean and Mathlib communities. The original formalization was enormous (~17M lines), and this project is a significantly golfed version.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generalized_Riemann_hypothesis">Generalized Riemann hypothesis</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the readability and the known-vs-new math split, noting it will greatly aid digestion. Some raised questions about whether this addresses Terence Tao's concern that huge proofs without insight are problematic, and whether smarter LLMs can now golf and explain proofs. Others shared resources like a Zulip discussion and a tool for navigating the Lean source.

**Tags**: `#Lean`, `#formal verification`, `#mathematics`, `#GRH`, `#proof golfing`

---

<a id="item-4"></a>
## [Polynomial Hirsch Conjecture Disproved by New Preprint](https://github.com/openai/math/blob/main/preprints/Superpolynomial-graph-diameter-of-simple-polytopes-November-24-2026/paper.pdf) ⭐️ 8.0/10

A new preprint posted on OpenAI's math GitHub repository disproves the polynomial Hirsch conjecture by constructing simple polytopes whose graph diameter is superpolynomial in the number of facets. This shows that no polynomial-time simplex algorithm can exist in general. This result settles a central open question in polyhedral combinatorics and rules out the possibility of a polynomial-time simplex method, affecting the theoretical foundations of linear programming and the analysis of pivot rules. It also has implications for complexity theory and combinatorial geometry. The preprint constructs simple polytopes with superpolynomial graph diameter, which is a stronger statement than the 2010 disproof of the original Hirsch conjecture. The original conjecture was already disproved by a 43-dimensional polytope with 86 facets and diameter greater than 43, but that counterexample did not rule out polynomial diameter.

hackernews · acossta · Nov 25, 17:34 · [Discussion](https://news.ycombinator.com/item?id=50644980)

**Background**: The Hirsch conjecture, posed in 1957, stated that the graph of a d-dimensional polytope with n facets has diameter at most n-d, providing a lower bound on the number of steps for the simplex method. It was disproved in 2010 by Francisco Santos Leal after more than 50 years. The polynomial Hirsch conjecture relaxes the bound to O(n^k) for some fixed k, and was a surviving question about whether the diameter is polynomially bounded.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polynomial_Hirsch_conjecture">Polynomial Hirsch conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hirsch_conjecture">Hirsch conjecture - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Simplex_algorithm">Simplex algorithm - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters clarified that this result means no polynomial-time simplex algorithm exists, and that it is a follow-up to the 2010 disproof of the original Hirsch conjecture. Some asked whether the proof is constructive, while others discussed the broader implications for solving major mathematical problems.

**Tags**: `#combinatorial geometry`, `#linear programming`, `#simplex algorithm`, `#Hirsch conjecture`, `#complexity theory`

---

<a id="item-5"></a>
## [Google Research Releases Cogentic Papers on Integer Factorization and Discrete Logs](https://github.com/google-research/google-research/tree/master/cogentic_research_papers) ⭐️ 8.0/10

Google Research has published a collection of papers under the 'cogentic_research_papers' directory on its GitHub repository, covering integer factorization, discrete logarithms, and related mathematical topics. The release has sparked speculation that these are early results from an AI-driven system called Cogentic, which may use LLMs to collaboratively solve mathematical conjectures. Integer factorization and discrete logarithms underpin widely used public-key cryptosystems such as RSA and Diffie-Hellman, so any significant advance in solving these problems could have major implications for digital security. The release also fuels the broader trend of using AI to accelerate mathematical discovery, which could reshape how research is conducted. According to community discussion, Cogentic appears to be a specialized harness that orchestrates existing LLMs to collaborate on mathematical conjectures, using a central orchestrator and a shared database of intermediate proofs. The papers themselves are hosted as PDFs in the Google Research GitHub repository, but the specific algorithms or results have not been detailed in the summary.

hackernews · rgwohlbold · Nov 25, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50642086)

**Background**: Integer factorization is the problem of breaking a number into its prime factors, and its assumed hardness is what makes RSA encryption secure. The discrete logarithm problem, similarly considered computationally intractable for classical computers, is the foundation of Diffie-Hellman key exchange and other cryptographic protocols. Recent advances in AI for mathematics, such as large language models assisting with proofs, have raised hopes and concerns about accelerating solutions to these long-standing problems.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50642086">Google releases Cogentic papers on integer... | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Discrete_logarithm">Discrete logarithm - Wikipedia</a></li>
<li><a href="https://github.com/google-research/google-research/blob/master/cogentic_research_papers/edge_reconstruction/paper.pdf">github.com/ google - research / google - research /blob/master/ cogentic ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (452 points, 337 comments) shows strong interest, with some users citing rumors from credible sources that this is 'the tip of something bigger.' Others compare the moment to AlphaGo's breakthrough, argue it's an exciting time for computer science, and express surprise that such daily breakthroughs aren't lifting the AI market. A notable sentiment is a shift in belief: mathematics may no longer be immune to being solved by throwing money and compute at problems.

**Tags**: `#cryptography`, `#integer factorization`, `#discrete logarithms`, `#Google Research`, `#AI for math`

---

<a id="item-6"></a>
## [Essay argues conscientious engineers should embrace LLM tools, sparking debate](https://www.iankduncan.com/engineering/2026-11-19-smart-people-who-give-a-shit-use-tools) ⭐️ 8.0/10

Ian K. Duncan published an essay arguing that smart, conscientious engineers should use LLM tools, which sparked a 231-comment Hacker News discussion challenging the 'higher-level abstraction' analogy and warning about eroded code comprehension. The debate highlights a growing tension in software engineering: while LLMs boost productivity, they may undermine the deep understanding that comes from hand-writing code, potentially allowing less careful developers to outpace more diligent ones. Commenters noted that using an LLM is qualitatively different from past abstraction shifts like assembly to C, because the developer is abstracted away rather than the code, and research shows self-written code is comprehended faster and more accurately than generated code.

hackernews · matthewsinclair · Nov 25, 07:46 · [Discussion](https://news.ycombinator.com/item?id=50639698)

**Background**: LLM-assisted coding tools like GitHub Copilot and ChatGPT have become widespread, prompting comparisons to historical abstraction layers such as high-level languages and compilers. However, critics argue that LLMs differ because they generate code without the developer necessarily modeling the problem themselves, which may lead to knowledge erosion.

**Discussion**: Commenters challenged the abstraction analogy, arguing that LLMs abstract the developer rather than the code, and warned that AI removes the guarantee of deep understanding from writing code oneself. Some noted that LLMs may let careless shippers outpace careful engineers, and that discipline is needed to prevent knowledge atrophy.

**Tags**: `#LLM`, `#software-engineering`, `#AI-assisted-coding`, `#developer-productivity`, `#code-quality`

---

<a id="item-7"></a>
## [FCC Approves SpaceX Plan for Orbital AI Data Centers](https://techcrunch.com/2026/11/25/fcc-approves-spacex-plan-to-put-ai-data-centers-in-space/) ⭐️ 8.0/10

The FCC approved SpaceX's plan to deploy AI data centers in space, while dismissing opponents' concerns about threats to scientific research as outside its regulatory authority. This approval is a major regulatory milestone that could accelerate the development of orbital computing infrastructure, with significant implications for space policy, AI infrastructure, and scientific research. The FCC determined that concerns about potential threats to scientific research fell outside its regulatory authority, focusing instead on its mandate to license the electromagnetic spectrum and satellite communications.

rss · TechCrunch · Nov 25, 20:56

**Background**: The FCC is responsible for managing and licensing the electromagnetic spectrum for commercial and non-commercial users, including satellite operators. SpaceX has been expanding its AI ambitions, including plans to use NVIDIA technology for orbital computing systems. Orbital data centers could tap into abundant solar energy and avoid some environmental challenges faced by terrestrial facilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedaily.com/releases/2026/06/260618041501.htm">SpaceX wants to build AI data centers in space . | ScienceDaily</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#AI infrastructure`, `#FCC regulation`, `#space policy`, `#data centers`

---

<a id="item-8"></a>
## [Security researcher criticizes Ubuntu's slow patch response](https://www.openwall.com/lists/oss-security/2026/11/25/9) ⭐️ 7.0/10

Security researcher Hanno Böck published a report on the oss-security mailing list arguing that Ubuntu is too slow to ship fixes for severe Linux kernel flaws, noting that a recent Ubuntu LTS system still ran kernel 7.0.0-44, suggesting Ubuntu backports patches to an old kernel rather than tracking kernel.org longterm releases. The report sparked a Hacker News discussion with 165 points and 77 comments, highlighting growing concerns about whether widely used enterprise distributions can keep pace with kernel security patches, and prompting some organizations to reconsider their choice of Ubuntu for servers and desktops. The core technical concern is that Ubuntu backports fixes onto an older kernel version instead of rebasing onto kernel.org's longterm-supported kernels, and the discussion notes that most major distributions spend significant time on regression testing, so slower patching can be a deliberate tradeoff rather than pure negligence.

hackernews · gslin · Nov 25, 20:38 · [Discussion](https://news.ycombinator.com/item?id=50647181)

**Background**: Linux distributions like Ubuntu package the Linux kernel and other software, and when a security vulnerability is disclosed, the distribution must backport or rebase the fix and test it before release. Ubuntu LTS releases prioritize stability over bleeding-edge packages, which can delay security updates compared with distributions that track upstream more closely. The oss-security mailing list is a public forum where researchers disclose and debate vulnerabilities in open-source software.

<details><summary>References</summary>
<ul>
<li><a href="https://www.openwall.com/lists/oss-security/2026/11/25/9">oss-security - Slow Ubuntu security response times</a></li>
<li><a href="https://seclists.org/oss-sec/2026/q4/890">oss-sec: Slow Ubuntu security response times</a></li>
<li><a href="https://daily.dev/posts/slow-ubuntu-security-response-times-9gafircej">Slow Ubuntu security response times - daily.dev</a></li>

</ul>
</details>

**Discussion**: Commenters debated which desktop distribution to use given supply-chain security concerns, with some saying they moved server images from Ubuntu to Debian because slow security response is unacceptable in 2026. Others cautioned that Debian has limited QA resources and regressions can occur, while one commenter quoted a stable kernel maintainer warning that cherry-picking patches can leave systems more insecure.

**Tags**: `#Linux`, `#Security`, `#Ubuntu`, `#Distributions`, `#Supply Chain`

---

<a id="item-9"></a>
## [NYT Warns Photographers Against Updating Photoshop Over AI Features](https://www.theverge.com/ai-artificial-intelligence/1041227/the-new-york-times-warns-photographers-not-to-update-photoshop-over-ai-features) ⭐️ 7.0/10

The New York Times has advised photographers not to update Adobe Photoshop because of its generative AI features, according to a report by The Verge. The warning highlights growing concerns about the stigma and credibility risks associated with AI-generated content in creative work. This stance from a major media outlet signals a significant industry shift: AI features in creative tools are becoming a liability rather than an asset. It could pressure Adobe and other software vendors to offer AI-free versions or clearer labeling, and it affects photographers, designers, and brands who rely on these tools for professional credibility. The NYT's warning is tied to the difficulty of distinguishing fully AI-generated images from those with minor AI-assisted edits, especially when platforms like Instagram and Facebook may tag content as 'AI generated,' potentially damaging a brand's credibility. Adobe's Generative Fill and Expand features, powered by Firefly models, are out of beta and widely used, but they embed AI provenance signals that can trigger such labels.

hackernews · rmason · Nov 25, 21:18 · [Discussion](https://news.ycombinator.com/item?id=50647673)

**Background**: Adobe Photoshop has integrated generative AI features like Generative Fill and Expand since 2023, allowing users to add or modify image content using text prompts. These features rely on Adobe Firefly, a family of generative AI models designed for commercial safety. Meanwhile, standards like C2PA Content Credentials aim to provide verifiable metadata about how images were created or edited, but they can also make AI involvement detectable. The New York Times has a long history of upholding strict photo ethics, and its warning reflects broader concerns about AI's impact on trust in visual media.

<details><summary>References</summary>
<ul>
<li><a href="https://contentauthenticity.org/how-it-works">How it works - Content Authenticity Initiative</a></li>
<li><a href="https://www.nytimes.com/2025/04/30/magazine/artificial-intelligence-photo-ethics.html">Can I Use A . I . to Look Better Online? - The New York Times</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely agree that generative AI in creative work carries a social stigma and reputational risk, with one professional noting it's nearly impossible to separate fully AI-generated images from minor AI-assisted edits. Others see an opportunity for competitors like Affinity and predict a shift away from subscription models, while some criticize Adobe's subscription strategy.

**Tags**: `#AI`, `#Adobe Photoshop`, `#creative tools`, `#AI stigma`, `#software subscriptions`

---

<a id="item-10"></a>
## [Blog claims Jev is likely Qwen3.5-35B-A3B based on latency](https://modaic.dev/blog/latency-doesnt-lie) ⭐️ 7.0/10

A blog post on modaic.dev argues that the proprietary model Jev, developed by TypeSafe AI, is likely a fine-tuned version of Qwen3.5-35B-A3B, citing latency analysis and self-identification responses. The post has sparked a critical discussion on Hacker News about the reliability of such methods. If true, this would suggest that a commercial 'decision model' is built on an open-source LLM, raising questions about transparency and provenance in the AI industry. The discussion also highlights the challenges of reliably identifying proprietary models, which is important for benchmarking and trust. The analysis relies on latency measurements and asking the model to identify itself, but commenters note that latency alone cannot distinguish between Qwen and Gemma, and self-identification is known to be unreliable. TypeSafe's website explicitly denies that Jev is an LLM, describing it as a 'System One Model' that returns typed decisions rather than generating text.

hackernews · csoham · Nov 25, 22:57 · [Discussion](https://news.ycombinator.com/item?id=50648823)

**Background**: Jev is a proprietary AI model developed by TypeSafe AI (founded in 2024) that is designed for classification or regression tasks, returning typed decisions with probabilities and confidence scores rather than generating text. Qwen3.5-35B-A3B is an open-source model from Alibaba Cloud's Qwen team, released on February 24, 2026, as part of the Qwen3.5 family. Model identification—determining which base model a proprietary service uses—is a common but challenging reverse-engineering task in the LLM community.

<details><summary>References</summary>
<ul>
<li><a href="https://speechmap.ai/models/qwen-qwen3-5-35b-a3b/">Model : qwen/ qwen 3 . 5 - 35 b - a 3 b</a></li>
<li><a href="https://playground.roboflow.com/models/compare/gpt-5-mini-vs-qwen3-5-35b-a3b">GPT-5 Mini vs Qwen 3 . 5 35 B A 3 B : Vision Model Comparison</a></li>
<li><a href="https://github.com/QwenLM/Qwen3.8">GitHub - QwenLM/ Qwen 3 .8: Qwen 3 .8 is the large language model ...</a></li>

</ul>
</details>

**Discussion**: Commenters are largely skeptical: one notes that the latency data cannot distinguish between Qwen and Gemma, and another points out that TypeSafe explicitly denies Jev is an LLM, calling for more conclusive evidence. Others question the reliability of self-identification and suggest alternative hypotheses, such as a LoRA fine-tune performing differently.

**Tags**: `#LLM`, `#model-identification`, `#Qwen`, `#latency`, `#Hacker News`

---

<a id="item-11"></a>
## [Developer reverse-engineers Windows Loudness Equalization for PipeWire](https://github.com/xoxorwr/pw-loudness-eq) ⭐️ 7.0/10

A developer has reverse-engineered Windows' Loudness Equalization feature and ported it to PipeWire, releasing the project as pw-loudness-eq on GitHub. The project aims to replicate the loudness normalization behavior found in Windows audio processing for Linux users. This brings a familiar Windows audio enhancement to Linux's modern audio server, potentially improving the listening experience for PipeWire users who want consistent volume levels. It also highlights the growing maturity of PipeWire as a platform for advanced audio processing. The implementation is based on reverse-engineering Windows' audio processing, which may raise ethical and legal questions about copying proprietary algorithms. Community members note that the algorithm is essentially loudness normalization and may require additional limiting to prevent excessive gain on pure tones.

hackernews · ThrowNotAway · Nov 25, 11:34 · [Discussion](https://news.ycombinator.com/item?id=50641171)

**Background**: Loudness Equalization is a Windows audio enhancement that reduces the difference between quiet and loud sounds, making dialogue easier to hear but potentially flattening music dynamics. PipeWire is a low-level multimedia framework for Linux that handles audio and video streams, aiming to unify and replace PulseAudio and JACK. Loudness normalization adjusts audio based on perceived loudness, unlike dynamic range compression which reduces the volume of louder parts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PipeWire">PipeWire - Wikipedia</a></li>
<li><a href="https://www.pipewire.org/">PipeWire</a></li>
<li><a href="https://www.thewindowsclub.com/disable-or-enable-loudness-equalization-in-windows-10">How to disable or enable Loudness Equalization in Windows 11/10</a></li>

</ul>
</details>

**Discussion**: Commenters debated the terminology, with one noting it should be called loudness normalization rather than equalization. Some questioned the need for reverse-engineering, suggesting simpler limiter algorithms could achieve similar results, while others raised ethical concerns about copying proprietary code. Another commenter pointed out that Windows itself applies a subtle limiter in shared mode audio paths.

**Tags**: `#audio-processing`, `#reverse-engineering`, `#pipewire`, `#windows`, `#loudness-normalization`

---

<a id="item-12"></a>
## [Author uses Lean to audit Clojure core, finds unreported bugs](https://s.conao3.com/blog/2026/e4f733) ⭐️ 7.0/10

An author applied the Lean theorem prover to formally check Clojure's core library and reported finding previously unreported bugs. The work was shared in a blog post and sparked a 67-comment discussion on verification tooling and the validity of the findings. This cross-language verification approach shows how formal methods can be applied to audit widely used dynamic language libraries like Clojure's core, potentially improving reliability for a large ecosystem. It also fuels debate about the practicality and noise level of such audits. Community members pointed out that some reported issues, such as (.indexOf (seq (byte-array [1 2 3])) 2) and (get "abc" 1.9), stem from expected type coercion behavior rather than genuine bugs, suggesting the need to reduce noise. The discussion also compared Lean with Rocq (formerly Coq) for program verification.

hackernews · encyclopedism · Nov 25, 14:56 · [Discussion](https://news.ycombinator.com/item?id=50642939)

**Background**: Lean is an interactive theorem prover used for formal verification of mathematical proofs and software properties. Clojure is a dynamic, functional Lisp dialect that runs on the JVM, and its core library provides fundamental functions and data structures. Formal verification involves mathematically proving that a system behaves correctly according to a specification.

<details><summary>References</summary>
<ul>
<li><a href="https://leanprover.github.io/theorem_proving_in_lean/introduction.html">1. Introduction — Theorem Proving in Lean 3 (outdated)...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>
<li><a href="https://clojuredocs.org/core-library">Clojure 's Core Library | ClojureDocs - Community-Powered Clojure ...</a></li>

</ul>
</details>

**Discussion**: Commenters critiqued specific findings as type coercion issues rather than bugs, and questioned whether Lean is now preferred over Rocq for verification, possibly due to better language model support. Others noted related audits of other Lisp implementations (SBCL, Clozure, ACL2) and expressed interest in learning Lean for testing.

**Tags**: `#Clojure`, `#Lean`, `#formal-verification`, `#programming-languages`, `#bug-hunting`

---

<a id="item-13"></a>
## [Scientists Define Boundaries for AI Agents in Research](https://huggingface.co/blog/allenai/where-scientists-draw-the-line-on-ai-agents) ⭐️ 7.0/10

A blog post published on Hugging Face by AllenAI explores where scientists draw the line on using AI agents in their work, highlighting concerns and acceptance criteria. The article surveys scientists' perspectives on the boundaries of AI agent use, offering insight into adoption and trust in AI for research. As AI agents become more autonomous and capable of multi-step tasks, understanding scientists' trust and acceptance criteria is crucial for responsible integration into research workflows. This analysis sheds light on the barriers to adoption and the conditions under which researchers would rely on AI agents, impacting tool developers and research institutions. The article likely discusses specific concerns such as traceability, reproducibility, and the risk of fabricated claims, which are critical for scientific rigor. It may also outline acceptance criteria like transparency and demonstrable trustworthiness that scientists require before delegating tasks to AI agents.

rss · Hugging Face Blog · Nov 25, 18:52

**Background**: AI agents are software systems that pursue goals and complete tasks autonomously, using reasoning, planning, and memory. In scientific research, trust in AI agents is a growing concern, with studies showing that AI-generated research can contain fabricated claims and fail to meet expert standards. Hugging Face is a major platform for sharing AI models and datasets, and AllenAI is a research institute known for developing AI technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.ontoforce.com/blog/can-you-trust-an-ai-agent-in-a-drug-discovery-pipeline-three-conditions">Can you trust an AI agent in a drug discovery pipeline? Three conditions</a></li>
<li><a href="https://huggingface.co/papers/2610.19159">Paper page - Into the Unknown: Benchmarking AI agents on open...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#scientific research`, `#AI adoption`, `#trust`, `#Hugging Face`

---

<a id="item-14"></a>
## [New York Bans AI Chatbot Toys for Five Years](https://techcrunch.com/2026/11/25/want-to-buy-your-kid-an-ai-toy-this-christmas-not-in-new-york/) ⭐️ 7.0/10

New York Governor Kathy Hochul signed legislation on Wednesday imposing a five-year ban on the manufacture and sale of AI chatbot-powered toys, including talking stuffed animals, for children under 13. The ban takes effect in February 2027 and carries penalties of up to $15,000 per day for violations. This is the first state-level ban on AI toys in the U.S., setting a significant regulatory precedent that could influence other states and force AI toy developers to rethink product design and safety standards. It directly affects manufacturers, retailers, and parents ahead of the holiday shopping season. The ban is backed by new research from Common Sense Media documenting safety failures such as exposure to inappropriate content and risks to emotional development. A March 2026 University of Cambridge study for the Childhood Trust found young children forming emotional bonds with AI toys and no evidence of developmental benefits, while separate research on Curio's Gabbo toy found it could misinterpret emotional cues.

rss · TechCrunch · Nov 25, 18:11

**Background**: AI chatbot toys are plush or interactive devices that use large language models to hold conversations with children, often marketed as educational companions. Common Sense Media is a nonprofit that studies youth and technology, and its Youth AI Safety Institute conducted testing that surfaced troubling responses from these toys. Child safety groups have also urged retailers like Amazon and eBay to stop selling AI toys until they are proven safe, invoking the precautionary principle.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/nov/25/new-york-bans-ai-toys">New York bans AI toys, including those using internet to talk ...</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/york-imposes-five-ban-ai-180458200.html?fr=sycsrp_catchall">New York Imposes Five-Year Ban on AI Chatbot Toys for Kids</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/23/child-safety-groups-urge-amazon-ebay-stop-selling-ai-toys-until-proved-safe">Child safety groups urge Amazon and eBay to stop selling AI toys until...</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#child safety`, `#AI toys`, `#policy`, `#consumer AI`

---

<a id="item-15"></a>
## [State AGs Challenge Character.AI's Plan to Auction User Chats in Bankruptcy](https://techcrunch.com/2026/11/25/state-ags-fight-character-ais-plan-to-auction-off-users-private-chats/) ⭐️ 7.0/10

A coalition of 42 state and territorial attorneys general is objecting to Character.AI's proposed Chapter 11 bankruptcy sale, which would transfer sensitive personal data from over 21 million U.S. accounts, including 2.1 million registered to minors, to a buyer. The AGs are asking the court to block the sale or impose data safeguards, and they want users to have a chance to delete their data before any transfer. This case sets a precedent for how user data—especially sensitive AI chat logs and minors' information—is treated in bankruptcy, potentially affecting millions of users and shaping future data governance and consumer protection standards in the AI industry. It highlights the tension between corporate asset liquidation and privacy rights, and could influence how other AI companies handle user data in financial distress. The sale includes chat records and related personal information from approximately 21 million U.S. accounts, with 2.1 million accounts declared as belonging to users under 18. New York Attorney General Letitia James and Connecticut AG are among those leading the objection, arguing that private conversations could be sold to the highest bidder without adequate privacy protections.

rss · TechCrunch · Nov 25, 17:35

**Background**: Character.AI is an AI chatbot platform that allows users to create and interact with customized characters. In October 2026, the company initiated a voluntary Chapter 11 bankruptcy to facilitate a court-supervised sale of its assets. In bankruptcy proceedings, a company's assets—including user data—can be sold to repay creditors, raising concerns about privacy and consent. State attorneys general often intervene in such cases to protect consumers, especially vulnerable groups like minors.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/25/state-ags-fight-character-ais-plan-to-auction-off-users-private-chats/">State AGs fight Character.AI’s plan to auction off users ...</a></li>
<li><a href="https://cctest.ai/en/articles/42-state-and-territorial-ags-oppose-character-ai-chat-data-sale">42 AGs Challenge Character.AI’s Planned Chat Data Auction ...</a></li>
<li><a href="https://www.aiaffairs.com/government/attorneys-general-character-ai-bankruptcy-data-protections/">Forty attorneys general seek data safeguards in Character.AI ...</a></li>

</ul>
</details>

**Tags**: `#AI privacy`, `#data governance`, `#consumer protection`, `#Character.AI`, `#regulation`

---