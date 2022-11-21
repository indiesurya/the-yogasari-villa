<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container">
      <a class="navbar-brand" href="#">The Yogasari Villa</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
      <span class="navbar-toggler-icon"></span>
        </button>
      <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
        <div class="offcanvas-header">
            <h5 class="offcanvas-title" id="offcanvasNavbarLabel">The Yogasari Villa</h5>
            <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
            <ul class="navbar-nav ml-auto mb-2 mb-lg-0">
            <li class="nav-item">
                <router-link class="nav-link" aria-current="page" to="/">About Us</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" aria-current="page" to="/facilities">Facilities</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" to="/review">Review</router-link>
            </li>
            <li class="nav-item">
                <router-link class="nav-link" to="/contact">Contact Us</router-link>
            </li>
            </ul>
        </div>
      </div>
      </div>
  </nav>
</template>

<script>
export default {
    props: ['activeNavbar']
}
</script>

