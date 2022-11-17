<template>
  <nav class="navbar navbar-expand-lg bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">The Yogasari Villa</a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link" :class="[activeNavbar == 'about' ? 'active' : '']" aria-current="page" to="/">About</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :class="[activeNavbar == 'facilities' ? 'active' : '']" aria-current="page" to="/facilities">Facilities</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :class="[activeNavbar == 'review' ? 'active': '']" to="/review">Review</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" :class="[activeNavbar == 'contact' ? 'active': '']" to="/contact">Contact Us</router-link>
          </li>
        </ul>
      </div>
      </div>
  </nav>
</template>

<script>
export default {
    props: ['activeNavbar']
}
</script>

