<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';

export default {
  name: 'Vite-comics',
  components: { AppHeader }

};
</script>

<template>
  <AppHeader />
  <AppMain />
</template>

<style lang="scss">
@use './assets/scss/style.scss';

/*Reset*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Generics */

img {
  max-width: 100%;
}

a {
  text-decoration: none;
}

/*Utilies*/
.container {
  max-width: 80%;
  margin: 0 auto;
}
</style>