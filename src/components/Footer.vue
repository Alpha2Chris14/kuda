<template>
    <footer>
        <div class="first_cat">
            <logo setheight="22px" setwidth="100px" />
        </div>
    </footer>
</template>

<script>
import LogoVue from './Logo.vue'

export default {
    components:{
        "logo":LogoVue,
    }
}
</script>

<style scoped>
    footer{
        border-top:1px solid rgba(223,227,255,.5);
        margin-top: 50px;
        display: grid;
    }

    .first_cat{

    }
</style>