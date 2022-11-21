<template>
  <MainNavbar activeNavbar="contact" />
  <div class="container">
    <div class="title text-center">
      <h2 class="display-3">Contact Us</h2>
    </div>
    <div class="row">
      <div class="col-md-4">
        <div class="location d-flex">
          <h1><i class="bi bi-geo-alt text-orange"></i></h1>
          <div class="detail-location mx-2">
            <li class="list-group-item fw-500">Jl. Dewi Saraswati III Blk. II No.9, Seminyak, Kec.Kuta, Kabupaten Badung, Bali 80361</li>
          </div>
        </div>
        <div class="email d-flex">
          <h1><i class="bi bi-envelope text-orange"></i></h1>
          <div class="detail-location mx-2 position-relative">
            <li class="list-group-item fw-500" style="top:35%;  transform: translateY(-50%); position:absolute;">theyogasariseminyak01@gmail.com</li>
          </div>
        </div>
        <div class="phone d-flex">
          <h1><i class="bi bi-telephone text-orange"></i></h1>
          <div class="detail-location mx-2 position-relative">
            <li class="list-group-item fw-500" style="top:35%;  transform: translateY(-50%); position:absolute;">081339782421</li>
          </div>
        </div>
      </div>
      <div class="col-md-8">
        <div class="row">
          <div class="col-md-6 mb-3">
            <input
              type="text"
              class="form-control"
              id="exampleFormControlInput1"
              placeholder="Your Name"
            />
          </div>
          <div class="col-md-6 mb-3">
            <input
              type="email"
              class="form-control"
              id="exampleFormControlInput1"
              placeholder="Your Email"
            />
          </div>
        </div>
        <div class="mb-3">
          <textarea
            class="form-control"
            id="exampleFormControlTextarea1"
            rows="3"
            placeholder="Your Message"
          ></textarea>
        </div>
        <input type="submit" value="Send" class="btn btn-contact float-end" />
      </div>
    </div>
    <div class="row mb-5">
      <h2 class="display-4">Picture</h2>
      <iframe
        width="600"
        height="500"
        id="gmap_canvas"
        src="https://maps.google.com/maps?q=the%20yogasari%20seminya&t=&z=13&ie=UTF8&iwloc=&output=embed"
        frameborder="0"
        scrolling="no"
        marginheight="0"
        marginwidth="0"
      ></iframe>
    </div>
  </div>
  <Footer />
</template>

<script>
import MainNavbar from "../partials/MainNavbar.vue";
import Footer from "../partials/FooterView.vue";
export default {
  components: { MainNavbar, Footer },
  data() {
    return {
      activeNavbar: "contact",
    };
  },
};
</script>