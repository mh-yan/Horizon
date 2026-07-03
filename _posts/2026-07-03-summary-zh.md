---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 40 条内容中筛选出 15 条重要资讯。

---

1. [调查间谍软件滥用的政客遭飞马间谍软件攻击](#item-1) ⭐️ 9.0/10
2. [Mistral 发布 Leanstral-1.5 形式验证模型](#item-2) ⭐️ 9.0/10
3. [llama.cpp 补丁让 DeepSeek V4 Flash 在 RTX 5090 上运行 1M 上下文](#item-3) ⭐️ 9.0/10
4. [Ubicloud 倡导对 PostgreSQL 使用严格内存过量提交](#item-4) ⭐️ 8.0/10
5. [Wordgard：ProseMirror 作者打造的新富文本编辑器](#item-5) ⭐️ 8.0/10
6. [螺旋蝇的衰落与复兴](#item-6) ⭐️ 8.0/10
7. [用户搭建 448GB 显存本地大模型极限配置](#item-7) ⭐️ 8.0/10
8. [本地运行 SOTA 大模型指南](#item-8) ⭐️ 7.0/10
9. [Costco 的反亚马逊策略：避开最后一公里配送](#item-9) ⭐️ 7.0/10
10. [Valve 开源 Steam Machine 电子墨水屏设计](#item-10) ⭐️ 7.0/10
11. [将代码转为图片再 OCR，LLM 成本降低 60%](#item-11) ⭐️ 7.0/10
12. [半成品：创业警示故事](#item-12) ⭐️ 7.0/10
13. [课程创作者报告收入因 AI 下降超 50%](#item-13) ⭐️ 7.0/10
14. [私人太空飞行员为美国太空部队执行轨道任务](#item-14) ⭐️ 7.0/10
15. [DeepSeek DSpark：推理速度提升高达 85%](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [调查间谍软件滥用的政客遭飞马间谍软件攻击](https://techcrunch.com/2026/07/02/politician-who-investigated-spyware-abuses-had-his-phone-hacked-with-pegasus-spyware/) ⭐️ 9.0/10

一名曾在欧盟委员会调查间谍软件行业的欧洲政客，其 iPhone 在 2022 年 10 月和 2023 年 3 月被 NSO 集团的一个政府客户使用飞马间谍软件感染。 这一事件凸显了间谍软件被用于对付调查者的讽刺，强调了商业监控工具对民主监督和隐私权构成的严重威胁。 公民实验室高度确信确认了感染，且攻击发生在该政客任职于调查间谍软件滥用的欧盟委员会期间。NSO 集团将飞马定位为打击犯罪和恐怖主义的工具，但该软件经常被用于监视记者、律师和活动人士。

rss · TechCrunch · 7月3日 05:05

**背景**: 飞马是由以色列公司 NSO 集团开发的复杂间谍软件，能够进行远程零点击监控，包括读取信息、跟踪位置以及访问麦克风和摄像头。它通常由政府客户部署用于高价值目标，其使用已在全球引发关于人权和隐私的争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/NSO_Group">NSO Group - Wikipedia</a></li>
<li><a href="https://www.theguardian.com/technology/2024/nov/14/nso-pegasus-spyware-whatsapp">NSO – not government clients – operates its spyware, legal documents reveal | Hacking | The Guardian</a></li>

</ul>
</details>

**社区讨论**: 评论者指出这是更广泛模式的一部分，有人提到希腊曾发生类似丑闻，政客遭飞马攻击，据称由总理办公室策划。另一评论者对游说者和美国公司对欧盟数据的影响表示怀疑。

**标签**: `#cybersecurity`, `#spyware`, `#NSO Group`, `#Pegasus`, `#surveillance`

---

<a id="item-2"></a>
## [Mistral 发布 Leanstral-1.5 形式验证模型](https://www.reddit.com/r/LocalLLaMA/comments/1umgdhx/mistral_released_leanstral15119ba6b/) ⭐️ 9.0/10

Mistral 发布了 Leanstral-1.5-119B-A6B 模型，该模型拥有 60 亿活跃参数，采用 Apache-2.0 许可证，在形式验证领域取得了最先进的结果：在 miniF2F 基准测试上达到饱和，解决了 PutnamBench 中 672 个问题中的 587 个，并在 FATE-H 和 FATE-X 上分别获得 87% 和 34% 的分数。 此次发布推动了自动定理证明和代码验证的发展，使开发者能够自动验证软件正确性并发现真实漏洞，该模型在 57 个开源仓库中发现了 5 个此前未知的 bug。 该模型通过中期训练、监督微调以及使用 CISPO（裁剪重要性采样策略优化）的强化学习进行训练，在智能体式证明工程和真实世界代码验证方面表现出色。

reddit · r/LocalLLaMA · /u/Tall-Ad-7742 · 7月3日 14:44

**背景**: 形式验证使用数学证明来确保软件正确性。miniF2F 和 PutnamBench 等基准测试用于评估 AI 解决形式数学问题的能力。CISPO 是一种强化学习算法，通过裁剪重要性采样权重来实现稳定训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/openai/miniF2F">openai/miniF2F: Formal to Formal Mathematics Benchmark - GitHub</a></li>
<li><a href="https://swift.readthedocs.io/en/latest/Instruction/GRPO/AdvancedResearch/CISPO.html">Clipped Importance Sampling Policy Optimization (CISPO) — swift 4.4.0.dev0 documentation</a></li>
<li><a href="https://huggingface.co/datasets/amitayusht/PutnamBench">amitayusht/ PutnamBench · Datasets at Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 该帖子的 Reddit 评论大多与 Leanstral-1.5 无关，讨论了 AMALIA 和 LongCat 等其他模型，以及一位用户使用 Qwen 27B 的经验。没有直接讨论 Leanstral-1.5 的内容。

**标签**: `#AI/ML`, `#formal verification`, `#theorem proving`, `#open-source`, `#Mistral`

---

<a id="item-3"></a>
## [llama.cpp 补丁让 DeepSeek V4 Flash 在 RTX 5090 上运行 1M 上下文](https://www.reddit.com/r/LocalLLaMA/comments/1ulymml/llamacpp_patch_deepseek_v4_flash_running_with/) ⭐️ 9.0/10

一个针对 llama.cpp 的自定义 CUDA 内核补丁使得 DeepSeek V4 Flash 能够在单张 RTX 5090 上运行完整的 100 万 token 上下文，将显存需求从约 256GB 降至约 31GB，并在 100 万上下文下达到 159 token/s 的预填充速度。 这一突破使得长上下文推理（高达 100 万 token）在消费级硬件上成为可能，极大降低了研究人员和开发者在本地实验最先进稀疏注意力模型的门槛。 该补丁为 DSA 闪电索引器实现了 CUDA 内核，此前 llama.cpp 中缺失该功能。它在 256K 上下文下达到 263 token/s 的预填充速度，在 1M 上下文下达到 159 token/s，1M 上下文时峰值显存使用约 31 GiB。

reddit · r/LocalLLaMA · /u/da_dragon321 · 7月2日 23:54

**背景**: DeepSeek V4 Flash 使用 DeepSeek 稀疏注意力（DSA）和闪电索引器来减少注意力计算。DSA 闪电索引器在 llama.cpp 中未得到适当支持，导致显存使用过高。此补丁将索引器接入模型图并添加了 CUDA 路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/lemyx/tilelang-dsa">DeepSeek-V3.2-Exp DSA Warmup Lightning Indexer training operator ...</a></li>
<li><a href="https://ninehills.github.io/jack-diary/articles/20260308-deepseek-dsa-analysis.html">20260308 / 稀疏的胜利：拆解 DeepSeek DSA 与 Lightning Indexer</a></li>

</ul>
</details>

**社区讨论**: 社区对这一成就感到兴奋，用户指出像 DeepSeek V4 Flash 这样的本地模型现在接近 Sonnet 质量，同时在挂钟时间上比基于 API 的模型更快。一些用户正在进行进一步基准测试并分享详细比较。

**标签**: `#llama.cpp`, `#DeepSeek`, `#CUDA`, `#LLM inference`, `#long context`

---

<a id="item-4"></a>
## [Ubicloud 倡导对 PostgreSQL 使用严格内存过量提交](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 发布了一篇博客文章，解释为何他们对 PostgreSQL 使用严格内存过量提交（vm.overcommit_memory=2），以防止 OOM 杀手终止数据库进程。文章详细说明了该设置如何避免内存压力下的系统不稳定。 这很重要，因为 PostgreSQL 是一个内存密集型数据库，在默认的过量提交设置下可能触发 Linux OOM 杀手，导致意外停机。采用严格过量提交可以提高可靠性，但该方法需要仔细的容量规划，并且可能不适用于所有工作负载。 严格过量提交（模式 2）会拒绝超过 CommitLimit 的分配，该限制通过 overcommit_kbytes 或 overcommit_ratio 设置。博客文章指出，如果内存紧张，此设置可能导致 fork() 调用失败，因此在生产部署前必须在 QA 环境中进行彻底测试。

hackernews · furkansahin · 7月3日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 内核使用内存过量提交来分配比物理 RAM 更多的虚拟内存，假设并非所有内存会同时被使用。当系统内存耗尽时，OOM 杀手会选择一个进程并终止它以释放内存。PostgreSQL 的内存密集型操作（如排序、哈希连接）在默认的启发式过量提交（模式 0）下可能触发 OOM 杀手，导致数据库崩溃。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://news.ycombinator.com/item?id=48774509">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit | Hacker News</a></li>
<li><a href="https://utcc.utoronto.ca/~cks/space/blog/linux/StrictOvercommitCanOOM">Chris's Wiki :: blog/linux/StrictOvercommitCanOOM</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了谨慎态度：一位用户警告模式 2 可能阻止 fork，并建议进行彻底测试。另一位用户分享了混合工作负载（Go 应用 + PostgreSQL）的经验，其中模式 2 导致了不稳定。博客作者（Ozgun）承认标题过于绝对，并指出严格过量提交在许多场景下可能产生未预料的副作用。

**标签**: `#PostgreSQL`, `#Linux`, `#memory management`, `#OOM killer`, `#database operations`

---

<a id="item-5"></a>
## [Wordgard：ProseMirror 作者打造的新富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

Wordgard 是 ProseMirror 作者 Marijn Haverbeke 发布的一款新的浏览器内富文本编辑器，提供了改进的设计、文档和开发者体验，作为现代替代方案。 这很重要，因为 ProseMirror 是 Tiptap 等编辑器的广泛使用的基础，而 Wordgard 旨在解决其陡峭的学习曲线和文档不足的问题，有可能成为基于 Web 的富文本编辑的新标准。 Wordgard 与 ProseMirror 共享许多概念，但并非直接替代品；没有升级路径，切换需要大量工作。该编辑器注重简洁设计和全面的文档。

hackernews · indy · 7月3日 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: ProseMirror 是一个久经考验的富文本编辑器框架，以其语义文档模型和高性能著称，但学习曲线陡峭且文档稀少。许多流行编辑器如 Tiptap 都基于 ProseMirror 构建。Wordgard 是同一作者的新项目，旨在提供更易用的替代方案，同时保留核心优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，用户称赞其设计和文档。一些人对新编辑器背后的“为什么”感兴趣，并指出缺乏从 ProseMirror 升级的路径。其他人分享了构建自定义编辑器的经验，并在 Wordgard 的方法中找到了验证。

**标签**: `#rich-text editor`, `#ProseMirror`, `#web development`, `#WYSIWYG`, `#open source`

---

<a id="item-6"></a>
## [螺旋蝇的衰落与复兴](https://www.construction-physics.com/p/the-fall-and-rise-of-screwworm) ⭐️ 8.0/10

一篇详细的历史记述，描述了利用昆虫不育技术（SIT）根除螺旋蝇的努力及其近期的失败，2026 年在南德克萨斯州确认了新病例。 昆虫不育技术涉及释放大量经辐射绝育的雄性苍蝇与野生雌性交配，从而减少繁殖。达连隘口的维护屏障多次失效，导致再次 infestation。

hackernews · crescit_eundo · 7月3日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=48774492)

**背景**: 新大陆螺旋蝇（Cochliomyia hominivorax）幼虫以温血动物（包括人类）的活体组织为食，若不治疗可能致命。美国农业部曾利用昆虫不育技术成功将其从美国和中美洲根除，但在巴拿马维持屏障已被证明具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aphis.usda.gov/sites/default/files/factsheet-eradicating-nws-sit.pdf">Eradicating New World Screwworm with Sterile Insect Technique</a></li>
<li><a href="https://www.aphis.usda.gov/sites/default/files/factsheet-sit-dispersal-methods.pdf">Sterile Fly Release Methods for Controlling Screwworm</a></li>
<li><a href="https://www.aphis.usda.gov/livestock-poultry-disease/cattle/ticks/screwworm">New World Screwworm Prevention for Animals</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了维持达连隘口屏障与全大陆根除的成本效益，并提出了对螺旋蝇种群产生辐射抗性选择的担忧。一些人赞扬了在资源有限的情况下历史性的根除努力。

**标签**: `#agriculture`, `#public health`, `#entomology`, `#science history`, `#pest control`

---

<a id="item-7"></a>
## [用户搭建 448GB 显存本地大模型极限配置](https://www.reddit.com/r/LocalLLaMA/comments/1umokhj/uh_honey_how_do_you_feel_about_takeout/) ⭐️ 8.0/10

一位 Reddit 用户分享了一台定制本地大模型设备，配备 448GB 显存，使用 AWQ-INT4 量化在 vLLM 上运行 MiniMax M3，批处理模式下达到约 960 tokens/秒。 这表明在足够硬件支持下，前沿模型的本地高吞吐推理是可行的，可能减少对云 API 的依赖，适用于隐私敏感或延迟关键的应用。 该设备组合了 2 块 RTX Pro 6000 Max-Q（96GB）、8 块 RTX 3090（24GB）和 2 块 RTX 5090（32GB），采用流水线并行（PP）结合张量并行（TP）组（每组 2 卡）。用户目标是实现 4 路并发和 1M 上下文长度。

reddit · r/LocalLLaMA · /u/MotorcyclesAndBizniz · 7月3日 20:02

**背景**: MiniMax M3 是一个开放权重的多模态 MoE 模型，支持 1M 上下文窗口，在编程和智能体任务上具有竞争力。AWQ-INT4 量化可将 GPU 内存减少约 50%，且精度损失极小。vLLM 是一个高吞吐推理引擎，支持分布式执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/models/text/m3">MiniMax M 3 - Coding & Agentic Frontier, 1M Context, Multimodal</a></li>
<li><a href="https://github.com/mit-han-lab/llm-awq">GitHub - mit-han-lab/llm-awq: [MLSys 2024 Best Paper Award ... Quantization Techniques for LLM Inference: INT8, INT4, GPTQ ... 4-Bit Quantization Decoded: INT4 QAT, MXFP4, and NVFP4 [2306.00978] AWQ: Activation-aware Weight Quantization for ... LLM Quantization Explained: INT8, INT4, GPTQ & AWQ</a></li>
<li><a href="https://github.com/vllm-project/vllm">GitHub - vllm-project/vllm: A high-throughput and memory-efficient ...</a></li>

</ul>
</details>

**社区讨论**: 社区以幽默和惊叹回应，调侃该配置对用户婚姻的影响以及高昂的电费。部分用户讨论了这种本地推理方案与云方案的实用性对比。

**标签**: `#LocalLLM`, `#Hardware`, `#Inference`, `#VRAM`, `#VLLM`

---

<a id="item-8"></a>
## [本地运行 SOTA 大模型指南](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob 在 GitHub 上发布了一份全面指南，详细介绍了如何在本地硬件上构建和运行最先进的大语言模型，包括具体的硬件物料清单和模型推荐。 该指南帮助爱好者和专业人士了解本地运行 LLM 的真实成本和性能权衡，这对隐私保护、离线使用以及避免云订阅费用至关重要。 该指南涵盖了从 3000 美元的双 RTX 3090 配置（48GB 显存）到 5 万美元以上的多 GPU 构建，并为中端硬件推荐了 Qwen3.6-27B 等模型。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 大语言模型（LLM）需要大量计算资源，尤其是显存（VRAM）用于推理。最先进的模型通常需要数百 GB 显存，使得本地部署成本高昂。量化技术可以减小模型大小，但可能影响质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/jamesob/local-llm">GitHub - jamesob/local-llm: Everything I know about running LLMs locally · GitHub</a></li>
<li><a href="https://enji.ai/tech-articles/how-to-switch-from-sota-llms-to-local-oss-llms/">Switching from SOTA to Local OSS LLMs: A Practical Guide</a></li>
<li><a href="https://www.pugetsystems.com/solutions/ai/enterprise-scale/hardware-recommendations/">Hardware Recommendations for Large Language Model Servers | Puget Systems</a></li>

</ul>
</details>

**社区讨论**: 评论者警告成本可能远超初始估算，有人指出 4 万美元预算的构建实际花费 5-5.5 万美元。其他人建议使用统一内存架构（如 128GB Mac）或云服务作为更经济的选择。

**标签**: `#LLM`, `#local inference`, `#hardware`, `#deep learning`, `#open source`

---

<a id="item-9"></a>
## [Costco 的反亚马逊策略：避开最后一公里配送](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

一篇分析文章指出，Costco 的商业模式刻意避开了最后一公里配送的物流复杂性，这与亚马逊将单个包装商品送货上门的做法形成鲜明对比。 这种对比凸显了零售业根本性的战略差异，质疑了送货上门所需物流复杂性的社会价值，并强调了 Costco 抵御电商巨头冲击的能力。 Costco 依赖顾客自行驾车前往仓库并运输大宗购买的商品，而亚马逊则处理到户的最后一公里配送，这是一个成本高昂的过程。

hackernews · bookofjoe · 7月3日 15:14 · [社区讨论](https://news.ycombinator.com/item?id=48776044)

**背景**: 最后一公里配送是指物流过程的最后一段，即将货物从配送中心运送到最终客户的家门口。对于亚马逊等电商公司来说，这是主要的成本和复杂性驱动因素。相比之下，Costco 的仓储会员店模式将运输负担转移给顾客，从而降低了物流开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Last_mile_(transportation)">Last mile (transportation) - Wikipedia</a></li>
<li><a href="https://www.businessinsider.com/why-costcos-business-model-is-so-great-2016-2">Costco is beating Walmart and Amazon with the 'best business model' in retail</a></li>
<li><a href="https://www.untaylored.com/post/how-costco-makes-money-business-model-explained">How Costco Makes Money: The Costco Business Model and Revenue Streams Explained | Untaylored</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，亚马逊也试图将购买集中在更少的 SKU 上以获得类似 Costco 的好处，但可以支持长尾 SKU。一些人称赞 Costco 避开最后一公里问题的智慧，而另一些人则提出了非美国的视角，例如 Costco 在英国会员资格的限制以及其对电子产品、轮胎等非食品类商品的侧重。

**标签**: `#business strategy`, `#logistics`, `#e-commerce`, `#retail`

---

<a id="item-10"></a>
## [Valve 开源 Steam Machine 电子墨水屏设计](https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/) ⭐️ 7.0/10

Valve 已开源 Steam Machine 上使用的电子墨水屏设计，允许任何人自行制作兼容屏幕。该公司不会自行生产该显示屏，但已发布社区制作所需的文件。 此举使社区能够自定义和维修 Steam Machine，促进了创新和可修复性。这与 Valve 更广泛的开源硬件战略一致，并可能激励整个行业采取类似做法。 该电子墨水屏被确认为标准的 Adafruit 5.83 英寸 eInk 显示屏（产品编号 6397）。开源版本包括设计文件和文档，使用户能够 3D 打印外壳并将屏幕与 Steam Machine 集成。

hackernews · ahlCVA · 7月3日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=48774518)

**背景**: Steam Machine 是 Valve 即将推出的游戏主机，最早于 2025 年底亮相，配备可选的电子墨水前面板用于自定义。Valve 有支持开源硬件和软件的历史，例如 Steam Deck 以及对图形驱动程序的贡献。开源电子墨水屏设计使社区能够创建自定义皮肤、动画或功能显示屏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gamingonlinux.com/2026/07/valve-open-source-the-steam-machine-e-ink-screen-so-you-can-make-your-own/">Valve open source the Steam Machine e-ink screen so you can make your own | GamingOnLinux</a></li>
<li><a href="https://www.notebookcheck.net/Valve-showcases-Steam-Machine-with-e-ink-display.1162643.0.html">Valve showcases Steam Machine with e-ink display - Notebookcheck News</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户称赞 Valve 让社区自由发挥可选配件的做法。一位用户识别出了具体的 Adafruit 面板，另一位用户表示有兴趣将该设计适配到 Framework Desktop 外形上。还出现了一个关于支持 HDMI 输入的更大尺寸电子墨水屏的技术问题。

**标签**: `#open-source`, `#hardware`, `#valve`, `#e-ink`, `#community`

---

<a id="item-11"></a>
## [将代码转为图片再 OCR，LLM 成本降低 60%](https://github.com/teamchong/pxpipe) ⭐️ 7.0/10

一名开发者发现，将代码文本转换为图像，然后利用 LLM 的 OCR 能力进行处理，可将 API 成本降低高达 60%，原因是图像输入的每 token 定价低于文本 token。 这一定价漏洞可能大幅降低重度 LLM 用户的运营成本，但也可能导致提供商调整定价或填补漏洞，从而可能增加 OCR 相关成本。 该技术通过 pxpipe 工具实现，利用了 LLM API 中文本和图像输入之间的 token 定价差异，但可能需要更多的生成 token 且速度较慢。

hackernews · dimitropoulos · 7月3日 15:50 · [社区讨论](https://news.ycombinator.com/item?id=48776464)

**背景**: LLM API 通常按 token 计费，文本 token 和图像 token 定价不同。OCR（光学字符识别）是从图像中提取文本的过程。一些提供商如 Gemini 在内部对 PDF 进行 OCR 处理而不额外收取文本 token 费用，这表明可能存在计费漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48776464">60% Fable cost cut by converting code to images and having the model OCR it | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这一技巧利用了可能被修复的 token 计费漏洞，类似于 Gemini 处理 PDF 的方式。有人提到去年尝试过类似方法（使用 OpenAI 模型），发现虽然减少了提示 token，但需要更多生成 token，最终成本更高且速度更慢。

**标签**: `#LLM`, `#cost optimization`, `#OCR`, `#pricing hack`, `#AI`

---

<a id="item-12"></a>
## [半成品：创业警示故事](https://weli.dev/blog/half-baked-product/) ⭐️ 7.0/10

一篇反思性文章通过虚构的烤箱公司，说明创业公司因激励错位和缺乏领域专业知识而失败。 这个故事引起广泛共鸣，因为它突出了常见的创业陷阱——创始人动机与产品现实错位、组织脱节——这些因素导致即使有资金和努力也最终失败。 该文章在 Hacker News 上获得 7.0/10 分，1163 个点赞和 355 条评论，表明社区参与度高，并认可这些熟悉但有价值的主题。

hackernews · weli · 7月3日 08:23 · [社区讨论](https://news.ycombinator.com/item?id=48772388)

**背景**: 这篇文章是一个警示故事，讲述一家创业公司打造了一个“半成品”——技术上可行但市场失败的烤箱。故事探讨了创始人的主要动机（致富）与深度领域专业知识需求之间的冲突，以及不同团队（工程、销售、管理）各自为政，导致产品无法满足任何人的需求。

**社区讨论**: 评论者指出创始人的动机错位（追求财富而非领域专业知识）是核心问题，并注意到角色之间的组织脱节。一些人幽默地分享了其他行业的类似经历，而另一些人则指出故事的主题具有永恒性，会反复出现。

**标签**: `#startups`, `#product development`, `#entrepreneurship`, `#failure analysis`

---

<a id="item-13"></a>
## [课程创作者报告收入因 AI 下降超 50%](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

知名课程创作者 Josh W. Comeau 报告称，其最新课程销量仅为通常水平的三分之一左右，现有课程收入同比下降超过 50%，他将此归因于 AI 引发的开发者就业不确定性以及 LLM 取代付费学习资源。 来自知名教育者的第一手数据凸显了 AI 对开发者教育市场的实际经济影响，可能预示着影响众多独立创作者和学习生态系统的更广泛趋势。 Comeau 指出，他交谈过的其他课程创作者也看到了同样的趋势，收入下降超过 50%，参与内容的人减少，因为学习者转向 LLM，而 LLM 未经同意或补偿就消耗了创作者的作品。

rss · Simon Willison · 7月3日 21:25

**背景**: Josh W. Comeau 是一位备受尊敬的前端开发者和教育者，以高质量的 CSS 和 React 交互式课程闻名。像 ChatGPT 这样的大型语言模型（LLM）的兴起使得个性化辅导和代码生成成为可能，可能减少了对结构化付费课程的需求。此外，广泛的裁员和 AI 自动化恐惧造成了软件开发工作未来的不确定性，抑制了学习投资。

**标签**: `#AI impact`, `#developer education`, `#online courses`, `#job market`, `#LLMs`

---

<a id="item-14"></a>
## [私人太空飞行员为美国太空部队执行轨道任务](https://techcrunch.com/2026/07/02/private-space-pilots-are-flying-orbital-missions-for-the-us-space-force/) ⭐️ 7.0/10

True Anomaly 和 Rocket Lab 正在为美国太空部队执行轨道卫星机动，进行类似《壮志凌云》式的飞越，以测试空间态势感知和快速响应能力。 这标志着太空领域商业与军事合作的重大转变，可能加速太空作战战术和卫星服务技术的发展。 在 Victus Haze 任务中，Rocket Lab 的卫星 Puma 在发射后 37 小时 36 分钟内完成激活并准备好首次轨道机动，展示了快速在轨就绪能力。

rss · TechCrunch · 7月2日 23:01

**背景**: True Anomaly 是一家专注于太空防御的国防技术公司，由前美国太空部队成员于 2022 年创立。Rocket Lab 提供专用小型卫星发射服务，可实现精确轨道注入。美国太空部队正越来越多地利用商业合作伙伴进行空间态势感知和快速响应任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.trueanomaly.space/">True Anomaly - Delivering Decisive Capabilities for Space Superiority.</a></li>
<li><a href="https://www.airandspaceforces.com/victus-haze-mission-rapid-maneuvers-satellites/">Satellites Maneuver on Rapid Timelines for Victus Haze Mission</a></li>
<li><a href="https://www.trueanomaly.space/careers">Careers - True Anomaly</a></li>

</ul>
</details>

**标签**: `#space`, `#military`, `#private space industry`, `#satellite operations`

---

<a id="item-15"></a>
## [DeepSeek DSpark：推理速度提升高达 85%](https://www.reddit.com/r/LocalLLaMA/comments/1um9j5q/deepseek_drops_another_huge_breakthrough_dspark/) ⭐️ 7.0/10

DeepSeek 开源了 DSpark，这是一个推测性解码框架，可在 V4-Flash 和 V4-Pro 模型上将推理速度提升高达 85%，且无需新硬件或重新训练。 这一突破显著降低了推理延迟，使大语言模型在实时应用中更加实用，并降低了运营成本，可能加速各行业的采用。 DSpark 是 DeepSpec 代码库的一部分，于 2026 年 6 月 27 日发布。加速效果取决于接受质量，实际收益可能有所不同。

reddit · r/LocalLLaMA · /u/BringTea_666 · 7月3日 09:19

**背景**: 推测性解码通过使用较小的草稿模型预测多个 token，再由大模型验证，从而加速 LLM 推理。多 token 预测（MTP）是一种替代方法，模型本身每步预测多个 token，无需单独的草稿模型。DSpark 通过优化草稿和验证过程改进了这些方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf">DeepSpec/DSpark_paper.pdf at main · deepseek-ai/DeepSpec</a></li>
<li><a href="https://www.techtimes.com/articles/319236/20260628/deepseek-releases-dspark-speculative-decoding-makes-v4-85-percent-faster.htm">DeepSeek Releases DSpark: Speculative Decoding Makes V4 Up to ...</a></li>
<li><a href="https://venturebeat.com/orchestration/deepseek-open-sources-dspark-a-new-framework-to-speed-up-llm-inference-by-up-to-85">DeepSeek open sources DSpark, a new framework to speed up LLM ...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI`, `#efficiency`, `#breakthrough`

---