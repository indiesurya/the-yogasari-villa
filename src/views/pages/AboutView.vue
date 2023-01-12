


<template>
  
  <div class="main-class">
    <!-- Jumbotron -->
    <section id="jumbotron" style="margin-top:-100px; position: relative;">
      <div class="welcome">
        Selamat Datang di Andong Village <br>
        <button class="btn btn-green p-3"><router-link class="nav-link" aria-current="page" to="/facilities">Mulai Virtual Tour</router-link></button>
      </div>
    
      <Slider/>
    </section>
    <!-- End Jumbotron -->

    <!-- Summary Content -->
    <div class="container my-5">
      <div class="description-content">
        <div class="row">
         
          <div class="col-12 col-md-4">
            <img
              src="../../assets/img/view/1.JPG"
              class="img-fluid"
              alt=""
              style="width: 100%; height:100%; object-fit:cover;"
            />
          </div>
           <div class="col-12 col-md-8">
            <h1 class="display-4">Andong Village</h1>
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
        </div>
      </div>
    </div>
    <!-- End Summary Content -->
  </div>
</template>

<script>
import MainNavbar from "../partials/MainNavbar.vue";
import Footer from "../partials/FooterView.vue";
import  Slider from "../components/Slider.vue";

export default {
  components: { MainNavbar, Footer, Slider },
  data() {
    return {
      activeNavbar: "about",
    };
  },
};
</script>

<style>
</style>