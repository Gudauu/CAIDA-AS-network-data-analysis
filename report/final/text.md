## 一 标题
## 二 摘要
## 三 引言
该论文旨在通过对网络的自治系统 (Autonomous System, 缩写 AS) 级别关系构成的图分析，深入探讨自治系统网络技术和经济方面的相关性。准确了解自治系统业务关系对于互联网的域间结构的技术和经济方面都具有弥足重要意义。首先，自治系统之间的关系决定了路由策略，这为互联网流量路径引入了一组非平凡的约束条件。这对网络的鲁棒性、流量工程、宏观拓扑测量策略以及其他研究和运营考虑都有影响。其次，对自治系统间关系的宏观分析不仅可以揭示当前互联网商业实现的经济基础，而且还为基于经济的互联网拓扑演化建模提供了一个坚实的验证框架。实际上，互联网自治系统级别的拓扑和其演化动态都是互联网参与者做出的商业决策的结果。因此，推断AS之间的关系是理解和建模驱动互联网拓扑及其层次结构演化的经济力量的有前途的工具。
由于自治系统研究对于互联网生态的重要性，不同学科，组织均对这一课题进行过研究。较早的研究如<Analysis of the Autonomous System Network Topology>，文章中研究者使用的是一个较为流行的数据集:NLANR组织收集和维护的BGP路由表信息。他们通过解析路由表得到自治系统数据，基于此剖析了1994至2000年自治系统的拓扑结构特点，收集得到了一系列符合幂定律(power-law)的统计学特征。较新的研究有<Research on Topology Evolution of Autonomous System Network>，基于与前述类似的数据处理方法，这篇文章覆盖了2000-2020年的自治系统网络分析结果，得到了网络发展演变逻辑方面的若干结论，并对于国家级别的拓扑逻辑进行了分析。除了宏观层面的网络分析外，亦有文章如<Evolution of the Internet AS-level topology: From nodes and edges to components>从底层案例出发，生动地阐述了自治系统偏低层构成部份的行为特征。
以上若干文章的数据初始形态均为原始BGP路由数据，研究者对其进行处理后方得到自治系统层面数据，因此带来因数据处理而生的不确定性，这对结果的验证，其他研究者对其实验的复现均带来了额外的难度。在本篇论文中，使用的数据集直接为处理后的自治系统关系数据，因而相较于前述研究去除了这份不确定性。此外，前述论文均主要针对自治系统的网络特性，即连通性特征进行研究，着眼于宏观的拓扑结构，或部件间的互连指标。而对于自治系统的贸易特征，亦或没有提及，亦或加以淡化。本篇论文则以自治系统的贸易关系为着眼点，从数据处理到模型建立，均致力于从利益、贸易角度探索规律，在需要时也兼顾部分网络特征研究。同时，由于本篇论文成文时世界各国已完整经历新型冠状病毒疫情对经济、政治等领域的影响，研究中也涉及疫情对于自治系统贸易演变的影响分析。
本篇论文主题部分将采用如下结构:
1. 对数据集的介绍（包括所述机构，收集方法，时间段，以及自治系统推演算法）
2. 实验环境（机器，编程语言，画图语言）
3. 数据总览
4. 宏观网络演变分析
5. 自治系统层级的实例分析
6. 以国家为单位的聚合分析
7. 新冠疫情的影响分析及启示

## 四 背景
互联网由成千上万个互联网服务提供商(ISP)组成。这些运营商拥有和控制自己名下的自治系统，构成BGP中的基础单位。ISP间存在沟通交流，以便协同和普遍地路由互联网流量，而这种沟通交流最终通常以商业协议的形式展现在网络中。这些商业协议的出发点可能来自利益链、政治因素等等，落实在协议内容中则成为网络中人为引入的路由规则。正因这类政策的存在，自治系统间的网络路由才变得复杂，不定，和难以预测。
研究自治系统间的关系，对BGP协议，对互联网的发展，都有重要意义。通过对它的研究，我们可以找到现有路由机制的弊端从而优化网络路径;我们可以通过评估自治系统关系对网络基础设施的影响，来构建更有扩展性的互联网增长模型架构;也可以通过它对现有同行和上游服务商的表现进行评估，从而帮助服务商进行选择。
然而，出于隐私，商业机密等等考虑，直接研究自治系统被证明是非常困难的，因为迄今为止并没有服务商或第三方机构提供公开透明的自治系统协议数据。这些数据只有参与协议运营商知晓。因此，在无法直接获得自治系统数据的情况下，研究者转而选择使用可以公开收集到的BGP路由数据，用算法处理后得到计算出的自治系统贸易数据。关于这类算法的研究最早

## 五 实验
## 六 结论
## 七 参考

### 数据集
这篇论文所采用的数据集是