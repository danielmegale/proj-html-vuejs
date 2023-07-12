<script>
export default {

}
</script>

<template>
    <div class="bg-img-black mt-5 mb-5 ">
        <img src="../assets/images/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg" alt="">
        <div class="paragraph">
            <i class="fa-solid fa-quote-left fa-2xl mt-5 pt-5"></i>
            <h3>When it comes to barbequing, there are two main schools of thought for the techniques that you can use.
                Freshly scrambled eggs with applewood smoked bacon - are amazing!</h3>
            <img class="mt-5" src="../assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
            <h4 class="mt-3">LISSA DURIN</h4>
            <p>Client</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

.bg-img-black {
    position: relative;
    height: 550px;

    img {
        height: 100%;
        width: 100%;
    }
}

.bg-img-black::after {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: linear-gradient(to bottom left, $color-gradient-black);
    opacity: 0.9;
}

.paragraph {
    position: absolute;
    top: 0;
    left: 25%;
    width: 50%;
    height: 100%;
    z-index: 1;
    text-align: center;
    color: white;


    i {
        color: $green;
    }

    h3 {
        line-height: 45px;
        padding-top: 15px;
    }

    h4 {
        color: $green;
    }

    img {
        height: 100px;
        width: 100px;
        border-radius: 50%;
        border: 2px solid lightgrey;
        margin: 0 auto;
    }
}
</style>