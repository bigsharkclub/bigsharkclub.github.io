---
title: 迟来的status ICO 总结
date: 2017-06-26 07:00:00
category: ICO
author: yuanchao
---

status 的 ICO 可谓是空前的火爆， status团队也是做足了充分的准备，使得大多数人都成功参与了ICO， 这次算是比较成功的一次ICO， 这篇文章我对status ICO 做一个简单总结。

 - 参数人数（地址数） **20405**
 - 历经 **4130** block   将近 **20** 小时
 - 大约 包含了 **65717** 笔交易
 - 总金额 **30万** Ether (非代投金额 176, 595 Ether)

鉴于之前BAT ICO 大户秒杀, status ICO 做了很多限制：
 
1. 动态 ceil 算法   （限制每次参投数量, 实际每次最多不超过40 ether）
2. gas price 限制（最多50Gwei， 限制通过提高手续费加速打包恶意插队）
3. 参投周期（成功参投之后过100个block才能再投， 大约25分钟）
4. 平台代投（通过imToken、ICOAge 等平台提前代投，将部分压力转移平台）

通过上面4点 限制了大户参投的难度， 使得大多数人都能够参投成功

对于第一点 动态ceil算法 大家可能都不太了解， 下面我给大家解释一下

### Status 动态limit

status 根据当前已经参投金额 计算出此次可以投的金额

将总众筹金额 176, 595 ether分为四个ceil， 每个ceil包含3个参数：**limit** （ceil 参投目标金额）、**slopeFactor** (斜率)、 **collectMinimum** (最小金额) ， 如下图所示：

![curevs](http://i1.buimg.com/1949/b618de40030914d2.png)
**maxCollected**列是我加的，这列是ceil内最大参投金额。

![Markdown](http://i1.buimg.com/1949/adf9356632d1c1bb.png)

**算法 :**
每次最多可投Ether数量 ***collected = Max(当前ceil剩余Ether / slopeFactor , collectMinimum)***

随着ICO人数越来越多 collected 越来越小 直到小于collectMinimum 进入下一个 ceil

具体每个ceil的数据是没有公布的， 提前半个小时status团队在合约里面进行了设置

发送的Ether小于 collected 都可以成功ICO， 大于 collected 部分成功，多余的ether 通过内部交易退回（在imtoken上看不到内部交易， 所以有的人说为什么交易成功了，怎么余额只少了一部分）


在ICO之前我通过ICO合约代码了解了这个规则，根据上面的规则，可以分析出应对策略： **多创建几个帐号（address）**, 将总金额平均分给几个address，保证每个address金额不是很高，不会再等100个block才能再投

多创建帐号就会增加操作的复杂度，忙不过来，容易搞错，这个时候我利用pairty的指定区块发送功能，提前设置好程序到指定区块的时候会自动发送，为了防止程序没有发送成功，每个帐号又分别准备了手动转账，设置好密码等到出块立即点发送。如果会写程序可以写个程序来做就很方便了。


**总结：**
Status ICO 显然是成功的，但是由于status 规则的复杂性，导致了以太网络的严重拥堵， 由于gas price 限制不能通过 gas price 提高来加速打包 反而导致交易失败 （正常的转账可以提高gas price 加速打包， 不是像之前一篇文章说的以太不满而堵）

近期以太坊上的ICO项目越来越多，在这种不正常的市场环境下， 以太坊网络不堪压力，显现出以太坊的性能瓶颈，以后ICO不断，以太坊智能合约应用也越来越多， 目前交易的处理速度需要大大提高

无论是ICO 还是以太坊，我们都在不断的尝试， 不断的改进

Vitalik Buterin 最近新增了一个 EIP提案 EIP648  https://github.com/ethereum/EIPs/issues/648  Easy parallelizability  简单并行化， 提高处理能力

接下来的大都会版本 会引入POS机制并逐渐替换到POW算法， 会大大提高交易的处理速度， 让我们拭目以待， 以太坊越来越好
