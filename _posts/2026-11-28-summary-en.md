---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 10 items, 7 important content pieces were selected

---

1. [WebRTC-based credit card skimming scripts found on popular shopping sites](#item-1) ⭐️ 8.0/10
2. [Convex skills plugin accused of uploading user app ideas without disclosure](#item-2) ⭐️ 8.0/10
3. [State AGs Sue SpaceX and xAI Over Grok's Harmful Image Generation](#item-3) ⭐️ 8.0/10
4. [Michael Nielsen Removes Neural Networks Book Over AI Safety Concerns](#item-4) ⭐️ 8.0/10
5. [Google's DeepCrossAttention speeds transformer training up to 3x](#item-5) ⭐️ 7.0/10
6. [Show HN: Bouncemarket – a live prediction market game for a bouncing ball](#item-6) ⭐️ 7.0/10
7. [D.J. Bernstein Critiques Reliance on Computer-Checked Proofs](#item-7) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [WebRTC-based credit card skimming scripts found on popular shopping sites](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 8.0/10

Security researchers discovered credit card skimming scripts that abuse WebRTC data channels on popular shopping sites, particularly targeting mobile devices during the Black Friday period. The scripts were injected into checkout pages to steal payment card details. This finding highlights the persistent risk of third-party scripts on e-commerce sites and shows how attackers continuously adapt techniques to evade detection. It affects online shoppers, especially mobile users, and underscores the need for stronger client-side security controls. The skimmers leverage WebRTC data channels, which are less commonly monitored for malicious activity, and target mobile devices because they are harder to detect. The attack could also be carried out with simple HTTP requests, indicating that the core vulnerability lies in the inclusion of third-party scripts.

hackernews · scanr · Nov 27, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50668145)

**Background**: WebRTC is a browser API that enables real-time peer-to-peer communication, including data channels that can transfer arbitrary data. Credit card skimming scripts, often called Magecart attacks, are malicious JavaScript injected into checkout pages to steal payment information. Third-party scripts are commonly embedded in e-commerce sites for analytics, ads, and functionality, but they introduce supply chain risks if compromised.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-google-apps-script-to-steal-credit-cards-bypass-csp/">Hackers abuse Google Apps Script to steal credit cards , bypass CSP</a></li>
<li><a href="https://www.akamai.com/glossary/what-is-magecart">What Is Magecart ? | Akamai</a></li>
<li><a href="https://webrtc.org/getting-started/overview">Getting started with WebRTC</a></li>

</ul>
</details>

**Discussion**: Commenters debated the root causes, with some arguing that blocking ads is justified, while others noted that the issue is not WebRTC's technical capability but its lack of monitoring. Several suggested sandboxing ads to prevent JavaScript execution, and some criticized the web's design of allowing third-party code execution, calling for asymmetric cryptography in payments.

**Tags**: `#security`, `#web-security`, `#webrtc`, `#credit-card-skimming`, `#third-party-scripts`

---

<a id="item-2"></a>
## [Convex skills plugin accused of uploading user app ideas without disclosure](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 8.0/10

A GitHub issue (convex/convex-backend-skill#64) alleges that Convex's skills plugin sends users' app ideas to a remote server without informing them, prompting a Hacker News discussion with 239 points and 76 comments. Convex CEO Jamie responded, clarifying that the prompt upload powers the Convex 'quickstart' feature and is the successor to the discontinued Convex Chef vibe-coding product. This incident highlights growing privacy and transparency concerns in AI-assisted developer tools, where plugins may transmit sensitive user input to remote servers by default. It affects developers using Convex's agent plugins and raises broader questions about data handling and consent in AI tooling. The plugin's prompt upload is tied to Convex's 'quickstart' feature, which lets developers describe an app in one sentence and have an agent scaffold it. The disclosure issue centers on whether users are adequately informed that their ideas are sent to a remote server, and the discussion also touched on prompt injection risks and self-hosted open-weight models.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**Background**: Convex is a full-stack development platform that provides a database, server functions, and an AI gateway for building and hosting software. It publishes official skills and plugins for major coding agents, enabling users to scaffold apps from natural language descriptions. Prompt injection is a technique where malicious instructions are hidden in input to manipulate AI model behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://www.convex.dev/">Convex | All gas, no breakages</a></li>
<li><a href="https://docs.convex.dev/">Convex Docs | Convex Developer Hub</a></li>
<li><a href="https://shir-man.com/llm-attack/">Prompt Injection Generator | Unicode Stealth Payload Builder</a></li>

</ul>
</details>

**Discussion**: Commenters debated the implications: one noted that self-hosted open-weight models may be the long-term solution, another pointed out that prompt injection is more common than models making malicious tool calls on their own, and a third dismissed the concern by saying 'ideas are cheap.' There was also confusion about a commenter promoting a personal media website in the issue thread.

**Tags**: `#privacy`, `#security`, `#AI-tools`, `#prompt-injection`, `#developer-tools`

---

<a id="item-3"></a>
## [State AGs Sue SpaceX and xAI Over Grok's Harmful Image Generation](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 8.0/10

A group of state attorneys general, including those from Virginia and Washington, D.C., filed a lawsuit against SpaceX and its subsidiary xAI, alleging that the Grok AI model generates child sexual abuse material and non-consensual intimate images. The suit claims the companies failed to implement adequate safeguards, prompting a legal battle over AI platform accountability. This lawsuit represents a significant escalation in regulatory scrutiny of generative AI, potentially setting a precedent for holding AI developers liable for harms caused by their models. It could influence how platforms moderate content and accelerate legislative efforts to regulate AI-generated explicit material. The suit targets Grok's image generation capabilities, which have been criticized for minimal censorship and easy circumvention. It also highlights the challenge of age verification and consent in AI-generated content, as Grok requires linking to an X account, raising privacy concerns.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**Background**: Grok is an AI assistant developed by xAI, founded by Elon Musk in 2023 and now a subsidiary of SpaceX. It is known for its minimal content restrictions compared to other AI models. The lawsuit comes amid growing global concern over AI-generated non-consensual intimate images, with emerging laws like the TAKE IT DOWN Act aiming to hold platforms accountable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">XAI (company)</a></li>
<li><a href="https://olartemoure.com/en/ai-non-consensual-intimate-images/">Misuse of AI to generate non - consensual intimate images</a></li>
<li><a href="https://www.igniterstech.com/publications/the-take-it-down-act-a-new-era-of-combat-against-nonconsensual-intimate-imagery">The Take It Down Act: A New Era of Combat Against Nonconsensual ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion about how Grok could generate such content, given that it requires linking a Twitter account, and questioned whether users had to trick the model. Some also asked about accountability for the individuals who created the images, while others noted the privacy risk of surrendering social media accounts to try the model.

**Tags**: `#AI ethics`, `#content moderation`, `#legal`, `#xAI`, `#Grok`

---

<a id="item-4"></a>
## [Michael Nielsen Removes Neural Networks Book Over AI Safety Concerns](https://neuralnetworksanddeeplearning.com/) ⭐️ 8.0/10

Michael Nielsen has taken down his free online book 'Neural Networks and Deep Learning' from his website, stating he no longer wants to help train people for frontier AI work. The removal sparked a Hacker News discussion with 267 comments about AI safety, open access, and the motivations behind the decision. The book was a widely used, high-quality educational resource that introduced many practitioners to neural networks, so its removal highlights growing tensions between open AI education and concerns about catastrophic AI risk. It also raises questions about whether withholding knowledge is an effective form of protest or simply pushes learners toward archived copies. Nielsen's stated reason is that he does not want to contribute to training people for frontier AI labs, framing the act as a protest rather than a technical change. Because the book was freely available online for years, archived versions remain accessible via the Internet Archive, and the removal may paradoxically increase interest in the material.

hackernews · brandonb · Nov 27, 19:31 · [Discussion](https://news.ycombinator.com/item?id=50670757)

**Background**: Michael Nielsen is a well-known researcher and writer on open science and deep learning, and his book 'Neural Networks and Deep Learning' has been a popular free introduction to the field since the mid-2010s. In recent years, Nielsen has written about existential risk from artificial superintelligence, arguing that frontier AI development poses severe risks. The Hacker News discussion reflects broader debates in the AI community about safety, open research, and the responsibilities of educators.

**Discussion**: Commenters were divided: some argued that removing the book is a misstep because understanding neural networks helps the public grasp what large companies are building, while others saw it as a symbolic protest that will mainly drive people to archived copies. Several noted that massive capital investment and widespread ETF holdings mean many people are indirectly complicit in frontier AI development, and one commenter linked an Internet Archive snapshot of the book.

**Tags**: `#neural-networks`, `#AI-safety`, `#open-education`, `#community-discussion`, `#protest`

---

<a id="item-5"></a>
## [Google's DeepCrossAttention speeds transformer training up to 3x](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 7.0/10

Google Research introduced DeepCrossAttention (DCA), a depthwise attention-like primitive that replaces standard residual connections in transformers with learnable, input-dependent weights to dynamically combine representations across layers. The method reportedly achieves comparable model quality while training up to 3x faster. This work could significantly reduce the cost and time of training large transformer models, making deep architectures more practical for resource-constrained teams. It also contributes to the broader trend of redesigning residual connections and attention primitives to improve efficiency in deep learning systems. DCA uses input-dependent cross-attention over Query, Key, and Value components across depth, and the full paper is available on arXiv (2502.06785). The work is from 2025, and community members note related approaches like AttnRes and looping layers that may further amplify gains.

hackernews · ComputedCamp995 · Nov 27, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50672565)

**Background**: Transformers rely on residual connections (skip connections) to train deep networks effectively, acting as information highways that help gradients flow. Attention mechanisms allow models to weigh the importance of different inputs, and recent research explores applying attention-like operations depthwise—across layers rather than just across tokens—to improve representation learning. DeepCrossAttention is part of a line of work that replaces static residual additions with learned, dynamic combinations.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.06785v1">DeepCrossAttention : Supercharging Transformer Residual Connections</a></li>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections - Google Research</a></li>
<li><a href="https://www.alphaxiv.org/overview/2502.06785v1">DeepCrossAttention : Supercharging Transformer Residual... | alphaXiv</a></li>

</ul>
</details>

**Discussion**: Commenters pointed to the full arXiv paper and noted that the work is from 2025, so it is not brand new. Some discussed related techniques like AttnRes and looping layers, suggesting that combining them with DCA could yield even larger gains, while others shared anecdotal experiences with model speed and cost.

**Tags**: `#transformers`, `#attention-mechanisms`, `#machine-learning`, `#model-training`, `#google-research`

---

<a id="item-6"></a>
## [Show HN: Bouncemarket – a live prediction market game for a bouncing ball](https://bouncemarket.minhanhday.com/) ⭐️ 7.0/10

A developer launched bouncemarket, a live prediction market game where players bet on where a server-simulated bouncing ball will land. The game features deterministic replays, server-sent events for streaming, and AI traders that drop out when more than five human players join a round. This project demonstrates a novel application of prediction market mechanics to a purely chaotic physical simulation, sparking discussion about bot-vs-bot dynamics and the legal status of event contracts. It also serves as a technical showcase for server-side deterministic simulation streamed via SSE. The ball's drop is simulated server-side and streamed to clients via server-sent events with a small buffer, ensuring deterministic replays from the same starting position. However, tiny variations in the starting position can drastically change the outcome due to chaotic dynamics, and the AI traders use a naive rule-based system that is easy to beat.

hackernews · mday404 · Nov 27, 15:01 · [Discussion](https://news.ycombinator.com/item?id=50667726)

**Background**: Prediction markets are financial markets where participants trade binary contracts that pay out based on the outcome of an event. Server-sent events (SSE) is a web technology that allows a server to push real-time updates to a browser over a persistent HTTP connection. Chaotic systems are deterministic but highly sensitive to initial conditions, making long-term prediction difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Server-sent_events">Server-sent events</a></li>

</ul>
</details>

**Discussion**: Commenters found the game fun but noted that the fast odds movement makes betting difficult, and some discovered that buying cheap shares on both sides can guarantee a profit. Others discussed the potential for AI bots to dominate and the legal implications of prediction markets on random events.

**Tags**: `#prediction-markets`, `#game-development`, `#server-sent-events`, `#chaotic-systems`, `#show-hn`

---

<a id="item-7"></a>
## [D.J. Bernstein Critiques Reliance on Computer-Checked Proofs](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

D. J. Bernstein published a page cataloging soundness bugs in seven proof checkers—HOL Light, Mizar, Metamath, Isabelle, Lean, HOL98/HOL4, and Coq/Rocq—arguing that such bugs undermine trust in computer-checked proofs and calling for smaller trusted checkers and machine-checked proofs of checker correctness. This critique matters because formal verification is increasingly used in mathematics and software, and a soundness bug in a checker could invalidate many proofs; the debate highlights the need for robust verification practices and affects researchers, tool developers, and users relying on these systems. The page lists specific soundness bugs for each checker and argues for reducing the trusted computing base; however, commenters note that in practice multiple independent verifiers are often required (e.g., Metamath proofs must pass five independently-created verifiers), making a single bug insufficient to cause widespread false acceptance.

hackernews · _tk_ · Nov 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50667989)

**Background**: Proof assistants like Lean and Metamath are tools for formalizing and verifying mathematical proofs; their kernels check proofs for correctness, but bugs in these checkers (soundness bugs) can allow false statements to be accepted as proven. The formal verification community has long been aware of such bugs and has developed practices like using multiple independent checkers to increase confidence.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metamath">Metamath - Wikipedia</a></li>
<li><a href="https://news.lavx.hu/article/d-j-bernstein-catalogs-soundness-bugs-in-seven-proof-checkers">D. J. Bernstein catalogs soundness bugs in seven proof ...</a></li>

</ul>
</details>

**Discussion**: HN commenters debated the practical impact: twotwotwo and dwheeler emphasized that multiple independent verifiers (e.g., five for Metamath) make it hard for a single soundness bug to mislead mathematicians, while gr_norm noted that known soundness bugs are few and require further exploitation to hide real issues. andai raised a deeper concern about agents proving correctness against their own misunderstanding of the problem.

**Tags**: `#formal-verification`, `#proof-assistants`, `#soundness`, `#lean`, `#metamath`

---