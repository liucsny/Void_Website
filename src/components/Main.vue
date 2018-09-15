<template>
  <div>
    <app-landing></app-landing>
    <app-intro></app-intro>
    <app-section-1></app-section-1>
     <section class="pv6 ph3 ph6-ns">
      <div class="mw-m flex-ns justify-center center">
        <div class="w-100 w-40-ns dark-gray">
          <div class="tracked fw9 mb3 f6">0010</div>
          <div class="fw7 tracked f-2 lh-sub-title">Void 的数据分布 <br/>与网络共识</div>
          <p class="text f6 fw3 lh-text mt4">造成当前以太坊等区块链性能瓶颈的其中一个原因，就是每个节点都要存储全量的数据，具备完全的处理能力。而 Void 是一个侧链的设计，每个节点只会存储相关的若干子链的数据，链与链之间互相 follow，形成类似 twitter 的网络，只有节点 follow 的链才会被缓存。follow 关系意味着关注和缓存对方链的数据，一种弱信任关系。follow 关系也是链上消息的一部分，通过读取链的 follow/unfollow 消息，其他节点可以知道这个节点存储哪些子链，优化数据的分布，加速网络同步过程。</p>
          <p class="text f6 fw3 lh-text mt4">网络中有一些帮助缓存和分发数据的中继节点，称为 hub。这些 hub 通过一定准入机制，自动 follow 一些子链，志愿提供服务，或者是通过服务合约，在一定的激励下提供可靠的服务。对于应用方，也可以设置特定应用的 hub，让用户可以不需要付费而得到基本的服务，降低网络进入门槛。 Void 是一个侧链的设计，每个节点只会存储相关的若干子链的数据，链与链之间互相 follow，形成类似 twitter 的网络，只有节点 follow 的链才会被缓存。follow 关系意味着关注和缓存对方链的数据，一种弱信任关系。follow 关系也是链上消息的一部分，通过读取链的 follow/unfollow 消息，其他节点可以知道这个节点存储哪些子链，优化数据的分布，加速网络同步过程。</p>
          <p class="text f6 fw3 lh-text mt4">Void 本身不依赖 PoW 或 PoS 等算法提供共识机制，而是通过与以太坊等支持智能合约的区块链主链交互，进行数据一致性的见证。Void 的可验证数据结构使用了 streaming merkle tree，每一个消息的 hash 和数字签名都包含了这个链的所有历史状态，将当前消息的 hash 和 signature 写入合约，保证子链有唯一的版本。子链之下可以衍生下级子链，将 hash 写入父链进行见证，或者由多条侧链进行见证。Void 的见证机制和侧链交互机制可以锚定到多条主链上，与 Ethereum，EOS ，Polkadot 或是新的区块链平台交互，与整个区块链生态的发展同步。</p>
        </div>
        <div class="w-100 w-50-ns dark-gray mt3">
          <!-- img -->
        </div>
      </div>
    </section>
    <section class="ph3 ph6-ns bg-light-gray pv4">
      <div class="mw-m flex-ns center dark-gray justify-between">
        <div class="w-100 w-30-ns pv4">
          <h2 class="fw6 f5 tracked tc">高性能</h2>
          <p class="text tl ph3 f6 fw3 lh-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam id eum dolores libero. Fugiat sint exercitationem quis.</p>
        </div>
        <div class="w-100 w-30-ns pv4">
          <h2 class="fw6 f5 tracked tc">可扩展</h2>
          <p class="text tl ph3 f6 fw3 lh-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam id eum dolores libero. Fugiat sint exercitationem quis.</p>
        </div>
        <div class="w-100 w-30-ns pv4">
          <h2 class="fw6 f5 tracked tc">轻量级</h2>
          <p class="text tl ph3 f6 fw3 lh-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquam id eum dolores libero. Fugiat sint exercitationem quis.</p>
        </div>
      </div>
    </section>
    <section class="pv6 ph3 ph6-ns">
      <div class="mw-m flex-ns justify-center center">
        <div class="w-100 w-50-ns dark-gray mt3">
          <!-- img -->
        </div>
        <div class="w-100 w-40-ns dark-gray">
          <div class="tracked fw9 mb3 f6">0101</div>
          <div class="fw7 tracked f-2 lh-sub-title">Void的灵活性和 <br/>应用友好性</div>
          <p class="text f6 fw3 lh-text mt4">Void 使用类似区块链的数据结构，每个用户或每个应用都是一条独立的链，即时发布消息，不需要等待矿工确认和负担矿工费。由于每一条链各自独立，不需要像比特币的区块链那样打包交易，所以 Void 以消息为链的基本单元，而不是区块，作为一个可验证数据结构（Authenticated Data Structure）和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。</p>
        </div>
      </div>
    </section>
    <section class="pt6 pb4 ph3 ph6-ns">
      <div class="mw-m tc center">
        <div class="dib tl dark-gray">
          <div class="tracked fw9 mb2 f6">0100</div>
          <div class="fw7 tracked f-2 lh-sub-title mb4">Void 的技术架构与生态系统</div>
        </div>
        <div class="flex-l">
          <div class="w-100-m w-50-l flex-ns" >
            <p class="text w-40-ns tl f6 fw3 lh-text center bg-white br3 pa3 pa4-ns mv4 ba b--black-10">和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。</p>
            <p class="text w-40-ns tl f6 fw3 lh-text center bg-white br3 pa3 pa4-ns mv4 ba b--black-10">和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。</p>
          </div>
          <div class="w-100-m w-50-l flex-ns">
            <p class="text w-40-ns tl f6 fw3 lh-text center bg-white br3 pa3 pa4-ns mv4 ba b--black-10">和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。</p>
            <p class="text w-40-ns tl f6 fw3 lh-text center bg-white br3 pa3 pa4-ns mv4 ba b--black-10">和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。</p>
          </div>
        </div>
      </div>
    </section>
    <section class="pv6 ph3 ph6-ns">
      <div class="mw-m flex-ns justify-center center">
        <div class="w-100 w-50-ns dark-gray mt3">
          <!-- img -->
        </div>
        <div class="w-100 w-40-ns dark-gray">
          <div class="tracked fw9 mb3 f6">0101</div>
          <div class="fw7 tracked f-2 lh-sub-title">Void 的进化</div>
          <p class="text f6 fw3 lh-text mt4">Void 使用类似区块链的数据结构，每个用户或每个应用都是一条独立的链，即时发布消息，不需要等待矿工确认和负担矿工费。由于每一条链各自独立，不需要像比特币的区块链那样打包交易，所以 Void 以消息为链的基本单元，而不是区块，作为一个可验证数据结构（Authenticated Data Structure）和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。</p>
        </div>
      </div>
    </section>
     <section class="pt3 pb6 ph3 ph6-ns">
       <div class="mw7 flex-ns center text fw3 lh-text">
         <p>Void 起源于对 git 分布式文件版本控制系统和 Couchdb 分布式最终一致数据库的探索。我们希望在区块链时代构造像 git 一样去中心，可验证，异步提交，灵活，高性能的机制，并且通过 merkle tree 的加密学证明，任何时刻 git 仓库的 head hash 都蕴含了对整个文件系统历史的见证。Couchdb 数据库则提供了一个基于 append-only log 的数据库机制，不同节点并行可入，系统性能水平扩展，在这个核心的 log 上面可以进行不同的查询，建立特定应用的视图。Couchdb 的 schemaless 设计也影响了 Void，我们提供一个统一的基础数据格式，但消息本身的内容只与应用相关，可以灵活的软分叉，不断为网络扩充新的能力。

