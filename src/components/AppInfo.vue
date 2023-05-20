<script>
export default {
    name: "AppInfo",
    data() {
        return {
            ComicsInfoShop : [
                {
                    path:"../assets/buy-comics-digital-comics.png",
                    text:"Digital Comics",
                },
                {
                    path:"../assets/buy-comics-merchandise.png",
                    text:"Digital Comics",
                },
                {
                    path:"../assets/buy-comics-subscriptions.png",
                    text:"Digital Comics",
                },
                {
                    path:"../assets/buy-comics-shop-locator.png",
                    text:"Digital Comics",
                },
                {
                    path:"../assets/buy-dc-power-visa.svg",
                    text:"Digital Comics",
                },
            ]
        }
    },
    methods: {
        getImagePath: function(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    },
    mounted() {

    }
}
</script>

<template>
    <div class="d-flex align-items-center text-white bg-primary py-5 z-1">
        <div class="container d-flex justify-content-evenly">
            <div v-for="info in ComicsInfoShop" class="d-flex align-items-center">
                <img v-bind:src="getImagePath(info.path)" alt="">
                <p>{{info.text}}</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
p {
    padding-left: 10px;
    font-size: 20px;
    font-weight: 500;
}

img {
    width: 60px;
}
</style>
