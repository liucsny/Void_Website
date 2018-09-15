<template>
  <section class="intro">
    <div class="container">
      <div class="title">传统区块链正面临着哪些挑战?</div>
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
          title:'网络吞吐量小',
          text:'比特币网络的信息吞吐量，目前理论上的最大值也只有 7tps；以太坊大约有 20tps。相对的，VISA吞吐量通常达到2000 tps，峰值可达 10000tps，而推特通常达到 5000tps，峰值15000tps。',
          img: require('../../assets/1-1.svg')
        },
        {
          title:'存储成本高昂',
          text:'在以太坊网络中，向主链储存数据是一项极其昂贵的操作，每一个写入数据的操作都需要支付相应的gas，而且这也会导致区块臃肿等问题，这对于区块链的商业应用落地等问题是一个极大的瓶颈。',
          img: require('../../assets/1-2.svg')
        },
        {
          title:'交易确认时间长',
          text:'为了保证比特币转账的安全性，比特币网络的交易确认时间大约为十分钟左右，如果网络拥堵或交易费过少，则可能长达数小时；而以太坊网络常常由于网络问题出现延时情况，这显然无法满足日常的需求。',
          img: require('../../assets/1-3.svg')
        }
      ]
    }
  }
}
</script>
