# 短周期多因子阿尔法选股策略
## 目标
2015年底 WorldQuant(世坤投资)发布了***WorldQuant Formulaic 101 Alphas***[1]，2017年6月15日国泰君安证券发表了[***基于短周期量价特征的多因子选股体系***](https://github.com/SelenaMa9812/Guotai-Junan-191-Alpha/blob/main/files/%E5%9B%BD%E6%B3%B0%E5%90%9B%E5%AE%89%EF%BC%8D%E5%9F%BA%E4%BA%8E%E7%9F%AD%E5%91%A8%E6%9C%9F%E4%BB%B7%E9%87%8F%E7%89%B9%E5%BE%81%E7%9A%84%E5%A4%9A%E5%9B%A0%E5%AD%90%E9%80%89%E8%82%A1%E4%BD%93%E7%B3%BB.pdf)，构造并运用191个短周期阿尔法因子搭建多因子选股策略。

因子生成过程基本上实现了自动化，产生的因子数量可以达到几十万甚至数百万，101 Alphas只是揭示了能够用显式公式表示的少量因子，国泰君安191 Alphas则是针对短周期量价构造的因子。

由于因子的数量庞大、市场参与者众多，单个因子的回测表现往往是失效的，因此我的研究目标在于找到**多因子的有效选股策略**。

### 短周期量价因子
短周期量价因子，属于市场情绪类因子，从股票的日线数据出发，根据墨菲的***股票/期货市场技术分析***所描述的股价波动规律，进一步构造技术指标衍生因子。比如：动量、反转、开盘缺口、量价背离、成交量放大等。技术分析流派认为某些特定形态描述了投资者的行为，可以甄别未来走势。短周期意味着，这类因子利用过去较短的日线数据构建，所以对未来短期1~5日有预测作用。研报中指出很多国外量化机构通过大量构造因子，来实现策略盈利。

### Alpha 模型


多因子模型相对于单因子模型，可以实现自动内部交叉交易的红利（从而对节省交易成本等盈利能力至关重要）、阿尔法投资组合多样化（对冲阿尔法的任何子集在任何给定的时间段内破产），等等组合alphas的挑战之一是通常的“变量太多，观测值太少”困境。因此，alpha样本协方差矩阵是严重奇异的。







### 参考文献/研报
[1] Zura Kakashadze. 101 Formulaic Alphas[J]. Wilmott,2016,2016(84).
