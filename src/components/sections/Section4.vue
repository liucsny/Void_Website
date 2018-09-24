<template>
  <section class="container section-text-right">
      <div class="img-box">
        <img src="../../assets/img_1.svg" alt="Landing img">
      </div>
      <div class="text-box">
        <div class="text-wrapper">
          <div class="digit">0101</div>
          <div class="title" v-html="content.title"></div>
          <p class="text" v-html="content.text"></p>
        </div>
      </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      content:{
        title: 'Void 的进化',
        text: `
<h4 class='sub-title'>multi consensus</h4>
Void 本身提供了一个轻量的侧链机制，依赖区块链主链提供共识，通过智能合约进行数据验证。随着区块链技术的进化，新的公链和联盟链平台，新的 PoW，PoS，BFT，DAG 等技术也会不断涌现，Void 能够与这些新的链，新的共识算法交互，提供一个粘合剂。各种共识算法都能在特定的应用场景下为 Void 提供数据的见证和互操作机制，让网络持续进化。
<h4 class='sub-title'>multi master</h4>

Void 一条侧链不光可以锚定到一条主链上，也可以锚定到多条主链，为多个网络服务，提供轻量的跨链机制，提供诸如跨链结算，代币互换等功能。多个主链也为 Void 侧链提供了更强的安全性，不同链之间的出块时间，交易成本，网络稳定性各不相同，多主链的 multi-master 架构可以提供更丰富的见证机制，避免主链的技术特性成为 Void 的瓶颈。
<h4 class='sub-title'>multi world</h4>

未来的区块链生态一定会更加丰富，形成计算/存储/通讯的三位一体的开放网络，Void 提供一个通用的数据流网络，可以承载数据存储，消息通讯，侧链交易等信息，为不同的 DApp 提供特定应用的数据类型，适配不同的应用场景，补充不同主链在应用层的可扩展性。这些子链独立的运作，高度并行，性能随着网络节点的增加水平扩展。`
      }
    }
  }
}
</script>