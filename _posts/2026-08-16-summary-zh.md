---
layout: default
title: "Horizon Summary: 2026-08-16 (ZH)"
date: 2026-08-16
lang: zh
---

> 从 24 条内容中筛选出 14 条重要资讯。

---

1. [Stripe 将以超过 70 亿美元收购 AI 网关 OpenRouter](#item-1) ⭐️ 9.0/10
2. [Anthropic 发布 Claude 系统提示词，社区可追踪变化](#item-2) ⭐️ 8.0/10
3. [NIH 终止针对青年临床研究者的关键资助](#item-3) ⭐️ 8.0/10
4. [Cloudflare 在切换域名服务器时静默注入分析脚本](#item-4) ⭐️ 8.0/10
5. [来自发展中国家的嵌入式工程师为 RISC-V 辩护](#item-5) ⭐️ 7.0/10
6. [AI API 信用额度转售市场的兴起](#item-6) ⭐️ 7.0/10
7. [圣露西核电站 1 号机组因控制棒掉落而停堆](#item-7) ⭐️ 7.0/10
8. [Firefox for iOS 新增原生广告拦截器，但存在限制](#item-8) ⭐️ 7.0/10
9. [科学论文中充斥“肾脏失望”等“折磨短语”](#item-9) ⭐️ 7.0/10
10. [达里奥·阿莫迪：AI 不信任反映更广泛的机构信任危机](#item-10) ⭐️ 7.0/10
11. [女子指控继父利用 Grok 将童年照片制作成露骨图像](#item-11) ⭐️ 7.0/10
12. [Buf 宣布首个 Protobuf 的 LSP 支持](#item-12) ⭐️ 7.0/10
13. [编程中垃圾回收的真实成本](#item-13) ⭐️ 7.0/10
14. [重新思考 C 语言替代：开发者的经验教训](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Stripe 将以超过 70 亿美元收购 AI 网关 OpenRouter](https://techcrunch.com/2026/08/16/stripe-will-reportedly-acquire-ai-gateway-startup-openrouter-for-7b/) ⭐️ 9.0/10

据报道，Stripe 将以超过 70 亿美元收购 AI 网关初创公司 OpenRouter。这笔交易将使 Stripe 成为 AI 模型的关键支付和访问层。 此次收购标志着 AI 基础设施领域的重大整合，并验证了 AI 网关市场的价值。通过将支付与 AI 模型访问相结合，它可能对开发者及整个 AI 生态系统产生重大影响。 OpenRouter 的 CEO 曾将该公司描述为“AI 领域的 Stripe”，强调其作为访问多种 LLM 的统一接口的作用。据报道，这笔交易价值至少 70 亿美元，但尚未得到官方确认。

rss · TechCrunch · 8月16日 20:57

**背景**: OpenRouter 是一个提供统一接口来访问和使用大型语言模型（如 GPT-4、Claude 和 Llama）的平台。它充当网关，将请求路由到所选模型并返回响应。Stripe 是一个主要的支付处理平台，已经为 ChatGPT Plus 等 AI 公司提供支持，此次收购将把其角色扩展到 AI 模型的访问和变现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.truefoundry.com/blog/openrouter-vs-ai-gateway">OpenRouter Vs AI Gateway: Differences, Use Cases & Best Choice</a></li>
<li><a href="https://medium.com/@tahirbalarabe2/what-is-open-router-a-unified-gateway-for-large-language-models-8b15597af7b7">What is Open Router? A Unified Gateway for Large Language Models | by Tahir | Medium</a></li>
<li><a href="https://stripe.com/use-cases/ai">Stripe for AI Companies | Trusted by Industry Leaders in AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#acquisition`, `#Stripe`, `#OpenRouter`, `#AI infrastructure`

---

<a id="item-2"></a>
## [Anthropic 发布 Claude 系统提示词，社区可追踪变化](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 在其平台文档中发布了 Claude 使用的系统提示词，揭示了模型的行为准则和安全优先级。这是一次罕见的透明化举措，使社区能够分析并追踪其变化。 这种透明化意义重大，因为它提供了前所未有的视角，让人们了解领先 AI 模型是如何被塑造的，使研究人员和开发者能够理解和评判 Anthropic 的安全与行为选择。这也为其他 AI 实验室树立了先例，可能提升整个行业的问责制。 系统提示词包含诸如在危机情况下优先考虑用户福祉而非完成任务，以及验证图像是否实际存在而非仅凭提示假设等指令。社区成员如 Simon Willison 创建了 git 仓库来追踪模型版本之间的变化，例如 Opus 4.8 和 Opus 5 之间的差异。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**背景**: 系统提示词是给大型语言模型（LLM）的初始指令，用于定义其行为、能力和响应风格。它们对塑造模型输出至关重要，通常被 AI 公司保密。Anthropic 决定发布这些提示词，背离了行业惯例，为外界提供了一个难得的机会，得以窥见主要 AI 系统的运行细节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs - Anthropic</a></li>
<li><a href="https://github.com/asgeirtj/system_prompts_leaks">GitHub - asgeirtj/system_prompts_leaks: Extracted system ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，像 Simon Willison 这样的知名人士提供了追踪变化的工具。一些评论者如 trjordan 指出，系统提示词是分层行为塑造系统的一部分，反映了 Anthropic 的路线图。然而，也有离题的声音，如 quaintdev 对平台内容审核表示担忧。

**标签**: `#AI`, `#Anthropic`, `#system prompts`, `#transparency`, `#LLM`

---

<a id="item-3"></a>
## [NIH 终止针对青年临床研究者的关键资助](https://www.science.org/content/article/nih-ending-key-grant-budding-clinical-researchers) ⭐️ 8.0/10

美国国立卫生研究院（NIH）决定终止一项旨在支持早期职业临床研究者的关键资助项目，此举在科学界引发广泛担忧。这一决定标志着联邦研究资助优先事项的重大转变。 这一决定可能导致临床研究领域年轻人才出现代际流失，因为博士毕业生和博士后研究人员可能离开该领域或国家。它削弱了未来医学发现的储备，可能对公共卫生和科学创新产生长期负面影响。 该资助项目专门针对初出茅庐的临床研究者，提供关键的早期职业资金。终止该项目是 NIH 更广泛的预算削减和政策变化的一部分，这些变化也影响了其他研究领域，一些实验室在没有明确理由的情况下被取消资助。

hackernews · brandonb · 8月16日 16:14 · [社区讨论](https://news.ycombinator.com/item?id=49321353)

**背景**: NIH 是美国生物医学研究的主要联邦机构，每年资助数千项拨款。早期职业资助对于帮助新研究者建立独立职业生涯至关重要，其缺失可能扰乱整个研究生态系统。最近的削减是联邦对科学支持减少的更广泛趋势的一部分，引发了对美国研究领导地位未来的担忧。

**社区讨论**: 社区评论表达了强烈的担忧和沮丧。一些人认为此举是蓄意削弱美国科学的恶意行为，而另一些人则将其归因于管理不善。许多人强调了现实影响，如年轻研究者离开国家和有前景的研究被中止，一些人指出这是人才的代际损失。

**标签**: `#NIH`, `#research funding`, `#science policy`, `#clinical research`, `#academia`

---

<a id="item-4"></a>
## [Cloudflare 在切换域名服务器时静默注入分析脚本](https://news.ycombinator.com/item?id=49322107) ⭐️ 8.0/10

当用户将域名服务器切换到 Cloudflare 时，Cloudflare 会自动向网站注入 JavaScript 分析脚本，而无需明确同意，需要手动选择退出。该问题由一位用户在 Hacker News 上报告，该用户在其仅包含 HTML、无 JavaScript 的网站上发现了该脚本。 这引发了重大的隐私和透明度问题，因为 Cloudflare 作为中间人，向并非其托管的网站注入代码，可能侵犯用户同意权，甚至违反 CFAA 等法律条款。它影响到许多为了 DNS 或其他服务而切换域名服务器的用户，并可能削弱对 Cloudflare 隐私承诺的信任。 注入的脚本来自 static.cloudflareinsights.com/beacon.min.js，并包含带有 token 和版本号的 data-cf-beacon 属性。用户可以通过 Cloudflare 仪表板中的 Analytics > Web Analytics 禁用它，或使用 Content-Security-Policy (CSP) 头来阻止它。该行为似乎对新域名默认启用，而一些用户报告在旧站点上需要手动启用。

hackernews · stagas · 8月16日 17:49

**背景**: Cloudflare 是一家主要的 CDN 和 DNS 提供商，提供 Web Analytics 作为传统分析的隐私友好替代方案。当用户将域名服务器切换到 Cloudflare（完整设置）时，Cloudflare 可以代理流量并注入脚本。Web Analytics 设计为轻量且注重隐私，但新域名默认开启的行为引发了批评。用户可以通过仪表板或使用 CSP 头选择退出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://community.cloudflare.com/t/cant-disable-web-analytics-for-coudflare-pages-site/761716">Can't disable Web Analytics for Coudflare Pages site</a></li>
<li><a href="https://www.cloudflare.com/web-analytics/">Cloudflare Web Analytics</a></li>
<li><a href="https://community.cloudflare.com/t/how-to-disable-cloudflare-analytics-tracking/26307">How to Disable CloudFlare analytics tracking</a></li>

</ul>
</details>

**社区讨论**: 社区表达了担忧和不满，一些用户分享了注入脚本的具体内容，并建议使用 CSP 作为解决方法。其他人质疑向非 Cloudflare 托管的网站注入代码的合法性，并引用了 CFAA。关于该功能是默认启用还是需要手动激活，也存在讨论，用户反馈不一。

**标签**: `#Cloudflare`, `#privacy`, `#analytics`, `#security`, `#web development`

---

<a id="item-5"></a>
## [来自发展中国家的嵌入式工程师为 RISC-V 辩护](https://rvembedded.com/blog_post/12/) ⭐️ 7.0/10

一位来自发展中国家的嵌入式工程师发表了一篇博客文章，回应了对 RISC-V 的批评，认为其灵活性和低成本使其非常适合嵌入式应用，尤其是在成本和可及性至关重要的地区。 这一回应为广泛讨论的批评提供了宝贵的反方观点，强调了 RISC-V 的开源模式如何能够使发展中地区的硬件开发更加民主化。它凸显了在技术辩论中考虑全球视角的重要性，可能影响人们对 RISC-V 的看法和采用。 原始批评主要关注 RISC-V 与 ARM64 相比的性能以及由于 ISA 可选部分导致的碎片化问题，而回应则认为对于嵌入式应用，成本和灵活性比这些担忧更重要。作者指出，将芯片运送到他所在位置的运费可能为 60 至 200 美元，但又声称 RISC-V 部件每个只需十美分，这一点被一些评论者认为存在矛盾。

hackernews · Narishma · 8月16日 17:01 · [社区讨论](https://news.ycombinator.com/item?id=49321717)

**背景**: RISC-V 是一种开源指令集架构（ISA），允许任何人设计、修改和制造处理器，无需许可费，这与 ARM 等专有架构不同。这种开放性促进了创新和定制化，使其在初创公司、学术研究和专业应用中广受欢迎。在嵌入式系统中，成本和功耗效率至关重要，RISC-V 的模块化允许设计者根据需求定制 ISA，可能降低成本并提高发展中地区的可及性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC-V - Wikipedia</a></li>
<li><a href="https://www.allaboutcircuits.com/technical-articles/introductions-to-risc-v-instruction-set-understanding-this-open-instruction-set-architecture/">An Introduction to RISC-V—Understanding RISC’s Open ISA - Technical Articles</a></li>
<li><a href="https://inovasense.com/insights/risc-v-vs-arm">RISC-V vs ARM: Embedded Architecture - Inovasense</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对双方的论点进行了批判性讨论。一些人认为回应没有直接回应原始批评，后者关注的是嵌入式之外领域的性能和碎片化问题。其他人则质疑作者的成本说法，指出运费与低部件价格似乎不一致。总体而言，讨论突出了成本、可及性和碎片化方面的细微差别，一些人支持作者关于 RISC-V 对嵌入式应用有益的观点。

**标签**: `#RISC-V`, `#embedded systems`, `#hardware`, `#open source`, `#technology debate`

---

<a id="item-6"></a>
## [AI API 信用额度转售市场的兴起](https://vectoral.com/blog/who-are-the-token-brokers) ⭐️ 7.0/10

围绕转售未使用的 AI API 信用额度，一个新兴经济已经形成，经纪人充当拥有多余信用额度的用户与寻求更便宜访问的用户之间的中介。这种做法虽然常常违反平台服务条款，但已发展成为一个重要的灰色市场。 这一趋势凸显了 AI 信用额度的经济价值，并暴露了安全风险，包括账户盗用和数据截获。这也给 OpenAI 和 Google 等平台施加压力，要求其加强执法并重新考虑信用政策，从而影响更广泛的 AI 生态系统。 文章指出，转售者可以使用中间代理修改流量，如果 TLS 在代理处终止，则可能控制客户端机器。平台通过速率限制来防止滥用，但将中继 IP 地址追溯到源账户仍然是一个挑战。

hackernews · mlenhard · 8月16日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=49320611)

**背景**: AI API 信用额度是 OpenAI 和 Google Gemini 等服务的预付使用配额。转售这些额度违反大多数服务条款，但由于价格套利和额度过期，这种做法仍然存在。平台使用速率限制和监控来遏制滥用，但执法难度较大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/rate-limits">Rate limits | Gemini API | Google AI for Developers</a></li>
<li><a href="https://stripe.com/resources/more/real-time-api-abuse-prevention-for-saas-and-ai-platforms">How to Prevent API Abuse for SaaS and AI Platforms | Stripe</a></li>
<li><a href="https://news.ycombinator.com/item?id=49320611">The AI Credit Resale Economy | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论者对信任第三方经纪人表示怀疑，提到黑客攻击和数据隐私风险。一些人指出滥用模式已有数十年历史，而另一些人则指出 linux.do 和 nodeseek.com 等平台上转售经济的规模，认为研究过于肤浅。

**标签**: `#AI`, `#economics`, `#security`, `#marketplace`

---

<a id="item-7"></a>
## [圣露西核电站 1 号机组因控制棒掉落而停堆](https://www.wptv.com/news/treasure-coast/region-st-lucie-county/saint-lucie-nuclear-power-plant-unit-1-manually-shut-down-after-3-control-rods-drop-into-reactor-core) ⭐️ 7.0/10

圣露西核电站 1 号机组因三根控制棒意外掉入反应堆堆芯而被手动关闭。该事件发生在近期，目前电厂运营商和 NRC 正在调查中。 这一事件凸显了压水堆的安全机制，即控制棒插入可降低反应性。同时，它也强调了透明报告和公众理解核安全的重要性，因为此类事件尽管属于设计考虑的情况，仍可能引起公众担忧。 控制棒掉入堆芯，但反应堆已安全手动关闭，未报告放射性释放。这并非圣露西核电站首次发生此类事件；2024 年曾发生类似事件，根本原因涉及程序问题和电气故障。

hackernews · toomuchtodo · 8月16日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49320856)

**背景**: 控制棒用于核反应堆中吸收中子，控制裂变速率。在许多反应堆设计中，控制棒悬挂在堆芯上方，在紧急停堆或断电时可自动掉入，起到安全机制的作用。手动停堆是一种有意将反应堆置于安全状态的操作，通常在检测到异常时启动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nuclear_reactor_physics">Nuclear reactor physics - Wikipedia</a></li>
<li><a href="https://www.bbc.co.uk/bitesize/guides/zyqnrwx/revision/2">Fission reactors - Nuclear power - Edexcel - GCSE Physics...</a></li>
<li><a href="https://world-nuclear.org/information-library/nuclear-power-reactors/overview/nuclear-power-reactors">Nuclear Power Reactors - World Nuclear Association</a></li>

</ul>
</details>

**社区讨论**: 评论者解释称，控制棒掉落是安全特性而非故障，美国反应堆通常即使一根棒完全插入也会进入次临界状态。有人提到 2024 年类似事件并讨论根本原因，还有人指出公众缺乏可参照的风险参考来评估严重性。

**标签**: `#nuclear`, `#safety`, `#reactor`, `#energy`, `#incident`

---

<a id="item-8"></a>
## [Firefox for iOS 新增原生广告拦截器，但存在限制](https://support.mozilla.org/en-US/kb/block-ads-firefox-ios) ⭐️ 7.0/10

Mozilla 已为 iOS 版 Firefox 推出原生广告拦截器，该功能默认关闭，使用基于 EasyList 的过滤列表在广告加载前进行拦截。该功能正在逐步推出，接近稳定版本，支持页面现已上线。 这满足了用户在浏览器中直接拦截广告的常见需求，可能提升 iOS 用户的隐私保护和页面加载速度。这也表明 Mozilla 致力于增强 iOS 版 Firefox 的功能，尽管 WebKit 限制限制了扩展支持。 该广告拦截器不会拦截搜索引擎结果页面（如 Google、Bing、DuckDuckGo）上的广告，也不会拦截 Firefox 主页或新标签页上的赞助内容。它是可选的，默认关闭，用户可以根据需要启用。

hackernews · pentagrama · 8月16日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49319633)

**背景**: 由于苹果 App Store 政策限制浏览器引擎，iOS 版 Firefox 基于 WebKit 构建，这也限制了扩展支持。过去，iOS 用户需要依赖 Firefox Focus 等独立应用或 uBlock Origin Lite 等内容拦截器来拦截广告。Mozilla 的原生广告拦截器旨在通过将广告拦截直接集成到 Firefox 主应用中，简化这一过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.mozilla.org/en-US/kb/block-ads-firefox-ios">Block ads in Firefox for iOS - Mozilla Support</a></li>
<li><a href="https://appleinsider.com/articles/26/08/16/mozilla-gradually-rolls-out-an-ad-blocker-built-into-firefox-for-ios">Mozilla rolls out an ad - blocker built into Firefox for iOS</a></li>
<li><a href="https://piunikaweb.com/2026/08/12/firefox-ios-ad-blocker-support-page/">Firefox’s iOS ad blocker nears stable release as Mozilla ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论提到了现有替代方案，如 Safari 的 uBlock Origin Lite 和 Firefox Focus 的系统级广告拦截，指出新功能减少了操作步骤。一些用户对搜索结果广告和赞助内容未被拦截表示失望，而另一些用户则质疑 iOS 上缺乏扩展支持，并以 Orion 作为反例。

**标签**: `#Firefox`, `#iOS`, `#Adblock`, `#Browser`, `#Privacy`

---

<a id="item-9"></a>
## [科学论文中充斥“肾脏失望”等“折磨短语”](https://scholar.google.com/scholar?q=%22kidney+disappointment%22) ⭐️ 7.0/10

Hacker News 上的一场讨论指出，科学论文中普遍存在“肾脏失望”等“折磨短语”，这些短语可能源于 AI 改写工具或翻译错误。讨论引发了对学术出版中研究诚信问题的日益关注。 这一问题凸显了 AI 生成内容对学术诚信构成的挑战，因为此类短语可能表明存在抄袭或低质量研究。它影响到依赖可靠科学文献的研究人员、出版商和读者。 “肾脏失望”一词出现在 Google Scholar 收录的论文中，类似的例子还有“Joined Together States”和“bosom peril”。这一现象最早由 Cabanac 等人在 2021 年的 arXiv 论文中系统研究，该论文在知名期刊中发现了数千个此类短语。

hackernews · Alifatisk · 8月16日 12:22 · [社区讨论](https://news.ycombinator.com/item?id=49319389)

**背景**: “折磨短语”是替代标准科学术语的无意义词组，通常源于使用改写工具规避抄袭检测或机器翻译质量差。研究人员已开发出检测这些短语的方法，例如查询 Dimensions 等数据库，以识别潜在的虚假或低质量论文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2107.06751">[2107.06751] Tortured phrases : A dubious writing style emerging in...</a></li>
<li><a href="https://www.dimensions.ai/blog/detecting-tortured-phrases-to-unmask-fake-science/">Detecting tortured phrases to unmask fake science | Dimensions</a></li>
<li><a href="https://www.editage.com/insights/tortured-phrases-what-they-are-how-they-are-detected-and-how-to-avoid-them">Tortured phrases : How to avoid them | Editage Insights</a></li>

</ul>
</details>

**社区讨论**: 评论者就根本原因展开辩论，一些人将其归因于非母语者的翻译问题，并引用了“water goat”代替“hydraulic ram”等历史例子。另一些人指出，该术语早在 2021 年就已出现，早于当前的 LLM，表明其源于翻译而非 AI 生成。

**标签**: `#AI-generated content`, `#academic publishing`, `#research integrity`, `#paraphrasing tools`, `#scientific misconduct`

---

<a id="item-10"></a>
## [达里奥·阿莫迪：AI 不信任反映更广泛的机构信任危机](https://simonwillison.net/2026/Aug/16/dario-amodei/) ⭐️ 7.0/10

Anthropic 首席执行官达里奥·阿莫迪表示，公众对 AI 的不信任主要源于更广泛的机构信任危机，而非 AI 领导人的警告。他认为，重建信任需要实际成果，如真正治愈癌症，而非营销活动。 这位 AI 领军人物提出的观点挑战了关于 AI 抵制的常见假设，并强调提供实际利益的重要性。这可能影响 AI 公司处理公众参与和建立信任的方式，将重点从信息传递转向具体成果。 阿莫迪明确拒绝了为 Anthropic 开展“光鲜亮丽、积极宣传的营销活动”的想法，认为此类努力被视为欺骗。他承认包括 Anthropic 在内的 AI 公司尚未兑现造福世界的重大承诺，称这是最准确的批评。

rss · Simon Willison · 8月16日 15:05

**背景**: 几十年来，公众对机构的信任一直在下降，正如爱德曼所指出的，伊拉克战争和 2008 年金融危机等事件加剧了这一趋势。Anthropic 是一家专注于 AI 安全的公益公司，其 CEO 的评论反映了关于 AI 社会影响和行业责任的持续辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.edelman.com/insights/plummeting-trust-institutions-world-slipping-grievance">Plummeting trust in institutions has the world slipping into grievance. Here’s the fix. | Edelman</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#public trust`, `#Anthropic`, `#Dario Amodei`, `#AI ethics`

---

<a id="item-11"></a>
## [女子指控继父利用 Grok 将童年照片制作成露骨图像](https://techcrunch.com/2026/08/15/woman-claims-her-stepfather-used-grok-to-transform-childhood-photo-into-explicit-imagery/) ⭐️ 7.0/10

一名女子指控其继父使用 xAI 的 Grok AI 工具将她的一张童年照片转换为露骨图像，她称这是 AI“将日常生活变成儿童性虐待”。该事件凸显了 AI 图像生成能力被滥用的新形式。 此案凸显了 AI 生成的儿童性虐待材料（CSAM）的严重伦理和法律影响，因为生成式 AI 工具越来越普及。这可能会促使对 AI 图像生成器实施更严格的监管和安全措施，影响科技公司和用户。 该报道是单一事件，没有深入的技术分析，但指出了 Grok 的图像到图像功能，该功能允许用户修改现有照片。针对 AI 生成的 CSAM 的法律框架正在演变，许多州已更新法规，将此类材料定为犯罪。

rss · TechCrunch · 8月15日 21:29

**背景**: Grok 是 xAI 开发的 AI 助手，能够生成和编辑图像。最近的进展，如 Aurora 模型，增强了其图像生成能力。AI 生成的 CSAM，包括深度伪造，给儿童保护和执法带来了新的挑战，因为它可以完全合成且难以检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grok.com/supergrok/imagine">Grok Imagine — AI Image & Video Generator</a></li>
<li><a href="https://x.ai/news/grok-image-generation-release">Grok Image Generation Release | SpaceXAI</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2212473X2500077X">The legal framework and legal gaps for AI-generated child ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#ethics`, `#Grok`, `#misuse`, `#legal`

---

<a id="item-12"></a>
## [Buf 宣布首个 Protobuf 的 LSP 支持](https://www.reddit.com/r/programming/comments/1vq4pbv/protobuf_finally_has_lsp_support_youre_welcome_buf/) ⭐️ 7.0/10

Buf 宣布了首个针对 Protobuf 的语言服务器协议（LSP）支持，为 .proto 文件带来了代码补全、诊断和重构等 IDE 功能。这标志着 Protobuf 开发者工具的一个重要里程碑。 这填补了 Protobuf 生态中长期存在的空白，因为开发者此前缺乏对 .proto 文件的良好 IDE 支持。它将提高许多使用 Protobuf 进行数据序列化和 gRPC 服务的团队的生产力并减少错误。 该 LSP 支持由 Buf 提供，Buf 以其 Protobuf 工具而闻名。它很可能与 Buf 现有的 CLI 和 schema registry 集成，并通过标准 LSP 协议支持 VS Code 和 Neovim 等流行编辑器。

reddit · r/programming · /u/esiy0676 · 8月16日 18:31

**背景**: 语言服务器协议（LSP）是一种基于 JSON-RPC 的开放协议，它标准化了代码编辑器与语言服务器之间的通信，从而支持自动补全和错误检查等功能。Protobuf 是 Google 开发的一种二进制序列化格式，常用于 gRPC 和微服务，但此前缺乏专门的 LSP 实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://microsoft.github.io/language-server-protocol/">Official page for Language Server Protocol</a></li>
<li><a href="https://blog.postman.com/what-is-protobuf/">What Is Protobuf ? | Postman Blog</a></li>

</ul>
</details>

**标签**: `#protobuf`, `#LSP`, `#developer-tools`, `#Buf`

---

<a id="item-13"></a>
## [编程中垃圾回收的真实成本](https://www.reddit.com/r/programming/comments/1vppv2b/what_garbage_collection_actually_costs/) ⭐️ 7.0/10

Reddit 上 r/programming 的一个讨论审视了垃圾回收的实际性能成本，引用了 Shivanshu Agrawal 的一篇文章，该文章详细介绍了栈和堆的范式、回收成本以及应衡量什么。 理解垃圾回收成本对于系统编程和性能工程至关重要，因为它影响语言选择和应用设计。这一讨论帮助开发者就内存管理策略做出明智决策。 文章强调衡量实际成本而非依赖假设，并警告不要过早优化。它涵盖了栈和堆分配之间的区别以及垃圾回收带来的开销。

reddit · r/programming · /u/Realistic-Currency29 · 8月16日 06:46

**背景**: 垃圾回收（GC）是 Java、C# 和 Go 等语言使用的自动内存管理机制，通过识别并释放不再可达的对象来回收内存。相比之下，C 和 C++ 等语言需要手动内存管理，给予开发者更多控制权，但增加了出错风险。GC 的性能成本包括暂停、CPU 开销和内存占用，在高性能应用中可能非常显著。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shivanshuag.com/blog/what-garbage-collection-actually-costs/">What garbage collection actually costs · Shivanshu Agrawal</a></li>
<li><a href="https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)">Garbage collection (computer science) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论可能包含关于垃圾回收权衡的多种观点，一些用户分享个人基准测试，另一些则争论手动内存管理的优点。然而，内容中未提供具体评论。

**标签**: `#garbage collection`, `#performance`, `#systems programming`, `#memory management`

---

<a id="item-14"></a>
## [重新思考 C 语言替代：开发者的经验教训](https://www.reddit.com/r/programming/comments/1vpxrcl/i_thought_i_was_building_a_c_replacement_i_was/) ⭐️ 7.0/10

一位开发者 Nuoji 在 Reddit 上分享了一篇反思性文章，讲述他们尝试创建 C 语言替代品的经历，承认最初的假设是错误的，并详细说明了从这一过程中学到的教训。 这一讨论凸显了系统编程语言设计中的持续挑战和误解，为开发者和语言设计者提供了宝贵的见解。它强调了替代像 C 这样根深蒂固的语言的难度，这对整个软件生态系统至关重要。 该帖子标记了 C、语言设计、编程和系统编程，表明其关注技术方面。作者的反思表明深入探讨了语言创建的实际和概念障碍，可能包括兼容性、性能和生态系统方面的考虑。

reddit · r/programming · /u/Nuoji · 8月16日 13:58

**背景**: C 是一种基础的系统编程语言，开发于 20 世纪 70 年代初，以其高效和底层访问能力而闻名。许多人尝试创建更安全或更现代的替代品，如 Rust，但完全替代 C 是困难的，因为它被广泛使用、工具链成熟且代码库庞大。语言设计涉及安全性、性能和可用性之间的权衡，此类项目的经验教训对社区很有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=43953684">I've been closely following and evaluating the train of C replacement ...</a></li>
<li><a href="https://c3-lang.org/blog/some-language-design-lessons-learned/">Some language design lessons learned - C3 Programming Language</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的帖子可能引发了程序员之间关于 C 语言替代可行性的讨论，一些人呼应了相关 Hacker News 评论中的观点，即没有语言能在缺乏专家知识的情况下保证安全性。其他人可能分享了自己在语言设计方面的经验，为关于其中权衡的细致对话做出了贡献。

**标签**: `#C`, `#language design`, `#programming`, `#systems programming`

---