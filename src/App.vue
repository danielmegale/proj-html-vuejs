<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components: { AppHeader, AppMain, AppFooter }
}
</script>


<template>
  <div class="bg-black sticky">
    <AppHeader />
  </div>
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@import './assets/sass/custom';

.sticky {
  position: sticky;
  top: 0;
  left: 0;
  right: 0;
  z-index: 2;
}

.my-btn {
  background-image: linear-gradient(to right, $color-gradient-green);
  padding: 10px 15px;
  border-radius: 30px;
  color: #ffffff;
  border: 0;

  &:hover {
    background-image: linear-gradient(to right, $color-gradient-black);
  }
}

.btn-black {
  background-image: linear-gradient(to right, $color-gradient-black);
  padding: 10px 15px;
  border-radius: 30px;
  color: #ffffff;
  border: 0;

  &:hover {
    background-image: linear-gradient(to right, $color-gradient-green);
  }
}
</style>
