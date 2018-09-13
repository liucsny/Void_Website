<template>
  <div id="app" class="sans-serif">
    <app-nav></app-nav>
    <router-view/>
    <app-footer></app-footer>
  </div>
</template>

<script>
import appNav from '@/components/Nav';
import appFooter from '@/components/Footer';

export default {
  name: 'App',
  components: { appNav, appFooter },
};
</script>

<style lang="scss">
@import './style/style.scss';
</style>
