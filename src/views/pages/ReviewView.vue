<template>
    <MainNavbar activeNavbar="review"/>
    <div>
        Review
    </div>
</template>

<script>
import MainNavbar from '../partials/MainNavbar.vue'
export default {
    components: { MainNavbar },
    data(){
        return{
            activeNavbar : 'review'
        }
    }
}
</script>