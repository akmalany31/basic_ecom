<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary bg-light">
    <div class="container">
      <img src="../assets/logo-mau-2.png" alt="logo" />
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">Shop</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">About</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">Blog</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">Contact</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">Pages</router-link>
          </li>
        </ul>

        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <router-link class="nav-link" to="/"> <b-icon icon="person-fill"></b-icon>Login / Register </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/"> <b-icon-search class="mr-2"></b-icon-search></router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/"> <b-icon-cart class="mr-2"></b-icon-cart></router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/"> <b-icon-heart class="mr-"></b-icon-heart></router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "AppNavbar",
};
</script>

<style scoped>
img {
  width: auto;
}

.navbar-nav li.nav-item {
  margin-right: 10px;
}

.navbar-nav li.nav-item a.nav-link {
  color: #333;
  text-decoration: none;
}

.navbar-nav li.nav-item a.nav-link:hover {
  color: #a37460;
}
</style>
