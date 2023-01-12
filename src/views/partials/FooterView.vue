<template>
    <footer class="footer separate-dashed">
    <div class="container mt-5 pb-5">
        <div class="row">
            <div class="col-md-3 text-center mb-3">
                <img src="../../assets/img/logo.png" alt="" class="img-fluid float-center text-center" width="200">
            </div>
            <div class="col-md-6 footer-contact">
                <h3 class="text-orange text-uppercase mb-4">Contact</h3>
                <div class="whatsapp d-flex mb-2 align-items-center">
                    <div class="icon-whatsapp">
                        <h1><i class="bi bi-whatsapp text-orange align-middle" style="vertical-align: middle;"></i></h1>
                    </div>
                    <div class="detail-whatsapp mx-2">
                        <li class="list-group-item fw-500">+62 8133 9782 421</li>
                    </div>
                </div>
                <div class="email d-flex align-items-center">
                    <div class="icon-email">
                        <h1><i class="bi bi-envelope text-orange"></i></h1>
                    </div>
                    <div class="detail-email mx-2">
                        <li class="list-group-item fw-500">theyogasariseminyak01@gmail.com</li>
                    </div>
                </div>
            </div>
            <div class="col-md-3 footer-feature">
                <ul class="list-group list-group-flush">
                    <div class="" v-for="(feature, index) in features" v-bind:key="index">
                        <router-link :to="feature.link" class="decoration-none"><li class="list-group-item text-orange px-0">{{feature.name}}</li></router-link>
                    </div>
                </ul>
            </div>
        </div>
        <div class="row d-flex justify-content-end">
            <div class="col-md-3 social-media px-0">
                <span class="text-orange" style="font-size: 3em;"><i class="bi bi-facebook mx-3"></i></span>
                <span class="text-orange" style="font-size: 3em;"><i class="bi bi-instagram mx-3"></i></span>
                <span class="text-orange" style="font-size: 3em;"><i class="bi bi-youtube mx-3"></i></span>
            </div>
        </div>
        <div class="row d-flex justify-content-center text-orange text-center">
            <div class="col-md-6">
                &copy; Copyright {{getDate}} {{author}}
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {
    data(){
        return {
            author: "Chindy Ayu Silsa Wijayanti",
            features: [
                {
                    name: "About Us",
                    link: "/"
                },
                {
                    name: "Facilities",
                    link: "/facilities"
                },
                {
                    name: "Review",
                    link: "/review"
                },
                {
                    name: "Contact Us",
                    link: "/contact"
                }
            ]
        }
    },
    computed:{
        getDate(){
            const d = new Date();
            const day = d.getFullYear();

            return day;
        }
    }
}
</script>