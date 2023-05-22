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
    <div class="col text-white">
        <div class="bg-dark my-3 text-center">
            <img class="rounded" :src="image" alt="">
            <div class="text-center">{{ title }}</div>
        </div>
    </div>
</template>

<style scoped>
img {
    width: 180px;
    height: 200px;
    object-fit: cover;
}
</style>
