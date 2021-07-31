<template>
  <div id="app">
    <navbar />
    <router-view/>
  </div>
</template>

<script>
import Navbar from './components/Navbar/index.vue'
export default {
  components: {
    Navbar
  }
}
</script>

<style lang="scss">
</style>
