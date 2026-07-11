---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 19 items, 9 important content pieces were selected

---

1. [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](#item-1) ⭐️ 9.0/10
2. [Einstein's relativity governs chemical bonds in heavy elements](#item-2) ⭐️ 8.0/10
3. [Building Docker Bridge Network from Scratch](#item-3) ⭐️ 8.0/10
4. [Official jscrambler npm Package Compromised at v8.14.0](#item-4) ⭐️ 8.0/10
5. [Programs, Not Objects: Data-Oriented 3D Editor Design](#item-5) ⭐️ 8.0/10
6. [ClickHouse scales PgBouncer 4x with SO_REUSEPORT and peering](#item-6) ⭐️ 7.0/10
7. [Prefer STRICT Tables in SQLite for Type Safety](#item-7) ⭐️ 7.0/10
8. [George Hotz Criticizes AI 2040 Report, Champions Freedom](#item-8) ⭐️ 7.0/10
9. [CISA built incident playbook during real breach](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 makes Model Runner V2 the default execution path for all dense models, removes the legacy PagedAttention implementation, and introduces a new Streaming Parser Engine for unified tool-call and reasoning parsing. The release also adds support for several new models including LLaVA-OneVision-2, GLM-5, and MiniMax-M3 with pipeline parallelism. This release marks a major architectural shift in vLLM, streamlining the inference engine by removing the legacy PagedAttention and making Model Runner V2 the standard. The performance improvements and new model support further solidify vLLM's position as a leading open-source LLM inference engine, benefiting developers and researchers deploying large language models in production. The release includes 558 commits from 232 contributors, with 64 new contributors. Model Runner V2 now supports EVS, realtime embeddings, prefix caching for Mamba hybrid models, and dynamic speculative decoding with full CUDA graphs. The Transformers modeling backend is now as fast as native vLLM and gained FP8 MoE support.

github · khluu · Jul 11, 20:06

**Background**: vLLM is an open-source high-throughput LLM inference engine that uses PagedAttention for efficient memory management of KV cache. Model Runner V2 is a newer execution backend that improves performance and flexibility. The removal of legacy PagedAttention indicates that vLLM has fully transitioned to its V1 and MRv2 backends.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention - Wikipedia</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#open source`, `#release`, `#AI infrastructure`

---

<a id="item-2"></a>
## [Einstein's relativity governs chemical bonds in heavy elements](https://www.brown.edu/news/2026-07-09/chemical-bonds-relativity) ⭐️ 8.0/10

Brown University chemists have provided the first direct experimental evidence that Einstein's theory of relativity fundamentally alters the structure of triple chemical bonds in heavy elements, specifically through spin-orbit coupling. The study, published in Science, shows that in heavy elements, the textbook distinction between sigma and pi bonds breaks down due to relativistic effects. This research deepens our understanding of chemical bonding in heavy elements, explaining long-known phenomena such as why mercury is liquid at room temperature and why gold appears yellow. It bridges relativity and chemistry, highlighting that Einstein's theories are essential for predicting the behavior of elements beyond the lighter ones. The study focuses on the breakdown of sigma and pi bonds in heavy elements due to spin-orbit coupling, a relativistic interaction between an electron's spin and its orbital motion. The researchers used spectroscopic techniques to observe these effects directly, confirming that relativistic corrections are necessary for accurate descriptions of bonding in elements like uranium and plutonium.

hackernews · hhs · Jul 10, 22:30 · [Discussion](https://news.ycombinator.com/item?id=48866134)

**Background**: In quantum mechanics, chemical bonds are typically described by the overlap of atomic orbitals, forming sigma and pi bonds. However, for heavy elements with high atomic numbers, the strong nuclear charge accelerates inner electrons to speeds approaching the speed of light, making relativistic effects significant. Spin-orbit coupling, a key relativistic effect, mixes spin and orbital angular momentum, altering the energy levels and bonding properties. This phenomenon is well-known in physics but its direct impact on chemical bonding had not been experimentally demonstrated until now.

<details><summary>References</summary>
<ul>
<li><a href="https://www.brown.edu/news/2026-07-09/chemical-bonds-relativity">Einstein’s relativity rules chemical bonds in heavy elements, new research shows | Brown University</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spin-orbit_coupling">Spin-orbit coupling</a></li>
<li><a href="https://whychemistry.com/explainer-hub/why-is-mercury-liquid-at-room-temperature">Why Is Mercury Liquid at Room Temperature? | Why Chemistry</a></li>

</ul>
</details>

**Discussion**: The community discussion shows strong engagement, with users noting that relativistic effects in heavy elements were already known (e.g., gold's color, mercury's liquidity), but the novelty lies in the specific mechanism affecting sigma/pi bonds. Some commenters expressed appreciation for seeing Einstein's work validated, while others shared related fun facts about the periodic table's symmetry.

**Tags**: `#physics`, `#chemistry`, `#relativity`, `#heavy elements`, `#quantum mechanics`

---

<a id="item-3"></a>
## [Building Docker Bridge Network from Scratch](https://www.reddit.com/r/programming/comments/1utfiq2/how_container_networking_works_building_a_bridge/) ⭐️ 8.0/10

A tutorial demonstrates how to build a container bridge network from scratch using Linux primitives like network namespaces, veth pairs, and bridges, explaining Docker's default networking mode. This deep-dive helps developers understand container networking internals, enabling better debugging, performance tuning, and security hardening in production environments. The tutorial covers creating network namespaces, connecting them via veth pairs, and attaching them to a Linux bridge, mirroring Docker's default bridge network behavior.

reddit · r/programming · /u/iximiuz · Jul 11, 09:33

**Background**: Docker networking relies on Linux kernel features: network namespaces provide isolation, veth pairs act as virtual cables, and Linux bridges serve as virtual switches. The default bridge network allows containers on the same host to communicate while isolating them from others.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.docker.com/engine/network/drivers/bridge/">Bridge network driver | Docker Docs</a></li>
<li><a href="https://labs.iximiuz.com/tutorials/container-networking-from-scratch">How Container Networking Works: Building a Bridge Network From Scratch | iximiuz Labs</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-02-08-how-to-understand-docker-networking-internals-veth-pairs-bridges/view">How to Understand Docker Networking Internals (veth pairs, bridges)</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion praises the tutorial for its clarity and hands-on approach, with users sharing additional tips on iptables and port forwarding. Some debate the trade-offs between bridge and overlay networks for multi-host setups.

**Tags**: `#container networking`, `#bridge network`, `#Docker`, `#Linux networking`, `#tutorial`

---

<a id="item-4"></a>
## [Official jscrambler npm Package Compromised at v8.14.0](https://www.reddit.com/r/programming/comments/1utqclm/official_jscrambler_npm_package_compromised_at/) ⭐️ 8.0/10

The official jscrambler npm package was compromised at version 8.14.0, indicating a supply chain attack where malicious code was injected into the package. This incident is significant because jscrambler is a widely-used tool for JavaScript code protection, and a compromised package could affect many downstream projects and users, potentially leading to data breaches or further malware distribution. The compromised version is 8.14.0; users are advised to avoid this version and check for any unusual behavior. The exact nature of the injected payload has not been fully disclosed yet.

reddit · r/programming · /u/BattleRemote3157 · Jul 11, 17:35

**Background**: Supply chain attacks on npm packages have become increasingly common, where attackers compromise maintainer accounts or inject malicious code into legitimate packages. Jscrambler is a commercial tool that obfuscates and protects JavaScript code, often used by enterprises to prevent reverse engineering. A compromised version could allow attackers to steal credentials, inject backdoors, or exfiltrate sensitive data from applications that use it.

<details><summary>References</summary>
<ul>
<li><a href="https://www.npmjs.com/package/jscrambler">jscrambler - npm</a></li>
<li><a href="https://www.linkedin.com/pulse/npm-malware-supply-chain-attack-what-developers-need-know-durrani-izt3f">The npm Malware Supply Chain Attack : What Developers Need to...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is likely analyzing the attack vector and sharing mitigation steps. Users are probably advising others to pin to a safe version and audit their dependencies.

**Tags**: `#supply chain attack`, `#npm`, `#security`, `#jscrambler`

---

<a id="item-5"></a>
## [Programs, Not Objects: Data-Oriented 3D Editor Design](https://www.reddit.com/r/programming/comments/1ut97oi/programs_not_objects_how_i_stopped_designing/) ⭐️ 8.0/10

The author shares their experience abandoning traditional object-oriented architecture for a data-oriented design approach when building a 3D editor, emphasizing programs and data flow over objects and encapsulation. This critique of OOP and advocacy for data-oriented design challenges widely held software engineering practices, potentially influencing how developers approach complex, performance-critical systems like 3D editors and games. The author argues that object-oriented architecture leads to poor cache utilization and unnecessary complexity, while data-oriented design focuses on data layout and transformation for better performance. The post likely includes concrete examples from the 3D editor implementation.

reddit · r/programming · /u/TheBear_at_SBB · Jul 11, 03:43

**Background**: Data-oriented design (DOD) is a programming paradigm that prioritizes efficient CPU cache usage by organizing data based on access patterns, often used in game development. It contrasts with object-oriented programming (OOP), which structures code around objects that combine data and behavior. Proponents like Mike Acton argue that DOD leads to simpler, faster code for performance-sensitive applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data-oriented design</a></li>
<li><a href="https://www.dataorienteddesign.com/dodmain/">Richard Fabian - Data-oriented design</a></li>

</ul>
</details>

**Tags**: `#software architecture`, `#data-oriented design`, `#3D editor`, `#OOP criticism`, `#programming paradigms`

---

<a id="item-6"></a>
## [ClickHouse scales PgBouncer 4x with SO_REUSEPORT and peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 7.0/10

ClickHouse engineers achieved a 4x throughput improvement for PgBouncer, a PostgreSQL connection pooler, by leveraging the SO_REUSEPORT socket option and implementing peering between PgBouncer instances. This optimization allows PgBouncer to handle significantly more connections without additional hardware, which is critical for high-traffic PostgreSQL deployments and reduces operational costs. SO_REUSEPORT enables multiple PgBouncer processes to bind to the same port, distributing incoming connections across them, while peering allows these processes to share connection state, ensuring efficient load balancing.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL that reduces the overhead of establishing new connections. Traditionally, PgBouncer runs as a single process, which can become a bottleneck under high concurrency. SO_REUSEPORT is a Linux kernel feature (since 3.9) that allows multiple sockets to listen on the same port, enabling kernel-level load balancing across processes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/how-modern-kernels-handle-massive-traffic-use-jisan-ahmed-ghg1c">How Modern Kernels Handle Massive Traffic : the use of...</a></li>
<li><a href="https://medium.com/@kartikey090803/complete-guide-to-fixing-postgresql-performance-with-pgbouncer-connection-pooling-51c7d1074d5d">Complete Guide to Fixing PostgreSQL Performance with PgBouncer ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peering">Peering - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters suggested alternative tools like Odyssey and pgdog, noting that Kubernetes users can achieve similar scaling by running multiple PgBouncer instances. Some expressed surprise that PostgreSQL's connection model hasn't improved, while others asked for more details on peering setup.

**Tags**: `#PostgreSQL`, `#PgBouncer`, `#connection pooling`, `#scalability`, `#ClickHouse`

---

<a id="item-7"></a>
## [Prefer STRICT Tables in SQLite for Type Safety](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

The article advocates using STRICT tables in SQLite, a feature introduced in version 3.37.0 (2021-11-27), to enforce strict type checking and prevent data corruption caused by dynamic type coercion. This matters because SQLite's default dynamic typing can silently coerce data, leading to subtle bugs and data corruption, especially in multi-application or long-lived databases. Adopting STRICT tables improves data integrity and aligns SQLite with the type safety expectations of other relational databases. STRICT tables must be explicitly enabled per table using the STRICT keyword in CREATE TABLE. They disallow type coercion and reject values that do not match the declared type, but also exclude some flexible features like DATE type and schema evolution via type affinity.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: SQLite traditionally uses dynamic typing, where column types are hints rather than rules, allowing any value to be stored in any column. This flexibility can cause unexpected behavior, such as a string being stored in an INTEGER column or a UUID being misinterpreted as an octal number. STRICT tables were introduced to provide an opt-in mode that enforces static typing, similar to most other SQL databases.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that STRICT should be the default, citing real-world bugs from type coercion, such as UUIDs being misinterpreted as octal numbers. Some note that STRICT tables lack certain types like DATE, but still advocate for stricter defaults to prevent data corruption.

**Tags**: `#SQLite`, `#database`, `#type safety`, `#best practices`

---

<a id="item-8"></a>
## [George Hotz Criticizes AI 2040 Report, Champions Freedom](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html) ⭐️ 7.0/10

George Hotz published a blog post critiquing the AI 2040 report's vision of controlled AI, arguing that such control threatens freedom and that AI systems are far from capable of handling real-world complexity. As a prominent AI researcher and entrepreneur, Hotz's contrarian views spark debate on AI regulation, safety, and freedom, influencing public discourse and policy considerations. Hotz argues that the AI 2040 report's approach to controlling AI is akin to thoughtcrime, and he emphasizes that real-world details can easily break AI systems, citing the example of changing a bike tire.

hackernews · rvz · Jul 11, 18:04 · [Discussion](https://news.ycombinator.com/item?id=48874200)

**Background**: The AI 2040 report, published by the AI Futures Project, calls for deliberately slowing AI development to ensure safety and control. George Hotz is known for his work on self-driving cars and his contrarian views on AI safety, often debating figures like Eliezer Yudkowsky.

<details><summary>References</summary>
<ul>
<li><a href="https://cryptobriefing.com/ai-futures-project-ai-2040-plan/">AI Futures Project publishes optimistic vision for AI 2040 , calling for...</a></li>
<li><a href="https://geohot.spicytakes.org/">George Hotz - AI , hardware, startups, and contrarian takes</a></li>

</ul>
</details>

**Discussion**: Comments on the post show mixed reactions: some agree with Hotz's freedom concerns, while others argue that freedom is not binary and that AI agents acting in the real world require regulation. The discussion highlights the tension between AI freedom and safety.

**Tags**: `#AI ethics`, `#AI safety`, `#freedom of speech`, `#geohot`, `#AI regulation`

---

<a id="item-9"></a>
## [CISA built incident playbook during real breach](https://techcrunch.com/2026/07/10/us-cyber-agency-cisa-had-to-build-its-incident-playbook-during-the-incident-agency-reveals/) ⭐️ 7.0/10

CISA revealed that it had to develop its incident response playbook during a real incident after a contractor exposed passwords on a public GitHub repository. This exposes serious preparedness gaps at the top US cybersecurity agency, undermining its credibility and highlighting systemic issues in incident response and contractor management. The exposed repository contained AWS GovCloud credentials, internal files, and passwords, and was discovered by a GitGuardian researcher who alerted journalist Brian Krebs.

rss · TechCrunch · Jul 11, 01:01

**Background**: CISA is responsible for leading the response to cybersecurity incidents for federal civilian agencies. Executive Order 14028 directed CISA to develop standard incident response playbooks, which were published in 2024. However, this incident shows that CISA itself was not following its own playbook.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cisa.gov/resources-tools/resources/federal-government-cybersecurity-incident-and-vulnerability-response-playbooks">Federal Government Cybersecurity Incident and Vulnerability Response Playbooks | CISA</a></li>
<li><a href="https://www.techrepublic.com/article/news-cisa-contractor-github-credential-leak/">CISA Contractor Exposed Sensitive Credentials in Public GitHub ...</a></li>
<li><a href="https://www.csoonline.com/article/4173305/contractors-public-github-account-exposed-govcloud-and-cisa-credentials.html">Contractor ’s public GitHub account exposed GovCloud... | CSO Online</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#CISA`, `#incident response`, `#data breach`, `#government`

---