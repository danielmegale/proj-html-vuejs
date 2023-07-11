<script>
export default {

}
</script>

<template>
    <main class="bg-secondary">
        <div class="container">
            <section class="center bg-img p-5">
                <div class="w-50">
                    <p class="text-success">17 YARS OF EXPERIENCE</p>
                    <h1>We are a</h1>
                    <h1>Web Design <span class="text-success">Agency</span></h1>
                    <div class="center my-w-80 py-3">
                        <div class="small-separator"></div>
                        <div class="separator"></div>
                    </div>
                    <p>Far far away,behind the word mountains,far from the countries Vokalia and Consonatia,there live the
                        blinds texts. Separated they live in Bookmarkgrove right at the coast of the semantics, a large
                        language
                        ocean.Separated they live in Bookmarkgrove.
                    </p>
                    <button class="btn-black mt-4">READ MORE</button>
                    <div class="mt-5 center">
                        <div class="social">
                            <a href="https://www.facebook.com/">Facebook</a>
                            <a href="https://www.instagram.com/">Instagram</a>
                            <a href="https://twitter.com">Twitter</a>
                            <a href="https://www.youtube.com/">YouTube</a>
                        </div>
                        <div class="counter-pages">
                            <a href="" class="text-white">1</a>
                            <a href="" class="text-white">2</a>
                            <a href="" class="text-white">3</a>
                        </div>
                    </div>
                </div>
            </section>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

@mixin center-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}

.center {
    @include center-flex;
}

.bg-img {
    background-image: url(../assets/images/Group-36-2x.png);
    background-size: 56%;
    background-repeat: no-repeat;
    background-position: right;
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

a {
    text-decoration: none;
    color: $black;
    padding: 0 10px;

}

.w-50 {
    width: 52%;
}

.social a:hover {
    color: $green;
}

.counter-pages {
    background-image: linear-gradient(to right, $color-gradient-black);
    border-radius: 15px;
    padding: 3px 6px;

    a {
        border-radius: 15px;


        &:hover {
            background-image: linear-gradient(to top left, $color-gradient-green);
        }
    }
}
</style>