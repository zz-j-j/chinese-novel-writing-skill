# 研究阅读笔记

这份笔记记录用于打磨小说创作方法的公开资料。这里只概括高层观点并提供原始链接，不收录原文段落或示例。它们是启发和校验，不是本 skill 的规则来源，更不构成每部小说都要遵守的定律。

## 情节由相连的行动组成

亚里士多德《诗学》讨论悲剧中的情节结构，强调行动组成的整体以及事件之间的可能性或因果联系。本 skill 将这个宽泛观点转为一个写作问题：删掉或挪动某段后，人物选择、后续因果或读者理解是否会受影响？这不是要求小说套用古典戏剧结构。

来源： [Project Gutenberg：The Poetics of Aristotle](https://www.gutenberg.org/files/1974/1974-h/1974-h.htm)（S. H. Butcher 英译本）。该页面说明了电子文本的使用地区与许可条件；本 skill 只提供链接和概述，没有复制译文。

## 悬念来自读者对后续的期待

Wilmot 与 Keller 的研究比较了“当前事件有多意外”和“后续结果还存在多少不确定性”两种悬念建模方式，并用短篇故事中的人工标注进行评估。论文报告，基于故事表征的不确定性减少是较好的预测因素。对创作的启发是：制造惊讶之外，还要让读者看见风险和正在等待的结果。研究讨论的是特定语料与建模任务，不能推成“每章必须设置悬念”。

来源： [arXiv：Modelling Suspense in Short Stories as Uncertainty Reduction over Neural Representation](https://arxiv.org/abs/2004.14905)。

## 人物的目标追求影响读者投入

Hamby、Shawver 与 Moreau 的两项研究考察人物目标追求如何关联读者的叙事投入。论文摘要报告，人物动机对叙事投入有稳定影响，尤其涉及情感投入。对本 skill 的启发是：让读者看见人物为何追求一件事、行动遇到什么困难。它不表示每个角色都要有宏大的明确目标，也不能替代题材、视角和情节的判断。

来源： [Media Psychology：How character goal pursuit “moves” audiences to share meaningful stories](https://doi.org/10.1080/15213269.2019.1601569)。

## 本 skill 自己整理的应用方法

“读者牵引四问”把上面的宽泛观点与本项目反复收到的改稿反馈合并成一个轻量工具：读者在等什么、人物为什么行动、阻力怎样改变行动、场景留下什么后果。这个名称、流程、指令和小说示例是为本 skill 重新编写的；它不是上述论文或古典文本中的现成模型，也不是对其内容的复述。

## 中文 AI 文本研究与小说审读的边界

中文检测研究对“统计特征可以帮助某个检测器区分特定语料”提供了证据，但不等于这些特征是中文小说的缺陷，更不能据此反推作者身份。现有研究的任务和语料差异很大：微博短评、跨领域文本、文学段落和人机协作文本不是同一类材料。

Su 等人的 2025 年研究构建了跨领域中文检测语料，其中包含文学文本，并报告其模型在不同生成模型上的表现不同；作者也将句长变化有限、标点密集等统计现象作为检测分析线索。这是模型和特定语料中的相关特征，不是编辑规范，不能转成“中文小说句长要参差”或“每章标点不得超过某数”的规则。

Li 与 Zhang 的 CCL 2025 研究面向 463,382 条微博评论，构建了中文社交媒体风格特征用于短评论检测。其语料规模虽大，但短评的长度、互动语境和表达目的与长篇小说不同，不能直接移植其特征权重。

Yang 等人的 C-HAT-Bench（2026 年 9 月发布的预印本）研究中文人机协作文本，语料覆盖新闻、法律、问答、百科和文学等领域。论文报告，检测器在不同协作方式间的表现会下降且迁移并不对称；这说明即便同为中文，生成、续写、改写等过程也会改变可观察信号。该工作仍是预印本，结论应视为持续发展的研究。

因此，`style-signal-review.md` 的 0–12 分只衡量中文小说中可引用、可讨论的表达模式及编辑优先级；它不是经中文小说平行语料校准的检测量表，不估算写作来源、作者身份或平台检测结果。比喻和特殊符号按照人物视角、篇章功能与作品基线审读，不能单独作为 AI 证据。

来源：

- [Su et al., *Research on AI-generated Chinese text detection method based on deep learning* (Big Data and Information Analytics, 2025)](https://aimspress.com/article/doi/10.3934/bdia.2025016)。研究含文学文本，但面向检测器构建与分类，不是中文小说编辑指南。
- [Li & Zhang, *Linguistic Differences between AI and Human Comments in Weibo: Detect AI-Generated Text through Stylometric Features* (CCL 2025)](https://aclanthology.org/2025.ccl-1.64/)。研究对象为微博短评论，结论不直接代表长篇叙事。
- [Yang et al., *C-HAT-Bench: Benchmarking Chinese AI-Text Detection Beyond Fully Generated Text* (2026 preprint)](https://arxiv.org/abs/2609.32770)。研究关注中文人机协作和跨条件检测，覆盖文学等多个领域；尚为预印本。
