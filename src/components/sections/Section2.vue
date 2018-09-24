<template>
  <section class="container section-text-left">
    <div class="text-box">
      <div class="text-wrapper">
        <div class="digit">0010</div>
        <div class="title" v-html="content.title"></div>
        <p class="text" v-html="content.text"></p>
      </div>
    </div>
    <div class="img-box">
      <img src="../../assets/img_1.svg" alt="Landing img">
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      content:{
        title: 'Void 的数据分布</br>与网络共识',
        text: `造成当前以太坊等区块链性能瓶颈的其中一个原因，就是每个节点都要存储全量的数据，具备完全的处理能力。而 Void 通过侧链设计，链与链之间互相 follow，形成类似 twitter 的网络，每个链关注和缓存对方链的数据，一种弱信任关系，其他节点可通过这种关系，以知道这个节点存储哪些子链，优化数据的分布，加速网络同步过程。
       </br>Void 本身不依赖 PoW 或 PoS 等算法提供共识机制，而是通过与以太坊等支持智能合约的区块链主链交互，进行数据一致性的见证。
        `
      }
    }
  }
}
</script>
