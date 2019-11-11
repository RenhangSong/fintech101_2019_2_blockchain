#  Blockchain 实验项目


Xubin Cao

SWUFE，2019.11.11

---


## 实验目标

* 阅读中本聪的区块链论文
  * [比特币白皮书英文](https://www.bitcoin.com/bitcoin.pdf)
  * [比特币白皮书中文](https://www.8btc.com/wiki/bitcoin-a-peer-to-peer-electronic-cash-system)
* 尝试实现区块链论文的代码实现（基于Python语言）
* 通过开源代码的学习，了解区块链的多种实现方法（基于Python语言）

---



## 实验要求

* 同学们根据兴趣组合形成小组来共同完成本实验项目。
* 每组成员数为3～6人。
---

## 实验准备

本实验可在Windows、MacOS、Linux的环境下运行，同学们可以根据自己的情况选择操作系统，同时根据不同操作系统的特点准备好应用程序环境，包括但不限于如下：

* 笔记本电脑
* git环境的准备
* 可访问GitHub网站
* python环境的准备（包括python虚拟环境的设置/Python库的安装等）
* node环境的准备（含npm，部分应用需要）
* 浏览器的准备（chrome/firefox/...）

---

基于jupyter notebook格式的代码同学们可以尝试使用我们的[jupyter实验平台](http://glab.swufe.edu.cn)。

---

## 实验报告

同学们根据分组情况提交小组实验报告。（命名规则： 2019_2_blockchain_lab_班级名_小组名.md)
实验报告包括:
1. 实验小组人员组成及分工;
2. 实验小组的实验计划（清单）;
3. 实验小组的实验结果（截图）;
4. 实验总结（不足/失败原因分析等/收获）
5. 实验自我评价（满分10分，自我评分）
6. 补充（需要说明的其他内容）

Deadline：2019-11-24 24:00 CST
（通过github提交）

---


## 实验内容

---

### 1. Blockchain Demo：


A web-based demonstration of blockchain concepts.
(https://www.youtube.com/watch?v=_160oMzblY8)

本开源项目由MIT的Anders提供，基于比特币的论文，尝试模拟实现区块链的构建和交易。包括两个部分，分别介绍了区块链的基本构成和链的产生，比特币地址（个人私钥/公钥对）的构建和如何参与区块链交易等。

---

本Demo有网站版本，可以直接点击[网站链接](http://anders.com/blockchain/)测试；
如果可能，建议尝试在GitHub中下载源代码，在本地进行测试。其地址如下：


  * [Part1:](https://github.com/anders94/blockchain-demo.git)

  * [Part2:](https://github.com/anders94/public-private-key-demo)

---


你可以直接下载代码或者采用git命令建立本地的git代码仓库。如下：

``` bash
git clone https://github.com/anders94/blockchain-demo.git

```
---

首先阅读README，了解代码的设计思想和安装运行指南，尝试自己在本地顺利运行。
如果可能，可以参照说明对参数进行调整，比如调整区块的生成困难度，进行比较，从而了解算法的设置对于区块生成的时间和难度影响。

**实验要求：选做。了解，运行代码**

---


### 2. [A Practical Introduction to Blockchain with Python](http://adilmoujahid.com/posts/2018/03/intro-blockchain-bitcoin-python/)

Adil Moujahid 于2018年发表了一篇文章来介绍如何使用python代码来了解区块链的工作原理。并提供了相应的源代码。
你可以下载或者通过```git clone```命令来建立本地的代码库，在本地运行代码。

---

[代码地址](https://github.com/adilmoujahid/blockchain-python-tutorial)

作者在项目介绍中进行了简单的描述，说明本项目主要用于教育，是通过python语言对区块链原理的基本模拟实现，包括区块的产生，区块链的生成，POW工作量证明的实现方法，如何处理节点间的冲突以及怎样生成一个客户端（公钥/私钥对）、交易发起等等。通过代码的实现，同学们可以通过分组运行，来熟悉代码的功能，代码的运行，并通过彼此之间的交易来感受交易的发生和区块链的产生流程等。

---
详情参见作者描述：

> The github repository contains a basic implementation of a blockchain and its client using Python. This blockchain has the following features:

> * Possibility of adding multiple nodes to the blockchain
> * (Proof of Work (PoW)
> * Simple conflict resolution between nodes
> * Transactions with RSA encryption

> The blockchain client has the following features:

> * Wallets generation using Public/Private key encryption (based on RSA algorithm)
> * Generation of transactions with RSA encryption
> * This github repository also contains 2 dashboards:

> "Blockchain Frontend" for miners
> "Blockchain Client" for users to generate wallets and send coins

---

本部分是本次实验项目的重点和难点，希望每个同学都能通过代码的运行，通过彼此之间的模拟交易来观察、熟悉整个交易的发生和区块链的生成过程，从而加深对区块链原理和特性的掌握。

**实验要求：必做。了解，运行代码**

---


### 3. Dumbcoin - An educational python implementation of a bitcoin-like blockchain

[代码地址](https://github.com/julienr/ipynb_playground/blob/master/bitcoin/dumbcoin/dumbcoin.ipynb)


> This is an experimental notebook that implements most of the concepts of a bitcoin-like blockchain in python. It is NOT secure neither a real blockchain and you should NOT use this for anything else than educational purposes.
---

这个项目是基于比特币的论文来模拟实现区块链原理的一个用于教育的项目。该项目采用jupyter notebook的开放格式，只有一个文件，非常便于我们学习和练习。

该项目主要包括了与区块链原理相关的如下部分：
* Hash function and mining
* Difficulty
* A wallet
* Transactions
* Blocks
* Attacks
* Majority attack
---

同时，本项目还提出了与比特币的具体实现还存在哪些不同，还有哪些没有实现之处，有助与我们进一步在此基础上思考或者完善代码。

这个项目建议每位同学都能够去阅读，并尝试运行所有的代码，进一步去了解区块链设计的巧妙构思，以及python语言实现的简易快捷。

这个项目既可以满足个人的学习，也适用于小组学习，同学们可以通过小组公共阅读代码来共同练习。

**实验要求：选做。了解，运行代码**

---


### 4. 其他

GitHub上有大量开源的有关区块链的项目可以参照学习。同学们可以选做其中一些，进行扩展学习：

* [开源教程：从零开始写区块链](https://github.com/OpensourceBooks/blockchain)
* [一个区块链原型程序](https://github.com/YngwieWang/blockchain)

**实验要求：选做。了解，运行代码**


---

# 课程实验说明

---

本部分实验主要是在实验室现场完成，分为两个部分，完成分组后每个小组选择自己的工作区域和小组名称，按以下步骤进行必做实验（实验项目2）。

---


# Step1:每个小组先完成小组内调试

* 完成blockchain.py正常运行；
* 完成blockchain_client.py正常运行
* 完成小组内部测试，包括：
  * 测试 node节点是否顺利运行；
  * 添加 node节点
  * 测试node节点的同步机制（后续加入的节点如何获取之前的区块链）
  * 测试交易
  * 测试发布交易在不同节点上时，节点的交易信息和区块信息
  * 测试区块链的分叉工作原理

---

# Step2：上线


1. 首先需要开放你们的ip地址，公告大家。
2. 添加之前上线的节点地址
3. 同步区块链
4. 生成区块
5. 小组之间相互交易
6. 交易信息生成区块，加入区块链
7. 测试区块链分叉机制的有效性
8. 测试区块链攻击

---
# 奖励：

奖励加分将与每小组的实验报告成绩累加，得到总成绩。

* 最先上线的小组每位成员有加分5分；
* 最先完成第一个有效交易区块的小组每位成员有加分5分；
* 最先完成有效攻击的小组（们）每位成员有加分10分；

友情提示：

---

# 项目2中blockchain.py代码需要修改最后一行：
```
app.run(host='127.0.0.1', port=port)
```

修改为：
```
app.run(host='0.0.0.0', port=port)
```

同学们要记住自己的ip地址和端口port，便于相互访问使用；
同学们要保存好自己的公钥/私钥，用于交易使用。
