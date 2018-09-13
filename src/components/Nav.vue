<template>
  <!-- <nav class="dt w-100 border-box pa3 ph5-ns"> -->
  <nav class="nav-bar" :class="{'nav-shadow': (this.$el.offsetHeight > 0)}">
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

