<script>
import AppNavbar from './components/AppNavbar.vue';
import AppContent from './components/AppContent.vue';
import AppInfo from './components/AppInfo.vue'
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppNavbar,
    AppContent,
    AppInfo,
    AppFooter,
  },
  data() {
    return {
      variabile: 42
    }
  },
  methods: {
    metodo() {
      
    }
  },
  mounted() {
    
  }
}

</script>

<template>
  <button class="m-5 p-1 btn btn-primary">ClickMe</button>
</template>

<style scoped>

</style>
