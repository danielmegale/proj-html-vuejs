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
                <img src="../assets/images/cropped-Group-39-2x.png" alt="">
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

.center {
    @include center-flex;
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

.box-shadow {
    box-shadow: 0px 10px 20px #BBB;
}
</style>