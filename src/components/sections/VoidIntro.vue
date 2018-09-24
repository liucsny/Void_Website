<template>
  <section class="intro">
    <div class="container section">
      <div class="box-flex">
        <div v-for="(item, index) in content" :key="index" class="box-flex-item">
          <img :src="item.img" alt="">
          <div class="text">
            <h2>{{item.title}}</h2>
            <p v-html="item.text"></p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return{
      content:[
        {
          title:'运行性能高',
          text:'Void的链与链之间follow的独特设计，使得每个应用，每个用户都能开设新的侧链，只需要链间异步的见证，使得整个侧链网络能够高度并行，这都增强了每一条链的运行性能，以及整个网络的吞吐性能。',
          img: require('../../assets/2-1.svg')
        },
        {
          title:'可拓展性好',
          text:'Void 可以承载不同的数据内容，不同类型的应用在消息体中扩展自己的消息类型；网络可以灵活的软分叉，随着新的应用出现，扩展新的能力。每一条链也可以分成不同的命名空间，分配不同的内容发布权限，以适应不同的应用。',
          img: require('../../assets/2-2.svg')
        },
        {
          title:'网络量级轻',
          text:'Void 使用类似区块链的数据结构，每个用户或每个应用都是一条独立的链，即时发布消息，形成高效的去中心自治网络，不需要等待矿工确认和负担矿工费，不需要像比特币的区块链那样打包交易，确保了网络的轻量化运行。',
          img: require('../../assets/2-3.svg')
        }
      ]
    }
  }
}
</script>
