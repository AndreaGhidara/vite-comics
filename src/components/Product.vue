<script>

export default {
    name: "Product",
    props: {
        image: String,
        title: String,
    },
}
</script>

<template>
    <div class="text-white">
        <div class="my-3 text-center">
            <img :src="image" alt="">
            <div class="bg-primary title">
                <div class="text-center">{{ title }}</div>
            </div>
        </div>
    </div>
</template>

<style scoped>
img {
    width: 250px;
    height: 350px;
    object-fit: cover;
    border-radius: 10px 10px 10px 10px;
}

.title{
    width: 80%;
    margin: auto;
    border-radius:0 0 10px 10px ;
}
</style>
