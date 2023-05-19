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
  <AppNavbar />
  
</template>

<style scoped>

</style>
