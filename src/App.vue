<script>
import AppHeader from './components/AppHeader.vue';
import BlueSection from './components/BluSection.vue';
import AppLinks from './components/AppLinks.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import Jumbotron from './components/Jumbotron.vue';

export default {
  components: {
    AppHeader,
    BlueSection,
    Jumbotron,
    AppMain,
    AppLinks,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <Jumbotron />
  <main>
    <AppMain />
  </main>
  <BlueSection />
  <AppLinks />
  <AppFooter />
</template>

<style lang="scss">
@use './temp/partials/variables.scss' as *;
@use './temp/general.scss' as *;

main {
  background: black;


  h1 {
    color: white;
  }
}
</style>
