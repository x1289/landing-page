<template>
  <div>
    <div id="login-form" class="pt-5">
      <div id="login-form-content">
        <h2 class="mb-4">Login</h2>
        <div class="input-group mb-3">
          <span class="input-group-text" id="inputGroup-sizing-default">Email</span>
          <input type="email" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
        </div>
        <div class="input-group mb-3">
          <span class="input-group-text" id="inputGroup-sizing-default">Password</span>
          <input type="password" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
        </div>
        <RouterLink to="/reset"><p><a href="#" class="link-primary">Forgot your password?</a></p></RouterLink>
        <button type="button" class="btn btn-primary w-100">Login</button>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
#login-form {
  height: calc(100vh - 100px);
  // background-color: green;
  display: flex;
  flex-direction: column;
  margin: auto;
  max-width: 600px;
}

#login-form-content {
  padding: 50px;
}

h3 {
  margin-bottom: 1rem;
}

.input-group-text {
  width: 100px;
}
</style>