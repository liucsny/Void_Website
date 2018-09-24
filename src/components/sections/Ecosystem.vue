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
      <!-- <div class="wrapper-cards">
        <div v-for="(item, index) in content.cards_2" :key="index" class="card">
          <h2>{{item.title}}</h2>
          <p>{{item.text}}</p>
        </div>
      </div> -->
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      content:{
        title: 'Void 的应用场景与生态系统',
        cards:[
          {
            title: '论坛 社交网络',
            text: '由于每条链相互follow的设计，Void天然适合与社交网络。每个用户形成一条子链，每个账户都可以发送消息，互相关注，评论和互动，所有这些行为都是子链上的事件，这些比传统区块链消息成本大大降低，数据同步效率更高。'
            // text: '每个用户都是一条子链  * 每个账户都可以发送消息，互相关注，评论和互动，所有这些行为都是子链上的事件  * 朋友的朋友通常也是朋友，子链之间具有逻辑的近邻性，利用数据的聚集性可以高效的同步  * 消息成本很低，可以自愿缓存数据  * 当用户存在滥用时，unfollow 这个子链，具有一定的内容控制能力'
          },
          {
            title: '数据同步与文件分发',
            text: '作为 authenticated feed 发布新版本的软件和文件资源  * 数据可验证，并且通过 message relay 提供权威性证明  * 稀疏的，增量的，实时的动态文件集更新'
          },
          {
            title: '区块链游戏',
            text: `在Void中，游戏的消息可以通过子链承载，部分消息可以提交到主链上见证，这样就大大减少了主链的负担；
                   基于Void的游戏平台可以为提供一定的消息分发，缓存服务，而游戏最后胜负则提交到主链上，触发合约行为。`
          },
        ],
        // cards_2: [
        //   {
        //     title: 'Hub',
        //     text: '每个用户都是一条子链  * 每个账户都可以发送消息，互相关注，评论和互动，所有这些行为都是子链上的事件  * 朋友的朋友通常也是朋友，子链之间具有逻辑的近邻性，利用数据的聚集性可以高效的同步  * 消息成本很低，可以自愿缓存数据  * 当用户存在滥用时，unfollow 这个子链，具有一定的内容控制能力'
        //   },
        //   {
        //     title: '数据同步与文件分发',
        //     text: '* 作为 authenticated feed 发布新版本的软件和文件资源  * 数据可验证，并且通过 message relay 提供权威性证明  * 稀疏的，增量的，实时的动态文件集更新'
        //   },
        //   {
        //     title: '区块链游戏',
        //     text: '* 作为 authenticated feed 发布新版本的软件和文件资源  * 数据可验证，并且通过 message relay 提供权威性证明  * 稀疏的，增量的，实时的动态文件集更新'
        //   },
        //   {
        //     title: '区块链游戏',
        //     text: '* 作为 authenticated feed 发布新版本的软件和文件资源  * 数据可验证，并且通过 message relay 提供权威性证明  * 稀疏的，增量的，实时的动态文件集更新'
        //   },
        // ]
      }
    }
  }
}
</script>
