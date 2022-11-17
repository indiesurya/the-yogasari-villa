<template>
    <MainNavbar activeNavbar="about"/>
    <div>
        About
        {{activeNavbar}}
    </div>
</template>

<script>
import MainNavbar from '../partials/MainNavbar.vue'
export default {
    components: { MainNavbar },
    data(){
        return{
            activeNavbar : 'about'
        }
    },
}
</script>