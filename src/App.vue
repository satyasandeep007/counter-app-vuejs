<template>
  <div id="app">
    
    <Navbar />
    <Counter />
    
  </div>
</template>

<script>
import Counter from './components/Counter.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'app',
  components: {
    Counter,
    Navbar
  }
}

</script>

<style scoped>

</style>
