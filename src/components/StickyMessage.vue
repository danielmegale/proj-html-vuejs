<script>
export default {
    data() {
        return {
            flag: false
        }
    }
}
</script>

<template>
    <section class="message" @click="flag = !flag">
        <div class="chat" :class="{ active: flag }">
            <div class="header-chat">

            </div>
        </div>
        <div class="chat-icon">
            <i class="fa-regular fa-comment fa-flip-horizontal"></i>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@import '../assets/sass/custom';

.chat {
    position: absolute;
    right: 0;
    top: -300px;
    height: 300px;
    width: 200px;
    background-color: #ffffff;
    display: none;
    border: 1px solid black;
}

.message {
    position: fixed;
    bottom: 37px;
    right: 44px;
    color: #ffffff;

    .chat-icon {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #527CEB;
        border-radius: 50%;
        height: 60px;
        width: 60px;
        font-size: 25px;
        cursor: pointer;


    }

}

.active {
    display: block;
}

.header-chat {
    height: 40px;
    width: 100%;
    background-color: #527CEB;
}
</style>