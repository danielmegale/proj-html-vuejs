<script>
import MainJumbotron from './MainJumbotron.vue';
import ChooseusCrard from './ChooseusCrard.vue'
export default {
    components: { MainJumbotron, ChooseusCrard }
}
</script>


<template>
    <MainJumbotron />
    <ChooseusCrard />
</template>

<style lang="scss">
@import '../assets/sass/custom';

@mixin center-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.center {
    @include center-flex;
}
</style>