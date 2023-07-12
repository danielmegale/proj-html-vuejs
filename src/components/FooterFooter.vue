<script>
export default {
}
</script>


<template>
    <footer>
        <section class="container">
            <div class="center">
                <p>© 2023 PHLOX BUSINESS THEME.</p>
                <div>
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-pinterest-p"></i>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

footer {
    background-image: linear-gradient(to right, $color-gradient-black);
}

section>div {
    height: 100px;
}

div p {
    margin: 0;
    color: $gray-600;
    font-size: 10px;
}

div i {
    color: $gray-600;
    padding: 10px;
}
</style>