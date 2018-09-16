<template>
  <section class="container section-ecosys">
    <div class="wrapper-ecosys">
      <div class="wrapper-title">
        <div class="digit">0100</div>
        <div class="title">{{content.title}}</div>
      </div>
      <div class="wrapper-cards">
        <div v-for="(item, index) in content.cards" :key="index" class="card">
          <h2>{{item.title}}</h2>
          <p>{{item.text}}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      content:{
        title: 'Void 的技术架构与生态系统',
        cards:[
          {
            title: 'Void',
            text: '和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。'
          },
          {
            title: 'Void',
            text: '和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。'
          },
          {
            title: 'Void',
            text: '和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。'
          },
          {
            title: 'Void',
            text: '和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。和只增日志结构（append-only log），数据在网络中广播（gossiping），并以一定的规则分布，形成高效的去中心自治网络。'
          },
        ]
      }
    }
  }
}
</script>
