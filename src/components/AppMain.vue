<script>
import MainJumbotron from './MainJumbotron.vue';
import ChooseusCrard from './ChooseusCrard.vue';
import MainMission from './MainMission.vue';
import MainGallery from './MainGallery.vue';
import ClientJumbotron from './ClientJumbotron.vue';
export default {
    components: { MainJumbotron, ChooseusCrard, MainMission, MainGallery, ClientJumbotron }
}
</script>


<template>
    <MainJumbotron />
    <ChooseusCrard />
    <MainMission />
    <MainGallery />
    <ClientJumbotron />
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

.bg-img-green {
    position: relative;

    img {
        border-radius: 35px;
    }
}

.bg-img-green::after {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: linear-gradient(to top right, $color-gradient-green);
    opacity: 0.9;
    border-radius: 35px;
}
</style>