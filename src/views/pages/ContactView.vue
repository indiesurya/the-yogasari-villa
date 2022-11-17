<template>
    <MainNavbar activeNavbar="contact"/>
    <div>
        Contact
    </div>
</template>

<script>
import MainNavbar from '../partials/MainNavbar.vue'
export default {
    components: { MainNavbar },
    data(){
        return{
            activeNavbar : 'contact'
        }
    }
}
</script>