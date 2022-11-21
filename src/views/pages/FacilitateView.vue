<template>
  <MainNavbar activeNavbar="facilities" />
  <div class="container">
    <div class="title text-center">
      <h2 class="display-3">Facilities</h2>
    </div>
    <div class="row justify-content-center">
      <div
        class="col-md-2 bg-grey mx-1 text-center align-items-center"
        style="height: 155px; weight: 175px"
      >
        <h1><i class="bi bi-wifi text-orange fw-bold" style="font-size:2em;"></i></h1>
        <h6 class="fw-bold">Wifi</h6>
      </div>
      <div
        class="col-md-2 bg-grey mx-1 text-center align-items-center"
        style="height: 155px; weight: 175px"
      >
        <h1><i class="bi bi-wifi text-orange fw-bold" style="font-size:2em;"></i></h1>
        <h6 class="fw-bold">Wifi</h6>
      </div>
     <div
        class="col-md-2 bg-grey mx-1 text-center align-items-center"
        style="height: 155px; weight: 175px"
      >
        <h1><i class="bi bi-wifi text-orange fw-bold" style="font-size:2em;"></i></h1>
        <h6 class="fw-bold">Wifi</h6>
      </div>
      <div
        class="col-md-2 bg-grey mx-1 text-center align-items-center"
        style="height: 155px; weight: 175px"
      >
        <h1><i class="bi bi-wifi text-orange fw-bold" style="font-size:2em;"></i></h1>
        <h6 class="fw-bold">Wifi</h6>
      </div>
    </div>

    <!-- Picture -->
    <div class="picture">
      <h2 class="display-4">Picture</h2>
      <div class="row pl-1">
        <div
          class="col-md-4 image p-0"
          v-for="(image, index) in images"
          v-bind:key="index"
        >
          <img
            src="https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80"
            class="img-fluid"
            alt=""
            style="width: 100%"
          />
        </div>
      </div>
    </div>

    <!-- Slide Picture -->
    <div class="slide-picture my-5">
      <swiper
        :loop="true"
        :loopFillGroupWithBlank="true"
        :pagination="{
          clickable: true,
        }"
        :navigation="true"
        :modules="modules"
        :breakpoints="swiperOptions.breakpoints"
        class="mySwiper"
      >
        <swiper-slide v-for="(image, index) in images" v-bind:key="index">
          <div class="card mx-auto" style="width: 18rem">
            <img :src="image.url" alt="" class="img-fluid" />
          </div>
        </swiper-slide>
      </swiper>
    </div>
    <div class="video my-5">
      <video-player :options="videoOptions" class="w-100" />
    </div>
  </div>

  <!-- Footer -->
  <Footer />
</template>

<script>
import MainNavbar from "../partials/MainNavbar.vue";
import Footer from "../partials/FooterView.vue";
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

// import required modules
import { Pagination, Navigation } from "swiper";
import VideoPlayer from "../components/VideoPlayer.vue";

export default {
  components: { MainNavbar, Footer, Swiper, SwiperSlide, VideoPlayer },
  data() {
    return {
      swiperOptions: {
        breakpoints: {
          // when window width is >= 320px
          320: {
            slidesPerView: 1,
            spaceBetween: 20,
          },
          // when window width is >= 480px
          480: {
            slidesPerView: 3,
            spaceBetween: 30,
          },
          // when window width is >= 640px
          640: {
            slidesPerView: 3,
            spaceBetween: 30,
            slidesPerGroup: 1,
          },
        },
      },
      images: [
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
        {
          url: "https://images.unsplash.com/photo-1596360576228-ee4970148b8a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1000&q=80",
        },
      ],
    };
  },
  setup() {
    return {
      modules: [Pagination, Navigation],
      videoOptions: {
        autoplay: false,
        controls: true,
        sources: [
          {
            src: "/src/assets/video/1.mp4",
            type: "video/mp4",
          },
        ],
      },
    };
  },
};
</script>