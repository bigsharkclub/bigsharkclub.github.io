---
title: 每周以太坊 - 第二十一期
date: 2017-06-19 23:02:05
category: 周报
author: MakoShan
---

# 热点
- 花了两个晚上翻译了 Vitalik 写的众筹模式分析，V 神写到文章信息量巨大，大家需要一点时间消化一下巨量信息。[众筹模式分析（第一部分)](http://ethfans.org/makoshan/articles/456) [众筹模式分析（第一部分)](http://ethfans.org/posts/458)
- [绘制未来去中心化的世界](http://ethfans.org/posts/461)
- [Vitalik：我完全没有贬低或唱衰比特币的想法，相反，我希望它能一直火下去。毕竟中本聪始终是加密货币之父。](https://file.xiaomiquan.com/201706/33b777c2b69e7ae7ef669bef89aeed6a0649b9ed0915cd4211713f8e2e1b4f7c.jpg)
- [基于IPO经济理论模型对目前ICO的理论研究和分析](http://ethfans.org/dragon/articles/462)

# 协议
- [Sharding 介绍脑图](https://www.mindomo.com/mindmap/sharding-d7cf8b6dee714d01a77388cb5d9d2a01)
- [Parity 1.6.8版本](https://github.com/paritytech/parity/releases/tag/v1.6.8)发布
-  [什么Oracle ？以太坊智能合约是在 EVM （以太坊虚拟机）中执行的，EVM 是个封闭的环境，换句话说，合约没法获取外部世界的任何信息，这个特性大大限制了DApp的发展，所以有人引入了预言机（Oracle）的概念，让智能合约能够透过 Oracle 取得外部信息，让合约调用外部 Web API 取得所需资料。](https://medium.com/taipei-ethereum-meetup/oracle%E7%B3%BB%E5%88%97%E4%B8%80-human-oracle-cb7ed8268030)
- [lightning-li ：  IC3有一篇论文Town Crier，讲得是利用Intel SGX 可信硬件实现对链上合约授权认证的数据喂养。链接：http://www.initc3.org/files/tc.pdf，解决了Oraclize 需传送大量数据给合约导致消耗大量gas的缺点。IC3是一个很牛的针对区块链的学术研究机构，包括 bitcoin-ng、honey badgerBFT等著名论文。近期也释放了针对以太坊合约的oracle alpha 服务，见链接链接：Announcing The Town Crier Service](http://hackingdistributed.com/2017/06/15/town-crier/)
- [开发者预览版即将发布，雷电网络的基本理念是，用户可以私下交换转账签名消息，而不是所有的交易都放到的区块链上处理。参与者越多，雷电网络处理转账能力越高（可以实现每秒1000000+笔转账）。](https://github.com/raiden-network/raiden/issues/653)


# 读书
[《价值起源》一本介绍世界金融史的金融入门书，我们所看到的证券、金融合约这些产品是什么时候在哪里起源的？他们是在什么样的历史条件下产生的？读史更好的理解现代金融创新。对这本书有兴趣的可以联系，图书漂流，邮寄传阅。](https://book.douban.com/subject/4882119/)

# 开发
- Yoichi博士的[以太坊合约分析人](http://dry.yoichihirai.com/)重新部署
- 接受[ETH支付方式](https://blog.haschek.at/2017/accepting-ethereum-without-external-services.html)只能用Parity
- Jordi Baylina[在以太坊上如何安全转账](https://gist.github.com/jbaylina/e8ac19b8e7478fd10cf0363ad1a5a4b3)
- [Vitalik推特提醒](http://mailchi.mp/ticketleap/week-in-ethereum-news-pvxskzbbrv?e=9eac9b5442)想节省矿工费用，可以精简合约（代码），转发器使用DELEGATECALL
- [干货 | Casper的历史起源--第四篇](https://mp.weixin.qq.com/s/Gp1AxoSHTA2R2pXhJF7WrQ)

# 生态系统
- [EOS 发布会（中文字幕）](http://m.youku.com/video/id_XMjgxMTM1MTY1Ng==.html?sharefrom=iphone&from=timeline&isappinstalled=1&source=)
- [美国商业杂志《公司 Inc.》网站报到：Siacoin 正在挑战 Dropbox 和 Amazon 云存储，本月 Siacoin 将在推出一个简单的文件共享功能，暂未看到官方博客更新，目前SC 市值在数字加密货币中排名前十六，过去一年中上涨了 2406 %](https://www.inc.com/brian-d-evans/blockchain-tech-company-sia-siacoin-could-disrupt-dropbox-and-amazon.html)
- [Bancor 现在帮官方找 bug ,有奖励～不管是网站上的还是智能合约的还是软件，都有奖励～](https://app.bancor.network/communities/59072cd673f6660001aa8e93/about)
- [路透社母公司汤森路透发布以太坊兼容的市场数据工具 blockone IQ](https://www.ethnews.com/thomson-reuters-to-provide-market-data-through-the-ethereum-compatible-blockone-iq-tool)
- [Cardano 正式版发布检查清单，Cardano的确定第一个版本的名称  Byron（拜伦），提供与比特币相同的基本功能也就是转账，目前可以查看剩余的任务关注项目的进展。testnet v0.5 将在本月底发布。正式版还是遥遥无期啊，难道老扎把钱都花到了 ETC 开发，Cardano 开发太慢了。](https://cardanolaunch.com/)
- [lightning-li: Status公布的智能合约总结了一下众筹的规则：status分两种币：SGT 与 SNT。SGT 是 status 官方分发给对status的发展起到贡献的人；SNT 是众筹过程中产生的币。根据最新的智能合约，有两种模式，一种是buyNormal（正常参与代币众筹的人），一种是buyGuaranteed（一定可以买到的地址，由status官方指定，可以理解成白名单）。在 buyNormal 模式下，开始区块过后的2000个区块里，只有拥有 SGT 的人才有资格参与众筹，另外合约限制了最高的gasPrice 为50000000000 Wei，超过此限制，合约会抛出异常，意味着不能通过高手续费来使矿工打包你的交易。此外，每一个区块都会根据已经披露的隐藏上限有一个上限值，打包在同一个区块内的交易，至多购买该区块还剩余的1/30。多余的会退还到原账户。除了一系列的隐藏上限，还存在一个特别高的 failsafe - 300000 个以太币。当所有的隐藏上限披露并达到目标（众筹的以太币数量大于等于最后一个披露的上限减去1个以太币即可）后，可以提前结束众筹过程。众筹结束后，SNT 的转移将会被锁定1周的时间，但是SGT可以立即兑换成SNT，至多兑换SNT总量的10%，当总分发的SGT数量小于等于SNT的10%，按照1：1进行兑换，超过时，按相应减少比例。](http://t.xiaomiquan.com/qr3FiqF)
- [ Shapeshift 创始人 在 Reddit AMA](https://www.reddit.com/r/ethereum/comments/6hfw8y/ama_w_erik_voorhees_shapeshift_ceo_ask_me_anything/)

# 币圈考古
Ripple协议的前身是 https://classic.ripplepay.com/ ，2004年由 Ryan Fugger 开发。他最初想开发一个新的去中心化货币系统，允许互连的朋友和企业之间的付款。
如果仅止于此，ripplepay 可能也就局限在小范围。转机发生在2012年，当时名叫 Chris Larsen 和 Jed McCaleb 的两人向  Ryan Fugger 提出了一个新的数字货币理念，随后三人共同成立的 OpenCoin。
OpenCoin 开发的新支付协议就是 Ripple协议。它允许交易双方即时直接进行转账，可以绕过传统代理银行系统的费用及时间，2014年 Ripple 迎来第一位银行用户：德国互联网银行 Fidor。再四个月后，它又获得两家美国银行对Ripple协议的支持，至此，Ripple才逐渐受到认可。
有意思的事情来了，开发以太坊闪电网络的团队 brainbot‏ 发现了 ripplepay 的价值, 发起了 http://trustlines.network/ 项目，在以太坊上实现 ripplepay ，每个用户都通过向信任的朋友授予信用额度作为银行,陌生人之间通过在一连串的信任朋友安全转账。目前 Trustlines 已经发布测试版 https://rmb.test.trustlines.network/ ,另外，6月19日18：30 杭州以太坊线下活动，有机会跟 Trustlines 创始人面对面交流，大家不要错过机会
http://www.huodongxing.com/event/7391914870400?td=1732279493183&from=groupmessage&isappinstalled=0


# 小课堂
什么是 Merkle Trees (默克尔树)?
简单地说，Merkle根是哈希的哈希。看下面我绘制的图表。
![](http://upyun-assets.ethfans.org/uploads/photo/image/0ffedcf28c194a6f908a993f6dbc3997.png)
上图中，你可以看到我之前的FUNDEMENTALS的哈希示例，以及我刚刚添加的另一个包含一些数据的随机哈希。 你可以看到两个哈希加在一起成为一个更长的字符串，然后再次被哈希化为所谓的Merkle根。
作为聪明的年轻人，你可能会想 “ 嘿，既然说它是哈希的哈希，那我们能不能把两个Merkle根也做同样的处理？” 你太机智了真的可以。
请看我的另一个艺术作品。
![](http://upyun-assets.ethfans.org/uploads/photo/image/074fb2c4130246bcafdd425299d5784b.png)
你可以看到，上图画了两个Merkle根（记住：Merkle根是哈希的哈希），把它们加在一起，就会得到一个哈希。
那么问题来了，为什么会有人要用这个？
三个词，有效的数据验证。 Merkle 树创建一个单一的值，来证明其下的所有交易的完整性。
Merkle 树提供了证明你的数据有效性的方法。
Merkle 树要求在计算上容易和快速。
Merkle 树不需要太多的记忆功能（将数据的验证与数据本身分开，可类比Google密码示例）。
好啦，解释的不能更详细了，如果你觉得这个有趣的话，[更多关于 Merkle Trees 的信息](https://blog.ethereum.org/2015/11/15/merkling-in-ethereum/)。

# Podcast
- [最近发现一个有意思的 Youtube 频道，Cedric Dahl，主要将数字货币投资和炫耀豪宅。他的投资三大定律和如何选择一个项目：1. 马克吐温测试，能否用简单的话描述项目，项目本身是不是与人们基础生活息息相关；2. 彼得·蒂尔测试，是不是行业中的垄断者。3. 梅特卡夫法，用户越多，网络的价值越大，联网的需求也就越大。他的三驾马车是：BTC、ETH、FileCoin, 他特别推荐的一书《从零到一》](https://www.youtube.com/watch?v=zePZEn7HFKo)

# 工具
- [“Flippening”一词是用来形容以太币市值超越比特币的一种潜在状况。flippening.watch 这个网站 从市值、24小时转账数、矿工奖励、节点数、谷歌搜索指数分析以太超比特的事实。](http://www.flippening.watch/)
- 考虑到目前ICO项目过多，做了一个 excel 用于管理ICO，这个表格可以帮助大家核算ICO成本，持仓时间，利润计算等内容，大家可以尝试使用，如果有想法可以跟我交流，只要时间允许一定会优化的；另外我们在进行ICO过程中碰到的问题，可以记录到第二个SHEET页的风险管理清单中，降低日后风险。自己写的所以大家使用中也许会有问题，使用中带来的问题，欢迎拍砖，[表格下载](http://t.xiaomiquan.com/EY3bIa2)

# ICO 时间 
- 2017-6-17 开始 -- [Status](https://status.im/) 以太坊上的微信
- 2017-6-22 开始 -- [OpenANX]() 去中心化交易平台
- 2017-6-24 开始 -- [TenX](https://www.tenx.tech/) 区块链资产平台 
- 2017-6-26 开始 -- [Adchain](https://adtoken.com/) 一套基于以太坊的广告开放协议
- 2017-6-27 开始 -- [Omise Go](https://omg.omise.co/)  一个去中心化交易所和支付平台
- 2017-6-30 开始 -- [Santiment](http://www.santiment.net/) 加密市场的信息平台











