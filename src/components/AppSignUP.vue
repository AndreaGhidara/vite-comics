<script>
    export default {
        name:"AppSignUP"
    }
</script>

<template>
    <div class="d-flex justify-content-between bgCustom z-1">
        <div class="container d-flex align-items-center justify-content-between py-4">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="social d-flex align-items-center">
                <p class="m-0 text-primary fw-bold">FOLLOW US</p>
                <img class="px-1" src="../assets/footer-facebook.png" alt="">
                <img class="px-1" src="../assets/footer-twitter.png" alt="">
                <img class="px-1" src="../assets/footer-youtube.png" alt="">
                <img class="px-1" src="../assets/footer-pinterest.png" alt="">
                <img class="px-1" src="../assets/footer-periscope.png" alt="">
            </div>
        </div>
    </div>
</template>

<style scoped>
    .bgCustom{
        background-color: #303030;
    }

    img{
        width: 40px;
    }

    button{
        font-weight: 600;
        padding: 0.5rem;
        color: royalblue;
        border: 2px solid royalblue;
        background-color: transparent;
    }
</style>
