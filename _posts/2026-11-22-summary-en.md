---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 15 items, 6 important content pieces were selected

---

1. [Lean Formalization of Riemann Hypothesis Sparks Debate on Verification](#item-1) ⭐️ 9.0/10
2. [Critical GPGME Vulnerability Allows Code Execution via Crafted OpenPGP Keys](#item-2) ⭐️ 8.0/10
3. [Army to Detonate Massive Pile of Lead Azide in Iowa](#item-3) ⭐️ 7.0/10
4. [Monitor's USB Hub Causes 75% Download Speed Drop](#item-4) ⭐️ 7.0/10
5. [gopgext Enables PostgreSQL Extensions in Go](#item-5) ⭐️ 7.0/10
6. [Muru: mod_wsgi Creator Builds AI-Assisted Rust ASGI/WSGI Server](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Lean Formalization of Riemann Hypothesis Sparks Debate on Verification](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 9.0/10

Mathematician Levent Alpöge announced a formal proof of the Riemann Hypothesis and its generalization to Dirichlet L-functions, developed with the assistance of an unreleased Anthropic AI model, and released it as a Lean formalization rather than a conventional paper. This is a major milestone for formal verification and mathematical foundations, as it demonstrates that AI-assisted tools can help formalize large chunks of modern mathematics, potentially accelerating both mathematical research and the adoption of proof assistants. The proof has not yet undergone expert mathematical review, and the formalization relies on multiple independent Lean kernels (con-leche and con-ron) with consistency proofs, making a bug-induced false proof extremely unlikely but not impossible.

hackernews · g-b-r · Nov 21, 14:36 · [Discussion](https://news.ycombinator.com/item?id=50589618)

**Background**: The Riemann Hypothesis is a famous unsolved conjecture about the distribution of prime numbers, and formal verification involves using computer programs like Lean to check mathematical proofs step by step. Lean is an interactive theorem prover that ensures proofs are correct according to a small trusted kernel, and recent efforts have produced multiple independent kernels to increase reliability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Riemann_hypothesis">Riemann hypothesis - Wikipedia</a></li>
<li><a href="https://lean-lang.org/doc/reference/latest/ValidatingProofs/">Validating a Lean Proof</a></li>
<li><a href="https://lean4.dev/proofs/riemann-hypothesis-claim">The Riemann Hypothesis: a claimed proof, delivered in Lean</a></li>

</ul>
</details>

**Discussion**: Commenters debated the reliability of independent checkers, noting that a fake Collatz refutation once passed a checker, but agreed that the human expert in the loop makes foul play unlikely. They also highlighted the massive scale of formalized mathematics involved and credited Levent Alpöge for his skill in eliciting the proof from Claude.

**Tags**: `#formal-verification`, `#lean`, `#riemann-hypothesis`, `#mathematics`, `#ai-assisted-proofs`

---

<a id="item-2"></a>
## [Critical GPGME Vulnerability Allows Code Execution via Crafted OpenPGP Keys](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

A double-free vulnerability (CVE-2026-129975) in GPGME, GnuPG's library for cryptographic operations, was disclosed on 2026-11-20. Triggered by an OpenPGP key with a crafted very long user ID, it affects all software using GPGME versions prior to 2.3.0, including Gpg4win, GnuPG Desktop, many mail clients, XMPP clients, Samba, and GitLab. This is a high-impact security issue because GPGME is widely used by critical applications like GitLab (for signed commits), email clients, and Samba, where code execution could lead to data breaches or system compromise. The vulnerability highlights the risks of memory-unsafe languages like C/C++ in security-sensitive code. The flaw is a double-free bug, not a full RCE chain, though it can potentially lead to code execution. Red Hat reportedly fixed it five years ago in CentOS Stream, but upstream GPGME missed the fix; GitLab released an Omnibus patch, and new versions of Gpg4win, GnuPG Desktop, and GnuPG VS-Desktop address the issue.

hackernews · gdgghhhhh · Nov 21, 08:32 · [Discussion](https://news.ycombinator.com/item?id=50587208)

**Background**: GPGME (GnuPG Made Easy) is a C library that provides a high-level API for applications to use GnuPG for encryption, decryption, signing, and key management. It is widely integrated into software that needs OpenPGP support, such as email clients and version control systems. A double-free vulnerability occurs when a program frees the same memory twice, which can be exploited to crash the program or execute arbitrary code.

<details><summary>References</summary>
<ul>
<li><a href="https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html">[Announce] GnuPG Security Advisory for GPGME (T8557,CVE-2026 ...</a></li>
<li><a href="https://www.gnupg.org/software/gpgme/index.html">GPGME - GNU Privacy Guard</a></li>
<li><a href="https://thehackernews.com/2026/11/gnupg-warns-critical-gpgme-flaw-could.html">GnuPG Warns Critical GPGME Flaw Could Expose App Data via ...</a></li>

</ul>
</details>

**Discussion**: Commenters debated the severity, with one noting it's a double-free bug rather than a full RCE chain, and questioned if reports are overstated. Others pointed out Red Hat fixed it years ago but upstream missed it, and some argued for using Rust-like tooling to prevent such memory safety issues in C/C++. There was also confusion about which software is affected, with clarification that it's GPGME and not apt.

**Tags**: `#security`, `#vulnerability`, `#GPGME`, `#RCE`, `#C/C++`

---

<a id="item-3"></a>
## [Army to Detonate Massive Pile of Lead Azide in Iowa](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really) ⭐️ 7.0/10

The U.S. Army is preparing to detonate nearly 10,000 pounds (about 68 barrels) of lead azide, a highly sensitive primary explosive, at the Iowa Army Ammunition Plant in Middletown, Iowa. The material had been sitting at the facility for almost 20 years, and the disposal operation has prompted warnings about toxic lead dust. The case highlights serious safety and environmental risks from decades of neglected hazardous waste at a former government-owned, contractor-operated military facility. It also raises questions about accountability for military contractors and the adequacy of oversight for explosive materials that become more dangerous over time. Lead azide is extremely sensitive, detonating after a fall of about 150 mm or a static discharge of just 7 millijoules, with a detonation velocity around 5,180 m/s. Because the material cannot be safely moved, the only viable option is to destroy it in place, and the detonations are expected to release lead dust that may affect air quality.

hackernews · beginning_end · Nov 21, 13:23 · [Discussion](https://news.ycombinator.com/item?id=50588982)

**Background**: Lead azide is a primary explosive commonly used in detonators to trigger larger secondary explosives. It is far more sensitive to shock, friction, and heat than typical explosives, making handling and disposal extremely hazardous. The Iowa Army Ammunition Plant was built for World War II and later transitioned to contractor operation, and the lead azide was left in storage for nearly two decades.

<details><summary>References</summary>
<ul>
<li><a href="https://www.accuweather.com/en/health-wellness/army-to-detonate-68-barrels-of-lead-azide-in-iowa-prompting-lead-dust-warnings/1961025">Army to detonate 68 barrels of lead azide in Iowa, prompting lead dust...</a></li>
<li><a href="https://www.wsws.org/en/articles/2026/11/20/iowa-n20.html">US Army to detonate nearly 10,000 pounds of lead azide in Iowa...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the military-industrial complex, blaming contractor negligence and institutional dysfunction for allowing the situation to deteriorate. Some noted that moving the material is impossible and that the only safe option is in-place destruction by bomb squads, while others criticized a broader pattern of hiding problems until they become unavoidable disasters.

**Tags**: `#chemistry`, `#explosives`, `#military-industrial`, `#safety`, `#hackernews`

---

<a id="item-4"></a>
## [Monitor's USB Hub Causes 75% Download Speed Drop](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

A blogger discovered that routing Ethernet through a monitor's USB hub reduced download speeds by 75% due to added latency, and fixed the issue by switching to a different adapter. This highlights how seemingly innocuous hardware configurations can introduce hidden latency and performance bottlenecks, affecting users who rely on USB hubs or monitor docks for networking. The extra latency from the USB hub prevented the laptop from acknowledging packets quickly enough, causing the Ethernet adapter's buffer to fill and drop packets; a different adapter with less frequent acknowledgment requirements resolved the issue.

hackernews · soheilpro · Nov 21, 10:36 · [Discussion](https://news.ycombinator.com/item?id=50587875)

**Background**: USB hubs, including those built into monitors, can add latency to network connections because USB is a serial bus that multiplexes data. When Ethernet is tunneled over USB, the additional overhead can affect TCP throughput, especially on high-speed links where timely acknowledgments are critical.

<details><summary>References</summary>
<ul>
<li><a href="https://superuser.com/questions/1592635/does-a-usb-c-ethernet-adapter-have-a-higher-latency-than-a-regular-ethernet-port">Does a USB-C ethernet adapter have a higher latency than a ...</a></li>
<li><a href="https://vtechinsider.com/usb-vs-ethernet-latency/">Usb Vs. Ethernet Latency: Uncovering The Truth About Network ...</a></li>

</ul>
</details>

**Discussion**: Commenters clarified that the root cause was increased latency causing bufferbloat and packet drops, and some shared similar experiences with Thunderbolt docks and other USB devices. Others noted that the monitor aspect is incidental and the issue is really about the USB network adapter.

**Tags**: `#networking`, `#debugging`, `#USB`, `#hardware`, `#latency`

---

<a id="item-5"></a>
## [gopgext Enables PostgreSQL Extensions in Go](https://jespino.github.io/gopgext/) ⭐️ 7.0/10

A new project called gopgext demonstrates how to write PostgreSQL extensions in Go, using TinyGo and generated C glue code to interface with PostgreSQL's C API. The project was shared on Hacker News, where it received 115 points and 20 comments. This approach lowers the barrier for Go developers to extend PostgreSQL without writing C code, potentially increasing the number of extensions built with Go's tooling and safety features. It also highlights growing interest in using non-C languages for database extension development. gopgext relies on TinyGo to compile Go code into a shared library and generates C glue code to connect with PostgreSQL's SPI and hooks, but it is marked as experimental and may not support all PostgreSQL versions or features. The project is created by the same author as gokm, a tool for writing Linux kernel modules in Go.

hackernews · valyala · Nov 21, 17:08 · [Discussion](https://news.ycombinator.com/item?id=50591260)

**Background**: PostgreSQL extensions are typically written in C using the PostgreSQL C API, which allows deep integration with the database but requires careful memory management and can break between major versions. Go is a popular language known for its simplicity and concurrency, but using it for extensions requires bridging to C, often via cgo or tools like TinyGo. Other projects like plgo and pgrx (for Rust) also aim to simplify extension development in higher-level languages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theprotec.com/blog/build-postgresql-extensions-in-go-with-gopgext/">Build PostgreSQL extensions in Go Without Hand-Written C Code</a></li>
<li><a href="https://github.com/microo8/plgo">GitHub - microo8/plgo: easily create postgresql extensions in ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/xfunc-c.html">PostgreSQL : Documentation: 19: 36.10. C -Language Functions</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm for the project, with one noting it's 'cool' and another pointing to related work like gokm and plgo. However, some still prefer pgrx for Rust, indicating that while Go is interesting, established alternatives have their advocates.

**Tags**: `#PostgreSQL`, `#Go`, `#extensions`, `#databases`, `#tooling`

---

<a id="item-6"></a>
## [Muru: mod_wsgi Creator Builds AI-Assisted Rust ASGI/WSGI Server](https://simonwillison.net/2026/Nov/21/muru/) ⭐️ 7.0/10

Graham Dumpleton, creator of mod_wsgi, is developing Muru, a new AI-assisted Rust server for running ASGI and WSGI Python applications in both development and production. Since November 4, 2026, he has published 18 detailed posts documenting the project's design and progress, covering topics from worker architecture and fork-based imports to Kubernetes integration and scaling to zero. Muru brings two decades of Python web hosting experience to a modern Rust-based server that aims to unify development and production serving for both WSGI and ASGI apps. If successful, it could offer Python web deployment practitioners a credible alternative to existing servers like Gunicorn, uWSGI, and Uvicorn, with built-in features such as canary releases and Kubernetes-native scaling. The project is early-stage and heavily AI-assisted, with Dumpleton emphasizing that human judgment still decides what is good enough, drawing on lessons from mod_wsgi's mistakes. Notable design choices include "import once, fork many" worker models, HTTPS support in development, running WSGI and ASGI together, releases without restarts, canaries without a service mesh, and a per-page toolbar with tracing.

rss · Simon Willison · Nov 21, 23:56

**Background**: WSGI (Web Server Gateway Interface) is the long-standing Python standard for synchronous web applications, while ASGI (Asynchronous Server Gateway Interface) is its successor for async and WebSocket-capable apps. mod_wsgi is an Apache module created by Graham Dumpleton 20 years ago that lets Apache host Python web applications via WSGI. Muru is his attempt to rethink Python web hosting without Apache's constraints, using Rust for performance and safety.

<details><summary>References</summary>
<ul>
<li><a href="https://grahamdumpleton.me/posts/2026/11/twenty-years-of-mod-wsgi/">Twenty years of mod_wsgi, and what comes next - Graham Dumpleton</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mod_wsgi">mod_wsgi - Wikipedia</a></li>
<li><a href="https://www.deployhq.com/blog/python-application-servers-wsgi-vs-asgi-guide">Python Application Servers in 2026: WSGI vs ASGI , Gunicorn to...</a></li>

</ul>
</details>

**Tags**: `#python`, `#asgi`, `#wsgi`, `#rust`, `#web-servers`

---