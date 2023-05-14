<template>
  <div>
    <div id="reset-view">
      <h3>Sign Up</h3>
      <div class="input-group mb-3">
        <span class="input-group-text" id="inputGroup-sizing-default">Email</span>
        <input type="text" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
      </div>
      <div class="input-group mb-3">
        <span class="input-group-text" id="inputGroup-sizing-default">Password</span>
        <input type="text" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
      </div>
      <div class="input-group mb-3">
        <span class="input-group-text" id="inputGroup-sizing-default">Confirm password</span>
        <input type="text" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
      </div>
      <RouterLink to="/" class="btn btn-primary me-md-2">Register</RouterLink>
      <p>Already registered? <a href="#" class="link-primary">Log in.</a></p>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
#reset-view {
  background-color: green;
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