timezone: UTC+8



# SixLi

1. 努力不落入败者组的古怪六六
2. 应该可以
3. 646767952@qq.com

## Notes

<!-- Content_START -->

### 2025.03.03

从两个属性理解web 3
- 一、去中心化：
对比web1，用户对于静态信息的单向接收，以及web2用户可以经过品牌或者大平台的背书，通过这些中心化的服务器接收动态信息并可以完成交互的行为，web 3则是给用户提供不需要第三方平台或者品牌背书的，由用户自己掌握数据的交互方式。
深入理解去中心化：不需要第三方平台或者品牌或者公信力组织的背书，不需要任何中介的信任机制。用户不仅仅直接跟用户交互（peer to peer），用户直接与程序交互。（vs现实世界用户不能轻易接触政府国家架构）

- 二、所有权归属：
web3的数据真正属于用户。web2时代，用户是内容的接收者、输出者与消费者，但是用户不拥有数据。数据掌握在集中服务器，掌握在大公司中。掌握数据的大公司是可以根据协议更改所有权归属、使用权等。

运作技术基础：
- 区块链技术，
   - 如何运作：一个新的交易发生，会通过广播告知所有节点，所有节点都有知情权以及监督权
   - 内容物包括：区块头（公区哈希函数previous hash + timestamp + merkle treeroot），以及区块主体（交易列表、数据）

- 公钥与私钥，
公钥用于加密信息
私钥用于解密信息，私人拥有

- 智能合约，
允许用户与程序直接交互。觉得这个功能很浪漫，在于个体是可以构建组织的基础设施直接交互的，个体可以留下自己的印记，上传自己的数据去影响这个基础设施。对比web2生活，个体对庞大的政府、公司组织的影响力是有限的，间接的，有滞后性的。而web3通过智能合约可以实现用于与程序的直接联系，可以组建即刻的关系，让交易行为瞬间发生、必然发生，不需要公信力组织的强制实行。（目前的理解，希望是正确的）

### 2025.03.04
理解区块链的运行机制同时也是保护机制

哈希函数-记录的同时也在防篡改
每个区块头都包含上一个区块数据的哈希值，如果需要伪造则需要把链条上的夫区哈希值都篡改一遍。而随着网络节点增多，篡改的算力不可能超过所有节点；另外一种可能性，就是某种既得利益方拥有超过50%算力进行篡改，利用区块链中少数服从多数的原则，但拥有超过50%的算力几乎不可能，而一个既得利益方会更坚定地维护区块链的稳定性。

P2P-实现去中心化
实现全民记账（取代公信力中心机构记账）
但是！需要确保全民记的是正确的帐，而这个保护机制就是共识算法。这里包括

1. PoW （类似比特币类区块链系统）
   - 基本原则：
     - 难题设计，要求节点解决一个复杂的数学难题（挖矿），一旦解出，其他节点则会验证其正确性助其生成新区块
     - 最长链原则，当一个节点解出难题并生成新区块后，会迅速广播全网，其他节点验证后即可基于这个节点形成一个区块。
       - 最长链的本质：1）只认可最长链，不论谁生成区块，大家都会选择最长的链作为有效链（诚实节点会不断在长链条上挖矿，不断验证不断延长这条链；恶意节点要想搞破坏，则需要自己生成一条更长的链条并获得大家的认可）2）算力耗费大。诚实节点会不断地在长链条上挖矿延长，形成新的区块速度会更快，恶意节点若想搞破坏，则需要比诚实节点有更强的算力（即超过50%的算力）3）区块传播速度的作用。诚实节点传播更快，因为他是有效的可被验证的，其他节点会容易接受，并在此基础上挖矿延长；恶意节点容易受阻，恶意节点产生无效区块，其他节点会拒绝接受他，影响他的传播速度）4）恶意节点攻击成本极高。算力要超过50%才能成功。
         所以，最长链原则通过“多数诚实节点力量集结”捍卫安全性。好人力量占据多数，良币驱逐恶币。

### 2025.03.05

2. BFT 拜占庭容错共识
   如果说比特币以竞争的方式去让各个节点解题、挖矿，BFT则是通过协同的方式让节点合作达成工作。定期推选出“领袖”节点，再由其他节点对其进行验证确认。可以支持它可以推翻它。
   比特币的PoW：允许各个节点的参与，且不需要信任任何节点，通过“算力竞争”来确保安全性
   BFT：解决分布式系统中的拜占庭将军问题，即在恶意节点存在的情况下，仍可达成一致。
   
![image](https://github.com/user-attachments/assets/5b8e4401-43e0-4eb8-bbcc-f3b5183538a8)
怎么在这里加表格啊


         
<!-- Content_END -->
