<template>
  <div class="container">
    <Description />
    <About />
  </div>
</template>

<script setup>
import Description from '../components/description.vue'
import About from '../components/about.vue'
</script>

<style scoped>
.container {
  display: flex;
}

@media (min-width: 250px) and (max-width: 870px) {
  .container {
    display: flex;
    flex-direction: column;
  }
}
</style>
