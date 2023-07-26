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
        <img class="jumbotron" src="../assets/jumbotron.jpg" alt="">
        <!-- <div class="currentSeries">
            <span class="text-white fw-bolder">CURRENT SERIES</span>
        </div> -->
    </div>
    <div class="container-fluid">
        <div class="container p-3">
            <div class="currentSeries">
                <span class="text-white fw-bolder">CURRENT SERIES</span>
            </div>
            <div class="row row-cols-5">
                <template v-for="film in dcComics" :key="film">
                    <div class="col p-0">
                        <Product :image="film.thumb" :title="film.series" />
                    </div>
                </template>
            </div>
            <div class="text-center py-5">
                <span class="btn text-white bg-primary fw-bolder rounded">LOAD MORE</span>
            </div>
        </div>
    </div>
</template>

<style scoped>
.jumbotronContainer {
    width: 100%;
    position: relative;
}

.jumbotron {
    width: 100%;
    height: 30rem;
    object-fit: cover;
    object-position: 10% 0%;

}

.currentSeries {
    background-color: royalblue;
    padding: 3px;
    border-radius: 5px;
    display: inline-block;
    position: relative;
    bottom: 30px;
}
</style>
