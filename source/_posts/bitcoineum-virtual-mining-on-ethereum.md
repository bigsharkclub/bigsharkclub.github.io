---
title: Bitcoineum：基于以太坊虚拟挖矿项目
date: 2017-07-29 13:47:50
category: 生态系统
author: MakoShan
---

北京时间 2017年7月19日17:00 Bitcoineum 开始挖矿，Bitcoineum 采用非常公平的挖矿方式 - PoB，创始人的没有早期奖励，没有预挖。Bitcoineum 和比特币一样, 货币总量上限 2100万个。不仅可以像比特币一样保值，也可以直接对接以太坊强大智能合约体系，为以太坊带来了比特币功能,而不是将智能合约加入到比特币。这是作者为什么要建立 Bitcoineum，比特币的政治僵局，集中化和企业控制的风险增加，获得积极的智能合同开发社区，以显着提升价值存储的能力。

Bitcoineum 采用的是销毁证明 PoB （proof-of-burn）的挖矿方式， PoB 是一种有趣共识算法，用来替代 PoW 和 PoS ，通过将币发送至一个无法生成私钥的地址来销毁的方式发行代币，以太坊正好非常简单做这件事情。

PoB 可以和信用体系结合在一起，用户可以选择通过销毁一定量的代币来证明他们对系统身份的承诺，销毁代币的行为表明用户致力于获得该网络的认可和获得一定声誉，因为他们现在已经花费了资源，如果出现负面事件，那么销毁代币获得的声誉将会浪费，通过这样的体系可以建立去中心化淘宝。

Bitcoineum 的设计结构是对通货膨胀的以太币的一种补充，你可以把 Bitcoineum 认为是更大结构世界的原子，更复杂功能的基础。Bitcoineum 建立了一套面向用户的简单挖矿协议和价值定义，可以为其他应用程序提供基础标记，这让 BTE 可以无缝地转变为一个尚未创建的其他ERC20 代币。可以通过以标准化的方式烧毁 BTE，直接将BTE 的价值转移到其他类型的代币中。举一个实际的例子，如果以太坊支持 ZkSnark（零知识证明），用户可以通过销毁 BTE 的方式升级到有ZkSnark 隐私的 Bitcoineum。

采用 PoB 的好处，任何可以链接到以太网的人，都可以从 web界面立即挖矿。这意味着任何设备都可以挖矿，手机，网页，嵌入式设备，树莓派，Bitcoineum 想创建一个公平、去中心化和可随出访问的挖矿系统，可以为其他代币带来价值。

目前仍然是 beta 产品，存在风险。作者希望这能为以太坊生态系统增添一个有益的补充，而且在开发人员可以在以太坊上创建这些类型的系统时，比特币可以简单地生存下来，从而使得它能够幸免于难。

### 如何参与 

1.启动 geth 节点，同步所有数据

```
geth --fast --cache=512 --rpc=true --rpcport 8545 --rpccorsdomain "*" --rpcapi "db,eth,net,personal,web3"
```

2.解锁挖矿钱包
```
personal.unlockAccount('0xfbe1515eaa094d302a25a34045ced472192893a9', 'balalalal, 25000)
```
3.Bitcoineum 挖矿页面设置 [http://www.bitcoineum.com/miner/](http://www.bitcoineum.com/miner/) 

设置挖矿钱包

```
set-mining-account '0xfbe1515eaa094d302a25a34045ced472192893a9'
```

设置奖励钱包
```
set-credit-account '0x0e5a28725531d4c345f2e0a290fbf565f71ff30f'
```

启动挖矿：

 ```
 automine
 ```

查看合同地址挖矿情况
https://etherscan.io/address/0x73dd069c299a5d691e9836243bcaec9c8c1d8734


### 加入矿池
BTE 是通过烧 ETH 获得的代币，为了方便大家挖矿，目前有 BTE 鲨鱼矿池 1和2，上限都是 100人，直接转账到合约地址，自动挖矿，
矿池1: https://etherscan.io/address/0x29aa20fb9b23421e310bdb8a7cfb81d7fbb4a1b3 
矿池2: https://etherscan.io/address/0x4c13184721de2d1b47a8875775ba3ce0b2e00ee0 ， 记得不能普通转账，需要用高级模式 ，gas 150000，目前可以至少转 0.01 加入矿池，矿池有 5% 的提币手续费, 挖矿进度查询工具: http://pools.bigshark.club/。使用工具查询到余额后，再转账一笔 0.01 ether 获取挖矿奖励，gas 也是 15万。

### 总结
bitcoineum 的价值，通过公平挖矿方式产生一个有价值的 BTE 代币（比特币模式），这个有价值的 BTE 代币可以通过以太坊强大智能合约的方式，直接兑换成其他拓展功能的代币，比如现在以太坊支持零知识证明，可以写一个零知识证明隐私保护的代币合约，BTE 的持有者可以直接调用智能合约，获得直接有价值的和具有零知识证明的代币。bitcoineum 的创新之处在于更公平的挖矿（手机挖矿）和 价值转换的方式。更多关于 BTE 的细节，请阅读 BSC 翻译的白皮书: bigshark.club/bitcoineum_white_paper_cn.pdf

### 参考：
https://www.reddit.com/r/ethereum/comments/6oo54i/bitcoineum_virtual_mining_on_ethereum/
https://en.bitcoin.it/wiki/Proof_of_burn

