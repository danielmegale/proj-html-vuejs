<script>
export default {

}
</script>

<template>
    <main class="bg-secondary pt-5 mb-5 pb-5 mb-5">
        <section class="container d-flex p-5">
            <div class="w-50">
                <div class="my-w-800">
                    <div class=" bg-img-green">
                        <img src="../assets/images/busy-architect-PYVKWM4-1024x872.jpg" alt="">
                    </div>
                    <img src="../assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
                </div>
            </div>
            <div class="w-50">
                <h2 class="my-w-40">learn more about our<span class="text-success"> missions</span></h2>
                <div class="center my-w-80 py-3">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
                <p>Far far away,behind the word mountains,far from the countries Vokalia and Consonatia,there live the
                    blinds texts. Separated they live in Bookmarkgrove right at the coast of the semantics, a large
                    language
                    ocean.Separated they live in Bookmarkgrove.
                </p>
                <button class="my-btn mt-4">READ MORE</button>
            </div>
        </section>
    </main>
</template>

<style lang="scss">
@import '../assets/sass/custom';

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
    opacity: 0.8;
    border-radius: 35px;
}

.my-w-800 {
    position: relative;
}

.my-w-800>img {
    border-radius: 20px;
    position: absolute;
    top: 10%;
    left: 15%;
    width: 100%;
    height: 100%;
}
</style>