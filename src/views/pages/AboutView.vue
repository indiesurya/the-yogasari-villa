


<template>
  <div class="main-class">
    <!-- Jumbotron -->
    <section id="jumbotron">
      <div class="bg-light rounded-3 text-center jumbotron">
        <div
          class="container-fluid"
          style="
            position: absolute;
            top: 40%;
            left: 50%;
            transform: translate(-50%, -50%);
          "
        >
          <div class="row justify-content-center text-center mb-3">
            <div class="col-md-6">
              <h1 class="display-5">Selamat Datang di The Yogasari Seminyak</h1>
            </div>
          </div>
          <button class="btn btn-orange btn-lg text-center" type="button">
            Mulai Virtual Tour
          </button>
        </div>
      </div>
    </section>
    <!-- End Jumbotron -->

    <!-- Summary Content -->
    <div class="container my-5">
      <div class="description-content">
        <div class="row">
          <div class="col-12 col-md-8 order-2 order-md-1">
            <h1 class="display-4">The Yogasari Seminyak</h1>
            <p class="text-justify">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nulla
              laborum qui, dolorem ullam voluptatum delectus blanditiis ea illo
              accusantium. Repellendus consequatur fuga laudantium quaerat
              numquam excepturi! Totam eum blanditiis perspiciatis. Excepturi
              esse blanditiis, accusantium repudiandae, enim, ipsum ex cumque
              magni at quas possimus. Voluptate quidem rerum eveniet, tempore
              reprehenderit dignissimos maiores repudiandae fuga voluptatem eos
              at dolorem labore voluptatibus consectetur! Quisquam aut labore
              nihil, at nobis ea explicabo quaerat accusantium error, debitis
              iste tempore quos molestias? Quis modi hic vitae ea. Illo, dolore
              sunt reiciendis iste provident libero! Ipsa, incidunt? Iusto
              repudiandae fugiat minima in! Expedita dolor corrupti eaque?
              Fugiat corrupti alias error dolores quae deleniti nam eos
              voluptatem esse. Labore praesentium voluptatum illum tempore
              eveniet tenetur inventore accusantium qui?
            </p>
            <div class="more-info d-flex align-items-center mt-5">
              <span class="text-orange">More Info About The Yogasari</span>
              <router-link to="/facilities"
                ><i
                  class="
                    mx-4
                    py-3
                    px-3
                    rounded-green
                    p-auto
                    bi bi-arrow-right
                    text-orange
                  "
                ></i
              ></router-link>
            </div>
          </div>
          <div class="col-12 col-md-4 order-1 order-md-2">
            <img
              src="https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80"
              class="img-fluid"
              alt=""
              style="width: 100%"
            />
          </div>
        </div>
      </div>
    </div>
    <!-- End Summary Content -->
  </div>
</template>

<script>
import MainNavbar from "../partials/MainNavbar.vue";
import Footer from "../partials/FooterView.vue";

export default {
  components: { MainNavbar, Footer },
  data() {
    return {
      activeNavbar: "about",
    };
  },
};
</script>

<style>
</style>