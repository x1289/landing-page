<template>
  <div>
    <div id="reset-view">
      <h3>Reset your Password</h3>
      <div class="input-group mb-3">
          <span class="input-group-text" id="inputGroup-sizing-default">Email</span>
          <input type="text" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
        </div>
        <div class="d-grid gap-2 d-md-flex">          
          <RouterLink to="/" class="btn btn-primary me-md-2">Reset password</RouterLink>
          <RouterLink to="/login" class="btn btn-primary me-md-2">Cancel</RouterLink>
        </div>
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

h3 {
  margin-bottom: 1rem;
}
</style>