<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppBlueBand from './components/AppBlueBand.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components:{
    AppHeader,
    AppMain,
    AppBlueBand,
    AppFooter,
  }
}
</script>

<template lang="">
  <div>
    <AppHeader />
    <AppMain />
    <AppBlueBand />
    <AppFooter />
  </div>
</template>

<style lang="scss">
  @use './styles/general.scss' as *;
</style>