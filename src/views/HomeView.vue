<template>
  <main>
    Hello
    <button type="button" class="btn btn-primary">Primary</button>
    <HomeCarousel />
  </main>
</template>

  <script setup>
  import HomeCarousel from "../components/home/HomeCarousel.vue"
  </script>

<style scoped>
main {
  display: flex;
  margin: auto;
  justify-content: center;
  max-width: 80%;
  background-color: red;
}
</style>