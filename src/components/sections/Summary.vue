<template>
  <section class="container summary">
    <div class="wrapper">
      <p>{{content.text}}</p>
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      content:{
        text:`Void 起源于对 git 分布式文件版本控制系统和 Couchdb 分布式最终一致数据库的探索。我们希望在区块链时代构造像 git 一样去中心，可验证，异步提交，灵活，高性能的机制，并且通过 merkle tree 的加密学证明，任何时刻 git 仓库的 head hash 都蕴含了对整个文件系统历史的见证。Couchdb 数据库则提供了一个基于 append-only log 的数据库机制，不同节点并行可入，系统性能水平扩展，在这个核心的 log 上面可以进行不同的查询，建立特定应用的视图。Couchdb 的 schemaless 设计也影响了 Void，我们提供一个统一的基础数据格式，但消息本身的内容只与应用相关，可以灵活的软分叉，不断为网络扩充新的能力。
Void 的设计也受到了 Dat 项目的影响，Dat 扩充了 git 的应用场景到结构化的数据，完善了加密学数字签名机制，并且引入了 ppspp 协议的 merkle-tree stream。Void 的数据分发和 follow 机制受到了 secure scuttlebutt 的影响，展现了一个在分布式网络中定向的，高效的分发数据的机制，能够在激励不充分的时候启动网络。Void 的数据同步协议来自于 Amazon DynamoDB 和 Riak 数据库的 Flow Gossip，以及 Epidemic Broadcast Tree 算法，能够利用向量钟高效同步数据，降低网络通讯成本，缩短 swarm 到达同步的时间。Vitalik 等提出的 Plasma 为 Void 的区块链可互操作性提供了一个很好的框架。
目前主流的区块链共识算法形态更像是强一致性数据库系统，要求在有限的时间内，已知的矿工中间达到一致的共识，并取得全网的认可。而 Void 保留了不可变的链式结构，但设计上强调异步性，并行性，灵活性，可扩展性，构建了一个更加低成本，更具包容性的网络，接近于一个最终一致数据库的模型，也从这样一个几十年研究历史的领域中得到了许多启迪。我们相信不同的哲学，不同的设计，不同的取舍，可以互相补充，构建更丰富的生态。如果有什么是 Void 真正的哲学理念，那就是灵活，简单，快！`
      }
    }
  }
}
</script>
