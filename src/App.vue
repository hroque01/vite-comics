<script>
import AppHeader from './components/AppHeader.vue';
import BlueSection from './components/BluSection.vue'

export default {
  components: {
    AppHeader,
    BlueSection
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <h1>content goes here</h1>
  </main>
  <BlueSection />
</template>

<style lang="scss">
@use './temp/partials/variables.scss' as *;
@use './temp/general.scss' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
  color: $primary;
}

main {
  height: 200px;
  background: black;

  main h1 {
    color: white;
  }
}
</style>
