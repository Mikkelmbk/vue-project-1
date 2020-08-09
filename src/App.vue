<template>
  <div class="min-h-screen" id="app">
    <Nav class="mb-6" />
    <Carousel class="center" />
  </div>
</template>

<script>

import Nav from './components/Nav.vue'
import Carousel from './components/Carousel.vue'

export default {
  name: 'App',
  components: {
    Nav,
    Carousel
  }
}
</script>

<style>

</style>
