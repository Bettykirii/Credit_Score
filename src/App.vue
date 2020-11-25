<template>
  <div id="app">
    <Nav />
    
  <router-view/>
  <Footer/>
  </div>
</template>
<script>
import Nav from './components/partials/Nav.vue'
import Footer from './components/partials/Footer.vue'
export default {
  name: 'app',
  components: {
    Nav,
    Footer
    
  }  
}
</script>
<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background:darkgray;
  
}
</style>