<script>
import AppHeader from './components/AppHeader.vue'
export default {
  name: 'Vite-comics',
  components: { AppHeader }

};
</script>

<template>
  <AppHeader />
</template>

<style lang="scss">
@use './assets/scss/style.scss';

/*Reset*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Gnereics */

img {
  max-width: 100%;
}

a {
  text-decoration: none;
}
</style>