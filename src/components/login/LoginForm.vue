<template>
  <div>
    <div id="login-form">
      <div id="login-form-content">
        <h3>Login</h3>
        <div class="input-group mb-3">
          <span class="input-group-text" id="inputGroup-sizing-default">Email</span>
          <input type="email" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
        </div>
        <div class="input-group mb-3">
          <span class="input-group-text" id="inputGroup-sizing-default">Password</span>
          <input type="password" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-default">
        </div>
        <RouterLink to="/reset"><p><a href="#" class="link-primary">Forgot your password?</a></p></RouterLink>
        <button type="button" class="btn btn-primary">Login</button>
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
  align-items: center;
  justify-content: center;
  flex-direction: column;
  margin: auto;
  max-width: 600px;
}

#login-form-content {
  background-color: red;
  padding: 50px;
}

input {
  max-width: 300px;
}
h3 {
  margin-bottom: 1rem;
}

.input-group-text {
  width: 100px;
}
</style>