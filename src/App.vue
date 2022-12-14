<script>
import AppHeader from './components/AppHeader.vue';
import BlueSection from './components/BluSection.vue'
import AppLinks from './components/AppLinks.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    BlueSection,
    AppLinks,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <h1> --> content goes here </h1>
  </main>
  <BlueSection />
  <AppLinks />
  <AppFooter />
</template>

<style lang="scss">
@use './temp/partials/variables.scss' as *;
@use './temp/general.scss' as *;

main {
  height: 200px;
  background: black;


  h1 {
    color: white;
  }
}
</style>
