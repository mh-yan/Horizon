---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 19 条内容中筛选出 9 条重要资讯。

---

1. [vLLM v0.25.0：Model Runner V2 成为默认，PagedAttention 被移除](#item-1) ⭐️ 9.0/10
2. [爱因斯坦相对论主导重元素化学键](#item-2) ⭐️ 8.0/10
3. [从零构建 Docker 桥接网络](#item-3) ⭐️ 8.0/10
4. [官方 jscrambler npm 包在 v8.14.0 版本被攻陷](#item-4) ⭐️ 8.0/10
5. [程序而非对象：数据导向的 3D 编辑器设计](#item-5) ⭐️ 8.0/10
6. [ClickHouse 通过 SO_REUSEPORT 和 peering 将 PgBouncer 吞吐量提升 4 倍](#item-6) ⭐️ 7.0/10
7. [在 SQLite 中优先使用 STRICT 表以确保类型安全](#item-7) ⭐️ 7.0/10
8. [乔治·霍茨批评 AI 2040 报告，倡导自由](#item-8) ⭐️ 7.0/10
9. [CISA 在真实事件中临时构建事件响应手册](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，PagedAttention 被移除](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有稠密模型的默认执行路径，移除了旧的 PagedAttention 实现，并引入了新的 Streaming Parser Engine 用于统一的工具调用和推理解析。该版本还新增了对多个模型的支持，包括 LLaVA-OneVision-2、GLM-5 以及支持流水线并行的 MiniMax-M3。 此版本标志着 vLLM 的重大架构转变，通过移除旧的 PagedAttention 并使 Model Runner V2 成为标准，简化了推理引擎。性能改进和新模型支持进一步巩固了 vLLM 作为领先的开源 LLM 推理引擎的地位，使在生产环境中部署大型语言模型的开发者和研究人员受益。 该版本包含来自 232 位贡献者的 558 次提交，其中有 64 位新贡献者。Model Runner V2 现在支持 EVS、实时嵌入、Mamba 混合模型的前缀缓存，以及带有完整 CUDA 图的动态推测解码。Transformers 建模后端现在与原生 vLLM 速度相当，并获得了 FP8 MoE 支持。

github · khluu · 7月11日 20:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，使用 PagedAttention 实现 KV 缓存的高效内存管理。Model Runner V2 是一个较新的执行后端，可提高性能和灵活性。移除旧的 PagedAttention 表明 vLLM 已完全过渡到其 V1 和 MRv2 后端。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention - Wikipedia</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#open source`, `#release`, `#AI infrastructure`

---

<a id="item-2"></a>
## [爱因斯坦相对论主导重元素化学键](https://www.brown.edu/news/2026-07-09/chemical-bonds-relativity) ⭐️ 8.0/10

布朗大学的化学家首次提供直接实验证据，证明爱因斯坦的相对论通过自旋-轨道耦合从根本上改变了重元素中三键的结构。这项发表在《科学》杂志上的研究表明，在重元素中，由于相对论效应，教科书上关于 sigma 键和 pi 键的区分被打破。 这项研究加深了我们对重元素化学键的理解，解释了长期已知的现象，例如为什么汞在室温下是液态以及为什么金子呈黄色。它连接了相对论和化学，强调爱因斯坦的理论对于预测较重元素的行为至关重要。 该研究聚焦于重元素中 sigma 键和 pi 键因自旋-轨道耦合（电子自旋与其轨道运动之间的相对论性相互作用）而失效的现象。研究人员使用光谱技术直接观察这些效应，证实了在描述铀和钚等元素的化学键时，相对论修正必不可少。

hackernews · hhs · 7月10日 22:30 · [社区讨论](https://news.ycombinator.com/item?id=48866134)

**背景**: 在量子力学中，化学键通常由原子轨道的重叠来描述，形成 sigma 键和 pi 键。然而，对于原子序数高的重元素，强大的核电荷使内层电子加速到接近光速，使得相对论效应变得显著。自旋-轨道耦合是一种关键的相对论效应，它混合了自旋和轨道角动量，改变了能级和成键性质。这种现象在物理学中众所周知，但其对化学键的直接影响直到现在才被实验证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.brown.edu/news/2026-07-09/chemical-bonds-relativity">Einstein’s relativity rules chemical bonds in heavy elements, new research shows | Brown University</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spin-orbit_coupling">Spin-orbit coupling</a></li>
<li><a href="https://whychemistry.com/explainer-hub/why-is-mercury-liquid-at-room-temperature">Why Is Mercury Liquid at Room Temperature? | Why Chemistry</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出强烈的参与度，用户指出重元素中的相对论效应早已为人所知（例如金子的颜色、汞的液态），但新颖之处在于影响 sigma/pi 键的具体机制。一些评论者对爱因斯坦的工作得到验证表示赞赏，而其他人则分享了关于元素周期表对称性的相关趣闻。

**标签**: `#physics`, `#chemistry`, `#relativity`, `#heavy elements`, `#quantum mechanics`

---

<a id="item-3"></a>
## [从零构建 Docker 桥接网络](https://www.reddit.com/r/programming/comments/1utfiq2/how_container_networking_works_building_a_bridge/) ⭐️ 8.0/10

一篇教程展示了如何使用 Linux 网络命名空间、veth 对和网桥等原语从零构建容器桥接网络，从而解释 Docker 的默认网络模式。 这一深入讲解帮助开发者理解容器网络内部机制，从而在生产环境中更好地进行调试、性能调优和安全加固。 该教程涵盖了创建网络命名空间、通过 veth 对连接它们以及将它们附加到 Linux 网桥的过程，模拟了 Docker 默认桥接网络的行为。

reddit · r/programming · /u/iximiuz · 7月11日 09:33

**背景**: Docker 网络依赖 Linux 内核特性：网络命名空间提供隔离，veth 对充当虚拟网线，Linux 网桥作为虚拟交换机。默认桥接网络允许同一主机上的容器通信，同时与其他容器隔离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.docker.com/engine/network/drivers/bridge/">Bridge network driver | Docker Docs</a></li>
<li><a href="https://labs.iximiuz.com/tutorials/container-networking-from-scratch">How Container Networking Works: Building a Bridge Network From Scratch | iximiuz Labs</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-02-08-how-to-understand-docker-networking-internals-veth-pairs-bridges/view">How to Understand Docker Networking Internals (veth pairs, bridges)</a></li>

</ul>
</details>

**社区讨论**: Reddit 讨论称赞该教程清晰且实践性强，用户分享了关于 iptables 和端口转发的额外技巧。部分用户讨论了多主机场景下桥接网络与覆盖网络的权衡。

**标签**: `#container networking`, `#bridge network`, `#Docker`, `#Linux networking`, `#tutorial`

---

<a id="item-4"></a>
## [官方 jscrambler npm 包在 v8.14.0 版本被攻陷](https://www.reddit.com/r/programming/comments/1utqclm/official_jscrambler_npm_package_compromised_at/) ⭐️ 8.0/10

官方 jscrambler npm 包在 8.14.0 版本被攻陷，表明发生了供应链攻击，恶意代码被注入到该包中。 此事件意义重大，因为 jscrambler 是广泛使用的 JavaScript 代码保护工具，被攻陷的包可能影响众多下游项目和用户，可能导致数据泄露或进一步恶意软件传播。 被攻陷的版本是 8.14.0；建议用户避免使用此版本并检查是否有异常行为。注入的恶意载荷的具体性质尚未完全披露。

reddit · r/programming · /u/BattleRemote3157 · 7月11日 17:35

**背景**: 针对 npm 包的供应链攻击日益常见，攻击者通过攻陷维护者账户或向合法包中注入恶意代码来实施攻击。Jscrambler 是一款商业工具，用于混淆和保护 JavaScript 代码，常被企业用于防止逆向工程。被攻陷的版本可能允许攻击者窃取凭据、注入后门或从使用该包的应用程序中窃取敏感数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npmjs.com/package/jscrambler">jscrambler - npm</a></li>
<li><a href="https://www.linkedin.com/pulse/npm-malware-supply-chain-attack-what-developers-need-know-durrani-izt3f">The npm Malware Supply Chain Attack : What Developers Need to...</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论可能正在分析攻击向量并分享缓解措施。用户可能建议其他人锁定安全版本并审计其依赖项。

**标签**: `#supply chain attack`, `#npm`, `#security`, `#jscrambler`

---

<a id="item-5"></a>
## [程序而非对象：数据导向的 3D 编辑器设计](https://www.reddit.com/r/programming/comments/1ut97oi/programs_not_objects_how_i_stopped_designing/) ⭐️ 8.0/10

作者分享了在构建 3D 编辑器时放弃传统面向对象架构，转而采用数据导向设计方法的经验，强调程序和数据流而非对象和封装。 这种对 OOP 的批评和对数据导向设计的倡导挑战了广泛接受的软件工程实践，可能影响开发者如何构建复杂、性能关键的系统，如 3D 编辑器和游戏。 作者认为面向对象架构导致缓存利用率低和不必要的复杂性，而数据导向设计关注数据布局和转换以获得更好的性能。该帖子可能包含来自 3D 编辑器实现的具体示例。

reddit · r/programming · /u/TheBear_at_SBB · 7月11日 03:43

**背景**: 数据导向设计（DOD）是一种编程范式，通过根据访问模式组织数据来优先考虑 CPU 缓存的高效使用，常用于游戏开发。它与面向对象编程（OOP）形成对比，后者围绕将数据和行为结合的对象来组织代码。Mike Acton 等支持者认为，DOD 能为性能敏感的应用带来更简单、更快的代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data-oriented design</a></li>
<li><a href="https://www.dataorienteddesign.com/dodmain/">Richard Fabian - Data-oriented design</a></li>

</ul>
</details>

**标签**: `#software architecture`, `#data-oriented design`, `#3D editor`, `#OOP criticism`, `#programming paradigms`

---

<a id="item-6"></a>
## [ClickHouse 通过 SO_REUSEPORT 和 peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 7.0/10

ClickHouse 工程师通过利用 SO_REUSEPORT 套接字选项并在 PgBouncer 实例之间实现 peering，将 PostgreSQL 连接池 PgBouncer 的吞吐量提升了 4 倍。 这一优化使得 PgBouncer 无需额外硬件即可处理更多连接，对于高流量 PostgreSQL 部署至关重要，并能降低运营成本。 SO_REUSEPORT 允许多个 PgBouncer 进程绑定到同一端口，将传入连接分布到各进程；而 peering 则让这些进程共享连接状态，确保高效的负载均衡。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是 PostgreSQL 的轻量级连接池，用于减少建立新连接的开销。传统上，PgBouncer 作为单进程运行，在高并发下可能成为瓶颈。SO_REUSEPORT 是 Linux 内核自 3.9 版本引入的特性，允许多个套接字监听同一端口，实现内核级别的跨进程负载均衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/how-modern-kernels-handle-massive-traffic-use-jisan-ahmed-ghg1c">How Modern Kernels Handle Massive Traffic : the use of...</a></li>
<li><a href="https://medium.com/@kartikey090803/complete-guide-to-fixing-postgresql-performance-with-pgbouncer-connection-pooling-51c7d1074d5d">Complete Guide to Fixing PostgreSQL Performance with PgBouncer ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peering">Peering - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者推荐了 Odyssey 和 pgdog 等替代工具，并指出 Kubernetes 用户可以通过运行多个 PgBouncer 实例实现类似扩展。有人对 PostgreSQL 连接模型未改进表示惊讶，也有人询问 peering 设置的更多细节。

**标签**: `#PostgreSQL`, `#PgBouncer`, `#connection pooling`, `#scalability`, `#ClickHouse`

---

<a id="item-7"></a>
## [在 SQLite 中优先使用 STRICT 表以确保类型安全](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

文章提倡在 SQLite 中使用 STRICT 表，该功能自 3.37.0 版本（2021-11-27）引入，用于强制执行严格类型检查，防止因动态类型转换导致的数据损坏。 这很重要，因为 SQLite 默认的动态类型会静默转换数据，导致难以发现的错误和数据损坏，尤其是在多应用或长期使用的数据库中。采用 STRICT 表可提高数据完整性，使 SQLite 符合其他关系数据库的类型安全预期。 STRICT 表需要在 CREATE TABLE 中显式使用 STRICT 关键字启用。它禁止类型转换，拒绝与声明类型不匹配的值，但也会排除一些灵活特性，如 DATE 类型和通过类型亲和性的模式演变。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 传统上使用动态类型，列类型只是提示而非规则，允许任何值存储在任何列中。这种灵活性可能导致意外行为，例如字符串被存入 INTEGER 列，或 UUID 被误解析为八进制数。STRICT 表作为一种可选模式被引入，强制执行静态类型，类似于大多数其他 SQL 数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 STRICT 应成为默认设置，并引用了类型转换导致的真实错误，例如 UUID 被误解析为八进制数。有人指出 STRICT 表缺少 DATE 等类型，但仍主张更严格的默认设置以防止数据损坏。

**标签**: `#SQLite`, `#database`, `#type safety`, `#best practices`

---

<a id="item-8"></a>
## [乔治·霍茨批评 AI 2040 报告，倡导自由](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html) ⭐️ 7.0/10

乔治·霍茨发表博客文章，批评 AI 2040 报告中关于受控 AI 的愿景，认为这种控制威胁自由，并且 AI 系统远未具备处理现实世界复杂性的能力。 作为知名 AI 研究员和企业家，霍茨的反主流观点引发了关于 AI 监管、安全和自由的辩论，影响公众讨论和政策考量。 霍茨认为 AI 2040 报告控制 AI 的方法类似于思想犯罪，并强调现实世界的细节很容易让 AI 系统失效，他以换自行车轮胎为例。

hackernews · rvz · 7月11日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=48874200)

**背景**: AI 2040 报告由 AI Futures Project 发布，呼吁有意放缓 AI 开发以确保安全和控制。乔治·霍茨以自动驾驶汽车工作和在 AI 安全方面的反主流观点而闻名，经常与 Eliezer Yudkowsky 等人辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cryptobriefing.com/ai-futures-project-ai-2040-plan/">AI Futures Project publishes optimistic vision for AI 2040 , calling for...</a></li>
<li><a href="https://geohot.spicytakes.org/">George Hotz - AI , hardware, startups, and contrarian takes</a></li>

</ul>
</details>

**社区讨论**: 帖子评论反应不一：一些人同意霍茨对自由的担忧，而另一些人则认为自由不是二元的，且在现实世界中行动的 AI 代理需要监管。讨论凸显了 AI 自由与安全之间的张力。

**标签**: `#AI ethics`, `#AI safety`, `#freedom of speech`, `#geohot`, `#AI regulation`

---

<a id="item-9"></a>
## [CISA 在真实事件中临时构建事件响应手册](https://techcrunch.com/2026/07/10/us-cyber-agency-cisa-had-to-build-its-incident-playbook-during-the-incident-agency-reveals/) ⭐️ 7.0/10

CISA 透露，在一名承包商将密码暴露在公开的 GitHub 仓库后，该机构不得不在真实事件中临时制定事件响应手册。 这暴露了美国最高网络安全机构在准备方面的严重缺陷，削弱了其公信力，并凸显了事件响应和承包商管理中的系统性问题。 暴露的仓库包含 AWS GovCloud 凭证、内部文件和密码，由 GitGuardian 的研究人员发现并告知记者 Brian Krebs。

rss · TechCrunch · 7月11日 01:01

**背景**: CISA 负责领导联邦民事机构的网络安全事件响应。第 14028 号行政令要求 CISA 制定标准的事件响应手册，并于 2024 年发布。然而，此次事件表明 CISA 自身并未遵循其手册。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/resources-tools/resources/federal-government-cybersecurity-incident-and-vulnerability-response-playbooks">Federal Government Cybersecurity Incident and Vulnerability Response Playbooks | CISA</a></li>
<li><a href="https://www.techrepublic.com/article/news-cisa-contractor-github-credential-leak/">CISA Contractor Exposed Sensitive Credentials in Public GitHub ...</a></li>
<li><a href="https://www.csoonline.com/article/4173305/contractors-public-github-account-exposed-govcloud-and-cisa-credentials.html">Contractor ’s public GitHub account exposed GovCloud... | CSO Online</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#CISA`, `#incident response`, `#data breach`, `#government`

---