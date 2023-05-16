<template>
  <div>
    <div id="login-view">
      <LoginForm />
    </div>
  </div>
</template>

<script setup>
import LoginForm from "../components/login/LoginForm.vue"
</script>

<style scoped>
#login-view {
  margin: auto;
  max-width: 600px;
}

@media only screen and (max-width: 500px) {
  #login-view {
    max-width: 100%;
  }
}
</style>