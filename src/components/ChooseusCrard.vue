<script>
export default {

}
</script>


<template>
    <main>
        <section class="container d-flex p-5">
            <div class="w-50">
                <h2 class="w-50">We Are Here To Make Your <span class="text-success">Website</span> Look More <span
                        class="text-success">Elegant</span> And Stylish!</h2>
                <div class="center my-w-80 py-3 mt-3">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
                <button class="my-btn mt-5">VIEW ALL</button>
            </div>
            <div class="w-50 row gap-4">
                <div class="card my-card box-shadow" style="width: 18rem;">
                    <div class="card-body">
                        <h2 class="card-title"><i class="fa-solid fa-gauge-high"></i></h2>
                        <h6 class="card-subtitle mb-2 ">Speed Optimization</h6>
                        <p class="text-black">Far far away,behind the word mountains,far from the countries Vokalia
                            Separated
                            ...</p>
                    </div>
                </div>
                <div class="card my-card box-shadow" style="width: 18rem;">
                    <div class="card-body">
                        <h2 class="card-title"><i class="fa-solid fa-cloud"></i></h2>
                        <h6 class="card-subtitle mb-2 ">Speed Optimization</h6>
                        <p class="text-black">Far far away,behind the word mountains,far from the countries Vokalia
                            Separated
                            ...</p>
                    </div>
                </div>
                <div class="card my-card box-shadow" style="width: 18rem;">
                    <div class="card-body">
                        <h2 class="card-title"><i class="fa-solid fa-mobile-screen-button"></i></h2>
                        <h6 class="card-subtitle mb-2 ">Speed Optimization</h6>
                        <p class="text-black">Far far away,behind the word mountains,far from the countries Vokalia
                            Separated
                            ...</p>
                    </div>
                </div>
                <div class="card my-card box-shadow" style="width: 18rem;">
                    <div class="card-body">
                        <h2 class="card-title"><i class="fa-regular fa-clock"></i></h2>
                        <h6 class="card-subtitle mb-2 ">Speed Optimization</h6>
                        <p class="text-black">Far far away,behind the word mountains,far from the countries Vokalia
                            Separated
                            ...</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss">
@import '../assets/sass/custom';

.my-card {
    cursor: pointer;

    &:hover {
        background-image: linear-gradient(to bottom left, $color-gradient-green);
        border: 0;
    }
}
</style>