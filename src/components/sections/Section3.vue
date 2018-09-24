<template>
  <section class="container section-text-right">
      <div class="img-box">
        <img src="../../assets/img_1.svg" alt="Landing img">
      </div>
      <div class="text-box">
        <div class="text-wrapper">
          <div class="digit">0011</div>
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
        title: 'Void 的灵活性和</br>应用友好性',
        text: `对于许多区块链应用来说，以太坊等基于复制状态机的区块链，很难与应用本身所需的数据结构匹配。而Void 不仅可以为应用提供定制的消息类型，还可以根据应用需求，方便的生成与应用结构相匹配的数据，简化 Dapp 的开发和集成难度。</br>
              基于消息的数据结构使得 Void 不需要大量的计算就能构造新的消息，保证了单节点的吞吐能力；</br>
              DApp 服务方也可以建立自己的节点，免费为用户存储/分发/见证数据，降低使用门槛，通过服务和内容盈利。这些设计都有助于构建一个高效的数据流网络，支撑通讯，媒体，社交，游戏等应用。`
      }
    }
  }
}
</script>
