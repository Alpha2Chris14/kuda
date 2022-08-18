<template>
    <div class="top_banner">
        <div class="banner">
        <div class="item">
            <div class="caption">
            We’re the bank of the free
            </div>
            <div class="desc">
                <p>We’re here to help you get the best out of</p>
                <p> your money, no strings attached.</p>
                <p>Welcome to your freedom!</p>                
            </div>
            <div class="app_section">
                <applestore class="apple"/>
                <googleplay class="play"/>
            </div>
            <div class="license">
                <cbn class="cbn"/>
                <ndic class="ndic"/>
            </div>
            <mobile/>
            <cardinfo/>            
        </div>
    </div>
    <phonesection/>
    <FooterWidget/>
    </div>
    
</template>

<script>
import googleplay from '../icons/googleplay.vue';
import applestore from '../icons/applestore.vue';
import cbn from '../icons/cbn.vue';
import ndic from '../icons/ndic.vue';
import mobile from '../icons/mobileillus.vue';
import cardinfo from '../icons/cardinfo.vue';
import PhoneSection from '../section/PhoneSection.vue';
import FooterWidget from '../Footer.vue';
export default {
    components:{
        'applestore':applestore,
        'googleplay':googleplay,
        'cbn':cbn,
        'ndic':ndic,
        'mobile':mobile,
        'cardinfo':cardinfo,
        'phonesection':PhoneSection,
        'FooterWidget':FooterWidget,
    }
}
</script>

<style scoped>
@media only screen and (max-width:768px) {
    .banner{
        display: grid;
        text-align: center;
        margin-top: 70px;
        padding: 50px 20px 63px;
    }

    .item{
        width: 100%;
        display: grid;
        width: 100%;
    }
    .caption{
        font-size: 2rem;
        color: #40196D;
        line-height: 1.33;
        margin:0px 0px 20px;
        font-weight: 900;
    }

    .desc{
        color:#000000;
        font-size: 98%;
        margin:0px 0px 20px;
        line-height: 1.5;
        word-spacing: 1px;
        text-align: center;
        font-weight: 600;
        opacity: .7;
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


}
</style>