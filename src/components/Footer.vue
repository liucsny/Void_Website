<template>
  <footer>
    <div class="container">
      <div class="wrapper-info">
        <h1 class="title">Void Project</h1>
        <div class="info-flex-box">
          <article v-for="(item, index) in content.info" :key="index">
            <h4>{{item.title}}</h4>
            <div>{{item.adress}}</div>
            <a href="#">{{item.contact}}</a>
          </article>
        </div>
      </div>
      <div class="copyright-flex" >
        <div>
          <p>{{content.copyright}}</p>
        </div>
        <div>
          <a class="icons" v-for="(item, index) in content.socialmedia" :key="index" :href="item.link" title="">
            <img :src="item.img" alt="">
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data(){
    return{
      content:{
        info:[
          {
            title:'SF',
            adress:'837 Larkin St.',
            contact: '+1 207-555-5555'
          },
          {
            title:'LA',
            adress:'837 Larkin St.',
            contact: '+1 207-555-5555'
          },
          {
            title:'London',
            adress:'837 Larkin St.',
            contact: '+1 207-555-5555'
          },
          {
            title:'Tokyo',
            adress:'837 Larkin St.',
            contact: '+1 207-555-5555'
          },
        ],
        copyright: 'Copyright © Void Project 2018',
        socialmedia:[
          {
            img: require('../assets/icons/github.svg'),
            link: 'www.github.com'
          },
          {
            img: require('../assets/icons/facebook.svg'),
            link: 'www.github.com'
          },
          {
            img: require('../assets/icons/medium.svg'),
            link: 'www.github.com'
          },
          {
            img: require('../assets/icons/linkedin.svg'),
            link: 'www.github.com'
          },
          {
            img: require('../assets/icons/twitter.svg'),
            link: 'www.github.com'
          },
        ]
      }
    }
  }
}
</script>


<style scoped>
img{
  height: 1.9rem;
}
</style>

