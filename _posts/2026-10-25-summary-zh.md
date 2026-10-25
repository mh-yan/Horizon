---
layout: default
title: "Horizon Summary: 2026-10-25 (ZH)"
date: 2026-10-25
lang: zh
---

> 从 28 条内容中筛选出 8 条重要资讯。

---

1. [Moderna 与 Merck 的 mRNA 癌症疫苗将黑色素瘤死亡和复发率降低 42%](#item-1) ⭐️ 9.0/10
2. [10 年前的 Inception v3 CNN 在皮肤癌诊断上超越前沿 LLM](#item-2) ⭐️ 7.0/10
3. [俄勒冈警方对一名警察的记录报价 250 万美元](#item-3) ⭐️ 7.0/10
4. [加州大学伯克利分校数学教授因 AI 使用质疑作业评分](#item-4) ⭐️ 7.0/10
5. [Cerebras 在晶圆级硬件上部署万亿参数 AI 模型](#item-5) ⭐️ 7.0/10
6. [OpenAI 与 Anthropic 阻止对智能电视的逆向工程](#item-6) ⭐️ 7.0/10
7. [RTX 3080 20GB 改装解锁 P2P 和 ReBAR，vLLM 提示处理速度提升最高 115%](#item-7) ⭐️ 7.0/10
8. [Lean-QwenFlash 通过 NVMe SSD 卸载在 16GB 显存和 8GB 内存上以 20 tok/s 运行 125B Qwen3.8-Flash-Next](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Moderna 与 Merck 的 mRNA 癌症疫苗将黑色素瘤死亡和复发率降低 42%](https://arstechnica.com/health/2026/10/personalized-mrna-cancer-vaccine-cut-melanoma-death-recurrence-by-42/) ⭐️ 9.0/10

Moderna 和 Merck 报告称，其个性化 mRNA 癌症疫苗在针对黑色素瘤患者的 2 期试验中将死亡或复发风险降低了 42%。 这是一项重大医学突破，验证了个性化 mRNA 癌症疫苗的方法，可能重塑癌症治疗，同时也提升了 Moderna 在 COVID-19 之外的平台战略。 该试验测量了黑色素瘤患者的无复发生存期，但数据来自 2 期试验，需要更大规模的 3 期试验来确认疗效和安全性。

hackernews · _Microft · 10月25日 19:29 · [社区讨论](https://news.ycombinator.com/item?id=50235217)

**背景**: 个性化 mRNA 癌症疫苗通过分析患者肿瘤突变，并将这些新抗原编码到 mRNA 中，递送后促使免疫系统攻击癌细胞。这种方法基于 COVID-19 疫苗中使用的 mRNA 平台技术，但针对每位患者进行定制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Personalized_mRNA_cancer_vaccine_therapy">Personalized mRNA cancer vaccine therapy - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11908549/">Challenges and opportunities of predicting overall survival ...</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 Moderna 的按需疫苗平台商业模式，指出尽管数据良好但股价因预期过高而下跌，并表达了对特朗普政府和 RFK Jr.对 mRNA 疫苗政治反对的担忧。

**标签**: `#mRNA`, `#cancer-vaccine`, `#biotech`, `#Moderna`, `#healthcare`

---

<a id="item-2"></a>
## [10 年前的 Inception v3 CNN 在皮肤癌诊断上超越前沿 LLM](https://lynchlab.net/llm-skin-cancer) ⭐️ 7.0/10

lynchlab.net 的一篇博客文章报告称，一个已有 10 年历史的 Inception v3 卷积神经网络在来自 ISIC 档案的 68,011 张皮肤镜和临床图像上进行了微调，在 200 个病变的测试集上诊断皮肤癌的表现优于两个前沿大语言模型（LLM）。该模型在单个 H100 GPU 上训练，并且在训练期间从未见过测试病变或同一患者的任何图像。 这一发现挑战了通用大语言模型总是专业任务最佳工具的假设，突显了小型的任务特定模型在医学影像等狭窄领域可以实现更高的准确性。它引发了关于专用架构与 LLM 的价值以及基准测试在模型评估中的作用的辩论。 该 CNN 使用在日常生活照片上预训练的 Inception v3，并在 ISIC 档案数据集上微调所有层；测试集经过精心策划，排除了训练中同一病变或患者的任何图像。然而，批评者认为这是“基准最大化”（benchmaxxing）的一个例子——专门针对基准进行优化——并且这种比较可能无法反映真实世界的临床性能。

hackernews · sungam · 10月25日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=50233779)

**背景**: Inception v3 是谷歌于 2016 年发布的卷积神经网络架构，以其高效性和使用因子化卷积而闻名。微调是指采用预训练模型并在特定数据集上进一步训练，使其适应新任务。LLM 是在大量文本数据上训练的大语言模型，具备通用推理能力，但并非天生专门用于图像分类。ISIC 档案是一个大型公共皮肤病变图像集合，用于皮肤病学研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Inception_(deep_learning_architecture)">Inception (deep learning architecture) - Wikipedia</a></li>
<li><a href="https://huggingface.co/docs/timm/main/models/inception-v3">Inception v3 - Hugging Face</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC7969634/">Convolutional Neural Network for Skin Lesion Classification ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者讨论了其影响：一些人认为对于规模化应用，专用分类器更准确，而 LLM 可以帮助廉价地构建它们；另一些人指出这种比较不公平，因为 CNN 是专门针对该基准优化的（“基准最大化”）。一些人指出像 KataGo 这样的专用模型在狭窄任务上优于 LLM，另一些人则欢迎对多样化机器学习技术的重新重视。

**标签**: `#machine-learning`, `#LLMs`, `#medical-imaging`, `#model-architecture`, `#benchmarking`

---

<a id="item-3"></a>
## [俄勒冈警方对一名警察的记录报价 250 万美元](https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/) ⭐️ 7.0/10

据 The Intercept 报道，俄勒冈州尤金警察局估计，处理一家当地新闻媒体针对一名警察的公共记录请求需要 44,816 个员工工时，费用约为 2,484,599.04 美元。 这一案例表明，高昂的费用估算可能被用来阻碍公众获取公共记录，从而削弱政府透明度和问责制。它引发了关于《信息自由法》实践以及需要改革以防止此类滥用的更广泛讨论。 44,816 小时的估算相当于一个人全职工作约 21 年，而报价超过 240 万美元。根据俄勒冈州的公共记录法，机构在满足请求之前必须提供费用和时间的书面估算，这可能被用来威慑请求者。

hackernews · tdeck · 10月25日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=50234232)

**背景**: 《信息自由法》（FOIA）和州级公共记录法旨在确保公众能够获取政府记录，促进透明度和问责制。然而，机构可以对搜索、审查和复制记录收取费用，而过高的估算实际上可能阻止请求。俄勒冈州的公共记录法（ORS 192.410 至 192.505）要求机构在五个工作日内确认请求并提供费用估算，但没有对费用设定上限，允许机构报出令人望而却步的金额。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.searchsystems.net/us/or/public-records-law">Oregon Public Records Law - Oregon Public ... | SearchSystems.net</a></li>
<li><a href="https://cdnsm5-hosted.civiclive.com/UserFiles/Servers/Server_3585797/File/Government/Public+Records+and+Regulations/Public+Records+Law/OregonPublicRecordLaw.pdf">A Quick Reference Guide to Oregon 's Public Records Law</a></li>
<li><a href="https://covenantforwarriors.org/advocacy-stories/what-they-dont-want-you-to-know/how-government-agencies-dodge-transparency-laws/">How U.S. Government Agencies dodge transparency laws | Covenant...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者对这一荒谬的估算表示愤怒，有人指出这相当于 21 年的工作量。其他人分享了机构使用拖延战术的类似经历，并将美国系统与英国《信息自由法》进行了不利的比较，后者要求 30 天内回复，以及德国关于 FOIA 费用的持续争论。一些人指出国防部甚至提出了更大的费用估算，突显了一种阻碍模式。

**标签**: `#public-records`, `#foia`, `#government-transparency`, `#police-accountability`, `#journalism`

---

<a id="item-4"></a>
## [加州大学伯克利分校数学教授因 AI 使用质疑作业评分](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 7.0/10

加州大学伯克利分校数学家、菲尔兹奖得主理查德·博切兹公开质疑在 AI 工具普及的情况下批改作业的价值，在 Hacker News 上引发了大量讨论。 这突显了 AI 如何迫使教育工作者重新思考传统的评估方法，可能重塑学生的评价方式以及高等教育所重视的技能。 博切兹是菲尔兹奖得主，以证明“魔群月光”猜想而闻名，讨论中透露他可能将评分工作委托给助教，这引发了关于作业目的和 AI 在学习中作用的疑问。

hackernews · romanhn · 10月25日 16:28 · [社区讨论](https://news.ycombinator.com/item?id=50233304)

**背景**: 像 ChatGPT 这样的大型语言模型（LLM）能够生成类似人类的文本并解决问题，使学生很容易使用 AI 完成作业。这引发了关于学术诚信和作业作为学习工具有效性的争论。理查德·博切兹是加州大学伯克利分校的著名数学家，因其在格、群论和无限维代数方面的工作于 1998 年获得菲尔兹奖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Richard_Borcherds">Richard Borcherds - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models ( LLMs )? | IBM</a></li>

</ul>
</details>

**社区讨论**: 评论者指出讽刺之处：博切兹可能多年没有亲自批改作业，并争论作业的目的是学习还是评估。一些人认为 AI 消除了迫使学生接触材料的强制功能，而另一些人则质疑为大学生批改作业的价值。

**标签**: `#AI`, `#education`, `#LLMs`, `#academia`, `#assessment`

---

<a id="item-5"></a>
## [Cerebras 在晶圆级硬件上部署万亿参数 AI 模型](https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras) ⭐️ 7.0/10

Cerebras 发布博客文章，详细介绍了如何在其晶圆级硬件上部署万亿参数的前沿 AI 模型，实现每秒 1,000 至 2,000 多个 token 的推理速度。文章解释了如何将模型映射到 WSE-3T 晶圆上，以实现可扩展的推理。 这表明晶圆级硬件能够以高吞吐量处理最大的 AI 模型，为推理提供了 GPU 集群之外的替代方案。这可能会影响企业部署前沿模型的方式，尤其是在速度和成本效率至关重要的场景中。 Cerebras 声称推理速度可达每秒 1,000 至 2,000 多个 token，但社区成员指出，Cerebras 上可用的模型往往比前沿模型落后。该硬件需要大量资源，而扩展以满足需求仍然是一个挑战。

hackernews · gmays · 10月25日 01:33 · [社区讨论](https://news.ycombinator.com/item?id=50227356)

**背景**: Cerebras Systems 以其晶圆级引擎（WSE）而闻名，这是一种硅晶圆大小的芯片，集成了数十万个 AI 优化核心。2024 年 3 月推出的 WSE-3 拥有 4 万亿个晶体管和 90 万个核心，为 CS-3 超级计算机提供动力。万亿参数模型是最大的语言模型，推理时需要巨大的计算和内存资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Cerebras WSE-3 Turbo | Wafer-Scale AI Chip</a></li>
<li><a href="https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras">How Cerebras Deploys Trillion-Parameter AI Models</a></li>

</ul>
</details>

**社区讨论**: 评论者就 Cerebras 满足需求的能力展开辩论，一些人指出该公司缺乏 OpenAI 那样的财务资源，难以制造足够的晶圆级节点。其他人批评该服务提供的模型过时，但一些人预计 Cerebras 很快会以更低成本和更高速度推出更好的模型。还有少数人对数据如何在晶圆的处理单元之间流动的技术细节提出了疑问。

**标签**: `#AI hardware`, `#large language models`, `#Cerebras`, `#wafer-scale`, `#inference`

---

<a id="item-6"></a>
## [OpenAI 与 Anthropic 阻止对智能电视的逆向工程](https://www.reddit.com/r/LocalLLaMA/comments/1xer30z/openai_and_anthropic_blocked_the_reverse/) ⭐️ 7.0/10

r/LocalLLaMA 上的一篇 Reddit 帖子指出，OpenAI 和 Anthropic 阻止了一项旨在调查智能电视间谍行为的逆向工程工作（REA），据报道 Claude 在一天后封禁了该工具。 这引发了人们对前沿模型提供商拒绝合法安全研究用例的担忧，可能阻碍隐私调查，并加剧关于开源权重模型作为此类工作替代方案的争论。 该帖子内容单薄，仅包含一个 X 帖子链接和简短评论，封禁似乎是由于安全护栏而非特定政策变更；据报道，REA 工具（Reverse Engineer Anything）在详细的二进制和固件分析过程中被中断。

reddit · r/LocalLLaMA · /u/kroggens · 10月25日 02:51

**背景**: 智能电视逆向工程涉及分析固件和二进制文件，以揭示隐藏的数据收集行为，例如常开麦克风或跟踪。最近对 LG 和三星电视的调查暴露了广泛的数据共享，促使研究人员使用 REA 等 AI 工具。OpenAI 和 Anthropic 的安全政策限制某些逆向工程请求，这可能无意中阻碍合法的安全研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=8eyy-Dri9dU">The LG Smart TV Spying Scandal: How Researchers Actually ... LG Smart TV Spying Exposed: 216M TVs, Full Breakdown | The ... Researcher says Samsung TV software tracks viewing and may ... LG Smart TVs Accused of Audio and Wi-Fi Data Collection Samsung TV Privacy Claims Raise Fresh Questions About AI ... Anthropic Limits Claude's Help with Reverse-Engineering T... People are now vibe-coding their smart TVs to strip them of ...</a></li>
<li><a href="https://ai-tldr.dev/learn/evaluation-safety/alignment-safety/why-llms-refuse/">Why Do LLMs Refuse? Over-Refusals Explained | AI/TLDR</a></li>

</ul>
</details>

**社区讨论**: r/LocalLLaMA 社区对模型拒绝合法安全研究表示不满，评论者认为这种过度拒绝强化了开源权重模型的理由，因为用户可以控制和本地运行这些模型。

**标签**: `#AI safety policy`, `#open weights`, `#reverse engineering`, `#LLM refusals`, `#privacy`

---

<a id="item-7"></a>
## [RTX 3080 20GB 改装解锁 P2P 和 ReBAR，vLLM 提示处理速度提升最高 115%](https://www.reddit.com/r/LocalLLaMA/comments/1xf9kmd/rtx_3080_20gb_got_rebar_and_p2p_unlock_70_prompt/) ⭐️ 7.0/10

社区成员 u/nathannguyennng 在改装的 RTX 3080 20GB 显卡上解锁了 PCIe 点对点（P2P）和 Resizable BAR（ReBAR）支持，另一位用户分享了基准测试结果：在张量并行的 vLLM 推理中，提示处理速度相比原始状态最高提升 115%。测试使用两块 RTX 3080 20GB 显卡，在 Proxmox 虚拟机中运行 vLLM 0.32.0 服务一个 27B AWQ-INT4 模型。 这对本地 LLM 社区来说是一个重大胜利，因为它表明通过固件/驱动层面的解锁，较旧的改装显卡在多 GPU 配置中可以实现大幅度的提示处理加速，可能延长经济型硬件在自托管推理中的使用寿命。这也凸显了 P2P 和 ReBAR 这些通常专属于较新或专业显卡的功能，可以在消费级显卡上启用以改善张量并行工作负载。 基准测试显示，同时启用 GPU 解锁和 P2P 时，提示处理速度相比原始状态提升 70% 到 115%，其中仅 P2P 就在 GPU 解锁的基础上贡献了最高 70% 的提升。然而，令牌生成（解码）性能没有一致改善，除超长提示（26.1 万令牌）有轻微提升外，基本在噪声范围内。测试系统使用 PCIe 3.0 x16 插槽，并将两块 GPU 的功耗限制在 240W。

reddit · r/LocalLLaMA · /u/No-Refrigerator-1672 · 10月25日 18:16

**背景**: P2P（点对点）允许 GPU 通过 PCIe 总线直接访问彼此的内存，绕过 CPU 和系统内存，从而降低多 GPU 通信的延迟并提高带宽。ReBAR（Resizable BAR）是一项 PCIe 功能，让 CPU 可以访问完整的 GPU 显存，而不是有限的 256MB 窗口，从而提高数据传输效率。vLLM 是一个流行的开源推理引擎，支持张量并行，将模型拆分到多个 GPU 上以容纳更大的模型并加速处理。RTX 3080 20GB 是原版 10GB 显卡的改装版本，显存可能翻倍，而这些解锁功能使消费级 Ampere 显卡能够使用 NVIDIA 官方未支持的特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.nvidia.com/ai-enterprise/release-8/latest/infra-software/vgpu/features/p2p.html">Peer-To-Peer (P2P) CUDA Transfers — NVIDIA AI Enterprise</a></li>
<li><a href="https://www.intel.com/content/www/us/en/support/articles/000090831/graphics.html">What Is Resizable BAR and How Do I Enable It? - Intel</a></li>
<li><a href="https://docs.vllm.ai/en/latest/serving/parallelism_scaling/">Parallelism and Scaling - vLLM</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#gpu-inference`, `#vllm`, `#tensor-parallelism`, `#hardware-modding`

---

<a id="item-8"></a>
## [Lean-QwenFlash 通过 NVMe SSD 卸载在 16GB 显存和 8GB 内存上以 20 tok/s 运行 125B Qwen3.8-Flash-Next](https://www.reddit.com/r/LocalLLaMA/comments/1xev6bo/leanqwenflash_qwen38flashnext_125b_running_at_20/) ⭐️ 7.0/10

一位 Reddit 用户将 sybil-solutions/glm-flash-lite 的 SSD 卸载设计适配到 Qwen3.8-Flash-Next（125B），在仅 16GB 显存和 8GB 系统内存的消费级硬件上运行，在 262k 上下文下达到约 20 tok/s 的解码速度。基准测试显示，在 8k 上下文下，散文生成速度为 28–33 tok/s，代码生成速度为 19–22 tok/s，在 RTX 4090 上预填充速度约为 1,080 tok/s。 这表明通过将专家卸载到 NVMe SSD 而不是保留在内存中，大型 MoE 模型可以在普通的消费级笔记本电脑上运行，显著降低了本地 LLM 部署的内存门槛。它可能使更多用户无需高端工作站就能试验 100B+ 参数模型。 基准测试使用 3.05bpw_h5_ng5 量化和 Q4 KV 缓存；在 RTX 3080 笔记本（16GB 显存，32GB 内存）上，100k 上下文下解码速度约为 18–21 tok/s，预填充速度约为 650–700 tok/s，峰值显存为 15.5GB。安装说明、模型下载器和打包脚本已在 GitHub 上提供。

reddit · r/LocalLLaMA · /u/MaxDev0 · 10月25日 06:41

**背景**: 像 Qwen3.8-Flash-Next 这样的混合专家（MoE）模型包含许多专门的子网络（专家），但每个 token 只激活其中一部分，从而减少计算量。然而，所有专家都必须存储在某个地方；通常它们被保存在系统内存中，一个 125B 模型需要 48–64GB。SSD 卸载将不活跃的专家移到快速的 NVMe 存储上，以一定的延迟换取大幅降低的内存需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://arxiv.org/pdf/2408.10013">SSDTrain: An Activation Offloading Framework to SSDs for ...</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#model-offloading`, `#moe`, `#qwen`, `#nvme-ssd`

---