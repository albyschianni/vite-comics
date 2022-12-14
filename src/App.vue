<script >
import AppHeader from './components/AppHeader.vue';
import AppMiddleVue from './components/AppMiddle.vue';
import AppUpFooter from './components/AppUpFooter.vue';
import AppFooter from './components/AppFooter.vue';
import AppContentMovieVue from './components/AppContentMovie.vue';
import AppJumboVue from './components/AppJumbo.vue';

export default{
  name: 'App',
  components: {
    AppHeader,
    AppMiddleVue,
    AppUpFooter,
    AppFooter,
    AppContentMovieVue,
    AppJumboVue
  }
}
</script>

<template>
  <AppHeader />
  <AppJumboVue />
  <AppContentMovieVue />
  <AppMiddleVue />

  <AppUpFooter />
  <AppFooter />

</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

h1,
h2,
h3,
h4,
h5,
h6 {
    color: $primary;
}
</style>
