<template>
  <div>
    <div id="sing-up-view" class="pt-5">
      <h2 class="mb-4">Sign Up</h2>
      <div class="input-group mb-3">
        <span class="input-group-text">Email</span>
        <input type="text" class="form-control" aria-label="Email input" aria-describedby="inputGroup-sizing-default">
      </div>
      <div class="input-group mb-3">
        <span class="input-group-text">Password</span>
        <input type="text" class="form-control" aria-label="Password input" aria-describedby="inputGroup-sizing-default">
      </div>
      <div class="input-group mb-3">
        <span class="input-group-text">Confirm password</span>
        <input type="text" class="form-control" aria-label="Confirm password input" aria-describedby="inputGroup-sizing-default">
      </div>
      <p class="mt-3">Already registered? <a href="#" class="link-primary">Log in.</a></p>
      <RouterLink to="/" class="btn btn-primary w-100 my-3 me-2">Register</RouterLink>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
#sing-up-view {
  margin: auto;
  max-width: 600px;
}

.input-group-text {
  width: 160px;
}

h3 {
  margin-bottom: 1rem;
}
</style>