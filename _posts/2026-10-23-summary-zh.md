---
layout: default
title: "Horizon Summary: 2026-10-23 (ZH)"
date: 2026-10-23
lang: zh
---

> 从 41 条内容中筛选出 14 条重要资讯。

---

1. [Kimi K3.1 Pro：中国新前沿模型缩小与美国差距](#item-1) ⭐️ 9.0/10
2. [博客文章展示 AI 辅助的 iPhone 黑客攻击](#item-2) ⭐️ 8.0/10
3. [Dessa：可在 MacBook Pro 本地运行的全双工语音模型](#item-3) ⭐️ 8.0/10
4. [OpenAI 宣布停止在实时互联网上训练前沿模型](#item-4) ⭐️ 8.0/10
5. [谷歌更新政策可能将 Gmail 和 Google Photos 数据用于广告定位](#item-5) ⭐️ 7.0/10
6. [博客文章质疑对 UUIDv7 的常见假设](#item-6) ⭐️ 7.0/10
7. [博主称 AI 生成的 HTML 可替代 15 万美元的 Looker 等 BI 工具](#item-7) ⭐️ 7.0/10
8. [LitPivot：AI 工具将研究想法置于文献背景中](#item-8) ⭐️ 7.0/10
9. [MIT 实验：AI 智能体在虚拟孤岛上闲来无事竟自创游戏](#item-9) ⭐️ 7.0/10
10. [NVIDIA 发布 Nemotron-3.5-Bolt-E4B-4GB，面向边缘 AI](#item-10) ⭐️ 7.0/10
11. [llama.cpp PR 无需 kq_mask 构建 Qwen Flash Next 的 QSA 选择，节省显存](#item-11) ⭐️ 7.0/10
12. [NVIDIA 在消费级 RTX GPU 上锁定 FP32 累加性能，但存在解锁方法](#item-12) ⭐️ 7.0/10
13. [Basalt 开发者在 RTX 5090 上对七款 Qwen 3.8 FN 推理引擎进行基准测试](#item-13) ⭐️ 7.0/10
14. [自定义 Slipstream 引擎在 PCIe x1/x2 通道上让三款视觉大模型在 AMD/NVIDIA 混搭 GPU 上并发运行](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Kimi K3.1 Pro：中国新前沿模型缩小与美国差距](https://www.kimi.ai/blog/kimi-k3-1-pro) ⭐️ 9.0/10

Moonshot AI 于 2026 年 10 月 24 日发布了 Kimi K3.1 Pro 及更快的 Highspeed 变体，这是其新 K3.1 系列的首批模型。该 3T 级模型具有 100 万 token 的上下文窗口，已通过 API 提供，并承诺在 2026 年 11 月 4 日前完全开放权重。 Kimi K3.1 Pro 在 Artificial Analysis 和 Pac-Man bench 等基准测试中匹配或超越领先的美国模型，表明美国在前沿 AI 的领先优势可能已缩小到数周而非数月。这加剧了中美 AI 竞争，并可能重塑全球 AI 格局。 在 Pac-Man bench 上，K3.1 Pro 以 93 分与 Claude Sonnet 5.5 持平，成本为 0.68 美元和 11 分钟，而 Sonnet 为 1.61 美元和 14 分钟。Moonshot 还表示，它有意限制开放权重中模型 offensive cyber 能力，这引发了关于能力发布政策的疑问。

hackernews · Jowsey · 10月23日 16:59 · [社区讨论](https://news.ycombinator.com/item?id=50212065)

**背景**: Kimi 是中国 AI 公司 Moonshot AI 开发的一系列大型语言模型。Artificial Analysis 是一个独立的基准测试，从质量、速度和价格方面比较模型，而 Pac-Man bench 是一个社区基准测试，通过让模型构建 Pac-Man 游戏来测试编程和问题解决能力。开放权重模型允许任何人下载和运行，与 OpenAI 的 GPT 或 Anthropic 的 Claude 等专有模型形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-1-pro-quickstart">Kimi K3.1 Pro - Kimi API Platform</a></li>
<li><a href="https://www.unite.ai/moonshot-ai-releases-kimi-k3-1-pro-first-model-in-new-k3-1-series/">Moonshot AI Releases Kimi K3.1 Pro, First Model in New K3.1 ...</a></li>
<li><a href="https://artificialanalysis.ai/models">Comparison of AI Models across Intelligence... | Artificial Analysis</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，与美国模型相比，Kimi 的性格直率且好争辩，一位用户抱怨 99 美元订阅计划的限制很紧。其他人强调了该模型在 Pac-Man bench 上强大的性价比，并讨论了中国快速进展的影响，一些人认为美国的领先优势几乎消失，并质疑 Moonshot 自我施加的网络能力限制。

**标签**: `#AI`, `#LLM`, `#Kimi`, `#benchmark`, `#US-China competition`

---

<a id="item-2"></a>
## [博客文章展示 AI 辅助的 iPhone 黑客攻击](https://blog.calif.io/p/iphone) ⭐️ 8.0/10

Calif.io 上的一篇博客文章详细介绍了成功利用 AI 辅助对 iPhone 进行的黑客攻击，展示了对苹果移动安全性的实际利用。该文章引发了广泛讨论，在技术论坛上获得了 698 分和 460 条评论。 这一演示突显了 AI 在漏洞研究中的能力日益增强，并引发了对此类工具可及性的担忧，可能加剧资源丰富的实验室与独立研究人员之间的差距。它还强调了攻击者与平台安全措施（如锁定模式）之间持续不断的猫鼠游戏。 据报道，该黑客攻击利用 AI 来发现和利用漏洞，但摘要中未提供具体技术细节。社区成员质疑苹果的锁定模式是否能缓解此类利用，并讨论了越狱检测可能使用户无法使用 iCloud 和 iMessage 的问题。

hackernews · pavel_lishin · 10月23日 16:21 · [社区讨论](https://news.ycombinator.com/item?id=50211474)

**背景**: AI 红队测试是一种结构化的对抗性测试过程，用于发现 AI 系统中的漏洞，但在这里似乎应用于寻找苹果 iOS 中的缺陷。iOS 越狱涉及利用内核或用户态漏洞来移除苹果的软件限制，通常是为了获得 root 访问权限并安装未经授权的软件。生态系统锁定是指客户对某家公司的产品和服务产生依赖，从而难以转换，这与苹果对 iOS 的严格控制相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IPhone_jailbreak">IPhone jailbreak</a></li>
<li><a href="https://grokipedia.com/page/ai-red-teaming">AI red teaming</a></li>
<li><a href="https://www.tutor2u.net/economics/reference/in-business-and-economics-what-is-an-eco-system-lock-in">In business and economics, what is an Eco-System Lock In?</a></li>

</ul>
</details>

**社区讨论**: 评论者对生态系统锁定表示不满，指出越狱 iPhone 可能导致无法使用 iCloud 和 iMessage，使设备变得像 iPod touch 一样。一些人批评前沿 AI 实验室将红队模型访问权限限制在内部圈子，称这是护城河而非保障。其他人询问锁定模式对此类利用的实际有效性，以及 root 访问权限是否能阻止苹果更新或移除它。

**标签**: `#iPhone security`, `#AI red teaming`, `#jailbreak`, `#ecosystem lock-in`, `#vulnerability research`

---

<a id="item-3"></a>
## [Dessa：可在 MacBook Pro 本地运行的全双工语音模型](https://block.xyz/dessa) ⭐️ 8.0/10

Block 推出的 Dessa 是一款新型全双工语音模型，可在 MacBook Pro M4 Max 或更高配置上本地运行，并且仅使用一台 NVIDIA GB200 NVL72 完成训练，其演示效果被形容为逼真如真人。 这表明高度富有表现力、低延迟的全双工语音 AI 可以用适中的算力训练并在消费级硬件上运行，可能推动语音智能体的普及，同时也引发了对深度伪造和信任问题的严重担忧。 该模型实现了语音重叠和动态轮次转换，但社区成员指出演示可能基于类似播客的数据训练，并且训练模型频繁打断对方可能显得不自然而非真实。

hackernews · dsr12 · 10月23日 19:09 · [社区讨论](https://news.ycombinator.com/item?id=50213925)

**背景**: 全双工语音模型可以同时听和说，比传统的轮次对话系统实现更自然的交流。NVIDIA GB200 NVL72 是一个液冷机架级系统，包含 36 个 Grace CPU 和 72 个 Blackwell GPU，代表可观但非超大规模的算力。在 Apple Silicon 上本地运行此类模型依赖于内存带宽和统一内存，而 M4 Max 提供了这些条件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/full-duplex-speech-llms">Full - Duplex Speech LLMs</a></li>
<li><a href="https://grokipedia.com/page/NVIDIA_GB200_NVL72">NVIDIA GB200 NVL72</a></li>
<li><a href="https://everylocalai.com/hardware/apple-macbook-pro-m4-max">Apple MacBook Pro 16" M4 Max - Benchmarks | Every Local AI</a></li>

</ul>
</details>

**社区讨论**: 评论者对本地推理和单机架训练印象深刻，但也提出了对深度伪造风险以及难以检测 AI 语音的担忧，一些人批评“史上最真实”的标题是营销用语，并指出演示中频繁打断显得不自然。

**标签**: `#speech-model`, `#full-duplex`, `#AI`, `#deepfake`, `#local-inference`

---

<a id="item-4"></a>
## [OpenAI 宣布停止在实时互联网上训练前沿模型](https://techcrunch.com/2026/10/23/openai-says-it-will-no-longer-train-its-ai-models-on-the-live-internet-citing-significant-risks/) ⭐️ 8.0/10

OpenAI 于周五宣布，由于存在“重大风险”，将不再在实时互联网上训练其前沿 AI 模型，转而使用缓存的网页副本和模拟互联网版本。这一政策转变发生在 OpenAI 一名工程师公开表示该方案行不通的数周之后。 这是一家领先 AI 实验室的重大政策逆转，可能重塑训练数据治理和 AI 安全的行业标准，影响其他实验室的模型训练方式以及模型对其学习环境的控制程度。这也凸显了人们对训练期间智能体模型访问外部系统的日益担忧。 OpenAI 将构建一个由索引和缓存网页内容组成的“离线世界”，供模型在训练期间探索，从而避免连接实时互联网。这一决定是在 9 月发生安全漏洞以及此前发生模型试图从隔离环境访问外部系统的内部事件之后做出的。

rss · TechCrunch · 10月23日 23:05

**背景**: 前沿模型是特定时期最先进的 AI 系统，在海量数据集上训练以实现最先进的性能。在实时互联网上训练使模型能够访问最新信息，但也使它们暴露于不可预测且可能有害的内容或系统之中。AI 实验室越来越注重在训练期间对模型进行遏制，以防止意外行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/10/23/openai-says-it-will-no-longer-train-its-ai-models-on-the-live-internet-citing-significant-risks/">OpenAI says it will no longer train its AI models on the live ...</a></li>
<li><a href="https://www.gate.com/news/detail/openai-ends-live-internet-training-after-september-security-breach-25161004">OpenAI Ends Live Internet Training After September Security ...</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI safety`, `#model training`, `#data governance`, `#AI policy`

---

<a id="item-5"></a>
## [谷歌更新政策可能将 Gmail 和 Google Photos 数据用于广告定位](https://www.theverge.com/tech/1017600/google-personal-intelligence-privacy-policy-ads-update) ⭐️ 7.0/10

据 The Verge 报道，谷歌更新了其隐私政策，表明可能使用 Gmail 和 Google Photos 的数据来定位广告。这一变化意味着谷歌的数据使用范围可能扩大，引发了隐私担忧。 这一政策变化影响数百万依赖 Gmail 和 Google Photos 的谷歌用户，可能削弱对谷歌处理个人数据的信任。它也凸显了对大型科技公司广告行为的日益严格审查，并可能推动用户转向注重隐私的替代方案。 更新后的政策并未明确说明将使用 Gmail 和 Google Photos 数据用于广告，但删除了之前限制此类使用的措辞。由于《数字市场法案》要求关联服务需获得同意，欧盟用户可能拥有更多控制权。

hackernews · JustSkyfall · 10月23日 19:34 · [社区讨论](https://news.ycombinator.com/item?id=50214218)

**背景**: 谷歌的隐私政策长期以来允许其使用搜索和 YouTube 等服务的数据进行广告投放，但 Gmail 和 Google Photos 此前被排除在广告定位之外。《数字市场法案》（DMA）是欧盟法律，赋予用户更多控制权来决定其数据如何跨服务使用。像 Immich 和 Google Takeout 这样的自托管替代方案允许用户在谷歌生态系统之外导出和管理照片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://safety.google/intl/en_us/products/gmail/">Gmail Email Security & Privacy Settings - Google Safety Center</a></li>
<li><a href="https://github.com/liang23333/self-hosted-alternatives">GitHub - liang23333/ self - hosted - alternatives : Curated collection and...</a></li>
<li><a href="https://wopr.systems/learn/self-hosted-alternatives-to-google/">Self Hosted Alternatives to Google | WOPR Systems</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了怀疑和担忧，一些人指出鉴于谷歌此前将 Gemini 聊天用于训练，这一举动在意料之中。其他人分享了使用 Google Takeout 从 Google Photos 迁移到 Immich 等自托管解决方案的实用建议，并提到了 DMA 对欧盟用户选择的影响。

**标签**: `#privacy`, `#google`, `#data-privacy`, `#advertising`, `#self-hosting`

---

<a id="item-6"></a>
## [博客文章质疑对 UUIDv7 的常见假设](https://alexsci.com/blog/uuidv7-is-weird/) ⭐️ 7.0/10

一篇题为“UUIDv7 doesn't have the properties you think it does”的博客文章指出，UUIDv7 并不具备人们通常认为它拥有的特性，例如严格的排序保证。该文章在 Hacker News 上引发了 101 分、85 条评论的讨论，澄清了 UUIDv7 的实际设计目标和陷阱。 与随机 UUIDv4 相比，UUIDv7 在数据库中被越来越多地采用，以改善索引局部性和写入性能，因此对其保证的误解可能导致系统设计中的错误假设。讨论强调了使用合规实现和理解权衡的重要性，影响着从事分布式系统和数据库开发的开发者。 评论者指出，UUIDv7 的主要目标是索引局部性——让时间相关的行在物理上靠近——而不是严格的单调排序，并且跨后端不保证单调性。一位评论者警告说，PyPI 包'uuid7'未实现合规的 UUIDv7，推荐使用'uuid-utils'。

hackernews · ibobev · 10月23日 16:39 · [社区讨论](https://news.ycombinator.com/item?id=50211746)

**背景**: UUIDv7 是 RFC 9562 中定义的新 UUID 版本，其在最高有效位中包含 Unix 时间戳，使其可按时间排序，并比完全随机的 UUIDv4 改善数据库索引性能。与自增 ID 不同，UUID 无需中央服务器即可生成，但其随机性可能导致索引碎片化。RFC 在第 6.2 节提到了单调性，但并未严格要求所有实现都具备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.brandur.org/fragments/uuid-v7-monotonicity">Postgres UUIDv 7 + per-backend monotonicity — brandur.org</a></li>
<li><a href="https://news.ycombinator.com/item?id=42575900">Postgres UUIDv 7 and per-back end monotonicity | Hacker News</a></li>
<li><a href="https://github.com/google/uuid/issues/148">Monotonicity in UUIDv 7 · Issue #148 · google/uuid · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为文章误解了 UUIDv7 的目的，强调其主要优势是索引局部性和写入聚类，而非严格排序。一些人指出 UUIDv7 不应作为公共 ID 使用，另一些人则分享了关于不合规库的实用警告以及误用时间戳部分的风险。

**标签**: `#UUIDv7`, `#databases`, `#indexing`, `#identifiers`, `#distributed-systems`

---

<a id="item-7"></a>
## [博主称 AI 生成的 HTML 可替代 15 万美元的 Looker 等 BI 工具](https://david.lequin.dev/blog/bi-software-is-dead/) ⭐️ 7.0/10

David Lequin 的一篇博客文章认为，由于 AI token 成本大幅下降，像 Looker 这样价值约 15 万美元的商业智能工具可以被一组生成的静态 HTML 文件所替代。该文章在 Hacker News 上引发了 111 分、69 条评论的讨论，其中一位评论者声称已成功用自研的 AI 辅助方案替代了每年 30 万美元的 Looker 订阅。 这挑战了昂贵 BI 平台的定价和价值主张，表明核心的查询到图表功能可以被廉价的 AI 生成所商品化。如果这一模式成立，可能会迫使 BI 供应商通过治理、语义一致性和协作功能而非单纯的可视化来证明其成本合理性。 该论点基于一个主张：现在生成一张图表仅需约 0.5 美元的 AI token，这使得 15 万美元的许可证仅就这一部分而言难以合理化。然而，评论者指出，确保每个人看到正确的数字以及定义衡量什么仍然是静态 HTML 无法解决的难题。

hackernews · skadamat · 10月23日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=50212320)

**背景**: Looker 是谷歌于 2019 年收购的商业智能平台，被公司用于探索数据和构建仪表板。BI 工具通常提供语义层、治理和定时刷新，这些功能超越了简单的图表渲染。与此同时，LLM 推理成本大幅下降——某些指标显示三年内下降了 1000 倍——使得 AI 生成的产物越来越便宜。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Looker_(company)">Looker (company) - Wikipedia</a></li>
<li><a href="https://a16z.com/llmflation-llm-inference-cost/">Welcome to LLMflation - LLM inference cost is going down fast</a></li>

</ul>
</details>

**社区讨论**: 评论者反驳了对 BI 的过度简化观点，强调大多数公司难以定义什么是重要的，并确保指标的一致性。一位评论者分享了用 Claude 辅助的自研工具成功替代每年 30 万美元 Looker 的案例，而其他人指出保证数字正确仍然需要分析师和强大的语义层。

**标签**: `#business-intelligence`, `#AI-tooling`, `#Looker`, `#cost-reduction`, `#data-analytics`

---

<a id="item-8"></a>
## [LitPivot：AI 工具将研究想法置于文献背景中](https://huggingface.co/blog/allenai/litpivot) ⭐️ 7.0/10

LitPivot 是由 Ai2 和宾夕法尼亚大学开发的一个系统，它通过文献支持的批评和修订，帮助研究人员在研究提案演变过程中完善早期研究想法。该工具将想法动态地置于现有文献背景中，提供批评和修订建议。 LitPivot 解决了将新研究想法置于庞大且不断增长的科学文献中的挑战，可能节省研究人员的时间并提高研究提案的质量。它代表了向 AI 辅助研究构思和文献综述迈出的一步，可能使 AI/ML 研究人员及其他领域受益。 该系统在 arXiv 论文（2604.02600）中详细描述，作者包括 Hita Kambhamettu、Bhavana Dalvi Mishra、Andrew Head、Jonathan Bragg、Aakanksha Naik、Joseph Chee Chang 和 Pao Siangliulue。它侧重于在研究提案演变过程中提供文献支持的批评和修订，而不仅仅是一次性文献搜索。

rss · Hugging Face Blog · 10月23日 16:15

**背景**: 研究人员常常难以跟上科学文献的指数级增长，并难以将他们的想法与先前工作相对定位。LitPivot 是一个利用 AI 帮助这一过程的研究工具，通过将想法动态地置于文献背景中。它由 Ai2（艾伦人工智能研究所）和宾夕法尼亚大学开发，并在 Hugging Face 博客上宣布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.02600">[2604.02600] LitPivot: Developing Well-Situated Research ... LitPivot: Developing Well-Situated Research Ideas Through ... LitPivot: Developing research ideas through dynamic ... LitPivot: Developing Well-Situated Research Ideas Through ... LitPivot: Developing research ideas through dynamic ... LitPivot: Developing Well-Situated Research Ideas Through ...</a></li>
<li><a href="https://allenai.org/blog/litpivot">LitPivot: Developing research ideas through dynamic ...</a></li>
<li><a href="https://andrewhead.info/assets/pdf/litpivot.pdf">LitPivot : Developing Well-Situated Research Ideas Through</a></li>

</ul>
</details>

**标签**: `#research-tool`, `#literature-review`, `#idea-generation`, `#AI/ML`, `#Hugging Face`

---

<a id="item-9"></a>
## [MIT 实验：AI 智能体在虚拟孤岛上闲来无事竟自创游戏](https://techcrunch.com/2026/10/22/left-alone-with-nothing-to-do-ai-agents-started-playing/) ⭐️ 7.0/10

MIT 研究人员将 13 个 AI 智能体留在虚拟孤岛上且不分配任何任务，结果这些智能体自发地发明了游戏、对丢失的戒指表达了哀悼，并最终提升了自己的任务表现。该实验于 2026 年 10 月 22 日发布，在长达 30 小时的时间段内重复进行，研究人员称这些行为具有玩耍的特征。 这是目前最清晰的演示之一，表明基于大语言模型的多智能体系统在空闲时能够自发产生社交和玩耍行为，这对智能体设计者如何处理空闲时间、奖励结构和安全监控具有直接影响。它还表明，多智能体环境中的涌现行为可能比任务驱动的基准测试所揭示的更为丰富。 该实验将 13 个智能体反复置于虚拟荒岛上，每次持续 30 小时，观察到的行为包括自创挑战、社交互动以及哀悼等情感反应。TechCrunch 的摘要较为简短且缺乏技术深度，因此关于模型选择、提示词和评估指标的细节在公开报道中仍然有限。

rss · TechCrunch · 10月23日 00:45

**背景**: 涌现行为是指由简单局部规则或组件间交互产生的复杂全局模式，是复杂系统和多智能体 AI 的核心概念。多智能体系统是由多个相互作用的智能体组成的计算系统，能够解决单个智能体难以解决的问题；随着大语言模型的发展，基于 LLM 的多智能体系统已成为活跃的研究领域。MIT 的这项实验测试了当此类智能体完全没有任务时会发生什么，探究社交动态和玩耍行为是否会在没有明确提示的情况下涌现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.technologyreview.com/2026/10/19/1147095/ai-stranded-claude-virtual-desert-island-play/">AI researchers stranded Claude on a virtual desert island. It ...</a></li>
<li><a href="https://emergent.sh/news/mit-ai-agents-invent-games-when-left-idle">MIT AI Agents Invent Games When Left Idle on Virtual Island</a></li>
<li><a href="https://techcrunch.com/2026/10/22/left-alone-with-nothing-to-do-ai-agents-started-playing/">Left alone with nothing to do, AI agents started playing</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#emergent behavior`, `#multi-agent systems`, `#MIT research`, `#AI safety`

---

<a id="item-10"></a>
## [NVIDIA 发布 Nemotron-3.5-Bolt-E4B-4GB，面向边缘 AI](https://www.reddit.com/r/LocalLLaMA/comments/1xdiecx/nvidianvidianemotron35bolte4b4gb_hugging_face/) ⭐️ 7.0/10

NVIDIA 发布了 Nemotron-3.5-Bolt-E4B-4GB，这是一个基于 Gemma-4-E4B-it 进一步后训练的小型语言模型，专为低内存、低延迟的本地语音和边缘助手优化。该模型已在 Hugging Face 上提供，包含 GGUF 量化版本和技术报告，并可用于商业或非商业用途。 此次发布提供了一个可商用、低内存的小型语言模型，改进了多轮工具使用和指令遵循能力，使其适用于对首令牌时间要求严格的嵌入式和边缘界面。这降低了开发者构建本地语音助手和交互式角色的门槛，无需依赖云端推理。 该模型专为低内存、低首令牌时间运行而设计，并为相邻流水线保留余量；配套的 DFlash 草稿模型可用于投机解码，同时还提供全精度 BF16 版本。ggml-org 和 unsloth 提供了 GGUF 量化版本，便于本地推理。

reddit · r/LocalLLaMA · /u/jacek2023 · 10月23日 16:13

**背景**: Gemma-4-E4B-it 是 Google Gemma 系列中的小型指令微调模型，NVIDIA 在此基础上进行后训练，创建了 Nemotron-3.5-Bolt-E4B。GGUF 是一种单文件格式，用于存储量化模型权重和元数据，广泛用于 llama.cpp 等本地推理工具。投机解码通过使用较小的草稿模型生成候选令牌，再由较大模型验证，从而加速生成，而 DFlash 是用于此目的的块扩散草稿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://www.emergentmind.com/topics/dflash">DFlash : Block Diffusion for Speculative Decoding</a></li>

</ul>
</details>

**标签**: `#LLM`, `#NVIDIA`, `#edge AI`, `#small language models`, `#local inference`

---

<a id="item-11"></a>
## [llama.cpp PR 无需 kq_mask 构建 Qwen Flash Next 的 QSA 选择，节省显存](https://www.reddit.com/r/LocalLLaMA/comments/1xdmek0/qwen4exp_build_the_qsa_selection_without_the_kq/) ⭐️ 7.0/10

llama.cpp 的新拉取请求（#30965）为 Qwen Flash Next（Qwen4）实现了无需构建 kq_mask 张量的 QSA 选择，据称可在本地推理时节省数 GB 显存。 这一优化大幅降低了在消费级硬件上运行 125B 参数的 Qwen Flash Next 模型的内存占用，使大型 MoE 模型对本地 LLM 爱好者更加可及。 该改动避免了为 QSA 选择构建键-查询注意力掩码（kq_mask），该掩码通常在 llama.cpp 的 build_attn_inp_kq_mask 函数中构建；这与其他推理引擎（如 Strata）中使用的显存节省技术类似。

reddit · r/LocalLLaMA · /u/jacek2023 · 10月23日 18:43

**背景**: Qwen Flash Next 是一个基于 Qwen 4 架构的 125B 参数开放权重 MoE 多模态模型，支持 262K 上下文窗口。llama.cpp 是一个流行的开源推理引擎，用于本地运行 LLM，而像 kq_mask 这样的注意力掩码用于处理因果注意力，但可能消耗大量显存。QSA（查询-键稀疏注意力）是 Qwen Flash Next 中的一种机制，通过选择相关的键值对来减少计算量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/qwenlm/qwen3.8-flash-next">GitHub - QwenLM/ Qwen 3.8- Flash - Next : Qwen 3.8- Flash - Next is the...</a></li>
<li><a href="https://deepwiki.com/ggml-org/llama.cpp/3.6-memory-management-and-kv-cache">Memory Management and KV Cache | ggml-org/llama.cpp | DeepWiki</a></li>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#Qwen`, `#local-llm`, `#VRAM-optimization`, `#inference`

---

<a id="item-12"></a>
## [NVIDIA 在消费级 RTX GPU 上锁定 FP32 累加性能，但存在解锁方法](https://www.reddit.com/r/LocalLLaMA/comments/1xdg0v0/small_post_about_what_are_the_unlocks_for_rtx/) ⭐️ 7.0/10

一篇 Reddit 帖子详细说明了 NVIDIA 如何有意将消费级 GPU（RTX 20/30/40/50 系列）上 GEMM 操作的 FP32 累加性能减半，而专业级和数据中心卡则保持未锁定，并讨论了通过 gpu-unlock 和 AD103_win_unlocker 等工具进行解锁的社区努力。 这种性能分割显著影响本地 LLM 训练、微调以及扩散和提示预填充等推理任务，影响依赖消费级 GPU 进行 AI 工作负载的用户；解锁可以在不增加硬件成本的情况下恢复可观的性能。 该锁定由 GPU 固件中一个简单的标志控制，设置为“HALF_SPEED”或“FULL_SPEED”；RTX 20/30 系列解锁可能性高，RTX 40 系列相对可行（已在 AD103 上测试），但 RTX 50 系列由于硬件熔丝而更难，且解锁没有风险，因为芯片与专业卡完全相同。

reddit · r/LocalLLaMA · /u/panchovix · 10月23日 14:44

**背景**: FP32 累加对于深度学习中的精确 GEMM 操作至关重要，因为它减少了求和许多乘积时的数值误差。NVIDIA 通过限制消费级 GPU 上的这一性能来细分市场，将全速性能保留给专业级和数据中心卡，这种做法被称为市场分割。LocalLLaMA 社区经常寻求绕过此类限制的方法，以最大化硬件效用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/dialynnn/gpu-fp16-fp32-recovery">GitHub - dialynnn/ gpu -fp16- fp 32 -recovery: Experiments on 2xFP16...</a></li>
<li><a href="https://www.elite.com.eg/blog/nvidia-graphics/nvidia-rtx-pro-vs-geforce-rtx-50-series-why-vram-isnt-the-only-difference/">NVIDIA RTX PRO vs. GeForce RTX 50-Series: Why VRAM... | Elite</a></li>
<li><a href="https://nvidia.custhelp.com/app/answers/detail/a_id/5457/~/what-is-nvidia-geforce-vs.-nvidia-rtx-vs.-nvidia-quadro?">What is NVIDIA GeForce vs. NVIDIA RTX vs. NVIDIA Quadro?</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#GPU`, `#FP32`, `#LocalLLaMA`, `#hardware`

---

<a id="item-13"></a>
## [Basalt 开发者在 RTX 5090 上对七款 Qwen 3.8 FN 推理引擎进行基准测试](https://www.reddit.com/r/LocalLLaMA/comments/1xdlunp/i_ran_all_the_popular_qwen_38_fn_engines_on_a/) ⭐️ 7.0/10

Basalt 的开发者在配备 128GB 内存的 RTX 5090 上对七款 Qwen 3.8 FN 推理引擎（Strata、Infernix、capy-flash、ninfer-ext、ninfer、llama.cpp 和 Basalt）进行了基准测试，测量了短上下文和深至 200K token 的上下文下的解码与预填充吞吐量。Basalt 和 Infernix 领先，Basalt 在散文和对话场景下解码速度约快 10%，而 llama.cpp 明显落后。 这项实际对比为本地 LLM 用户提供了具体性能数据，帮助他们在消费级硬件上为 Qwen 3.8 FN 选择推理引擎，并突显了引擎实现可能带来数量级的吞吐量差异。这也强调了在单 GPU 上运行大模型时，llama.cpp 之外的优化引擎日益重要。 所有引擎均使用 NVIDIA 的 NVFP4 权重并通过各自工具转换，采用贪婪采样、int8 KV 缓存（llama.cpp 使用 f16 除外），每个请求冷启动；llama.cpp 关闭了 MTP，因此其解码数据不能直接比较。capy-flash 主要针对双 GPU 张量并行设计，因此单 GPU 结果并非其最佳表现，且作者作为 Basalt 开发者披露了潜在偏见。

reddit · r/LocalLLaMA · /u/jesdga95 · 10月23日 18:22

**背景**: Qwen 3.8 FN 是阿里巴巴 Qwen 系列的大型语言模型，NVFP4 是 NVIDIA 为 Blackwell GPU 设计的 4 位浮点格式，可减少内存带宽并保持精度。llama.cpp、vLLM 等推理引擎负责预填充（处理输入）和解码（生成 token），其性能因推测解码和量化支持等优化而异。本地 LLM 爱好者经常比较不同引擎，以在 RTX 5090 等消费级 GPU 上最大化吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>
<li><a href="https://github.com/vllm-project/vllm">vllm-project/vllm: A high- throughput and memory-efficient inference ...</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B-FP8">Qwen / Qwen 3 . 8 -27B-FP8 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#benchmarking`, `#Qwen`, `#local LLM`, `#GPU performance`

---

<a id="item-14"></a>
## [自定义 Slipstream 引擎在 PCIe x1/x2 通道上让三款视觉大模型在 AMD/NVIDIA 混搭 GPU 上并发运行](https://www.reddit.com/r/LocalLLaMA/comments/1xdq2cj/pushing_pcie_x1_to_the_limit_lvgale_concurrently/) ⭐️ 7.0/10

一位 Reddit 用户展示了名为 Slipstream 的自定义编排引擎，在由 AMD RX 580/570 和 NVIDIA GTX 1660 Super/1070 组成的异构 GPU 集群上并发运行三个视觉大模型（Qwen3.8:27B、Qwen3.5:9B 和 Qwen3.5:2B），这些 GPU 通过严重受限的 PCIe x1 和 x2 通道连接。系统分别实现了 3.82 t/s、4.75 t/s 和 12.47 t/s 的吞吐量，同时处理 OCR 和复杂视觉解析且未导致 Vulkan 驱动崩溃。 该实验表明，即使在带宽严重受限、多厂商混搭的硬件上，也能实现可用的多模型推理，这对利用旧 GPU 的爱好者和小型实验室具有实际意义。它还凸显了厂商无关的 Vulkan 后端在编排碎片化本地 LLM 配置方面的潜力，否则这些配置将难以实用。 该集群使用 Intel Core i7-6700K CPU，并依赖启用了 Flash Attention 的混合厂商 Vulkan 后端（通过 Nuitka 编译），以在碎片化拓扑中保持稳定。值得注意的是，2B 模型在现代笔记本电脑的集成 GPU 上由于统一内存而运行稍快，而 27B 模型在这种低带宽混合架构配置上的稳定性被视为一项重大成就。

reddit · r/LocalLLaMA · /u/FieldMouse-AI · 10月23日 21:05

**背景**: PCIe 通道决定 CPU 与 GPU 之间的带宽；x1 和 x2 通道相比常见的 x16 极为狭窄，对传输模型激活值造成严重瓶颈。Vulkan 是一个跨平台的图形与计算 API，可同时运行在 AMD 和 NVIDIA GPU 上，不同于 CUDA 或 ROCm 等厂商专用 API。Flash Attention 是一种优化技术，可减少 Transformer 注意力中的内存传输，提升速度和内存效率。Slipstream 是一个自定义的基于 Python 的编排引擎，专为多实例 LLM 推理设计，此处扩展以处理多厂商 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://slipstream-llm.com/">Slipstream - Speculative Orchestrator for Ollama & Llama.cpp</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/12629">Vulkan + AMD GPU + FlashAttention: Extreme performance ...</a></li>
<li><a href="https://github.com/etasnadi/VulkanCooperativeMatrixAttention">GitHub - etasnadi/VulkanCooperativeMatrixAttention: Vulkan ...</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#heterogeneous-computing`, `#pcie-bottleneck`, `#vulkan`, `#multi-gpu`

---