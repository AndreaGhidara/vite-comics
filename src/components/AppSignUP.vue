<script>
    export default {
        name:"AppSignUP",
    data() {
        return {
            socials: [
                {
                    path:"../assets/footer-facebook.png",
                    name:"Facebook",
                },
                {
                    path:"../assets/footer-twitter.png",
                    name:"Twitter",
                },
                {
                    path:"../assets/footer-youtube.png",
                    name:"youtube",
                },
                {
                    path:"../assets/footer-pinterest.png",
                    name:"pinterest",
                },
                {
                    path:"../assets/footer-periscope.png",
                    name:"periscope",
                },
            ]
        }
    },
    methods: {
        getImagePath: function(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    },
    }
</script>

<template>
    <div class="d-flex justify-content-between bgCustom">
        <div class="container d-flex align-items-center justify-content-between py-4">
            <div>
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="social d-flex align-items-center">
                <p class="m-0 text-primary fw-bold">FOLLOW US</p>
                <div v-for="social in socials">
                    <img class="px-1" :src="getImagePath(social.path)" alt="">
                </div>
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

    img:hover{
        filter: drop-shadow(0 0 20px #ababb4);
    }

    button{
        font-weight: 600;
        padding: 0.5rem;
        color: royalblue;
        border: 2px solid royalblue;
        background-color: transparent;
    }
</style>
