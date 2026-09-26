---
layout: default
title: "Horizon Summary: 2026-09-26 (EN)"
date: 2026-09-26
lang: en
---

> From 29 items, 15 important content pieces were selected

---

1. [Terry Tao: AI Era Demands Far More Mathematicians](#item-1) ⭐️ 8.0/10
2. [Hacker News Debates Keeping Joy in Programming Amid LLMs](#item-2) ⭐️ 8.0/10
3. [Conversations leaves Google Play and goes free over poor support and fees](#item-3) ⭐️ 8.0/10
4. [DeepSeek Unveils DSec Sandbox System for Agentic Training at Scale](#item-4) ⭐️ 7.0/10
5. [Reladraw: A Diagram Language That Lets You Control Element Placement](#item-5) ⭐️ 7.0/10
6. [Fifteen Years Later, Apple's Cards App Origin Story](#item-6) ⭐️ 7.0/10
7. [Economist Warns Plunging Test Scores Are a Slow-Moving Catastrophe](#item-7) ⭐️ 7.0/10
8. [Floci: Free Open-Source Tool Emulates Any Cloud Service Locally](#item-8) ⭐️ 7.0/10
9. [Automattic Forms New Board After Failed Attempt to Sideline CEO Matt Mullenweg](#item-9) ⭐️ 7.0/10
10. [Insurers Say AI Coding Tools Added $942M to Hospital Costs](#item-10) ⭐️ 7.0/10
11. [KoboldCpp Ships Built-in Lightweight Agent Harness With 9 Tools](#item-11) ⭐️ 7.0/10
12. [Fixed GPT-OSS Chat Template Patches Unsloth Reasoning-History Bug](#item-12) ⭐️ 7.0/10
13. [4x RTX 3060 Ti Rig Hits 120 t/s Local LLM Inference via Tensor Parallelism](#item-13) ⭐️ 7.0/10
14. [Ling Tiny 3.0 runs agentic coding on a 2017 laptop without GPU](#item-14) ⭐️ 7.0/10
15. [Splash 1.1.0 adds GGUF quantization and MLX import for Apple Silicon](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Terry Tao: AI Era Demands Far More Mathematicians](https://terrytao.wordpress.com/2026/09/24/were-gonna-need-a-lot-more-mathematicians/) ⭐️ 8.0/10

Terry Tao published an essay on his blog arguing that as AI systems grow more capable, society will need far more mathematicians to understand, verify, and justify the safety of AI-driven designs. The post sparked a 458-comment Hacker News discussion about the irreplaceable role of human comprehension. The essay reframes AI safety as a demand for human mathematical expertise rather than only better models, and it arrives as Fields Medalists and researchers debate AI's role in mathematics. It affects mathematicians, software engineers, and anyone relying on AI-generated designs whose correctness must be justified to the public. Tao's argument centers on the idea that approving a design requires communities of humans to understand why it works and what justifies confidence in its safety, a standard that becomes harder to meet as AI outputs outpace human review. The discussion also highlighted that formal verification tools like Lean can check AI-generated proofs, but human judgment is still needed to decide what is worth proving and how to interpret results.

hackernews · srcreigh · Sep 26, 02:46 · [Discussion](https://news.ycombinator.com/item?id=49852717)

**Background**: Terry Tao is one of the world's most prominent mathematicians and has written extensively about how AI is changing mathematical research, including formal proof assistants such as Lean that let computers mechanically verify proofs. Recent work has shown LLM-based agents can generate proofs that Lean then checks, but unreliability remains a barrier to using AI in serious research. The Hacker News thread reflects a broader debate about whether AI-generated code and designs can be trusted without deep human understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://teorth.github.io/tao-web/ai-views.html">Terence Tao on AI in mathematics (and beyond)</a></li>
<li><a href="https://arxiv.org/abs/2605.22763">[2605.22763] Advancing Mathematics Research with AI-Driven Formal Proof Search</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed that human comprehension is essential, with one noting they now catch fewer bugs in Claude-generated code and worry about becoming less careful under shipping pressure. Others argued that studying mathematics transforms the mind rather than producing commodities, and that LLM output is useless without a human to comprehend it; some observed that colleagues who hand everything to Claude run into XY problems, poor UX, and over-complex solutions.

**Tags**: `#AI`, `#mathematics`, `#software-engineering`, `#human-comprehension`, `#LLM`

---

<a id="item-2"></a>
## [Hacker News Debates Keeping Joy in Programming Amid LLMs](https://discourse.haskell.org/t/how-to-keep-enjoying-programming-in-a-world-of-llms/14705) ⭐️ 8.0/10

A Hacker News discussion titled "How to keep enjoying programming in a world of LLMs" drew 134 points and 190 comments, with developers sharing personal experiences about how AI coding assistants are changing their motivation, skills, and satisfaction. The thread, originally linked from the Haskell Discourse, surfaced diverse viewpoints ranging from skill atrophy and lost motivation to renewed enjoyment after offloading tedious work to LLMs. As LLM-based coding tools like GitHub Copilot, Cursor, and Claude become standard in developer workflows, this conversation highlights a growing tension between productivity gains and the erosion of hands-on skills and intrinsic motivation. The sentiment matters for engineering teams, tool builders, and educators who must decide how to integrate AI without hollowing out the craft of programming. Commenters described concrete effects: one developer said punting any task to an LLM causes that skill to atrophy, citing sudden difficulty planning a small project's architecture; another reported losing motivation entirely with agentic coding, feeling like "meat shuffling data and permissions between bots." A contrasting view noted that using a very fast, low-reasoning model (e.g., GPT-6 Luna low effort + fast mode) keeps the developer hands-on and avoids long waits.

hackernews · signa11 · Sep 26, 09:41 · [Discussion](https://news.ycombinator.com/item?id=49854875)

**Background**: Hacker News is a social news site run by Y Combinator, focused on computer science and entrepreneurship, where discussions often shape industry sentiment. LLM-based coding tools such as GitHub Copilot, Cursor, and Claude can generate, complete, and refactor code from natural-language prompts, and they have been widely adopted since 2023. "Skill atrophy" refers to the weakening of learned abilities—like debugging or architectural planning—through disuse when those tasks are delegated to AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hacker_News">Hacker News</a></li>
<li><a href="https://blog.stackademic.com/skill-atrophy-the-engineers-who-cant-debug-without-ai-anymore-afe212162ef7">“ Skill Atrophy ” — the engineers who can’t debug... | Stackademic</a></li>
<li><a href="https://simonwillison.net/2025/Mar/11/using-llms-for-code/">Here’s how I use LLMs to help me write code</a></li>

</ul>
</details>

**Discussion**: The community sentiment is mixed but leans toward concern: several developers reported skill atrophy, lost motivation, and frustration with buggy generated code, while others said LLMs let them offload boring work and enjoy programming more. A recurring theme was the analogy to car mechanics—some prefer hand tools, others tune with software—and one commenter suggested fast, low-reasoning models preserve hands-on engagement.

**Tags**: `#LLM`, `#programming`, `#developer experience`, `#skill atrophy`, `#Hacker News`

---

<a id="item-3"></a>
## [Conversations leaves Google Play and goes free over poor support and fees](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 8.0/10

The developer of Conversations, the popular open-source XMPP/Jabber messaging client for Android, announced that the app is leaving Google Play and becoming free of charge. The decision was driven by Google's poor developer support and the fees the platform charges. This highlights growing friction between independent open-source developers and Google Play's dominance over Android app distribution, and it could push more users toward direct APK downloads or alternative stores. It also fuels the broader debate about app store monopolies and developer treatment. Conversations is a free and open-source XMPP client for Android 6.0+ that emphasizes open standards, and the developer's post specifically cites poor support and fees as reasons for leaving. The move means users will need to obtain the app outside Google Play, such as via direct APK or alternative distribution channels.

hackernews · ezst · Sep 26, 10:55 · [Discussion](https://news.ycombinator.com/item?id=49855315)

**Background**: Conversations is a widely used instant messaging app for Android built on the open XMPP (Extensible Messaging and Presence Protocol) standard, rather than a proprietary protocol. Google Play is the default app store on most Android devices and charges developers service fees while enforcing content and distribution policies. Leaving it means the app must rely on direct downloads or third-party stores, which can reduce visibility but give the developer more control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Conversations_(software)">Conversations (software) - Wikipedia</a></li>
<li><a href="https://conversations.im/">Conversations : the very last word in instant messaging</a></li>
<li><a href="https://support.google.com/googleplay/android-developer/answer/112622?hl=en-EN">Service fees - Play Console Help</a></li>

</ul>
</details>

**Discussion**: Commenters largely sympathized with the developer, arguing that Google's 15% fee would be acceptable if the company provided good support and timely reviews, and that its monopoly lets it neglect developers. Several shared frustrations about Google's terrible customer support and burdensome verification requirements, while others warned that Android is making it harder to install apps outside the Play Store.

**Tags**: `#Google Play`, `#app distribution`, `#monopoly`, `#developer experience`, `#open source`

---

<a id="item-4"></a>
## [DeepSeek Unveils DSec Sandbox System for Agentic Training at Scale](https://arxiv.org/abs/2609.22978) ⭐️ 7.0/10

DeepSeek has introduced DeepSeek Elastic Compute (DSec), a sandbox infrastructure that achieves 380,000 concurrent sandboxes on 160 AMD EPYC nodes, as detailed in an arXiv paper. The system is co-designed with DeepSeek's reinforcement learning framework and, starting with DeepSeek-V4.1, moves rollout execution onto DSec by splitting it into an agent sandbox and a worker container. DSec's scale and tight coupling with RL training could significantly lower the cost and complexity of running large-scale agentic training, a key bottleneck for building capable AI agents. The system's design also hints at broader serverless computing implications, as the community quickly noted. DSec decouples stateful rollout execution from preemptible GPU training and coordinates sandbox lifecycle with training to preserve rollout state while reclaiming idle resources. The paper is also notable for its unusually large author list of 131 people, which dominated community discussion.

hackernews · shenli3514 · Sep 26, 18:22 · [Discussion](https://news.ycombinator.com/item?id=49859112)

**Background**: In AI agent training, a sandbox is an isolated environment where untested code and agent actions can run without affecting production systems. AMD EPYC is a brand of multi-core x86-64 server processors, and 160 such nodes hosting 380,000 concurrent sandboxes illustrates the density of the virtualization layer. DeepSeek is a Chinese AI company known for its large language models and reinforcement learning research.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.22978">[2609.22978] DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>
<li><a href="https://technode.com/2026/09/23/deepseek-dsec-agent-training-sandbox-infrastructure/">DeepSeek details DSec sandbox infrastructure for agent training · TechNode</a></li>
<li><a href="https://arxiv.org/html/2609.22978v1">DeepSeek Elastic Compute (DSec): A Sandbox Infrastructure for Effective Agentic Training at Scale</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were most struck by the paper's 131 authors, with one joking that the topic is less interesting than how so many authors communicated to publish it. Others expressed disbelief at the scale of 380,000 concurrent sandboxes on 160 EPYC nodes, and one commenter asked simply whether this amounts to serverless computing.

**Tags**: `#deepseek`, `#elastic-compute`, `#serverless`, `#distributed-systems`, `#arxiv`

---

<a id="item-5"></a>
## [Reladraw: A Diagram Language That Lets You Control Element Placement](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw is a new open-source diagramming language that combines the convenience of declarative diagram-as-code tools with manual control over element placement. It ships with a browser playground for no-install testing, an npm package, and an agent skill for Claude and other AI agents. Existing diagram-as-code tools force a trade-off: auto-layout languages like Mermaid and Graphviz decide the layout for you, while GUI editors like Draw.io are powerful but slow and hard for AI agents to manipulate. Reladraw targets both human authors and AI agents, addressing a real pain point as agent-driven development workflows grow. The language uses relative positioning instructions rather than absolute coordinates, which early users found sufficient for most needs. Community members reported minor bugs, such as an edge not rendering as a curved arrow, and suggested that a renderer-agnostic backend could let the same layout instructions target multiple rendering engines.

hackernews · jpwalsh234 · Sep 26, 17:10 · [Discussion](https://news.ycombinator.com/item?id=49858513)

**Background**: Declarative diagramming tools such as Mermaid, Graphviz (using the DOT language), and D2 let users describe diagrams in text and have the software automatically compute the layout. This is fast and version-controllable but gives authors little say in where nodes end up, which matters for flowcharts where position carries meaning. Reladraw aims to keep the text-based workflow while restoring placement control.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49858513">Show HN: Reladraw – A diagram language where you... | Hacker News</a></li>
<li><a href="https://6ic.com/news/reladraw-a-new-precision-tool-for-diagram-design-emerges">Reladraw : A New Precision Tool for Diagram Design Emerges</a></li>
<li><a href="https://blog.logrocket.com/complete-guide-declarative-diagramming-d2/">A complete guide to declarative diagramming with D2 - LogRocket Blog</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive, with one noting that Mermaid works well for fixed layouts like sequence diagrams and Gantts but is poor for flowcharts where position is king, and that relative positioning is probably enough. Others reported early bugs, asked whether the tool needs to ship with its own renderer or could target multiple backends, and compared it to alternatives like D2. One user observed that AI assistants writing .dot diagrams struggle with placement in the same way humans do.

**Tags**: `#diagramming`, `#developer-tools`, `#visualization`, `#DSL`, `#AI-agents`

---

<a id="item-6"></a>
## [Fifteen Years Later, Apple's Cards App Origin Story](https://lexontech.org/fifteen-years-later-the-apple-cards-origin-story) ⭐️ 7.0/10

A retrospective article recounts the origin story of Apple's Cards app, the 2011 iPhone-to-printed-card service announced by Apple, detailing the technical and business challenges behind it. The piece is accompanied by community comments, including a firsthand account from the co-founder of the competing startup Sincerely, who felt his company had been "Sherlocked" by Apple's announcement. The story offers a rare behind-the-scenes look at how Apple develops and launches products, and how a major platform announcement can upend smaller startups building similar features. It also highlights the unusual technical partnership between Apple and the USPS, showing how much custom engineering was needed to make a seemingly simple consumer feature work. Because Apple refused to print visible barcodes on the envelopes but still wanted end-to-end tracking, Apple and its printing partner developed an invisible barcode sprayed onto the envelope that was only visible under certain UV light, and the USPS agreed to scan the cards at sending and at mail processing facilities. Community commenters also noted that the app was used for frictionless, spontaneous photo cards to offline family members, and debated how letterpress and debossing aesthetics shaped the product.

hackernews · ksec · Sep 26, 09:13 · [Discussion](https://news.ycombinator.com/item?id=49854693)

**Background**: Apple's Cards app was announced in 2011 as part of the iPhone ecosystem, letting users design a physical card on their phone and have it printed and mailed by Apple. "Sherlocking" is a term in the Apple developer community for when Apple builds a feature into its own operating system that duplicates a third-party app's functionality, potentially killing that business. Letterpress is a traditional printing technique that presses inked type into paper, and debossing is a related method that creates a recessed impression, which some commenters argue shaped how digital-to-physical card products looked and felt.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Card">Apple Card - Wikipedia</a></li>
<li><a href="https://www.apple.com/apple-card/">Apple Card - Apple</a></li>

</ul>
</details>

**Discussion**: The discussion is rich and mixed in tone: the co-founder of Sincerely describes feeling "Sherlocked" and a mix of fear and anger when Apple announced Cards, while others share personal anecdotes about using the app to send spontaneous photos to offline elderly relatives. Commenters also reflect critically on founder-led companies and on how the aesthetics of letterpress and debossing shaped the product, adding both personal and technical nuance.

**Tags**: `#Apple`, `#startups`, `#product development`, `#USPS`, `#Hacker News`

---

<a id="item-7"></a>
## [Economist Warns Plunging Test Scores Are a Slow-Moving Catastrophe](https://www.economist.com/leaders/2026/09/10/plunging-test-scores-are-a-slow-moving-catastrophe) ⭐️ 7.0/10

An Economist leader article published on September 10, 2026 argues that declining student test scores constitute a slow-moving catastrophe, prompting a substantial Hacker News discussion about its causes. Commenters debated whether AI, algorithmic social media, screen-based learning, or demographic shifts are primarily responsible for the decline. Standardized test scores are a key indicator of future workforce skill and economic competitiveness, so a sustained multi-year decline signals long-term damage to human capital. The debate also matters because proposed remedies—phone bans, returning to textbooks, handwriting instead of Chromebooks—depend heavily on correctly diagnosing the root cause. One commenter noted that the drop from 2018 to 2022 is as large as the one from 2022 to 2026, making AI's role ambiguous, and observed that science scores were less affected than math and reading, which rely more on attention and practice. Another commenter argued that re-weighting 1998 NAEP 8th-grade reading scores by 2024 demographics predicts a 4.6-point decline, close to the actual 4-point fall, suggesting demographic change explains much of the trend.

hackernews · vinni2 · Sep 26, 15:24 · [Discussion](https://news.ycombinator.com/item?id=49857442)

**Background**: The article appears in The Economist's leaders section, which presents the magazine's editorial stance on major issues. The discussion references the attention economy—the competitive market in which platforms monetize users' limited attention—as well as NAEP, the National Assessment of Educational Progress, often called the Nation's Report Card, which tracks US student achievement over time. It also touches on the ongoing debate over AI's impact on education and on social media's effects on students' attention, sleep, and academic performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coursera.org/articles/attention-economy">What Is the Attention Economy ? | Coursera</a></li>
<li><a href="https://www.publicschoolreview.com/blog/the-impact-of-social-media-on-students-2026-update">The Impact of Social Media on Students (2026 Update)</a></li>
<li><a href="https://www.clrn.org/how-does-social-media-affect-students-academic-performance/">How Does Social Media Affect Students’ Academic Performance?</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters broadly agreed the decline is real but disagreed on its main cause: some blamed the optimized monetization of human attention and algorithmic social media, others pointed to AI, and one argued demographic change explains most of the drop. Several commenters shared personal observations about phone bans, a return to textbooks and handwriting, and even declining physical fitness, with the general sentiment that screens and the online social environment have rewired children's attention.

**Tags**: `#education`, `#test scores`, `#AI impact`, `#social media`, `#attention economy`

---

<a id="item-8"></a>
## [Floci: Free Open-Source Tool Emulates Any Cloud Service Locally](https://floci.io/) ⭐️ 7.0/10

Floci is a community-driven, MIT-licensed tool that locally emulates AWS, Azure, GCP, and OCI services in milliseconds without requiring a cloud account, auth token, or paid feature gates. It offers an alternative to LocalStack and emphasizes extensible, AI-assisted test suite creation so developers can write their own cloud-compatible tests and implement matching features. Local cloud emulation addresses a real developer pain point by enabling fast, credential-free feedback loops for development, testing, and CI, which is especially valuable for AI coding agents that need to validate behavior without provisioning real infrastructure. Floci's community-driven, AI-assisted approach could lower the barrier to contributing new service emulations and challenge LocalStack's dominance in this space. Floci is MIT licensed and free, with no account or auth token required, and it supports multiple clouds including AWS, GCP (Cloud Storage, Pub/Sub, Firestore, Datastore, Secret Manager, IAM, Managed Kafka, Cloud Tasks, Cloud Run), Azure, and OCI. A key caveat raised in discussion is the risk of drift between emulated and real cloud service behavior, which could cause show-stopping differences when switching to production.

hackernews · theanonymousone · Sep 26, 08:31 · [Discussion](https://news.ycombinator.com/item?id=49854416)

**Background**: Local cloud emulators like LocalStack simulate cloud provider APIs on a developer's machine so applications can be built and tested without provisioning real cloud infrastructure. This is useful for unit and integration testing, CI pipelines, and offline development, but emulators may not perfectly match real cloud behavior. Floci enters this space as a free, open-source alternative that supports multiple cloud providers and encourages community contributions.

<details><summary>References</summary>
<ul>
<li><a href="https://floci.io/">Floci — Local Cloud Emulators</a></li>
<li><a href="https://github.com/floci-io/floci">GitHub - floci-io/floci: Light, fluffy, and always free - The ...</a></li>
<li><a href="https://docs.localstack.cloud/">Welcome to LocalStack Docs</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted Floci's lightweight nature and ease of writing custom test suites, with one user noting it is much lighter than LocalStack and works well with Testcontainers. Others raised concerns about behavioral drift between mocked and real APIs, and questioned whether emulators are needed when cloud-specific code is already abstracted away. A humorous note pointed out that 'Floci' means 'pubic hairs' in Romanian.

**Tags**: `#cloud-emulation`, `#local-development`, `#testing`, `#open-source`, `#developer-tools`

---

<a id="item-9"></a>
## [Automattic Forms New Board After Failed Attempt to Sideline CEO Matt Mullenweg](https://techcrunch.com/2026/09/25/automattic-has-a-new-board-after-failed-attempt-to-put-ceo-on-leave/) ⭐️ 7.0/10

Automattic has formed a new board of directors after its original board voted to place CEO Matt Mullenweg on paid leave, a move Mullenweg reversed by taking back control of the company and letting go of those involved, which he described on X as a 'coup attempt.' The episode raises questions about board efficacy given Mullenweg's roughly 84% voting control of the company. This is a notable corporate governance story for Automattic, the company behind WordPress, which powers a large share of the web, and it highlights how founder-controlled multi-class share structures can render boards powerless even when directors attempt to act. The outcome may influence how investors, employees, and the broader open-source community view governance at founder-led technology companies. Mullenweg reportedly holds about 84% of Automattic's voting shares, meaning the original board's vote to put him on leave was effectively pre-ordained to fail, and he told staff via Slack that he had regained control days later. Community members also noted that the outgoing board members allegedly granted themselves generous severance packages during their brief interim.

hackernews · ilamont · Sep 26, 15:40 · [Discussion](https://news.ycombinator.com/item?id=49857572)

**Background**: Automattic is the company behind WordPress, the open-source publishing platform that powers a large portion of websites worldwide, and Matt Mullenweg is its co-founder of WordPress and founder and CEO of Automattic. Corporate boards are typically responsible for overseeing management and protecting shareholder interests, but in multi-class share structures where a founder holds a supermajority of voting power, the board's practical authority is sharply limited. This episode is part of a broader pattern of founder-controlled tech companies where governance mechanisms struggle to constrain the founder.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/25/automattic-has-a-new-board-after-failed-attempt-to-put-ceo-on-leave/">Automattic has a new board after failed attempt to put... | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Matt_Mullenweg">Matt Mullenweg - Wikipedia</a></li>
<li><a href="https://cryptobriefing.com/mullenweg-regains-automattic-control-board-ouster/">Matt Mullenweg claims he's back in charge at Automattic days after...</a></li>

</ul>
</details>

**Discussion**: Commenters broadly questioned how the board could have expected to succeed given Mullenweg's 84% voting control, with some calling the attempt value-destroying negligence and others suggesting the board's real goal may have been generous severance packages. A few defended Mullenweg's power move, while others said the drama makes them less inclined to use WordPress.

**Tags**: `#Automattic`, `#WordPress`, `#corporate-governance`, `#Matt Mullenweg`, `#tech-industry`

---

<a id="item-10"></a>
## [Insurers Say AI Coding Tools Added $942M to Hospital Costs](https://techcrunch.com/2026/09/26/insurers-claim-ai-is-already-increasing-healthcare-costs/) ⭐️ 7.0/10

Blue Cross Blue Shield Association (BCBSA) released an analysis of its claims data concluding that hospitals' growing use of AI coding and billing tools contributed an additional $942 million in healthcare spending over a two-year period. The insurer group says the tools drive higher billing by generating more severe diagnosis codes without corresponding increases in treatment. This is one of the first concrete, quantified claims that AI adoption in hospitals is raising rather than lowering costs, directly challenging the industry narrative that AI will make healthcare cheaper. The finding could shape payer audits, reimbursement policy, and regulatory scrutiny of AI billing tools, affecting hospitals, insurers, and patients alike. The $942 million figure comes from BCBSA's analysis of its own claims data, and the mechanism cited is essentially AI-assisted upcoding — billing for more severe or complex conditions than the delivered care supports. Hospitals dispute this interpretation, arguing the AI tools improve documentation accuracy rather than inflate charges.

rss · TechCrunch · Sep 26, 21:02

**Background**: Upcoding is a long-standing billing practice in which a provider submits a code for a more severe or complex condition than the care actually delivered, resulting in higher reimbursement. AI coding tools can listen to doctor-patient conversations, auto-generate diagnosis codes, and optimize claims submissions, which supporters say reduces administrative burden and errors. Insurers argue the same automation can systematically inflate diagnoses and spending, making this an emerging flashpoint in the debate over AI's real economic impact on healthcare.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bcbs.com/about-us/association-news/new-bcbsa-research-on-ai-hospital-billing-driving-higher-health-care-costs">New BCBSA Research Shows AI Billing Raises Health Care Costs</a></li>
<li><a href="https://www.medicaldaily.com/blue-cross-ai-coding-medically-complex-hospital-records-479102">Blue Cross Ties $942 Million in Added Hospital Costs to AI Coding...</a></li>
<li><a href="https://cryptobriefing.com/blue-cross-hospital-ai-billion-cost-rise/">Blue Cross report links hospital AI to $1B rise in costs</a></li>

</ul>
</details>

**Tags**: `#AI in healthcare`, `#healthcare costs`, `#AI economics`, `#insurance`, `#AI policy`

---

<a id="item-11"></a>
## [KoboldCpp Ships Built-in Lightweight Agent Harness With 9 Tools](https://www.reddit.com/r/LocalLLaMA/comments/1wqlyp8/introducing_koboldcpp_agent_and_a_plea_for_help/) ⭐️ 7.0/10

KoboldCpp, the popular local LLM inference tool maintained by LostRuins (concedo), now ships with a built-in agent harness that can be enabled with a single checkbox in the Admin tab or the --agent launch flag. It includes 9 built-in tools and a compact system prompt of only about 2k tokens including all tool definitions, and it can also connect to third-party OpenAI Chat Completions-compatible backends or load extra tools via an mcp.json file. This lowers the barrier to agentic workflows for local LLM users, offering a much lighter alternative to heavier harnesses like Claude Code, Codex, or Opencode that often require complicated external setup. Since KoboldCpp is widely used in the local AI community, bundling agent capabilities directly into the tool could make simple autonomous tasks accessible to far more users. To run effectively the agent needs at least 28k context and 8k generation tokens, with larger values recommended, and roughly 12GB of VRAM for a good experience; it also offers three tool-call approval modes (on/auto/off) and supports AGENTS.md plus context compaction. Note that MCP tools execute on the KoboldCpp server while agent tools execute on the agent client, and the maintainer warns users to exercise caution when approving tool calls.

reddit · r/LocalLLaMA · /u/HadesThrowaway · Sep 26, 09:13

**Background**: An agent harness (also called agent scaffolding) is the software layer around a language model that lets it act as an agent: it manages tool use, memory, state persistence, and multi-step feedback loops, so that agent = model + harness. KoboldCpp itself is a self-contained, easy-to-use text-generation program for GGML and GGUF models, built on top of llama.cpp with a KoboldAI-inspired interface. Until now, local users who wanted agentic behavior typically had to set up separate external harnesses such as Claude Code, Codex, or Opencode.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://github.com/LostRuins/koboldcpp">GitHub - LostRuins/koboldcpp: Run GGUF models easily with a ...</a></li>
<li><a href="https://grokipedia.com/page/KoboldCpp">KoboldCpp</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#koboldcpp`, `#ai-agents`, `#llm-tooling`, `#open-source`

---

<a id="item-12"></a>
## [Fixed GPT-OSS Chat Template Patches Unsloth Reasoning-History Bug](https://www.reddit.com/r/LocalLLaMA/comments/1wr0wki/improved_and_fixed_template_for_gptoss_again/) ⭐️ 7.0/10

A LocalLLaMA user (arbv) released an updated GPT-OSS Jinja chat template on Hugging Face that fixes a serious bug inherited from Unsloth's version, where messages containing both reasoning and final content only rendered the reasoning trace during chat history replay. The new template also adds a preserve_thinking option so prior analysis turns are kept intact across multi-turn inference. Many inference tools and API harnesses now replay prior reasoning turns by default, so this bug could silently degrade GPT-OSS output quality in common multi-turn and agentic workflows. Fixing it restores correct context for the model and, with preserve_thinking, enables prefix caching that speeds up multi-turn inference. The buggy branch in Unsloth's template drops the model's answer whenever a message contains both thinking and content, and its comment claiming CoT is dropped is itself incorrect; OpenAI's reference template does not have this branch. The reporter observed GPT-OSS 20B going badly off the rails, while GPT-OSS 120B could often recover from reasoning traces alone, and notes preserve_thinking increases token usage in exchange for faster prefix-cached inference.

reddit · r/LocalLLaMA · /u/arbv · Sep 26, 20:35

**Background**: GPT-OSS is OpenAI's open-weight reasoning model family (20B and 120B) that uses a structured 'harmony' response format with separate analysis and final channels. Chat templates are Jinja files that convert conversation history into the exact token sequence a model expects, so a flawed template can corrupt context without any obvious error. Unsloth is a popular library for efficient fine-tuning and quantized inference, and its templates are widely reused by the community.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/openai/gpt-oss-120b/blob/main/chat_template.jinja">chat _ template .jinja · openai/ gpt - oss -120b at main</a></li>
<li><a href="https://github.com/openai/gpt-oss">GitHub - openai/ gpt - oss : gpt - oss -120b and gpt - oss -20b are two...</a></li>
<li><a href="https://huggingface.co/unsloth/gpt-oss-20b-GGUF">unsloth/gpt-oss-20b-GGUF · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#GPT-OSS`, `#chat-template`, `#Unsloth`, `#LocalLLaMA`, `#bug-fix`

---

<a id="item-13"></a>
## [4x RTX 3060 Ti Rig Hits 120 t/s Local LLM Inference via Tensor Parallelism](https://www.reddit.com/r/LocalLLaMA/comments/1wqv9o8/getting_stupidly_good_results_on_my_4x3060ti_setup/) ⭐️ 7.0/10

A Reddit user on r/LocalLLaMA reported building a 4x RTX 3060 Ti rig (8GB VRAM each, power-limited to 110W) and achieving roughly 70 t/s with Exl3 tensor parallelism and about 120 t/s at bf16 with HyperQwen on vLLM, supporting up to a 150k context window. By quantizing the KV cache to kv8, the full 262k context becomes available, though throughput drops back to around 70 t/s. This shows that consumer-grade Ampere GPUs, including cards originally bought for crypto mining, can be repurposed into a capable local LLM inference cluster without buying expensive new hardware. It highlights how tensor parallelism and optimized serving stacks like Exl3 and HyperQwen are making high-throughput, long-context local inference accessible to hobbyists and small teams. The setup uses tensor parallelism (TP=4) across four 8GB cards, which llama.cpp does not support, leading the user to Turboderp's Exl3 and later the HyperQwen repo designed for Ampere GPUs. Concurrency is reported to add barely any slowdown, allowing either one agent at 120 t/s or two concurrent agents with a large context window.

reddit · r/LocalLLaMA · /u/DontWinFrensWthSalad · Sep 26, 16:47

**Background**: Tensor parallelism splits a model's tensors across multiple GPUs so that both parameters and intermediate activations are sharded, enabling models too large for a single card to run collectively. Exl3 (ExLlamaV3) is a quantization and inference project from Turboderp that brings state-of-the-art quantization to consumer hardware, while HyperQwen is a serving stack optimized for running large Qwen models on consumer Ampere GPUs via vLLM.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/turboderp-org/exllamav3">GitHub - turboderp -org/exllamav3: An optimized quantization and...</a></li>
<li><a href="https://github.com/syv-ai/HyperQwen">GitHub - syv-ai/HyperQwen: Serve large Qwen models fast on ...</a></li>
<li><a href="https://awsdocs-neuron.readthedocs-hosted.com/en/latest/libraries/nxd-inference/app-notes/parallelism.html">Parallelism Techniques for LLM Inference — AWS Neuron ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#multi-gpu`, `#tensor-parallelism`, `#exl3`, `#hardware`

---

<a id="item-14"></a>
## [Ling Tiny 3.0 runs agentic coding on a 2017 laptop without GPU](https://www.reddit.com/r/LocalLLaMA/comments/1wqcrly/ling_tiny_30_is_a_glimpse_of_the_future/) ⭐️ 7.0/10

A Reddit user demonstrated that Ling Tiny 3.0, an 8B-parameter Mixture-of-Experts model with only 1B active parameters, can autonomously write, run, and iterate on code using llama.cpp on a 2017 laptop with a 7th-gen i5 CPU and 8GB of RAM, with no GPU or VRAM. The model generated roughly 10 tokens per second and completed a multi-turn agentic coding task—scanning the local network for llama.cpp servers—in about 20 minutes. This demonstrates that capable agentic coding is no longer limited to expensive GPU rigs, potentially turning the vast installed base of older CPUs and edge devices into useful AI-capable machines without new hardware. It signals a broader trend where small MoE models make local AI practical for casual and edge computing. The model ran with a Q6 quantization built directly from llama.cpp with no optimization effort, achieving about 10 tokens per second on CPU alone. The task was relatively simple, and the user notes that more expensive hardware will always be faster and more power-efficient, so using old hardware may not be practical for all workloads.

reddit · r/LocalLLaMA · /u/netherreddit · Sep 26, 00:40

**Background**: Mixture-of-Experts (MoE) is an architecture where a model contains many specialized sub-networks (experts) but only activates a small fraction of them per prompt, so an 8B-parameter model can use just 1B active parameters at inference time. llama.cpp is an open-source C/C++ inference engine that has become the de facto standard for running large language models locally on consumer hardware, including CPUs. Agentic coding refers to AI agents that can autonomously write, run, and debug code in an iterative loop.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://www.microcenter.com/site/mc-news/article/mixture-of-experts-moe-for-ai-explained.aspx">Mixture of Experts ( MoE ) Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#moe`, `#llama.cpp`, `#edge-ai`, `#agentic-coding`

---

<a id="item-15"></a>
## [Splash 1.1.0 adds GGUF quantization and MLX import for Apple Silicon](https://www.reddit.com/r/LocalLLaMA/comments/1wqw9rn/splash_110_released_gguf_quants_support_mlx/) ⭐️ 7.0/10

Splash 1.1.0 has been released, adding support for GGUF quantized models and MLX import, as announced on the r/LocalLLaMA subreddit. A user reports running a 27B Qwen3 model (Unsloth UD-Q4_K_XL) at roughly 50 tokens per second on an M5 Pro with 64GB of unified memory in an agentic workflow. This release matters because it consolidates optimized kernels, speculative decoding, prefix caching, and mixed-weight support into a single tool for Apple Silicon, making high-quality local LLM inference more practical. It lowers the barrier for Mac users who want to run large models locally without relying on cloud APIs. The reported 50 t/s figure comes from a single user's M5 Pro 64GB setup using a 27B model at Q4_K_XL quantization, so real-world performance will vary by hardware and model. Splash combines several acceleration techniques—optimized kernels, speculative decoding, prefix cache, and mixed-weight support—which together contribute to the speedup.

reddit · r/LocalLLaMA · /u/wojtek15 · Sep 26, 17:27

**Background**: GGUF is a file format for storing quantized large language models, widely used in the local AI community because it reduces model size and memory requirements while preserving quality. MLX is Apple's array framework for machine learning on Apple Silicon, optimized for the unified memory architecture of M-series chips. Speculative decoding is a technique that speeds up inference by using a smaller draft model to predict multiple tokens, which are then verified in parallel by the larger model. Splash appears to be a new inference engine that brings these technologies together for Mac users.

<details><summary>References</summary>
<ul>
<li><a href="https://ggufloader.github.io/what-is-gguf.html">What is GGUF? Complete Guide to GGUF Format & Quantization</a></li>
<li><a href="https://github.com/ml-explore/mlx">GitHub - ml-explore/mlx: MLX: An array framework for Apple ...</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency ...</a></li>

</ul>
</details>

**Discussion**: The Reddit post frames Splash as a breakthrough for local inference on Apple Silicon, with the author highlighting the combination of optimized kernels, speculative decoding, prefix cache, and mixed-weight support. While the discussion is positive, the performance claim rests on a single user's experience, so broader community validation is still pending.

**Tags**: `#local-llm`, `#apple-silicon`, `#gguf`, `#mlx`, `#inference-optimization`

---