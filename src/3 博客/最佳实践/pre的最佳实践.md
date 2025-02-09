---
draw:
title: pre的最佳实践
tags: [最佳实践]
date created: 2024-04-09
date modified: 2024-12-27
---

excerpt

<!-- more -->

- pre 准备，其实第一优先级的是自我逻辑，因为这会极大影响现场发挥的状态，一个事情换一百种方式讲给别人中，留下的大家认识的子集是一次 pre 的底色，其他的临场因素是能出彩的点。
- 复杂问题的讲解，是否可以 demo 先行，抽象后行。
- 意识到组内周会【RDQA 结果介绍】部分的重要性，这是感知行业动态，熟悉产品策略的一个很好的机会。
- 在完成需求的时候，新增的逻辑如果仅仅通过 if~else 来完成，虽然可以降低风险、快速完成需求，但是会带来代码的冗余性，逻辑不够简洁，长此以往代码就变的晦涩难懂、排查问题难度加大。如果遇见以前老代码存在不和合理或者新增逻辑后不能够很好的适配，在 排期时间内可以进行小范围的重构，简洁明了的代码是靠大家日常工作中共同维护的。并且重构的过程也是锻炼自己思考和创新的过程。期待后续的需求你能自己发现代码的优化点并实现，加油！在导师的帮助下重构了【FD-208543 变价消息支持 seq】的代码，使得这次新增逻辑的改动范围更加容易测试和定位，减少了代码的冗余。
- 这周有一个对于日报的思考，起因是发现一些曾经学习过的，甚至当天写在日报里的东西，过了一段时间后自己还是忘了，甚至翻找都很麻烦。我想底层的原因是日报天然的独立性，不太容易增量地呈现信息。对于某时刻的状态来说，可能过去日报的有些信息成了 nonsense 的东西，而另一些当时的心得经验由于没有及时地复习和框架性地归纳白白流失。自己过去每天发完邮件会把自己的日报更新到 wiki，所以决定改进一下自己的这个动作，变为增量更新。只是 merge 进去一些新东西，减少工作量的同时，保证了定期的回顾和思考，利用好自己产出的信息。
- 解决需求时，实践了培训中学到的最小 commit 原则，尽可能细地拆分任务，让每一个最小单元的动作十分清晰，同时将 commit 维度也与其对齐，保证 commit message 的规范。好处是在任务执行中，对于之前的操作都能及时定位和 undo，今天的需求中有大量的 replace，涉及的监控埋点比较多，不是很清楚替换逻辑时，利用这个方法提高了出现 undo 时的解决效率。
- 名与实的距离，领域知识的理解和代码实现之间存在一定的鸿沟，当我们用自然语言表述一件事时往往存在语义上的含糊，甚至代码中变量与方法的取名也是如此，代码的准确性无非来自于每个变量和方法被逻辑门牢牢卡在了一个地方，才有了所谓逻辑上的清晰边界。如何减少这个鸿沟，似乎是软件开发一个永恒的话题。从实践上来讲，个人感觉比较好操作的是两方面，一是不吝啬于编码中取名的长度，赋予更准确、贴合领域知识的命名。二是保持代码和注释的同步更新，不让注释腐化。
- 个人提效上，作为一个程序员，我觉得应该具有天然的对重复的警觉性，任何的操作（无论是工作向还是个人向），如果有五次以上的重复，都应该考虑做工具提效了，希望自己能做好这一点，并在这个过程中了解其他语言或者工具，保持技术上的开放性。
