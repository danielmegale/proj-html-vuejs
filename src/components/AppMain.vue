<script>
import MainJumbotron from './MainJumbotron.vue';
import ChooseusCrard from './ChooseusCrard.vue';
import MainMission from './MainMission.vue';
import MainGallery from './MainGallery.vue';
export default {
    components: { MainJumbotron, ChooseusCrard, MainMission, MainGallery }
}
</script>


<template>
    <MainJumbotron />
    <ChooseusCrard />
    <MainMission />
    <MainGallery />
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