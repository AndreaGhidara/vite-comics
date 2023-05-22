<script>
import dcComics from '../data/dc-comics';
import Product from './Product.vue'

export default {
    name: "AppContent",
    components: {
        Product,
    },
    data() {
        return {
            dcComics
        }
    }
}
</script>

<template>
    <div class="jumbotronContainer">
        <img class="jumbotron"  src="../assets/jumbotron.jpg" alt="">
        <div class="currentSeries">
            <span class="text-white fw-bolder">CURRENT SERIES</span>
        </div>
    </div>
    <div class="container-fluid bg-dark">
        <div class="container p-3">
            <div class="row">
                <Product v-for="film in dcComics" :image="film.thumb" :title="film.series" />
            </div>
            <div class="text-center py-5">
                <span class="btn text-white fw-bolder rounded">LOAD MORE</span>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .jumbotronContainer{
        width: 100%;
        position: relative;
    }
    .jumbotron{
        width: 100%;
        height: 30rem;
        object-fit: cover;
        object-position: 10% 0%;
        
    }

    .currentSeries{
        background-color: royalblue;
        padding: 3px;
        border-radius: 10px;
        position: absolute;
        bottom: -13px;
        left: 10%;
    }
</style>