Void 的设计也受到了 Dat 项目的影响，Dat 扩充了 git 的应用场景到结构化的数据，完善了加密学数字签名机制，并且引入了 ppspp 协议的 merkle-tree stream。Void 的数据分发和 follow 机制受到了 secure scuttlebutt 的影响，展现了一个在分布式网络中定向的，高效的分发数据的机制，能够在激励不充分的时候启动网络。Void 的数据同步协议来自于 Amazon DynamoDB 和 Riak 数据库的 Flow Gossip，以及 Epidemic Broadcast Tree 算法，能够利用向量钟高效同步数据，降低网络通讯成本，缩短 swarm 到达同步的时间。Vitalik 等提出的 Plasma 为 Void 的区块链可互操作性提供了一个很好的框架。

目前主流的区块链共识算法形态更像是强一致性数据库系统，要求在有限的时间内，已知的矿工中间达到一致的共识，并取得全网的认可。而 Void 保留了不可变的链式结构，但设计上强调异步性，并行性，灵活性，可扩展性，构建了一个更加低成本，更具包容性的网络，接近于一个最终一致数据库的模型，也从这样一个几十年研究历史的领域中得到了许多启迪。我们相信不同的哲学，不同的设计，不同的取舍，可以互相补充，构建更丰富的生态。如果有什么是 Void 真正的哲学理念，那就是灵活，简单，快！</p>
       </div>
     </section>
  </div>
</template>

<script>
import appLanding from './sections/Landing.vue';
import appIntro from './sections/Intro.vue';
import appSection_1 from './sections/Section_1.vue';

export default {
  name: '',
  components: { 
    appLanding,
    'app-intro':appIntro,
    'app-section-1': appSection_1
  }
};
</script>

<style scoped>
</style>
