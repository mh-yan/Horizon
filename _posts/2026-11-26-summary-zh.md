---
layout: default
title: "Horizon Summary: 2026-11-26 (ZH)"
date: 2026-11-26
lang: zh
---

> 从 36 条内容中筛选出 15 条重要资讯。

---

1. [斯科特·阿伦森对 AI 数学突破发出警告](#item-1) ⭐️ 9.0/10
2. [1Password 披露安全事件：员工笔记本电脑被入侵导致恶意代码推送](#item-2) ⭐️ 8.0/10
3. [GRH 的 Lean 验证从 1700 万行缩减至 7.6 万行](#item-3) ⭐️ 8.0/10
4. [新预印本否定了多项式 Hirsch 猜想](#item-4) ⭐️ 8.0/10
5. [Google Research 发布关于整数分解和离散对数的 Cogentic 论文](#item-5) ⭐️ 8.0/10
6. [文章主张有责任心的工程师应拥抱 LLM 工具，引发辩论](#item-6) ⭐️ 8.0/10
7. [FCC 批准 SpaceX 在太空部署 AI 数据中心计划](#item-7) ⭐️ 8.0/10
8. [安全研究员批评 Ubuntu 补丁响应缓慢](#item-8) ⭐️ 7.0/10
9. [《纽约时报》警告摄影师不要因 AI 功能更新 Photoshop](#item-9) ⭐️ 7.0/10
10. [博客称 Jev 很可能是 Qwen3.5-35B-A3B，依据延迟分析](#item-10) ⭐️ 7.0/10
11. [开发者逆向工程 Windows 响度均衡并移植到 PipeWire](#item-11) ⭐️ 7.0/10
12. [作者用 Lean 审计 Clojure 核心库，发现未报告的错误](#item-12) ⭐️ 7.0/10
13. [科学家界定 AI 代理在研究中的使用边界](#item-13) ⭐️ 7.0/10
14. [纽约州对 AI 聊天机器人玩具实施五年禁令](#item-14) ⭐️ 7.0/10
15. [州总检察长挑战 Character.AI 破产拍卖用户聊天记录的计划](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [斯科特·阿伦森对 AI 数学突破发出警告](https://scottaaronson.blog/?p=10379) ⭐️ 9.0/10

斯科特·阿伦森发表博客文章，对一项重大 AI 驱动的数学突破作出反应，并链接到 OpenAI 的一篇预印本论文，该论文声称矩阵乘法指数恰好为 9/4。这篇文章在 Hacker News 上引发了大规模讨论，获得超过 1000 分和 847 条评论。 矩阵乘法指数恰好为 9/4 这一主张，将是自 1979 年以来这一基础复杂度界上的最大变动，对算法设计具有广泛影响。更广泛地说，AI 系统解决长期未解的数学难题，标志着数学研究方式可能发生范式转变。 OpenAI 的预印本声称找到了与矩阵乘法指数ω已知上界相匹配的下界，这意味着没有算法能实现更小的指数。然而，社区成员质疑如何验证 AI 生成的 Lean 证明确实证明了预期命题，而不是其他可编译的代码。

hackernews · Kotlopou · 11月25日 19:11 · [社区讨论](https://news.ycombinator.com/item?id=50646108)

**背景**: 矩阵乘法指数ω描述两个 n×n 矩阵相乘的渐近复杂度；朴素算法给出ω=3，而自 1986 年以来已知的最佳上界约为 2.37。斯科特·阿伦森是德克萨斯大学奥斯汀分校的理论计算机科学家，以其博客 Shtetl-Optimized 闻名，他在博客中记录了 OpenAI 近期大量 AI 生成的数学成果。2026 年，OpenAI 发布了众多由 AI 发现的开放问题证明，引发了关于信任、验证以及数学研究未来的争论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xenospectrum.com/en/matrix-multiplication-nine-fourths-lower-bound/">OpenAI Preprint Claims the Matrix Multiplication Exponent Is ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_bulk_release_of_mathematical_papers">OpenAI bulk release of mathematical papers - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_mathematical_discoveries_made_with_artificial_intelligence">List of mathematical discoveries made with artificial ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对 AI 进展的速度表示敬畏，一些人认为人类在生物学上无法理解这种变化的规模。另一些人则反驳说，在公理化数学上的成功并不意味着 AI 能解决所有领域或构成生存风险，并对 Lean 证明的验证提出了担忧。

**标签**: `#AI`, `#mathematics`, `#research breakthrough`, `#philosophy of science`, `#community discussion`

---

<a id="item-2"></a>
## [1Password 披露安全事件：员工笔记本电脑被入侵导致恶意代码推送](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password 披露了一起安全事件，攻击者获取了一名员工的公司 GitHub 账户访问权限，并利用该账户将恶意代码推送到后端服务，这些服务下载了与客户相关的管理数据。公司确认客户密码库未被访问，仍然安全。 这一事件凸显了关键的 SaaS 供应链风险：一台被入侵的员工笔记本电脑可能导致代码被推送到生产环境，从而可能泄露敏感客户数据。鉴于 1Password 作为广泛使用的密码管理器的角色，该事件强调了在整个 SaaS 提供商中实施强健的分支保护和终端安全的必要性。 攻击者利用被入侵的 GitHub 账户访问源代码，并将恶意代码推送到后端服务，这些服务随后下载了关于客户的管理数据。1Password 尚未详细说明是否缺少分支保护规则或这些规则被绕过，这是评论者提出的一个问题。

hackernews · lxhrstn · 11月25日 17:18 · [社区讨论](https://news.ycombinator.com/item?id=50644817)

**背景**: 1Password 是一款流行的密码管理器，将用户凭据存储在加密的密码库中。在典型的 SaaS 供应链攻击中，攻击者入侵员工设备以获取代码仓库的访问权限，并将恶意代码注入生产系统。此次事件遵循了在其他入侵事件中看到的模式，例如 2026 年通过被入侵员工设备导致的 GitHub 入侵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://1password.com/blog/update-on-nov-2026-security-incident">Update on a security incident involving 1Password’s backend ...</a></li>
<li><a href="https://www.1password.community/announcements-52/update-on-a-security-incident-involving-1password-s-backend-systems-customer-vaults-were-not-affected-and-all-vault-contents-remain-secure-26259">Update on a security incident involving 1Password’s backend ...</a></li>
<li><a href="https://www.pcmag.com/news/hackers-infiltrate-github-by-compromising-employee-device">Hackers Infiltrate GitHub by Compromising Employee Device</a></li>

</ul>
</details>

**社区讨论**: 评论者强调，被入侵的员工笔记本电脑是 SaaS 公司最重要的攻击向量，随着员工数量增长，可能性接近 1。一些人对将恶意代码推送到后端服务表示担忧，认为这表明缺少分支保护；另一些人则担心在线密码库与仅本地密码库的安全性对比。还有人指出，通行密钥实现通常缺少第二因素，可能削弱安全性。

**标签**: `#security`, `#SaaS`, `#supply-chain`, `#1Password`, `#incident-response`

---

<a id="item-3"></a>
## [GRH 的 Lean 验证从 1700 万行缩减至 7.6 万行](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

lsernau 在 GitHub 上发布了一个新仓库，提供了广义黎曼假设（GRH）的 Lean 验证，其代码量从约 1700 万行大幅缩减至约 7.6 万行，减少了 99.56%。该项目包含清晰的文档，并明确区分了已知数学与新数学。 这一大幅缩减使得形式化证明更易于数学家审阅和理解，可能回应了关于庞大形式化证明缺乏洞察力的担忧。同时，它也凸显了 AI 辅助的证明高尔夫在使形式验证更实用方面日益重要的作用。 这一缩减是通过证明高尔夫实现的，可能借助了 LLM 辅助，且仓库中遍布人类可读的文档。一个相关工具 slim 可用于浏览 Lean 源代码，而无需设置 Lean 或构建项目。

hackernews · nb-t · 11月25日 21:48 · [社区讨论](https://news.ycombinator.com/item?id=50648050)

**背景**: 广义黎曼假设（GRH）是数论中一个重要的未解决猜想，它将黎曼假设推广到狄利克雷 L 函数和其他全局 L 函数。Lean 是一个证明助手和函数式编程语言，用于形式化验证数学证明。2026 年 11 月，数学家 Levent Alpöge 提出了一个 AI 辅助的 GRH 证明，并得到了 Lean 和 Mathlib 社区的验证。原始形式化代码量巨大（约 1700 万行），而本项目是其大幅精简后的版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Generalized_Riemann_hypothesis">Generalized Riemann hypothesis</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了其可读性以及已知数学与新数学的区分，认为这将大大有助于理解。一些人提出疑问：这是否回应了陶哲轩关于庞大但缺乏洞察力的证明是个问题的观点，以及更智能的 LLM 现在能否对证明进行高尔夫并解释它们。还有人分享了 Zulip 讨论和用于浏览 Lean 源代码的工具等资源。

**标签**: `#Lean`, `#formal verification`, `#mathematics`, `#GRH`, `#proof golfing`

---

<a id="item-4"></a>
## [新预印本否定了多项式 Hirsch 猜想](https://github.com/openai/math/blob/main/preprints/Superpolynomial-graph-diameter-of-simple-polytopes-November-24-2026/paper.pdf) ⭐️ 8.0/10

OpenAI 的数学 GitHub 仓库上发布的一篇新预印本通过构造图直径在面数上超多项式的简单多面体，否定了多项式 Hirsch 猜想。这表明一般不存在多项式时间的单纯形算法。 这一结果解决了多面体组合学中的一个核心开放问题，并排除了多项式时间单纯形法的可能性，影响了线性规划的理论基础及主元规则分析。它还对复杂性理论和组合几何学具有重要意义。 该预印本构造了图直径超多项式的简单多面体，这比 2010 年对原始 Hirsch 猜想的否定更强。原始猜想已被一个 43 维、86 个面且直径大于 43 的多面体否定，但那个反例并未排除多项式直径的可能性。

hackernews · acossta · 11月25日 17:34 · [社区讨论](https://news.ycombinator.com/item?id=50644980)

**背景**: Hirsch 猜想于 1957 年提出，断言一个具有 n 个面的 d 维多面体的图直径至多为 n-d，这为单纯形法的步数提供了下界。该猜想在 50 多年后于 2010 年被 Francisco Santos Leal 否定。多项式 Hirsch 猜想将界放宽为 O(n^k)（k 为某个固定常数），是关于直径是否有多项式界的遗留问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polynomial_Hirsch_conjecture">Polynomial Hirsch conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hirsch_conjecture">Hirsch conjecture - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Simplex_algorithm">Simplex algorithm - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者澄清这一结果意味着不存在多项式时间的单纯形算法，并且这是对 2010 年原始 Hirsch 猜想否定的后续工作。有人询问证明是否是构造性的，其他人则讨论了这对解决重大数学问题的更广泛影响。

**标签**: `#combinatorial geometry`, `#linear programming`, `#simplex algorithm`, `#Hirsch conjecture`, `#complexity theory`

---

<a id="item-5"></a>
## [Google Research 发布关于整数分解和离散对数的 Cogentic 论文](https://github.com/google-research/google-research/tree/master/cogentic_research_papers) ⭐️ 8.0/10

Google Research 在其 GitHub 仓库的“cogentic_research_papers”目录下发布了一系列论文，涵盖整数分解、离散对数及相关数学主题。此次发布引发了猜测，认为这些是名为 Cogentic 的 AI 驱动系统的早期成果，该系统可能利用大语言模型协作解决数学猜想。 整数分解和离散对数是 RSA 和 Diffie-Hellman 等广泛使用的公钥密码系统的基础，因此在这些问题上取得任何重大进展都可能对数字安全产生深远影响。此次发布也推动了利用 AI 加速数学发现的更广泛趋势，这可能改变研究的开展方式。 根据社区讨论，Cogentic 似乎是一个专门的框架，用于协调现有的大语言模型协作解决数学猜想，它使用一个中央协调器和一个共享的中间证明数据库。论文本身以 PDF 形式托管在 Google Research 的 GitHub 仓库中，但摘要中并未详细说明具体的算法或结果。

hackernews · rgwohlbold · 11月25日 13:33 · [社区讨论](https://news.ycombinator.com/item?id=50642086)

**背景**: 整数分解是将一个数分解为质因数的过程，其假定的困难性是 RSA 加密安全性的基础。离散对数问题同样被认为对经典计算机而言是计算上不可行的，它是 Diffie-Hellman 密钥交换和其他密码协议的基础。近期 AI 在数学领域的进展，例如大语言模型辅助证明，引发了人们对加速解决这些长期问题的希望和担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50642086">Google releases Cogentic papers on integer... | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Discrete_logarithm">Discrete logarithm - Wikipedia</a></li>
<li><a href="https://github.com/google-research/google-research/blob/master/cogentic_research_papers/edge_reconstruction/paper.pdf">github.com/ google - research / google - research /blob/master/ cogentic ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论（452 分，337 条评论）显示出强烈的兴趣，一些用户引用可靠消息来源的传言称这只是“更大事物的冰山一角”。其他人将这一刻比作 AlphaGo 的突破，认为这是计算机科学的激动人心的时刻，并对如此每日的突破未能提振 AI 市场表示惊讶。一个值得注意的情绪是信念的转变：数学可能不再免疫于通过投入资金和算力来解决问题。

**标签**: `#cryptography`, `#integer factorization`, `#discrete logarithms`, `#Google Research`, `#AI for math`

---

<a id="item-6"></a>
## [文章主张有责任心的工程师应拥抱 LLM 工具，引发辩论](https://www.iankduncan.com/engineering/2026-11-19-smart-people-who-give-a-shit-use-tools) ⭐️ 8.0/10

Ian K. Duncan 发表了一篇文章，主张聪明且有责任心的工程师应该使用 LLM 工具，这在 Hacker News 上引发了 231 条评论的讨论，质疑了“更高层次抽象”的类比，并警告代码理解力可能被侵蚀。 这场辩论凸显了软件工程中日益增长的矛盾：虽然 LLM 提高了生产力，但它们可能削弱手写代码带来的深度理解，可能让不够谨慎的开发者超越更勤勉的开发者。 评论者指出，使用 LLM 与过去从汇编到 C 的抽象转变有本质不同，因为被抽象掉的是开发者而非代码，并且研究表明自写代码比生成代码理解得更快、更准确。

hackernews · matthewsinclair · 11月25日 07:46 · [社区讨论](https://news.ycombinator.com/item?id=50639698)

**背景**: 像 GitHub Copilot 和 ChatGPT 这样的 LLM 辅助编码工具已广泛使用，人们将其与高级语言和编译器等历史抽象层进行比较。然而，批评者认为 LLM 不同，因为它们生成代码时开发者不一定自己建模问题，这可能导致知识侵蚀。

**社区讨论**: 评论者质疑了抽象类比，认为 LLM 抽象的是开发者而非代码，并警告 AI 消除了通过自己写代码来确保深度理解这一保障。一些人指出，LLM 可能让粗心的发布者超越谨慎的工程师，需要自律来防止知识退化。

**标签**: `#LLM`, `#software-engineering`, `#AI-assisted-coding`, `#developer-productivity`, `#code-quality`

---

<a id="item-7"></a>
## [FCC 批准 SpaceX 在太空部署 AI 数据中心计划](https://techcrunch.com/2026/11/25/fcc-approves-spacex-plan-to-put-ai-data-centers-in-space/) ⭐️ 8.0/10

美国联邦通信委员会（FCC）批准了 SpaceX 在太空部署 AI 数据中心的计划，同时驳回了反对者关于该计划威胁科学研究的担忧，认为这超出了其监管权限。 这一批准是一个重要的监管里程碑，可能加速轨道计算基础设施的发展，对太空政策、AI 基础设施和科学研究产生重大影响。 FCC 认定，关于对科学研究潜在威胁的担忧超出了其监管权限，而是专注于其管理电磁频谱和卫星通信的职责。

rss · TechCrunch · 11月25日 20:56

**背景**: FCC 负责管理和许可商业及非商业用户（包括卫星运营商）的电磁频谱。SpaceX 一直在扩展其 AI 雄心，包括计划使用 NVIDIA 技术构建轨道计算系统。轨道数据中心可以利用丰富的太阳能，并避免地面设施面临的一些环境挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencedaily.com/releases/2026/06/260618041501.htm">SpaceX wants to build AI data centers in space . | ScienceDaily</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#AI infrastructure`, `#FCC regulation`, `#space policy`, `#data centers`

---

<a id="item-8"></a>
## [安全研究员批评 Ubuntu 补丁响应缓慢](https://www.openwall.com/lists/oss-security/2026/11/25/9) ⭐️ 7.0/10

安全研究员 Hanno Böck 在 oss-security 邮件列表上发文指出，Ubuntu 对严重 Linux 内核漏洞的修复发布过于缓慢，并提到近期一台 Ubuntu LTS 系统仍运行内核 7.0.0-44，表明 Ubuntu 是在旧内核上回移补丁，而非跟随 kernel.org 的长期支持内核。 该报告在 Hacker News 上引发热议（165 分、77 条评论），凸显出人们对广泛使用的企业级发行版能否跟上内核安全补丁节奏的担忧，并促使一些组织重新考虑在服务器和桌面上是否继续选用 Ubuntu。 核心技术问题在于，Ubuntu 将修复回移到较旧的内核版本上，而不是基于 kernel.org 的长期支持内核进行变基；讨论还指出，大多数主流发行版都会花大量时间做回归测试，因此补丁较慢可能是有意为之的权衡，而非单纯的疏忽。

hackernews · gslin · 11月25日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=50647181)

**背景**: Ubuntu 等 Linux 发行版负责打包 Linux 内核及其他软件，当安全漏洞被披露时，发行版必须回移或变基修复，并在发布前进行测试。Ubuntu LTS 版本优先考虑稳定性而非最新软件包，因此与更紧密跟随上游的发行版相比，安全更新可能更慢。oss-security 邮件列表是研究人员公开披露和讨论开源软件漏洞的公共论坛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.openwall.com/lists/oss-security/2026/11/25/9">oss-security - Slow Ubuntu security response times</a></li>
<li><a href="https://seclists.org/oss-sec/2026/q4/890">oss-sec: Slow Ubuntu security response times</a></li>
<li><a href="https://daily.dev/posts/slow-ubuntu-security-response-times-9gafircej">Slow Ubuntu security response times - daily.dev</a></li>

</ul>
</details>

**社区讨论**: 评论者围绕供应链安全担忧下该选用哪个桌面发行版展开讨论，有人表示已因 Ubuntu 安全响应缓慢不可接受而将服务器镜像从 Ubuntu 迁至 Debian。也有人提醒 Debian 的 QA 资源有限、可能出现回归问题，还有评论者引用稳定内核维护者的警告称，随意挑选补丁反而可能让系统更不安全。

**标签**: `#Linux`, `#Security`, `#Ubuntu`, `#Distributions`, `#Supply Chain`

---

<a id="item-9"></a>
## [《纽约时报》警告摄影师不要因 AI 功能更新 Photoshop](https://www.theverge.com/ai-artificial-intelligence/1041227/the-new-york-times-warns-photographers-not-to-update-photoshop-over-ai-features) ⭐️ 7.0/10

据 The Verge 报道，《纽约时报》建议摄影师不要因为 Adobe Photoshop 的生成式 AI 功能而更新该软件。这一警告凸显了人们对创意工作中 AI 生成内容所带来的污名和信誉风险的日益担忧。 一家主要媒体的这一立场标志着行业的重要转变：创意工具中的 AI 功能正成为负担而非优势。这可能迫使 Adobe 和其他软件供应商提供无 AI 版本或更清晰的标签，并影响依赖这些工具维护专业信誉的摄影师、设计师和品牌。 《纽约时报》的警告与区分完全由 AI 生成的图像和仅经过轻微 AI 辅助编辑的图像之困难有关，尤其是当 Instagram 和 Facebook 等平台可能将内容标记为“AI 生成”时，这可能损害品牌信誉。Adobe 由 Firefly 模型驱动的生成填充和扩展功能已结束测试并被广泛使用，但它们会嵌入 AI 来源信号，从而可能触发此类标签。

hackernews · rmason · 11月25日 21:18 · [社区讨论](https://news.ycombinator.com/item?id=50647673)

**背景**: 自 2023 年以来，Adobe Photoshop 集成了生成式 AI 功能，如生成填充和扩展，允许用户使用文本提示添加或修改图像内容。这些功能依赖于 Adobe Firefly，这是一个为商业安全设计的生成式 AI 模型系列。同时，C2PA 内容凭证等标准旨在提供关于图像如何创建或编辑的可验证元数据，但它们也能使 AI 参与变得可检测。《纽约时报》在维护严格的照片伦理方面有着悠久历史，其警告反映了对 AI 影响视觉媒体信任的更广泛担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://contentauthenticity.org/how-it-works">How it works - Content Authenticity Initiative</a></li>
<li><a href="https://www.nytimes.com/2025/04/30/magazine/artificial-intelligence-photo-ethics.html">Can I Use A . I . to Look Better Online? - The New York Times</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者普遍认为，创意工作中的生成式 AI 带有社会污名和信誉风险，一位专业人士指出，几乎无法将完全由 AI 生成的图像与轻微的 AI 辅助编辑区分开来。其他人看到了 Affinity 等竞争对手的机会，并预测将转向非订阅模式，还有一些人批评 Adobe 的订阅策略。

**标签**: `#AI`, `#Adobe Photoshop`, `#creative tools`, `#AI stigma`, `#software subscriptions`

---

<a id="item-10"></a>
## [博客称 Jev 很可能是 Qwen3.5-35B-A3B，依据延迟分析](https://modaic.dev/blog/latency-doesnt-lie) ⭐️ 7.0/10

modaic.dev 上的一篇博客文章认为，TypeSafe AI 开发的专有模型 Jev 很可能是 Qwen3.5-35B-A3B 的微调版本，依据是延迟分析和自我识别回答。该文章在 Hacker News 上引发了关于此类方法可靠性的批判性讨论。 如果属实，这将表明一个商业化的“决策模型”是建立在开源 LLM 之上的，引发了对 AI 行业透明度和来源的质疑。讨论还凸显了可靠识别专有模型的挑战，这对基准测试和信任至关重要。 该分析依赖于延迟测量和询问模型自身身份，但评论者指出仅凭延迟无法区分 Qwen 和 Gemma，且自我识别已知不可靠。TypeSafe 的网站明确否认 Jev 是 LLM，称其为“System One Model”，返回类型化决策而非生成文本。

hackernews · csoham · 11月25日 22:57 · [社区讨论](https://news.ycombinator.com/item?id=50648823)

**背景**: Jev 是 TypeSafe AI（成立于 2024 年）开发的专有 AI 模型，专为分类或回归任务设计，返回带有概率和置信度分数的类型化决策，而非生成文本。Qwen3.5-35B-A3B 是阿里巴巴云 Qwen 团队的开源模型，于 2026 年 2 月 24 日发布，属于 Qwen3.5 系列。模型识别——确定专有服务使用哪个基础模型——是 LLM 社区中常见但具有挑战性的逆向工程任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://speechmap.ai/models/qwen-qwen3-5-35b-a3b/">Model : qwen/ qwen 3 . 5 - 35 b - a 3 b</a></li>
<li><a href="https://playground.roboflow.com/models/compare/gpt-5-mini-vs-qwen3-5-35b-a3b">GPT-5 Mini vs Qwen 3 . 5 35 B A 3 B : Vision Model Comparison</a></li>
<li><a href="https://github.com/QwenLM/Qwen3.8">GitHub - QwenLM/ Qwen 3 .8: Qwen 3 .8 is the large language model ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍持怀疑态度：有人指出延迟数据无法区分 Qwen 和 Gemma，另一人指出 TypeSafe 明确否认 Jev 是 LLM，呼吁提供更确凿的证据。其他人质疑自我识别的可靠性，并提出替代假设，例如 LoRA 微调表现不同。

**标签**: `#LLM`, `#model-identification`, `#Qwen`, `#latency`, `#Hacker News`

---

<a id="item-11"></a>
## [开发者逆向工程 Windows 响度均衡并移植到 PipeWire](https://github.com/xoxorwr/pw-loudness-eq) ⭐️ 7.0/10

一位开发者逆向工程了 Windows 的响度均衡功能，并将其移植到 PipeWire，在 GitHub 上发布了名为 pw-loudness-eq 的项目。该项目旨在为 Linux 用户复现 Windows 音频处理中的响度归一化行为。 这将 Windows 常见的音频增强功能带到了 Linux 的现代音频服务器上，可能改善希望获得一致音量水平的 PipeWire 用户的聆听体验。这也凸显了 PipeWire 作为高级音频处理平台日益成熟。 该实现基于对 Windows 音频处理的逆向工程，这可能引发关于复制专有算法的伦理和法律问题。社区成员指出，该算法本质上是响度归一化，可能需要额外的限制器来防止纯音增益过大。

hackernews · ThrowNotAway · 11月25日 11:34 · [社区讨论](https://news.ycombinator.com/item?id=50641171)

**背景**: 响度均衡是 Windows 的一项音频增强功能，可缩小安静和响亮声音之间的差异，使对话更容易听清，但可能使音乐动态变得平淡。PipeWire 是 Linux 上的低级多媒体框架，处理音频和视频流，旨在统一并取代 PulseAudio 和 JACK。响度归一化根据感知响度调整音频，不同于动态范围压缩（后者降低较响部分的音量）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PipeWire">PipeWire - Wikipedia</a></li>
<li><a href="https://www.pipewire.org/">PipeWire</a></li>
<li><a href="https://www.thewindowsclub.com/disable-or-enable-loudness-equalization-in-windows-10">How to disable or enable Loudness Equalization in Windows 11/10</a></li>

</ul>
</details>

**社区讨论**: 评论者就术语展开辩论，有人指出应称为响度归一化而非均衡。一些人质疑逆向工程的必要性，认为更简单的限制器算法也能达到类似效果，而另一些人则对复制专有代码提出伦理担忧。另一位评论者指出，Windows 本身在共享模式音频路径中应用了微妙的限制器。

**标签**: `#audio-processing`, `#reverse-engineering`, `#pipewire`, `#windows`, `#loudness-normalization`

---

<a id="item-12"></a>
## [作者用 Lean 审计 Clojure 核心库，发现未报告的错误](https://s.conao3.com/blog/2026/e4f733) ⭐️ 7.0/10

一位作者使用 Lean 定理证明器对 Clojure 核心库进行形式化检查，并报告发现了此前未报告的错误。这项工作在博客文章中分享，并引发了 67 条评论的讨论，内容涉及验证工具和发现的有效性。 这种跨语言验证方法展示了如何将形式化方法应用于审计广泛使用的动态语言库（如 Clojure 核心库），有望提升庞大生态系统的可靠性。它也引发了关于此类审计实用性和噪声水平的争论。 社区成员指出，一些报告的问题（如(.indexOf (seq (byte-array [1 2 3])) 2)和(get "abc" 1.9)）源于预期的类型强制转换行为，而非真正的错误，建议减少噪声。讨论还比较了 Lean 与 Rocq（原 Coq）在程序验证方面的应用。

hackernews · encyclopedism · 11月25日 14:56 · [社区讨论](https://news.ycombinator.com/item?id=50642939)

**背景**: Lean 是一个交互式定理证明器，用于数学证明和软件属性的形式化验证。Clojure 是一种运行在 JVM 上的动态函数式 Lisp 方言，其核心库提供基础函数和数据结构。形式化验证涉及通过数学方法证明系统按照规范正确运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leanprover.github.io/theorem_proving_in_lean/introduction.html">1. Introduction — Theorem Proving in Lean 3 (outdated)...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>
<li><a href="https://clojuredocs.org/core-library">Clojure 's Core Library | ClojureDocs - Community-Powered Clojure ...</a></li>

</ul>
</details>

**社区讨论**: 评论者批评某些发现是类型强制转换问题而非错误，并质疑 Lean 是否因语言模型支持更好而比 Rocq 更受青睐。其他人提到了对其他 Lisp 实现（SBCL、Clozure、ACL2）的相关审计，并表示有兴趣学习 Lean 进行测试。

**标签**: `#Clojure`, `#Lean`, `#formal-verification`, `#programming-languages`, `#bug-hunting`

---

<a id="item-13"></a>
## [科学家界定 AI 代理在研究中的使用边界](https://huggingface.co/blog/allenai/where-scientists-draw-the-line-on-ai-agents) ⭐️ 7.0/10

AllenAI 在 Hugging Face 上发表的一篇博客文章探讨了科学家在研究中运用 AI 代理的界限，并强调了相关担忧和接受标准。该文章调查了科学家对 AI 代理使用边界的看法，为理解 AI 在研究中的采用和信任提供了见解。 随着 AI 代理变得更加自主并能执行多步骤任务，了解科学家的信任和接受标准对于负责任地将其整合到研究工作流程中至关重要。该分析揭示了采用障碍以及研究人员依赖 AI 代理的条件，对工具开发者和研究机构具有影响。 文章可能讨论了诸如可追溯性、可重复性以及捏造声明的风险等具体问题，这些对科学严谨性至关重要。它还可能概述了科学家在将任务委托给 AI 代理之前所要求的接受标准，如透明度和可证明的可信度。

rss · Hugging Face Blog · 11月25日 18:52

**背景**: AI 代理是能够自主追求目标并完成任务的软件系统，具备推理、规划和记忆能力。在科学研究中，对 AI 代理的信任日益受到关注，研究表明 AI 生成的研究可能包含捏造声明且无法达到专家标准。Hugging Face 是分享 AI 模型和数据集的主要平台，而 AllenAI 是一家以开发 AI 技术闻名的研究机构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.ontoforce.com/blog/can-you-trust-an-ai-agent-in-a-drug-discovery-pipeline-three-conditions">Can you trust an AI agent in a drug discovery pipeline? Three conditions</a></li>
<li><a href="https://huggingface.co/papers/2610.19159">Paper page - Into the Unknown: Benchmarking AI agents on open...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#scientific research`, `#AI adoption`, `#trust`, `#Hugging Face`

---

<a id="item-14"></a>
## [纽约州对 AI 聊天机器人玩具实施五年禁令](https://techcrunch.com/2026/11/25/want-to-buy-your-kid-an-ai-toy-this-christmas-not-in-new-york/) ⭐️ 7.0/10

纽约州州长凯西·霍楚尔于周三签署立法，对面向 13 岁以下儿童的 AI 聊天机器人玩具（包括会说话的毛绒动物）的制造和销售实施五年禁令。该禁令将于 2027 年 2 月生效，违规者每天最高可被罚款 15,000 美元。 这是美国首个州级 AI 玩具禁令，树立了重要的监管先例，可能影响其他州，并迫使 AI 玩具开发商重新思考产品设计和安全标准。该禁令在假日购物季前直接影响到制造商、零售商和家长。 该禁令基于 Common Sense Media 的新研究，该研究记录了不当内容暴露和情感发展风险等安全失败案例。2026 年 3 月剑桥大学为 Childhood Trust 进行的一项研究发现，幼儿会对 AI 玩具形成情感依恋，且没有证据表明其对发展有益；另一项针对 Curio 公司 Gabbo 玩具的研究发现，它可能误解情感线索。

rss · TechCrunch · 11月25日 18:11

**背景**: AI 聊天机器人玩具是使用大型语言模型与儿童进行对话的毛绒或互动设备，通常被宣传为教育伴侣。Common Sense Media 是一家研究青少年与技术的非营利组织，其青年 AI 安全研究所进行的测试揭示了这些玩具令人不安的回应。儿童安全组织还援引预防原则，敦促亚马逊和 eBay 等零售商在 AI 玩具被证明安全之前停止销售。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/nov/25/new-york-bans-ai-toys">New York bans AI toys, including those using internet to talk ...</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/york-imposes-five-ban-ai-180458200.html?fr=sycsrp_catchall">New York Imposes Five-Year Ban on AI Chatbot Toys for Kids</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/23/child-safety-groups-urge-amazon-ebay-stop-selling-ai-toys-until-proved-safe">Child safety groups urge Amazon and eBay to stop selling AI toys until...</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#child safety`, `#AI toys`, `#policy`, `#consumer AI`

---

<a id="item-15"></a>
## [州总检察长挑战 Character.AI 破产拍卖用户聊天记录的计划](https://techcrunch.com/2026/11/25/state-ags-fight-character-ais-plan-to-auction-off-users-private-chats/) ⭐️ 7.0/10

由 42 个州和地区总检察长组成的联盟反对 Character.AI 提出的第 11 章破产出售计划，该计划将把超过 2100 万个美国账户（其中包括 210 万个注册为未成年人的账户）的敏感个人数据转移给买家。总检察长们请求法院阻止该出售或施加数据保护措施，并希望用户能在数据转移前有机会删除自己的数据。 此案为用户数据（尤其是敏感的 AI 聊天记录和未成年人信息）在破产中的处理方式树立了先例，可能影响数百万用户，并塑造 AI 行业未来的数据治理和消费者保护标准。它凸显了企业资产清算与隐私权之间的紧张关系，并可能影响其他 AI 公司在财务困境中处理用户数据的方式。 此次出售涉及约 2100 万个美国账户的聊天记录及相关个人信息，其中 210 万个账户声明属于 18 岁以下的用户。纽约州总检察长 Letitia James 和康涅狄格州总检察长等人牵头反对，认为私人对话可能在缺乏足够隐私保护的情况下被卖给出价最高者。

rss · TechCrunch · 11月25日 17:35

**背景**: Character.AI 是一个 AI 聊天机器人平台，允许用户创建和与自定义角色互动。2026 年 10 月，该公司启动了自愿的第 11 章破产程序，以促进法院监督下的资产出售。在破产程序中，公司的资产（包括用户数据）可以被出售以偿还债权人，这引发了隐私和同意方面的担忧。州总检察长经常介入此类案件以保护消费者，尤其是未成年人等弱势群体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/25/state-ags-fight-character-ais-plan-to-auction-off-users-private-chats/">State AGs fight Character.AI’s plan to auction off users ...</a></li>
<li><a href="https://cctest.ai/en/articles/42-state-and-territorial-ags-oppose-character-ai-chat-data-sale">42 AGs Challenge Character.AI’s Planned Chat Data Auction ...</a></li>
<li><a href="https://www.aiaffairs.com/government/attorneys-general-character-ai-bankruptcy-data-protections/">Forty attorneys general seek data safeguards in Character.AI ...</a></li>

</ul>
</details>

**标签**: `#AI privacy`, `#data governance`, `#consumer protection`, `#Character.AI`, `#regulation`

---