<script>
import AppHeader from './components/AppHeader.vue';
import BlueSection from './components/BluSection.vue'
import AppLinks from './components/AppLinks.vue'

export default {
  components: {
    AppHeader,
    BlueSection,
    AppLinks,
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <h1>content goes here</h1>
  </main>
  <BlueSection />
  <AppLinks />
</template>

<style lang="scss">
@use './temp/partials/variables.scss' as *;
@use './temp/general.scss' as *;

main {
  height: 200px;
  background: black;

  main h1 {
    color: white;
  }
}
</style>
