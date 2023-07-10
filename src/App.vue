<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: { AppHeader, AppMain, AppFooter }
}
</script>


<template>
  <div class="bg-black fixed">
    <AppHeader />
  </div>
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
.fixed {
  position: sticky;
  top: 0;
  left: 0;
  right: 0;
}
</style>
