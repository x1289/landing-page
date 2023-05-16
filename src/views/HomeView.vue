<template>
  <div>
    <div id="home-view">
      <h1>Welcome to this sample app!</h1>
      <p class="my-3">This app was built in just a few hours. With a little effort so much more is possible!</p>
      <div class="container d-flex justify-content-center align-items-center flex-column">
        <HomeCarousel class="mt-4"/>
        <hr class="border border-primary border-3 mt-5 w-75 opacity-75" />
        <HomeShowCase />
      </div>
    </div>
  </div>
</template>

  <script setup>
  import HomeCarousel from "../components/home/HomeCarousel.vue"
  import HomeShowCase from "../components/home/HomeShowCase.vue"
  </script>

<style scoped>
button {
  max-width: 120px;
}
#home-view {
  margin: auto;
  max-width: 900px;
}
</style>