<template>
    <div class="app_box">
        <h1 class="head shrink">Get the app now, dump bank fees for good.</h1>
        <p>
It only takes a few minutes to start enjoying free benefits. Download Kuda on Google Play or the App Store</p>
        <div class="app_section">
                <applestore class="apple"/>
                <googleplay class="play"/>
            </div>
            <div class="license">
                <cbn class="cbn"/>
                <ndic class="ndic"/>
            </div>
    </div>
</template>

<script>
import applestoreVue from '../icons/applestore.vue'
import cbnVue from '../icons/cbn.vue'
import googleplayVue from '../icons/googleplay.vue'
import ndicVue from '../icons/ndic.vue'
export default {
    components:{
        "applestore":applestoreVue,
        "googleplay":googleplayVue,
        "cbn":cbnVue,
        "ndic":ndicVue,
    }
}
</script>

<style scoped>
    .app_box{
        background: #eff1ff;
        border: 1px solid rgba(219,220,224,.5);
        box-shadow: 15px 30px 40px rgb(64 25 109 / 7%);
        border-radius: 5px;
        position: relative;
        overflow: hidden;
        margin: 20px 5% 0px;
        display: flex;
        flex-direction: column;
        align-content: space-around;
        padding-top: 30px;
        padding-bottom: 30px;
    }

    .app_box p{
        font-size: 0.98rem;
        line-height: 1.5;
        word-wrap: break-word;
        padding-left: 10%;
        padding-right: 10%;
        margin-bottom: 20px;
    }

    .app_section{
        display: grid;
        grid-template-columns: repeat(4,1fr);
        gap: 10px;
        margin: 10px 0px 32px;
    }

    .apple{
        grid-column: 2/3;
    }

    .license{
        display: grid;
        gap:16px;
        grid-template-columns: repeat(2,1fr);
    }

    .cbn{
        justify-self: end;
    }
</style>