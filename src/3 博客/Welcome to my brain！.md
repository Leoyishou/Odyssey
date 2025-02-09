---
draw:
tags: []
title: Welcome to my brain！
date created: 2024-10-23
date modified: 2024-12-27
---

![image.png|1000](https://imagehosting4picgo.oss-cn-beijing.aliyuncs.com/imagehosting/fix-dir%2Fpicgo%2Fpicgo-clipboard-images%2F2024%2F11%2F12%2F01-13-27-940e914a4a2b396431a33c442512f94f-202411120113094-324476.png)

如果你需要一个闹钟的话，那么你也一定需要一个第二大脑。
『计算机科学只存在两个难题：缓存失效和命名』，学习或者知识管理也是如此。

<!-- more -->

## 一、本质

[缓存](缓存.md)，浏览维基百科的时候，可以看到很多关键性的『词汇』，标记为蓝色，并且可以点击跳转到对应的词条。再扩大一点，乃至整个互联网，无非就是将各种概念信息相互联系，能彼此间跳转的一张巨大的网络。我们可以删繁就简，随着自己对这个世界实践和认识的加深，构建起一张世界的缓存网，作为世间真理的抽象，岂不美哉！

[命名](命名.md)，每一个 [concept](concept.md) 对应一种概念，本质是对世界的某个抽象，对应着的其实是编程中的命名。选择并组织好整个第二大脑的各个 node，是第二大脑的关键。目前的一个经验是，每当命名找**大词**，比如说『前端从 A 子页面跳到 B 子页面，切回来的时候仍然能看到之前的数据』，这样的表达就不如『状态管理』这一个大词好用，起码在信息保留和传递中是如此。大词往往意味着更大范围的共识和更标准化的表达，意味着更容易组织起周围的概念，意味着未来复习知识时更低的搜索成本！

也就不奇怪那句话了，『计算机科学只存在两个难题：缓存失效和命名』，学习或者知识管理也是如此。

## " 什么是好的笔记系统？"

正如 Jeff Su 所说，" 你经历的摩擦越少，笔记系统就越有效。"

1. before: 你能轻松开始做笔记吗？
2. during: 你能多快写下所有内容？
3. complete: 你能轻松的共享你的笔记吗？
4. after: 您能轻松地重新呈现相关笔记吗？

## 二、过去的怀疑

起初，我并没有那么看好第二大脑，也不是特别相信这种类似知识图谱的笔记组织方式。我甚至怀疑其可视化的美观性远远大于了它的实用性。

当然，从 [知识图谱](知识图谱.md) 的角度来看，第二大脑可能只是看起来炫酷。

知识图谱有很好的可解释性。但可解释性本身就是一个很尴尬的东西，以生成模型为例，从 GAN，到 VAE，再到 NF，模型的约束越来越大，当然可解释性也越来越强，但落地应用最广泛的却是最不可控 GAN。再往大了说，所有的深度学习方法都是不可解释的，但这并没有影响深度学习的广泛应用，当一个黑箱模型确实好用的时候，谁会去关注它内部的原理呢？

以学 Java 为例，拿搜索引擎用知识图谱分析各个技术点，不如直接找个黑马的课程，对着 JD 来学来的高效。黑马的课程设计者就类似一个不可解释的深度学习框架。凭着市场嗅觉，给出了一个课程大纲，来保证学员的竞争性。

参考：知识图谱是否是 NLP 的未来？- Maple 小七的回答 - 知乎  
https://www.zhihu.com/question/267242467/answer/1862160175

我们的大脑就是一个超级版本的不可解释的知识图谱，并且已经被证明非常 work。我们更重要的，可能是加深对于原子化的概念，也就是各个 [concept](concept.md) 的理解。然后通过人类大脑对于概念的自组织的机制，强化我们的能力，拓展我们的边界。

> 这里我说的可能是 [隐形知识](隐形知识) 的概念

那我们为什么还要费尽心思再去体外构建一个呢？

## 三、可能的好处

### 为什么需要概念库？

为什么要收集定义，并借此厘清自己脑子里有哪些清晰的概念？

李笑来一直在强调概念很重要，甚至把判断聪明人的标准是脑子中有多少清晰准确的概念。

语言学家告诉我们：如果我们的大脑对一件事情没有概念，那么我们的大脑就倾向于不去想那件事情；如果一个民族的语言里缺少某个概念，那么这个民族就倾向于从未思考过那个概念。

回想自己学习和精进一个领域的过程，本质上就是对这个领域内各个重要概念不断接触 - 理解 - 领悟的过程。不管是精通一门知识，还是掌握一项技能，fundamentals 都至关重要，与之对应的，便是第二大脑的 [知识图谱](知识图谱.md) 上的一个个 [concept](concept.md)。

### 为什么需要双链特性？

原子化、唯一更新处。

在概念库的基础上，会引申出另一个问题，就是重复的问题。如同 [软件工程@](软件工程@.md) 的 [设计模式@](设计模式@.md) 中对高内聚、低耦合的追求一样，我们在构建概念库的同时，最清晰的方式也是原子化地处理，一处更新则处处迭代。这就需要我们用到类似代码中引用、import 这样的特性了。OB 的 [双向链接](双向链接.md) 无疑是一个很好的实现，给了每个概念一个*唯一*更新处。我想，这一点也是极重要的。解耦之后，我们少了很多繁琐的反复定义，能专心在一处将我们对于某个概念的最新认知更新好。

就比如这篇文章，我差不多前后修改了十多次，大部分都是新认知的迭代，而这在我过去的记录方式中几乎是不可想象的。

### 为什么需要记录下来？

一、对于单个概念，避免注意力资源的重复投入。

比如 markji 中的卡片，有些之前总结的宝贵经验如果没有记录留存的话，之后过了一段时间，要对某个问题达到当时的认知，确实需要再投入一些重复的精力。一份组织好的，由自己切身总结出的知识库，确实可以避免这种重复的投入。

如果我们真的将专注力视为脑力工作者最弥足珍贵的资源，那就绝不能眼睁睁地坐视我们所取得的阶段性成果付诸东流；如果我们真的认识到生命中可用于非凡创作的时间无比珍贵，那就务必要构建起一个给力的知识系统，对各种过程性信息进行有效的回收再利用。

资产可以带来回报，而回报又可作为再投资创造其他价值。知识同样也可以随着时间推移而产生收益和复利，从而成为一种高回报的资产。就像每个月都在股市里投入一小笔资金一样，你在知识领域投入的每一分精力，都让你变得更加博学和聪慧。

二、对于整个网络，可以提示我们对于边缘节点的重视，

工作中，或者对于某个领域的学习了解中，我们常常会陷入一种境地，就是对核心概念了解比较深入了，但是对于目前的边缘概念无法很好拓展出去。一个重要的原因就是生物大脑要触达边缘概念本身就比较费力。第二大脑从整体上构建出概念网络后，其实相当于储存了我们当前网络能触达的边缘，这对于下一次的进一步拓展，其实是非常有利的。

## 混乱性

I try to embrace messiness because my brain is also messy.

### 数据结构与数据的视角

同一份数据，不同的数据结构导致 sort 的时间复杂度不同，知识可能也是如此，有效的组织可能会带来效率的提升。

## 四、操作细节

> [!最佳实践]
> 1. 每一篇 markdown 对应一个概念、文章或者方案。`$`符号结尾的是一些行动计划和执行方案，比如[托福考到100$](托福考到100$.md)，@结尾的是一些带有目录性质的概念，比如[Java@](Java@.md)。除了`$`行动方案外，其他文章的标题都尽可能用大词、术语，这是为了降低和 AI 交流，和他人交流，以及自己未来回溯搜索时的成本，因为大词就以为着更广泛的共识。
> 2. [面向对象](面向对象.md)，[原子笔记](原子笔记.md)
>    - 单个文件命名上尽量用标准化的大词，就比如『设计模式』比『高内聚低耦合的设计思想』这样的话标准化和大众接受化程度高。这样以后搜索和引用都会比较方便
>    - 当一个概念的 usage 次数足够多的时候，才拆成原子笔记/ [concept](concept.md)，如果被引高，抽出来收益就比较大。反之，就像 Java 中的[内部类](内部类.md)一样。
> 3. [常青笔记](常青笔记.md)，处处留意，常常迭代。
>    - 一篇内，围绕一个概念经常性地将更新上最新的认知，保持缓存的实时性。用---语法做分割，区分出 Unstaged 区域
>    - 文件夹内，随项目进度不断移动和调整file tree，一般是按照 最近项目->第二大脑和博客的方向做沉淀。Just do it！The most valuable notes I have today would never come to be if I needed to think about a folder or category for it.
> 4. [最佳实践](最佳实践.md)，将一些总结出的最佳实践用call out 语法 hightlight 出来。

整体是从信息 -> 知识 -> 习惯和智慧 的一个过程  
![image.png|1000](https://imagehosting4picgo.oss-cn-beijing.aliyuncs.com/imagehosting/fix-dir%2Fpicgo%2Fpicgo-clipboard-images%2F2024%2F09%2F29%2F11-56-56-af81333825b6dabd4f2320f56690cd8c-202409291156311-ac525e.png)

1. [滴答清单](滴答清单.md)做 inbox 收集闪念笔记
2. 项目驱动, 制定方案，吸收信息，项目结束后，信息部分归入 2.1，项目部分归入 2.3
3. 结构化吸收新信息，逐步沉淀吸收，从知识-> 沉淀
4. 一些输出性质的东西放到 3 博客部分
5. 整个文档做版本控制，基于 commit 的 diff 定期做 AI 复盘

```shell
├── 1 一切皆项目           
├── 2 第二大脑            
│   ├── 1 知识
│   ├── 2 沉淀
│   ├── 3 存档
│   └── PARA.md
├── 3 博客
├── 4 复盘
│   ├── 2024-10-10.md
│   ├── 2024-10-11.md
│   ├── 2024-10-12.md
│   ├── 2024-10-13.md
│   ├── 2024-10-15.md
```

> **比如记录「反常识」「人名」「术语」**，「反常识」主要是用来拓展认知边界；「人名」是找到知识源头的创造者；「术语」是找到知识的源头  
> [📥 为何收藏无用 | flomo 101 (flomoapp.com)](https://help.flomoapp.com/thinking/stop-fav.html)

![image.png#pic_center|650](https://imagehosting4picgo.oss-cn-beijing.aliyuncs.com/imagehosting/fix-dir%2Fpicgo%2Fpicgo-clipboard-images%2F2024%2F06%2F11%2F15-54-33-93ecdfc66154666a85ca72a0cf3b4320-20240611155433-abfdd0.png)

如果你有这个问题，推荐阅读我们撰写的 flomo 方法：

- [用自己的话，写卡片](https://help.flomoapp.com/method/use-card.html)（阅读需 3 分钟）
- [用标签，让结构生长](https://help.flomoapp.com/method/use-tag.html)（阅读需 4 分钟）
- [用回顾，持续刺激记忆](https://help.flomoapp.com/method/use-review.html)（阅读需 4 分钟）

第一次主动输出 -> 有规则组织输出成果 -> 第二次避免注意力重复投入 -> 有新认知能继续更新

形成 [习惯](习惯) -> 降低心智负担

## 它山之石

- obsidian 官方，obsidian 部署，[Obsidian 中文帮助 - Obsidian Publish](https://publish.obsidian.md/help-zh/)
- 在读博士 - 落山鸡，obsidian 部署，[Obsidian中文教程 - Obsidian Publish](https://publish.obsidian.md/chinesehelp)
- 后端程序员，群友，logseq 部署，[https://notes.singee.me](https://notes.singee.me/)
- 学生，群友，jekyll 部署，[骏豪的梦呓小站](https://notes.zustcv.fun)
- 设计师，obsidian 部署，[chi's memory - chi's memory - Obsidian Publish](https://publish.obsidian.md/chiux/chi's+memory)
- [2022-08-24](2022-08-24) 收录
	- sspai 作者，vuepress 部署，[LearnData 开源笔记 | LearnData-开源笔记](https://newzone.top/)
- [2023-03-21](2023-03-21) 更新
	- 网友，quartz 部署，[知识Cool😊](https://ob.tianzhongs.ml)  
[Quartz Showcase (jzhao.xyz)](https://quartz.jzhao.xyz/showcase)  
[Digital Garden - Publish Obsidian Notes For Free (ole.dev)](https://dg-docs.ole.dev/)
- [Knowledge - Nikita Voloboev](https://github.com/nikitavoloboev/knowledge) is the one that made me discover this concept, I really love the way he structure things.  
    [知识 - Nikita Voloboev](https://github.com/nikitavoloboev/knowledge)是让我发现这个概念的人,我真的很喜欢他组织事物的方式。
- [Maggie Appleton](https://maggieappleton.com/garden-history), mostly about second brain and productivity  
    [玛吉·阿普尔顿](https://maggieappleton.com/garden-history),主要关于第二大脑和生产力
- [Ness Lab - Anne-Laure LeCunff](https://nesslabs.com/), awesome articles about productivity, mindfulness, neurosciences...  
    [Ness Lab - 安-勒库夫](https://nesslabs.com/),关于生产力、正念和神经科学的优秀文章...
- [Joel Hooks](https://joelhooks.com/), various things, mostly about programming with a great manifesto on digital gardening  
    [乔尔·胡克斯](https://joelhooks.com/)，各种各样的事情,主要是关于编程,还有一篇很棒的关于数字园艺的宣言
- [Tynan](https://tynan.com/), I don't think Tynan will call he's blog a digital garden, but it's very close to. About investing and travels  
    [泰南](https://tynan.com/)，我不认为泰南会把他的博客称为数字花园,但这非常接近。关于投资和旅行
- [Notes - Andy Matuschak](https://notes.andymatuschak.org/About_these_notes), one of the most iconic digital garden. Mostly on software, ed-tech, research...  
    [笔记 - Andy Matuschak](https://notes.andymatuschak.org/About_these_notes),这是最具标志性的数字花园之一。主要关注软件、教育技术、研究等方面。
- [Paul Graham's notes](http://www.paulgraham.com/index.html), from one of the most iconic entrepreneurs.  
    [保罗·格雷厄姆的笔记](http://www.paulgraham.com/index.html)，来自最具标志性的企业家之一。


- [Nikita Voloboev's favorites  
    尼基塔·沃洛勃耶夫的最喜欢的](https://docs.google.com/spreadsheets/d/1KtEjnuZEHxUmoiA37_MMM4OFyQcbwVUaLBFa12P8cnU/edit#gid=0)
- [A digital gardeners spreadsheet  
    一个数字园丁的电子表格](https://docs.google.com/spreadsheets/d/1KtEjnuZEHxUmoiA37_MMM4OFyQcbwVUaLBFa12P8cnU/edit#gid=0)
- [Second-Brain list on Github  
    Github 上的第二大脑列表](https://github.com/KasperZutterman/Second-Brain)

## 过程容器

因此我通过 Obsidian 来写作，进行思考。笔记软件就是我思考过程的运行时载体，也就是思考的过程容器。

就像平时思考总会中断，或不完善。笔记库有很多笔记没写完整，或只是挖了个坑，待以后有新的机缘巧合可以引用、填充和迭代。生命不息，挖坑不止。

同时也是一个 [博客](博客.md) 的功能，在博客区输出一些东西，来对抗[知识诅咒](知识诅咒.md)。

[渐进式](渐进式.md)
