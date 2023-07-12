<script>
export default {

}
</script>

<template>
    <main class="bg-secondary pt-5">
        <section class="container">
            <div class="center">
                <div class="big-card black-card m-3 p-5">
                    <div class="d-flex flex-column align-items-center justify-content-center h-100 ">
                        <p>Are You Ready?</p>
                        <h2>Start a New Project</h2>
                        <div class="input-group mt-3">
                            <input type="email" class="form-control" placeholder="Enter Your Email Address"
                                aria-label="Recipient's username" aria-describedby="button-addon2">
                            <button class="btn btn-outline-secondary" type="button" id="button-addon2">Button</button>
                        </div>
                    </div>
                </div>
                <div class="big-card green-card m-3 p-5">
                    <div class="d-flex flex-column align-items-center justify-content-center h-100 ">
                        <p>What Are You Waiting for?</p>
                        <h2>Let's Talk About Work</h2>
                        <button class="btn-black mt-5">START NOW</button>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>
<style lang="scss" scoped>
@import '../assets/sass/custom';

.big-card {
    height: 260px;
    width: 50%;
    border-radius: 13px;
    color: #ffffff;
    text-align: center;
}

.black-card {
    background-image: linear-gradient(to right, $color-gradient-black);
}

.green-card {
    background-image: linear-gradient(to left, $color-gradient-green);
}

.input-group {
    width: 80%;

    button {
        border: 0;
        background-color: #00000073;
        margin-left: 0;
    }
}

.form-control {
    background-color: #00000073;
    color: #ffffff;
    border: 0;
}

.form-control::placeholder {
    color: #70707059;
}
</style>