---
layout: default
title: "Horizon Summary: 2026-11-22 (ZH)"
date: 2026-11-22
lang: zh
---

> 从 15 条内容中筛选出 6 条重要资讯。

---

1. [黎曼猜想的 Lean 形式化引发验证可靠性大讨论](#item-1) ⭐️ 9.0/10
2. [GPGME 严重漏洞：特制 OpenPGP 密钥可导致代码执行](#item-2) ⭐️ 8.0/10
3. [美军将在爱荷华州引爆大量叠氮化铅](#item-3) ⭐️ 7.0/10
4. [显示器 USB 集线器导致下载速度下降 75%](#item-4) ⭐️ 7.0/10
5. [gopgext 项目实现用 Go 语言编写 PostgreSQL 扩展](#item-5) ⭐️ 7.0/10
6. [Muru：mod_wsgi 作者打造 AI 辅助的 Rust ASGI/WSGI 服务器](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [黎曼猜想的 Lean 形式化引发验证可靠性大讨论](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 9.0/10

数学家 Levent Alpöge 宣布了黎曼猜想及其对 Dirichlet L 函数推广的形式化证明，该证明是在 Anthropic 未发布的 AI 模型协助下完成的，并以 Lean 形式化代码而非传统论文的形式发布。 这是形式化验证和数学基础领域的重大里程碑，表明 AI 辅助工具能够帮助形式化大量现代数学内容，可能加速数学研究和证明助手的采用。 该证明尚未经过专家数学审查，且形式化依赖于多个独立的 Lean 内核（con-leche 和 con-ron）及其一致性证明，这使得因 bug 导致错误证明的可能性极低但并非不可能。

hackernews · g-b-r · 11月21日 14:36 · [社区讨论](https://news.ycombinator.com/item?id=50589618)

**背景**: 黎曼猜想是关于素数分布的著名未解猜想，形式化验证则是使用 Lean 等计算机程序逐步检查数学证明。Lean 是一个交互式定理证明器，它通过一个小型可信内核确保证明的正确性，近期的工作已经产生了多个独立内核以提高可靠性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Riemann_hypothesis">Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://lean-lang.org/doc/reference/latest/ValidatingProofs/">Validating a Lean Proof</a></li>
<li><a href="https://lean4.dev/proofs/riemann-hypothesis-claim">The Riemann Hypothesis: a claimed proof, delivered in Lean</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了独立检查器的可靠性，指出曾有一个虚假的 Collatz 反证通过检查器，但一致认为人类专家的参与使得作弊可能性降低。他们还强调了所涉及的形式化数学规模巨大，并赞扬 Levent Alpöge 从 Claude 中引出证明的技巧。

**标签**: `#formal-verification`, `#lean`, `#riemann-hypothesis`, `#mathematics`, `#ai-assisted-proofs`

---

<a id="item-2"></a>
## [GPGME 严重漏洞：特制 OpenPGP 密钥可导致代码执行](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

GPGME（GnuPG 的加密操作库）中的一个双重释放漏洞（CVE-2026-129975）于 2026 年 11 月 20 日披露。该漏洞可通过包含特制超长用户 ID 的 OpenPGP 密钥触发，影响所有使用 2.3.0 之前版本 GPGME 的软件，包括 Gpg4win、GnuPG Desktop、许多邮件客户端、XMPP 客户端、Samba 和 GitLab。 这是一个高影响的安全问题，因为 GPGME 被 GitLab（用于签名提交）、电子邮件客户端和 Samba 等关键应用广泛使用，代码执行可能导致数据泄露或系统沦陷。该漏洞凸显了在安全敏感代码中使用 C/C++ 等内存不安全语言的风险。 该缺陷是一个双重释放漏洞，并非完整的 RCE 利用链，但可能潜在导致代码执行。据报道，Red Hat 五年前在 CentOS Stream 中修复了此问题，但上游 GPGME 遗漏了该修复；GitLab 发布了 Omnibus 补丁，新版本的 Gpg4win、GnuPG Desktop 和 GnuPG VS-Desktop 已解决该问题。

hackernews · gdgghhhhh · 11月21日 08:32 · [社区讨论](https://news.ycombinator.com/item?id=50587208)

**背景**: GPGME（GnuPG Made Easy）是一个 C 语言库，为应用程序提供使用 GnuPG 进行加密、解密、签名和密钥管理的高级 API。它被广泛集成到需要 OpenPGP 支持的软件中，如电子邮件客户端和版本控制系统。双重释放漏洞发生在程序两次释放同一块内存时，可被利用来使程序崩溃或执行任意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html">[Announce] GnuPG Security Advisory for GPGME (T8557,CVE-2026 ...</a></li>
<li><a href="https://www.gnupg.org/software/gpgme/index.html">GPGME - GNU Privacy Guard</a></li>
<li><a href="https://thehackernews.com/2026/11/gnupg-warns-critical-gpgme-flaw-could.html">GnuPG Warns Critical GPGME Flaw Could Expose App Data via ...</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了严重性，有人指出这是双重释放漏洞而非完整的 RCE 利用链，并质疑报告是否夸大。其他人指出 Red Hat 多年前已修复但上游遗漏，还有人主张使用类似 Rust 的工具来防止 C/C++ 中的此类内存安全问题。还有关于哪些软件受影响的困惑，澄清是 GPGME 而非 apt。

**标签**: `#security`, `#vulnerability`, `#GPGME`, `#RCE`, `#C/C++`

---

<a id="item-3"></a>
## [美军将在爱荷华州引爆大量叠氮化铅](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really) ⭐️ 7.0/10

美国陆军计划在爱荷华州米德尔敦的爱荷华陆军弹药厂引爆近 1 万磅（约 68 桶）叠氮化铅，这是一种极敏感的主炸药。这些材料已在厂区存放近 20 年，此次处置行动引发了关于有毒铅尘的警告。 此事件凸显了前政府所有、承包商运营的军事设施中数十年来被忽视的危险废物所带来的严重安全和环境风险。它还引发了对军事承包商责任以及爆炸物监管是否充分的质疑，因为这些材料会随时间推移变得更加危险。 叠氮化铅极其敏感，约 150 毫米的坠落或仅 7 毫焦耳的静电放电即可引爆，爆速约为 5180 米/秒。由于该材料无法安全移动，唯一可行的选择是在原地销毁，而引爆预计会释放铅尘，可能影响空气质量。

hackernews · beginning_end · 11月21日 13:23 · [社区讨论](https://news.ycombinator.com/item?id=50588982)

**背景**: 叠氮化铅是一种常用于雷管中引爆更大规模次级炸药的主炸药。它对冲击、摩擦和热的敏感度远高于普通炸药，因此处理和处置极其危险。爱荷华陆军弹药厂建于二战时期，后来转为承包商运营，而叠氮化铅在储存中遗留了近二十年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.accuweather.com/en/health-wellness/army-to-detonate-68-barrels-of-lead-azide-in-iowa-prompting-lead-dust-warnings/1961025">Army to detonate 68 barrels of lead azide in Iowa, prompting lead dust...</a></li>
<li><a href="https://www.wsws.org/en/articles/2026/11/20/iowa-n20.html">US Army to detonate nearly 10,000 pounds of lead azide in Iowa...</a></li>

</ul>
</details>

**社区讨论**: 评论者对军工复合体表示愤怒，将问题恶化归咎于承包商的疏忽和制度失灵。一些人指出，移动这些材料是不可能的，唯一安全的选择是由拆弹小组原地销毁；另一些人则批评了一种更普遍的模式：掩盖问题，直到其变成不可避免的灾难。

**标签**: `#chemistry`, `#explosives`, `#military-industrial`, `#safety`, `#hackernews`

---

<a id="item-4"></a>
## [显示器 USB 集线器导致下载速度下降 75%](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

一位博主发现，通过显示器的 USB 集线器连接以太网会使下载速度降低 75%，原因是增加了延迟；他通过更换不同的适配器解决了问题。 这凸显了看似无害的硬件配置如何引入隐藏的延迟和性能瓶颈，影响依赖 USB 集线器或显示器扩展坞进行网络连接的用户。 USB 集线器带来的额外延迟使笔记本电脑无法及时确认数据包，导致以太网适配器的缓冲区填满并丢包；更换一个确认频率要求较低的适配器解决了问题。

hackernews · soheilpro · 11月21日 10:36 · [社区讨论](https://news.ycombinator.com/item?id=50587875)

**背景**: USB 集线器（包括显示器内置的）可能会增加网络连接的延迟，因为 USB 是一种多路复用数据的串行总线。当以太网通过 USB 传输时，额外的开销会影响 TCP 吞吐量，尤其是在需要及时确认的高速链路上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://superuser.com/questions/1592635/does-a-usb-c-ethernet-adapter-have-a-higher-latency-than-a-regular-ethernet-port">Does a USB-C ethernet adapter have a higher latency than a ...</a></li>
<li><a href="https://vtechinsider.com/usb-vs-ethernet-latency/">Usb Vs. Ethernet Latency: Uncovering The Truth About Network ...</a></li>

</ul>
</details>

**社区讨论**: 评论者澄清，根本原因是延迟增加导致缓冲区膨胀和丢包，一些人分享了类似的经验，涉及 Thunderbolt 扩展坞和其他 USB 设备。还有人指出，显示器本身并非关键，问题实际上在于 USB 网络适配器。

**标签**: `#networking`, `#debugging`, `#USB`, `#hardware`, `#latency`

---

<a id="item-5"></a>
## [gopgext 项目实现用 Go 语言编写 PostgreSQL 扩展](https://jespino.github.io/gopgext/) ⭐️ 7.0/10

一个名为 gopgext 的新项目展示了如何用 Go 语言编写 PostgreSQL 扩展，它使用 TinyGo 和生成的 C 胶水代码来对接 PostgreSQL 的 C API。该项目在 Hacker News 上分享后获得了 115 分和 20 条评论。 这种方法降低了 Go 开发者扩展 PostgreSQL 的门槛，无需编写 C 代码，可能会增加使用 Go 工具链和安全特性构建的扩展数量。它也凸显了使用非 C 语言进行数据库扩展开发的日益增长的兴趣。 gopgext 依赖 TinyGo 将 Go 代码编译为共享库，并生成 C 胶水代码来连接 PostgreSQL 的 SPI 和钩子，但它被标记为实验性项目，可能不支持所有 PostgreSQL 版本或功能。该项目与 gokm（用 Go 编写 Linux 内核模块的工具）出自同一位作者。

hackernews · valyala · 11月21日 17:08 · [社区讨论](https://news.ycombinator.com/item?id=50591260)

**背景**: PostgreSQL 扩展通常使用 PostgreSQL C API 以 C 语言编写，这允许与数据库深度集成，但需要仔细的内存管理，并且可能在主要版本之间不兼容。Go 是一种流行的语言，以其简单性和并发性著称，但将其用于扩展需要桥接到 C，通常通过 cgo 或 TinyGo 等工具实现。其他项目如 plgo 和 pgrx（用于 Rust）也旨在简化使用高级语言进行扩展开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theprotec.com/blog/build-postgresql-extensions-in-go-with-gopgext/">Build PostgreSQL extensions in Go Without Hand-Written C Code</a></li>
<li><a href="https://github.com/microo8/plgo">GitHub - microo8/plgo: easily create postgresql extensions in ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/xfunc-c.html">PostgreSQL : Documentation: 19: 36.10. C -Language Functions</a></li>

</ul>
</details>

**社区讨论**: 评论者对该项目表示热情，有人称其“很酷”，还有人提到了 gokm 和 plgo 等相关工作。然而，一些人仍然更喜欢 Rust 的 pgrx，这表明尽管 Go 很有趣，但成熟的替代方案也有其支持者。

**标签**: `#PostgreSQL`, `#Go`, `#extensions`, `#databases`, `#tooling`

---

<a id="item-6"></a>
## [Muru：mod_wsgi 作者打造 AI 辅助的 Rust ASGI/WSGI 服务器](https://simonwillison.net/2026/Nov/21/muru/) ⭐️ 7.0/10

mod_wsgi 的创造者 Graham Dumpleton 正在开发 Muru，这是一个全新的 AI 辅助 Rust 服务器，用于在开发和生产环境中运行 ASGI 和 WSGI Python 应用。自 2026 年 11 月 4 日起，他已发布 18 篇详细文章记录该项目的设计与进展，内容涵盖 worker 架构、基于 fork 的导入、Kubernetes 集成以及缩容到零等主题。 Muru 将二十年的 Python Web 托管经验带入一个现代化的 Rust 服务器，旨在统一 WSGI 和 ASGI 应用在开发与生产环境中的服务方式。如果成功，它可能为 Python Web 部署从业者提供一个可靠的替代方案，取代 Gunicorn、uWSGI 和 Uvicorn 等现有服务器，并内置金丝雀发布和 Kubernetes 原生扩缩容等功能。 该项目处于早期阶段，且大量借助 AI 辅助，Dumpleton 强调最终判断“是否足够好”仍由人来做，并借鉴了 mod_wsgi 犯错的教训。值得注意的设计选择包括“一次导入、多次 fork”的 worker 模型、开发环境中的 HTTPS 支持、WSGI 与 ASGI 共存、无需重启的发布、无需服务网格的金丝雀发布，以及带追踪功能的每页工具栏。

rss · Simon Willison · 11月21日 23:56

**背景**: WSGI（Web 服务器网关接口）是 Python 长期使用的同步 Web 应用标准，而 ASGI（异步服务器网关接口）是其继任者，支持异步和 WebSocket 应用。mod_wsgi 是 Graham Dumpleton 在 20 年前创建的 Apache 模块，让 Apache 能够通过 WSGI 托管 Python Web 应用。Muru 是他摆脱 Apache 限制、重新思考 Python Web 托管的尝试，使用 Rust 以获得性能和安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grahamdumpleton.me/posts/2026/11/twenty-years-of-mod-wsgi/">Twenty years of mod_wsgi, and what comes next - Graham Dumpleton</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mod_wsgi">mod_wsgi - Wikipedia</a></li>
<li><a href="https://www.deployhq.com/blog/python-application-servers-wsgi-vs-asgi-guide">Python Application Servers in 2026: WSGI vs ASGI , Gunicorn to...</a></li>

</ul>
</details>

**标签**: `#python`, `#asgi`, `#wsgi`, `#rust`, `#web-servers`

---