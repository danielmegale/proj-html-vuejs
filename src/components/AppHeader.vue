<script>

export default {

}
</script>


<template>
    <header>
        <section class=" container text-white center">
            <div>
                <i class="fa-solid fa-phone"></i>
                <span>(001)88451234</span>
                <span>88455438</span>
            </div>
            <div>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-pinterest-p"></i>
            </div>
        </section>
        <!-- NavBar -->
        <section class="bg-white my-h-100 box-shadow">
            <div class="container center">
                <a href="">

                    <img src="../assets/images/cropped-Group-39-2x.png" alt="">
                </a>
                <div class="center my-w-40">
                    <a href=""><span>HOME</span></a>
                    <a href=""><span>ABOUT</span></a>
                    <a href=""><span>SERVICE</span></a>
                    <a href=""><span>SHOWCASE</span></a>
                    <a href=""><span>BLOG</span></a>
                    <a href=""><span>CONTACT</span></a>
                </div>
                <div class="text-success">
                    <button type="button" class="my-btn">PURCHASE</button>
                    <i class="fa-solid fa-magnifying-glass"></i>
                </div>
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

@mixin center-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}

section {
    i {
        padding: 10px;
    }

    span {
        padding-right: 20px;
    }
}

// NavBar
.center {
    @include center-flex;
}
</style>