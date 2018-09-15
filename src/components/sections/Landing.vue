<template>
  <section class="landing">
    <div class="container box-flex">
      <div class="box-left">
        <div class="box-left-wrapper">
          <div>
            <p class="digit">0000</p>
            <h1>VOID</h1>
            <h2>{{content.title}}<span>.</span></h2>
          </div>
          <div class="link-group">
            <a target="_blank" href="https://github.com/voidproject/about-void" class="link">技术文档 <img class="arrow" src="@/assets/icons/arrow.svg" alt="arrow"></a>
            <a href="#" class="link">Github <img class="arrow" src="@/assets/icons/arrow.svg" alt="arrow"></a>
          </div>
        </div>
      </div>
      <div class="box-right">
        <img class="w-80-ns w-100" src="../../assets/img_1.svg" alt="Landing img">
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data(){
    return {
      content: {
        title: '一个可扩展的高性能分布式网络'
      }
    }
  }
}
</script>
