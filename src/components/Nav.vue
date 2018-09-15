<template>
  <!-- <nav class="dt w-100 border-box pa3 ph5-ns"> -->
    <!-- :class="{'nav-shadow': scrollToTop} -->
  <nav ref='nav' class="nav-bar" :class="{'nav-shadow': hasShadow}">
    <div class="nav-wrapper">
      <a class="dtc v-mid mid-gray link dim w-25" href="#" title="Home"></a>
      <!-- <div class="dtc v-mid w-75 tr fw4"> -->
      <div class="nav-btn-group">
        <!-- <a class="link dim dark-gray f6 f5-ns dib mr3 mr4-ns text" href="#" title="About">GitHub</a> -->
        <a href="#" title="About">GitHub</a>
        <a href="#" title="Store">About</a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data(){
    return {
      hasShadow: false
    }
  },
  mounted(){
    window.addEventListener('scroll', ()=>{
      if(window.pageYOffset>10){
        this.hasShadow = true
      } else {
        this.hasShadow = false
      }
    })
  },
  computed:{
  }
}
</script>

