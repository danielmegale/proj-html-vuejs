<script>
export default {
    data() {
        return {
            images: [
                {
                    img: 'ina-soulis-227104-unsplash-1024x1024.jpg'
                },
                {
                    img: 'sunisa-misa-531163-unsplash-1024x1024.jpg'
                },
                {
                    img: '355H-1024x1024.jpg'
                },
                {
                    img: 'photo-1448932252197-d19750584e56-1024x1024.jpg'
                },
                {
                    img: 'business-competition-PB366D8-1024x1024.jpg'
                },
                {
                    img: 'cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg'
                },
                {
                    img: 'aa9a4539-PQGJ7HU-1024x1024.jpg'
                },
                {
                    img: 'cody-davis-253928-unsplash-1024x1024.jpg'
                },
            ],

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
    <section class="container mt-5 pt-5">
        <div class="d-flex align-items-end mb-5">
            <div class="w-50">
                <div class="my-w-80 center mb-5">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
                <div>
                    <h2 class="font-50">Our recent <span class="text-success">web designs</span> & some examples of past
                        <span class="text-success">projects</span>
                    </h2>
                </div>
                <div class="my-w-80 center mt-5">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
            </div>
            <div class="w-50">
                <p>Far far away,behind the word mountains,far from the countries Vokalia and Consonatia,there live the
                    blinds texts. Separated they live in Bookmarkgrove right at the coast of the semantics, a large
                    language
                    ocean.Separated they live in Bookmarkgrove.</p>
            </div>
        </div>
        <div class="d-flex flex-wrap justify-content-between mt-5">
            <div class="my-w-25 gallery-hover" v-for="image in images">
                <img :src="getImg(image.img)" alt="">
            </div>
        </div>
        <div class="d-flex justify-content-center mt-5 pt-5 mb-5">
            <button class="my-btn box-shadow-green">READ MORE</button>
        </div>
    </section>
</template>


<style lang="scss" scoped>
@import '../assets/sass/custom';

.my-w-25 {
    padding: 3px 0;

    img {
        border-radius: 5px;
    }
}

.gallery-hover {
    position: relative;
}

.gallery-hover::after {
    content: '';
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: linear-gradient(to top right, $color-gradient-green);
    opacity: 0.9;
    display: none;
    border-radius: 5px;
}

.gallery-hover:hover.gallery-hover::after,
.gallery-hover:hover img {
    display: block;
    transform: scale(1.1);
    z-index: 1;
}
</style>