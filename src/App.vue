<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppUpperFooter from './components/AppUpperFooter.vue';
import AppBottomFooter from './components/AppBottomFooter.vue';

export default {
  name: 'Vite-comics',
  components: { AppHeader, AppMain, AppUpperFooter, AppBottomFooter }

};
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppUpperFooter />
  <AppBottomFooter />
</template>

<style lang="scss">
@use './assets/scss/style.scss';
</style>