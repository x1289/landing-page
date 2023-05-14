<template>
  <div id="navbar">
    <nav class="navbar fixed-top navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <RouterLink to="/" class="navbar-brand">Navbar</RouterLink>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <RouterLink to="/" class="nav-link active">Home</RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink to="/pricing" class="nav-link active">Pricing</RouterLink>
            </li>
            <li class="nav-item">
              <RouterLink to="/api-doc" class="nav-link active">API Doc</RouterLink>
            </li>
          </ul>
          <div class="d-grid gap-2 d-md-flex">          
            <RouterLink v-if="$route.path != '/login'" to="/login"><button id="login-btn" class="btn btn-outline-primary" type="submit">Login</button></RouterLink>
            <RouterLink v-if="$route.path != '/sign-up'" to="/sign-up"><button id="login-btn" class="btn btn-primary" type="submit">Sign Up</button></RouterLink>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>


<style scoped>
</style>