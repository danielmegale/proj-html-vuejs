<script>
export default {
    data() {
        return {
            images: [
                {
                    img: 'serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg',
                    date: 'May 24, 2018-by Alex',
                    title: 'Marketing Ideas'
                },
                {
                    img: 'Businessman-at-the-desk-in-his-office-resting--1024x768.jpg',
                    date: 'May 24, 2018-by Alex',
                    title: 'Rest During Working Hours'
                },
                {
                    img: 'simple-home-office-with-tree-PBXRXYB-large-1024x768.jpg',
                    date: 'May 24, 2018-by Alex',
                    title: 'Develop Your Startup Idea'
                }
            ]
        }
    },
    methods: {
        getImg(target) {
            const url = new URL(`../assets/images/${target}`, import.meta.url)
            return url.href
        }
    }

}
</script>

<template>
    <section class=" container mt-5 pt-5 mb-5">
        <div class="text-center">
            <h2>Latest News & Our <span class="text-success">Blog</span></h2>
            <div class="my-w-80 center mb-5 mt-5">
                <div class="small-separator"></div>
                <div class="separator"></div>
            </div>
        </div>
        <div class="d-flex flex-wrap">
            <div class="card-container" v-for="image in images">
                <img :src="getImg(image.img)" alt="">
                <div class="card-description">
                    <p>{{ image.date }}</p>
                    <h5><i class="fa-solid fa-circle fa-2xs"></i>{{ image.title }}</h5>
                </div>
            </div>
        </div>
        <div class="text-center">
            <button class="btn-black">VIEW ALL POST</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

.text-center .my-w-80 {
    margin: 0 auto;
}

.card-container {
    width: calc(100% / 3);
    padding: 10px;

    img {
        border-radius: 8px;
    }
}

.card-container:hover .card-description {
    background-color: transparent;
    background-image: linear-gradient(to left bottom, $color-gradient-green);
    color: #ffffff;

    i {
        color: #ffffff;
    }
}

.card-description {
    position: relative;
    padding: 20px;
    bottom: 35px;
    left: 15px;
    width: 380px;
    background-color: #ffffff;
    box-shadow: 0px 0px 10px black;
    border-radius: 5px;

    i {
        color: $green;
        padding-right: 5px;
    }
}
</style>