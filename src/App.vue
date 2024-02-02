<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppJumbotron from './components/AppJumbotron.vue';


export default {
  name: 'Vite-comics',
  components: { AppHeader, AppMain, AppFooter, AppJumbotron }

};
</script>

<template>
  <AppHeader />
  <AppJumbotron />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>