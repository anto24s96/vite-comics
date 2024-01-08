<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppSubmain from './components/AppSubmain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppSubmain,
    AppFooter
  }
}
</script>
<template lang="">
  <div>
    <AppHeader />
    <AppMain />
    <AppSubmain />
    <AppFooter />
  </div>
</template>
<style lang="scss">
@use "./styles/generals.scss" as *;
@use "./styles/partials/variables" as *;
</style>