<template>
  <div>
    <app-landing/>
    <app-intro/>
    <app-section-1/>
    <app-section-2/>
    <app-section-3/>
    <app-void-intro/>
    <app-ecosystem/>
    <app-section-4/>
    <app-summary/>
  </div>
</template>

<script>
import appLanding from './sections/Landing.vue';
import appIntro from './sections/Intro.vue';
import appSection1 from './sections/Section1.vue';
import appSection2 from './sections/Section2.vue';
import appSection3 from './sections/Section3.vue';
import appSection4 from './sections/Section4.vue';
import appVoidIntro from './sections/VoidIntro.vue';
import appEcosystem from './sections/Ecosystem.vue';
import appSummary from './sections/Summary.vue';

export default {
  name: '',
  components: { 
    appLanding,
    'app-intro':appIntro,
    'app-section-1': appSection1,
    'app-section-2': appSection2,
    'app-section-3': appSection3,
    'app-section-4': appSection4,
    'app-void-intro': appVoidIntro,
    'app-ecosystem': appEcosystem,
    'app-summary': appSummary
  }
};
</script>

<style scoped>
</style>
