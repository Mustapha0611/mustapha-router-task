<template>
 <nav class="navbar navbar-expand-lg bg-secondary">
  <div class="container-fluid">
    <a class="navbar-brand" style="color:whitesmoke;">Musteey</a>
    <!-- <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button> -->
    <div class="collapse navbar-collapse d-flex justify-content-end me-4" id="navbarNav">
      <div class="navbar-nav">
          <router-link class="nav-link" aria-current="page" to="/">Home</router-link>
          <router-link class="nav-link" to="/about">About</router-link>
          <router-link class="nav-link" to="/contact">Contact us</router-link>
          <!-- <router-view></router-view> -->
    </div>
  </div>
  </div>
</nav>
</template>

<script>
export default {
name:'navBar'
}
</script>

<style>
.nav-link{
  color:white;
}
</style>