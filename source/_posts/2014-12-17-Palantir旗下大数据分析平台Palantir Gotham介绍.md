---
title: "Palantir旗下大数据分析平台Palantir Gotham介绍"
tags: ["其他"]
date: 2014-12-17
author: admin
mathjax: true
---

![img](http://www.cad.zju.edu.cn/home/vagblog/wp-content/uploads/2014/12/image25.png)

译者：36大数据编辑 原上草 **（36大数据专稿，本博客已获取本文转载授权）**

Palantir，提起这家公司就会让人觉得如雷贯耳。之前36大数据已经花了非常多的时间去收集和整理了关于这家公司背后的故事，参考揭秘：[曾用大数据帮助CIA干掉本·拉登的公司Palantir Technologies ](http://www.36dsj.com/archives/13425)，在2013年美国大数据公司收入排行榜中，Palantir排名第一。

[Palantir中国专区>>>](http://www.36dsj.com/archives/tag/palantir)

Palantir也被称为大数据行业的印钞机，它的客户包括美国国家安全局（NSA）、美国联邦调查局（FBI）、美国中央情报局（CIA）和很多其他的美国反恐和军事机构。那么，Palantir公司的大数据产品和技术又是怎么样的呢？带着这个问题，36大数据特别编译了Palantir官网上的产品资料，今天先放出上篇。

## **一、产品概述**

[英语原文>](https://www.palantir.com/palantir-gotham/)

**它如何运作**

**多源数据为起点**

各个机构都有各自的数据，它们中有很多是结构化数据，如日志文件，财务数据表和电子表格，还有一些是非结构化数据，如电子邮件，文件，图片和视频。这些数据通常情况下存储在分离系统中。每一天它们的类型都在迅速变化，体量都在呈指数性增长，并且变得越来越难以被利用。

机构内部看重这些数据的人并不是从它们有多少行，多少列，原始文本是什么，这些角度来思考它们的作用的，而是从当前本机构所负担的任务和面临的挑战来思考。他们需要一种方法，以此来探寻已有的数据，并且能用自己能理解的方式得到反馈。

**融合数据为人本模型**

通过与客户一起近距离的协作，我们的工程师能够摒除数据类型和数据容量带来的限制，将多个相关的源数据整合并绘制为简洁、一致的模型。

你可以设想一下这样的情景：这些数据一个字节、一个字节地涌入 Palantir Gotham 平台，在这里它们被转换为人群，地点，事物，事件以及他们相互之间的联系，这些有意义的实体和关系。

**标签，安全追踪所有数据**

这个模型一经建立后，数据流就会持续不断的流入Palantir Gotham 平台。与此同时，相应的安全守则也已建立，只有被授权用户才可登入。

这些数据的任何更新都会同步到平台，并且用户进行分析时，他们所有的行为都会被自动记录、归因分析和储存。

**人本驱动赋予数据活力**

用户可以通过建立在此平台上的各种综合性应用与数据进行互动。他们可以即刻搜索所有数据源，将数据关系可视化，探索不同的假设，发现未知的关系，揭示隐藏的模式，与同事分享自己的见解。

## **二、平台介绍**

平台后端集成了一系列功能，它们主要用来整合不同数据源以便于进行安全、协同的分析。

平台此时扮演着企业知识库的角色，收容着企业全部分析活动的所有记录。

**建模灵活性**

摒弃传统数据建模死板的行和列，Palantir Gotham利用数据建模时采用真实世界的实例如“人群”、“组织”，他们相关的特征以及相互之间的联系，这大大提高了建模的灵活性。

Palantir Gotham平台的数据模型，能快速定义和重定义数据，这让它被称为“动态本体”，同时也让整合不同来源的不同数据为一个整体成为可能，这个过程正符合人们对信息的自然设想。

**隐私和安全控制**

平台的架构一开始就设计了隐私保护功能，用来支持精确的数据处理，多层次的安全保护，完全性的审核。首先，被整合进平台的每个对象的每一项特性都和它的原始数据源相关联，这样准入限制就建立在每个属性的基础上（有时也被称为“次单元层级安全保护”）。

然后，用户会被分配给不同层级的准入许可，以此来管制他们与数据互动的权力。最后，所有用户和管理员与数据的互动行为都会被记录在一个防干扰的审计日志当中。

**合作**

版本控制数据库（The Revisioning Database）和Palantir Gotham平台的关联技术（Nexus Peering technology）让机构内部和机构之间的多个用户可以对同样的数据无缝、安全地进行合作性分析。Palantir Gotham平台支持多样性的合作，包括能突破跨越机构、功能、地域间限制的合作，连接安全模型和数据模型间的合作，连接低频、高延时下的不同网络、甚至卫星的合作；同时数据的安全性和完整性都有可靠的保障。

**可扩展性，可定制性，应用程序接口**

Palantir Gotham 平台每一层的堆栈都被设计成可扩展的：从底层数据集成、进口管道定制到用户界面，它都被设计成一个完全开放的平台。经由动态本体技术（Dynamic Ontology）整合的数据可以通过Java入口作为Palantir 对象（Palantir Objects）接入。这些数据同时也可以整体导出用于其它的框架和工具。

**知识管理**

所有被整合的数据都存储在Palantir Gotham平台的版本控制数据库 （Revisioning Database.）中。对数据对象的任何改动，不论是来自数据源还是产生自用户，都会被记录于其中。在概念上，版本控制数据库 （Revisioning Database.）与Git和其它分布式版本控制系统类似，它允许数据分析人员在个人沙箱中工作，这里留有各个修订版本的历史分支记录方便修改，工作完成才需要将发现提交给企业。

用户可以探索不同方向的推理想法，一路记录下每一步，并可以跳回他们探索过程中的早期节点。同时，数据分析者还可以在不丢失自己工作进度的情况下与他人分享自己的见解。这些便利条件会促成一个版本控制知识库的诞生。它将机构内不同分析者对数据的见解累积起来，并将之转换为数据。在未来，企业可以利用这些分析成果取得杠杆式飞跃。

**算法处理**

内置的算法功能自动将有趣的集群数据有序排列在使用者的面前，以供其检视，这样就提高了使用者理解大规模数据的能力。Palantir Phoenix 工具提供了编译和分析大规模数据集的功能，同时还提供了一个强大而灵活的框架用来实现该功能的自动化。非技术出身分析师也可以利用我们的种子框架（seed-generation framework）在不用写一行代码的情况下创作出一份精彩的成果。

**规模**

通过结合可伸缩的架构和联合数据库两者，我们平台可以处理P字节规模级别的数据。Phoenix 服务 扮演着数据仓库系统的角色，存储着大量结构性数据集，如日志文件，网络流量记录和交易数据。Raptor联合搜索服务（Raptor federated search server）保有大量非结构性文本数据，如文档，电子邮件和电报文件。这两种服务经由搜索功能和增强的查询助手功能的辅助极大提高了用户处理数据的便捷性。当用户向Phoenix 和 Raptor请求数据时，它们也同时被集成到RevDB供进一步分析。

## **三、应用程序**

Palantir Gotham平台前端提供了一整套的集成工具，这套工具在语义分析、时间分析、地理空间分析、全文分析方面均做了优化。用户可以将数据对象在不同应用之间拖放以获得流畅、全面的分析经验。

**图表**

图表应用可以视觉化数据对象间的语义关系。数据对象被以网络中的点和边界的形式形象地描绘出来。

过滤工具使用户可以深度探讨感兴趣的数据对象。图表应用具有时间线功能可以可视化事件顺序，还有时间轮功能能展示重复事件的周期和频率。综合性柱状图可以选出和过滤具有相同属性的数据对象，比如相同的地址，电话号码、城市或者相同领域名称。图表应用还具有将通讯数据、支付数据、船运数据及其他数据通过网络时的情况可视化的功能。

用户还可以通过调整图表中网络节点和边界的分布来可视化网络中的不同特点，例如层属关系。一套演示工具可以方便用户注释图表并提高他们在展示会议中图表的说服力。

**地图**

地图应用程序提供地理空间分析功能。它将地图中的对象基于地理位置进行可视化，提供直方图，时间线、时间轮这些可视化形式。可视化热点图阐释了一幅地图上关注对象的密度。在地图中的意象是完全可插入式的，可以实现不同来源意象的的转换，整合自有的意象，通过联合两个或两个以上的意象创建复合的意象集。

标记语言和电子地图文件可以作为独立地图层导入，并且这些图层包含的特征点可以被用作选择和过滤具有相似特征（如一个县，人口普查点，州）的对象。图层可以根据其包含的数据进行计算的结果来着色和加标签。

**对象资源管理器**

对象资源管理器应用程序允许用户在大规模数据集中根据自己关注点进行深入挖掘。在Palantir 具有的地平线技术（Horizon technology）的支持下，对象资源管理器应用程序允许分析人员定义一系列过滤器并将之运用在数以十亿计的数据对象中，以此得到值得关注的下层数据，它们可以被其它的Palantir Gotham应用程序进行分析，例如图表应用程序或者地图应用程序。

**浏览器**

在浏览器应用程序内，用户可以查看数据并可将结构性的性质应用于非结构文件中。在浏览器读取原始文本时，用户可以“标记”特定文字，从而将一个文件与动态本体（Dynamic Ontology）中的某一个或者某一些特定对象联系起来，使这些数据能够在其他Palantir Gotham应用程序中得到分析。

**移动端**

Palantir 移动平台将Palantir Gotham的作用范围扩大到实时领域。像灾后人道主义救援响应和联合执法行动这些实时活动，它们行动分散需要进行统一，数据收集面临着环境变化迅速的挑战。Palantir 移动平台的客户端在安卓和IOS两种系统上均能运行，这让它能实现现场工作人员和基地人员的实时合作。移动平台用户可以整理现场报告，上传照片和视频，记录小组成员位置，并且搜索和利用整合在Palantir Gotham平台上的数据。

## **四、技术**

Palantir Phoenix技术是一种集群式的数据存储技术，支持在P字节规模的数亿万亿计的数据记录中进行亚秒级别的查询。利用Phoenix技术可以使其他一些开源技术在处理大规模数据和进行高级分析时达到杠杆效率。

The Palantir Raptor技术支持对外部数据源的就地联合查询。它利用动态方法完成数据集成。当一次联合查询被确认为Raptor技术的查询时，此记录会被就地转移到版本控制数据库中（Revisioning Database）

The Palantir Gotham平台搜索技术可对平台中的所有数据，不论是结构化数据还是非结构化数据，进行全文查询。

Horizon技术是由Palantir创建的内存数据库，用来对引导大规模数据下工作流的交互作用。Horizon技术使分析人员能查询数十亿级的对象并在10秒内得到结果。它创建于2009年，与 Apache Spark™在设计上相似。Horizon技术作为支撑Palantir Gotham对象浏览器（Object Explorer）关键技术，让分析人员把大数据过滤为一些方便管理的次级数据以供进一步详细分析。

Palantir Gotham 中的动态本体（Dynamic Ontology）是一种定义灵活，基于对象的数据模型，这个特点使它能将来源多样化的数据整合在一起，并将存储的原始数据格式转化为Palantir Gotham上使用的数据对象格式。此种格式表示的是现实世界中的人、地点、事物、事件及彼此间的关系的特性。不同的机构对现实情境有着不同的认识，需要不同的模型。这些模型随着时间而改变，因而动态本体的具体含义也就在现实的基础上不断重塑，并且会跟着新数据源一起增减，甚至会重新概念化。Palantir Gotham平台上这些灵活而统一的数据模型能极大地简化数据整合的过程。以往企业多年才能完成的数据整合项目，现在只要几周时间便可完成。

**版本控制数据库技术**

版本控制数据库技术（The Revisioning Database）简称为RevDB，为Palantir Gotham技术提供了持续稳定的数据存储能力。它增强了平台的访问控制，审计，知识管理和协同工作能力。此中所有数据都附有它们的历史信息，包括创建和修改日期，创建和修改者身份，数据来源地以及数据自身的安全设定和访问限制。这些原资料都可以被客户接触，使用户能够获得背景信息丰富的条件下的分析经验，并且可以保证不同权限用户间的合作安全和不同分析方式用户间的合作安全。广泛的原始资料，可靠的安全规范和完善的版本控制，这些条件可以使不同用户对给定的数据对象从不同角度进行审视，同时也维持着数据的完整性。

AtlasDB是版本控制数据库（Revisioning Database）的数据存储器。它既具有现代分布式非关系型数据库的简洁性和可扩展性，也具有传统关系型数据库的保证数据交易安全和相容性高的特点。AtlasDB菜单处理ACID（指数据库事务正确执行的四个基本要素的缩写）的兼容性方面远高于key-value分布式存储系统。AtlasDB在底层的程序界面便注重了便捷性和可插入性，这使它既可以处理数据库级别的数据要求也可以处理笔记本级别的数据要求同时保持良好的性价比。

Palantir Gotham是一个分布式系统，而Nexus Peered网是它的一个实例，也就是一个分布式系统的分布式系统。每一个Palantir Gotham平台的实例在RevDB中都包含自己的”nexus’数据。一个”nexus”可以包含Palantir Gotham平台实例通过同步或者”peering”产生的数据和分析。Nexus Peering技术通过捕获、循环、融合数据变动实现Palantir Gotham 实例的数据共享。不能解决的冲突性变化会留待人工解决并会以图解的形式展现在界面上。Nexus Peering技术可以在保证实例间的稳定状态的同时实现动态本体的多样化和控制权限制度的多样化。我们开发Nexus Peering技术的目的便在于使不同机构，不同功能部门，不同地域使用者之间能安全地分享数据和合作式的分析数据。

**36大数据原文链接：http://www.36dsj.com/archives/18430**

End.