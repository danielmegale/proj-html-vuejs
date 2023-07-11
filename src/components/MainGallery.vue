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
    <section>
        <div class="d-flex flex-wrap justify-content-between">
            <div class="my-w-25" v-for="image in images">
                <img :src="getImg(image.img)" alt="">
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped>
.my-w-25 {
    padding: 3px 0;

    img {
        border-radius: 15px;
    }
}
</style>