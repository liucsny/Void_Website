<template>
  <section class="container section-text-right">
      <div class="img-box">
        <img src="../../assets/img_1.svg" alt="Landing img">
      </div>
      <div class="text-box">
        <div class="text-wrapper">
          <div class="digit">0001</div>
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
        title: '一个高性能  高度可扩展 轻量级的区块链侧链网络',
        text: 'Void 是一个高性能，高度可扩展的分布式数据流网络，也是一个轻量级的区块链侧链网络。</br>Void 使用类似区块链的数据结构，每个用户或每个应用都是一条独立的链，即时发布消息，不需要等待矿工确认和负担矿工费。由于每一条链各自独立，不需要像比特币的区块链那样打包交易，所以 Void作为一个可验证数据结构和只增日志结构，数据在网络中广播，并以一定的规则分布，形成高效的去中心自治网络。</br>这些数据结构设计赋予了Void良好的网络吞吐量和可拓展性。'
      }
    }
  }
}
</script>
