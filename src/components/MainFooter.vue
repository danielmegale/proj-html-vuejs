<script>
export default {
    data() {
        return {
            links: ['Careers', 'News', 'Terms of use', 'Privacy Projects', 'About', 'Contact']
        }
    }
}
</script>


<template>
    <section class="container mt-5 mb-5">
        <div class="d-flex">
            <div>
                <img class="pb-4" src="../assets/images/cropped-Group-39-2x.png" alt="">
                <p class="p-3">While the lovely valley teems with vapour around me, and the meridian sun strikes the upper
                    surface of
                    the impenetrable foliage of my trees.While the lovely valley teems with vapour around me.</p>
            </div>
            <div>
                <h3>QUICK LINKS</h3>
                <div class="my-w-80 center mb-5">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
                <p class="line-height" v-for="link in links">{{ link }}</p>
            </div>
            <div>
                <h3>CONTACT</h3>
                <div class="my-w-80 center mb-5">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
                <p>Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, TX 76051</p>
                <p>info@yourdomain.com</p>
                <p>+99 (0) 101 0000 888</p>
            </div>
            <div>
                <h3>LOCATION ON MAP</h3>
                <div class="my-w-80 center mb-5">
                    <div class="small-separator"></div>
                    <div class="separator"></div>
                </div>
                <img src="../assets/images/map.png" alt="">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

.d-flex>div {
    flex-basis: calc(100% / 4);
    padding: 15px;
}

.line-height {
    line-height: 10px;
    cursor: pointer;
}

.line-height:hover {
    color: $green;
}
</style>