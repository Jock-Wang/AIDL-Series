![default](https://user-images.githubusercontent.com/5803001/44629093-c753d900-a97c-11e8-8c16-9d0e96b149aa.png)

# 人工智能与深度学习实战

在本系列中，你可能会接触到数据挖掘、机器学习、深度学习、自然语言处理、人工智能等很多的概念。最后，如果你想了解数据结构与传统算法，那么可以参考[数据结构与算法](http://ngte-se.gitbook.io)。

值得说明的是，鉴于很多的算法实现是以文字结合代码介绍为最佳，因此工具实践篇中的大部分内容是以 Juypter Notebook 的形式放在该仓库中，并且在 Colab 中进行浏览、编辑与实验。

# Preface | 前言

1956 年，几个计算机科学家相聚在达特茅斯会议，提出了“人工智能”的概念，梦想着用当时刚刚出现的计算机来构造复杂的、拥有与人类智慧同样本质特性的机器。2012 年以后，得益于数据量的上涨、运算力的提升和机器学习新算法（深度学习）的出现，人工智能开始大爆发。

![](https://i.postimg.cc/26CpMVQK/image.png)

机器学习是一种实现人工智能的方法，机器学习最基本的做法，是使用算法来解析数据、从中学习，然后对真实世界中的事件做出决策和预测。与传统的为解决特定任务、硬编码的软件程序不同，机器学习是用大量的数据来“训练”，通过各种算法从数据中学习如何完成任务。机器学习直接来源于早期的人工智能领域，传统的模型算法包括决策树、聚类、贝叶斯分类、支持向量机、EM、Adaboost 等等。从任务类型上来分，机器学习算法可以分为监督学习（如分类问题）、无监督学习（如聚类问题）、半监督学习、集成学习和强化学习的等。传统的机器学习算法在指纹识别、基于 Haar 的人脸检测、基于 HoG 特征的物体检测等领域的应用基本达到了商业化的要求或者特定场景的商业化水平，但每前进一步都异常艰难，直到深度学习算法的出现。

1. 弱人工智能Artificial Narrow Intelligence (ANI): 弱人工智能是擅长于单个方面的人工智能。比如有能战胜象棋世界冠军的人工智能，但是它只会下象棋，你要问它怎样更好地在硬盘上储存数据，它就不知道怎么回答你了。

2. 强人工智能Artificial General Intelligence (AGI): 人类级别的人工智能。强人工智能是指在各方面都能和人类比肩的人工智能，人类能干的脑力活它都能干。创造强人工智能比创造弱人工智能难得多，我们现在还做不到。Linda Gottfredson教授把智能定义为“一种宽泛的心理能力，能够进行思考、计划、解决问题、抽象思维、理解复杂理念、快速学习和从经验中学习等操作。”强人工智能在进行这些操作时应该和人类一样得心应手。

3. 超人工智能Artificial Superintelligence (ASI): 牛津哲学家，知名人工智能思想家Nick Bostrom把超级智能定义为“在几乎所有领域都比最聪明的人类大脑都聪明很多，包括科学创新、通识和社交技能。”超人工智能可以是各方面都比人类强一点，也可以是各方面都比人类强万亿倍的。超人工智能也正是为什么人工智能这个话题这么火热的缘故。

深度学习是一种实现机器学习的技术，深度学习本来并不是一种独立的学习方法，其本身也会用到有监督和无监督的学习方法来训练深度神经网络。最初的深度学习是利用深度神经网络来解决特征表达的一种学习过程。深度神经网络本身并不是一个全新的概念，可大致理解为包含多个隐含层的神经网络结构。为了提高深层神经网络的训练效果，人们对神经元的连接方法和激活函数等方面做出相应的调整。其实有不少想法早年间也曾有过，但由于当时训练数据量不足、计算能力落后，因此最终的效果不尽如人意。深度学习摧枯拉朽般地实现了各种任务，使得似乎所有的机器辅助功能都变为可能。无人驾驶汽车，预防性医疗保健，甚至是更好的电影推荐，都近在眼前，或者即将实现。

第一阶段（20 世纪50 年代中期到80 年代初期）：深耕细作，30 年技术发展为人工智能产业化奠定基础。在1956 年之前，人工智能就已经开始孕育。神经元模型、图灵测试的提出以及SNARC 神经网络计算机的发明，为人工智能的诞生奠定了基础。1956 年的达特茅斯会议代表人工智能正式诞生和兴起。此后人工智能快速发展，深度学习模型以及AlphaGo 增强学习的雏形——感知器均在这个阶段得以发明。随后由于早期的系统适用于更宽的问题选择和更难的问题时效果均不理想，因此美国、英国相继缩减经费支持，人工智能进入低谷。

第二阶段（20 世纪80 年代初期至21 世纪初期）：急功近利，人工智能成功商用但跨越式发展失败。80 年代初期，人工智能逐渐成为产业，第一个成功的商用专家系统R1 为DEC 公司每年节约4000 万美元左右的费用。截止到20 世纪80 年代末，几乎一半的“财富500 强”都在开发或使用“专家系统”。受此鼓励，日本、美国等国家投入巨资开发第5 代计算机——人工智能计算机。在90 年代初，IBM、苹果推出的台式机进入普通百姓家庭中，奠定了计算机工业的发展方向。第5 代计算机由于技术路线明显背离计算机工业的发展方向，项目宣告失败，人工智能再一次进入低谷。尽管如此，浅层学习如支持向量机、Boosting 和最大熵方法等在90 年代得到了广泛应用。

第三阶段（21世纪初期至今）：量变产生质变，人工智能有望实现规模化应用。摩尔定律和云计算带来的计算能力的提升，以及互联网和大数据广泛应用带来的海量数据量的积累，使得深度学习算法在各行业得到快速应用，并推动语音识别、图像识别等技术快速发展并迅速产业化。2006年，Geoffrey Hinton和他的学生在《Science》上提出基于深度信念网络（Deep Belief Networks,DBN）可使用非监督学习的训练算法，使得深度学习在学术界持续升温。2012年，DNN技术在图像识别领域的应用使得Hinton的学生在ImageNet评测中取得了非常好的成绩。深度学习算法的应用使得语音识别、图像识别技术取得了突破性进展，围绕语音、图像、机器人、自动驾驶等人工智能技术的创新创业大量涌现，人工智能迅速进入发展热潮。

不同的模型、策略、算法的搭配，不断地推动着人工智能的发展，其又可以被分为三个阶段：计算智能、感知智能和认知智能。

- 第一阶段的计算智能即快速计算和记忆存储，像机器人战胜围棋大师，靠的就是超强的记忆能力和运算速度。人脑的逻辑能力再强大，也敌不过人工智能每天和自己下几百盘棋，通过强大的计算能力对十几步后的结果做出预测，从这一角度来说，人工智能多次战败世界级围棋选手，足以证明这一领域发展之成熟。

- 第二阶段的感知智能，即让机器拥有视觉、听觉、触觉等感知能力。自动驾驶汽车做的就是这一方面的研究，使机器通过传感器对周围的环境进行感知和处理，从而实现自动驾驶。感知智能方面的技术目前发展比较成熟的领域有语音识别和图像识别，比如做安全领域人脸识别技术的 Face++，以成熟的计算机视觉技术深耕电商、短视频等领域的 Yi+，能够对多种语言进行准确识别翻译的科大讯飞等。

- 第三阶段的认知智能就是让机器拥有自己的认知，能理解会思考。认知智能是目前机器和人差距最大的领域，因为这不仅涉及逻辑和技术，还涉及心理学、哲学和语言学等学科。

# Home & More | 延伸阅读

![](https://i.postimg.cc/CMDmg2SQ/image.png)

您可以通过以下导航来在 Gitbook 中阅读笔者的系列文章，涵盖了技术资料归纳、编程语言与理论、Web 与大前端、服务端开发与基础架构、云计算与大数据、数据科学与人工智能、产品设计等多个领域：

- 知识体系：《[Awesome Lists | CS 资料集锦](https://ngte-al.gitbook.io/i/)》、《[Awesome CheatSheets | 速学速查手册](https://ngte-ac.gitbook.io/i/)》、《[Awesome Interviews | 求职面试必备](https://github.com/wx-chevalier/Awesome-Interviews)》、《[Awesome RoadMaps | 程序员进阶指南](https://github.com/wx-chevalier/Awesome-RoadMaps)》、《[Awesome MindMaps | 知识脉络思维脑图](https://github.com/wx-chevalier/Awesome-MindMaps)》、《[Awesome-CS-Books | 开源书籍（.pdf）汇总](https://github.com/wx-chevalier/Awesome-CS-Books)》

- 编程语言：《[编程语言理论](https://ngte-pl.gitbook.io/i/)》、《[Java 实战](https://ngte-pl.gitbook.io/i/java/java)》、《[JavaScript 实战](https://ngte-pl.gitbook.io/i/javascript/javascript)》、《[Go 实战](https://ngte-pl.gitbook.io/i/go/go)》、《[Python 实战](https://ngte-pl.gitbook.io/i/python/python)》、《[Rust 实战](https://ngte-pl.gitbook.io/i/rust/rust)》

- 软件工程、模式与架构：《[编程范式与设计模式](https://ngte-se.gitbook.io/i/)》、《[数据结构与算法](https://ngte-se.gitbook.io/i/)》、《[软件架构设计](https://ngte-se.gitbook.io/i/)》、《[整洁与重构](https://ngte-se.gitbook.io/i/)》、《[研发方式与工具](https://ngte-se.gitbook.io/i/)》

* Web 与大前端：《[现代 Web 开发基础与工程实践](https://ngte-web.gitbook.io/i/)》、《[数据可视化](https://ngte-fe.gitbook.io/i/)》、《[iOS](https://ngte-fe.gitbook.io/i/)》、《[Android](https://ngte-fe.gitbook.io/i/)》、《[混合开发与跨端应用](https://ngte-fe.gitbook.io/i/)》

* 服务端开发实践与工程架构：《[服务端基础](https://ngte-be.gitbook.io/i/)》、《[微服务与云原生](https://ngte-be.gitbook.io/i/)》、《[测试与高可用保障](https://ngte-be.gitbook.io/i/)》、《[DevOps](https://ngte-be.gitbook.io/i/)》、《[Node](https://ngte-be.gitbook.io/i/)》、《[Spring](https://github.com/wx-chevalier/Spring-Series)》、《[信息安全与渗透测试](https://ngte-be.gitbook.io/i/)》

* 分布式基础架构：《[分布式系统](https://ngte-infras.gitbook.io/i/)》、《[分布式计算](https://ngte-infras.gitbook.io/i/)》、《[数据库](https://ngte-infras.gitbook.io/i/)》、《[网络](https://ngte-infras.gitbook.io/i/)》、《[虚拟化与编排](https://ngte-infras.gitbook.io/i/)》、《[云计算与大数据](https://ngte-infras.gitbook.io/i/)》、《[Linux 与操作系统](https://ngte-infras.gitbook.io/i/)》

* 数据科学，人工智能与深度学习：《[数理统计](https://ngte-aidl.gitbook.io/i/)》、《[数据分析](https://ngte-aidl.gitbook.io/i/)》、《[机器学习](https://ngte-aidl.gitbook.io/i/)》、《[深度学习](https://ngte-aidl.gitbook.io/i/)》、《[自然语言处理](https://ngte-aidl.gitbook.io/i/)》、《[工具与工程化](https://ngte-aidl.gitbook.io/i/)》、《[行业应用](https://ngte-aidl.gitbook.io/i/)》

* 产品设计与用户体验：《[产品设计](https://ngte-pd.gitbook.io/i/)》、《[交互体验](https://ngte-pd.gitbook.io/i/)》、《[项目管理](https://ngte-pd.gitbook.io/i/)》

* 行业应用：《[行业迷思](https://github.com/wx-chevalier/Business-Series)》、《[功能域](https://github.com/wx-chevalier/Business-Series)》、《[电子商务](https://github.com/wx-chevalier/Business-Series)》、《[智能制造](https://github.com/wx-chevalier/Business-Series)》

此外，你还可前往 [xCompass](https://wx-chevalier.github.io/home/#/search) 交互式地检索、查找需要的文章/链接/书籍/课程；或者在 [MATRIX 文章与代码索引矩阵](https://github.com/wx-chevalier/Developer-Zero-To-Mastery)中查看文章与项目源代码等更详细的目录导航信息。最后，你也可以关注微信公众号：『**某熊的技术之路**』以获取最新资讯。

# About

![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg) ![](https://parg.co/bDm)

笔者所有文章遵循[知识共享 署名-非商业性使用-禁止演绎 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh)，欢迎转载，尊重版权。

![default](https://i.postimg.cc/y1QXgJ6f/image.png)
