<template>
  <div>
    <div class="card mb-5" @mouseover="isHovering = true"  @mouseout="isHovering = false" :class="{'shadow bg-body-tertiary rounded': isHovering}" >
      <div class="card-body">
        <div class="d-flex justify-content-center align-items-center flex-column">
          <h4 class="mt-5 card-title">{{ props.title }}</h4>
          <h5 class="my-3">{{ props.pricePerMonth }} / month</h5>
          <p v-for="(point, index) in props.includedPoints" :key="index" class="card-text text-center">{{ point }}</p>
        </div>
        <RouterLink v-if="$route.path != '/login'" to="/login"><button id="login-btn" class="btn" :class="props.active ? 'btn-success' : 'btn-outline-success'" type="submit">CHOOSE THIS PLAN</button></RouterLink>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isHovering = ref(false);

const props = defineProps({
  title: String,
  pricePerMonth: String,
  includedPoints: Array,
  active: Boolean
})

</script>

<style lang="scss" scoped>
.card {
  width: 15rem !important;
  height: 34rem;
}

.card-body {
  display: flex;
  flex-flow: column wrap;
  justify-content: space-between;
  align-items: center;
}
</style>