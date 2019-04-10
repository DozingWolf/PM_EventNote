# PM_EventNote
写个项目事件记录工具

## 对，没错，我又开了个坑
你们咬我啊～～～

啊哈哈哈哈～～～

## 为什么要做这个东西
我是一个PM，兼职敲敲代码写写SQL。

做项目，免不了和三教九流的人打交道。可能年纪比较轻PM道行比较浅，时常会被一些四六不着调的家伙气得半死。

不是做了这个没汇报造成项目组干等，就是忘了执行某些任务所有人等他，诸如此类等等。

还有理解错，听错，看错，各种错。

总言而之最后整个项目进度被各种各样的问题延期。

虽然问题往往都不是PM所造成，但是作为一个有节操有理想的PM，实在受不了。

私下花了一点时间也和几个项目组里的同事聊过，有的时候因为公司并行项目实在太多，确实忘记了。

也有的时候是因为这个同事也不知道他的前置任务完成得如何，又不善于打交道或者前置任务的执行人也很忙没有交代，就搁置下来了。

更多的时候是在执行的时候发现这个事件已经牵一发而动全身，关联关系复杂，怕了。

作为一个PM，我只能请相关同事不畏艰辛去多交流多沟通。

但反过来作为一个敲代码的IT，我也觉得有时候繁杂的事情涌过来，了无头绪，实在也很郁闷。

突然有一天洗澡时想到(*对，没错，伟大的想法都诞生于————澡堂子*😂)，如果一个项目能够构成知识图谱，那应该会很容易吧？

以前学PMP时，我们讲究要记录风险，记录干系人，记录各种各样的资料形成各种各样的过程资产。

那是不是能把这些资料也记录到知识图谱中？

再由此及彼想到，项目中大部分要执行的事件都是有前驱事件和后继事件的(当然结束没有后继事件)。有前驱有后继就代表所有的事件都是有先后顺序而不是乱序的。

抽象整理后一个项目理论上应该是一棵树形结构(不存在有两个项目发起节点的项目吧？🧐暂时没碰到过，哪位PM同学碰到过可以告诉我下是什么类型的项目会有多个发起节点，多谢)。

再进一步，我们少许简化，可以在更小的尺度上把关系简化到一个链表。也就是一个项目的发起是链表表头，项目中的一切事务都会这个链表上的有序节点。

此时，我所说的“项目”可能更像通常意义上说的项目中的“工作包”。

当我们有了工作包，让我们稍微开阔一下视野，回到传统意义上的“项目”中来。这个时候我们就可以把前期的“工作包”通过树形结构形成一个明确的前后顺序关系，也就是形成了PMP所说的“项目”。

这样就可以把相对复杂的图形结构转化成相对简单的树形结构。

**当然了，PM脑子里面还是需要始终牢记，这个项目是个图，是个图，是个图。**🤣

## 准备怎么做这个东西

其实按照上面的分析思路，最小单位都是链表的话，用RDBMS就能做了。

但是呢，最近玩腻RDBMS了，准备玩点没玩过的。同时考虑可靠性，就看上非关系库BerkeleyDB了。

前期已经在一个小项目里面使用过一次BerkeleyDB，使用起来也算是比较简单方便。估计后期最大的问题会是我极其缺乏NOSQL数据库的设计经验。

不过这也算是我开这个项目的一个初衷了，学习一下NOSQL。

那数据持久化方面的方案可以确定了。

程序代码方面，我不是个专业的敲代码IT，也就只会些简单的。所以决定使用Python进行代码工作。

Python在前期也已经在几个小项目中应用过，写得不好但也还算能实现功能。

前端方面，实在是苦手。从大学毕业我就再也没有碰过前端代码，实在是不知道要用什么来做前端，思量再三决定先放弃前端，用Python把中台代码先构建出来。有必要的话，也可以先使用Py_wxFromeBuilder画一个窗体界面。

或者我也考虑把前端的工作交给其他更专业的IT来进行————毕竟，我还有PM的事情要做呢😣。

## 时间

准备慢慢做了，就和之前做微信项目一样，反正也是自己的私人项目，有学习到好玩的东西都会在这边用用看。

也很有可能会写完大部分代码后突然全部重构(就和微信项目的代码一样，初期写的代码基本全部被我自己重构了)。

这个项目就作为学习敲代码的一个见证吧。

以上～
