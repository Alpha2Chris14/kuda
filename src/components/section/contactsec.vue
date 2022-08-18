<template>
    <div class="contact">
        <h2 class="contact_text">Contact</h2>
        <a  class="help_link" href="#">help@kuda.com</a>
        <div class="contact_media">
            <twitter/>
            <instagram/>
            <facebook/>
            <youtube/>
            <mail/>
            <linkin/>
        </div>
        <div>
            <div class="location_group">
                <div class="fir_venue">
                    <h3 class="contact_text">Lagos</h3>
                    <p>151 Herbert Macaulay Way, Yaba, <br> Lagos,
                        <br> Nigeria</p>
                </div>

                <div class="fir_venue">
                    <h3 class="contact_text">London</h3>
                    <p>5 New Street Square, London, <br> EC4A 3TW,
                       <br> UK</p>
                </div>
            </div>
        </div>
        <div class="det">
            <p>*Kuda Customers get 25 free transfer to other banks every month. Extra transfers to other banks cost ₦10 each.
**Kuda account holders can deposit money in over 10,000 branches across Nigeria for free.</p>
<p>
    © 2022 Kuda Microfinance Bank (RC796975). All rights reserved. All deposits are insured by the Nigerian Deposit Insurance Corporation (NDIC). Kuda Microfinance Bank is licensed by the Central Bank of Nigeria. “Kuda” and “Kudabank” are trademarks of Kuda Technologies Ltd Lagos: 151 Herbert Macaulay Way, Yaba, Lagos. London: 5 New Street Square, London, EC4A 3TW, UK
</p>

<p>
    Kuda Current Account is provided through Kuda Microfinance Bank. All text, graphics, audio files, code, downloadable material, and other works on this website are the copyrighted works of Kuda Microfinance Bank. All Rights Reserved. Any unauthorized redistribution or reproduction of any copyrighted materials on this website is strictly prohibited. Other product and company names are trademarks of their respective owners. This website contains simulated images; actual appearance may vary.
</p>
        </div>

        <div class="kuda_feet">
            <kudastar/>
            <a href="#" class="kuda_get_App">Get the app</a>
        </div>
    </div>
</template>

<script>
import facebookVue from '../icons/facebook.vue'
import instagramVue from '../icons/instagram.vue'
import kudastarVue from '../icons/kudastar.vue'
import linkinVue from '../icons/linkin.vue'
import mailVue from '../icons/mail.vue'
import twitterVue from '../icons/twitter.vue'
import youtubeVue from '../icons/youtube.vue'
export default {
    components:{
        "twitter":twitterVue,
        "instagram":instagramVue,
        "facebook":facebookVue,
        "youtube":youtubeVue,
        "mail":mailVue,
        "linkin":linkinVue,
        "kudastar":kudastarVue
    }
}
</script>

<style scoped>
.contact{
    margin-top:40px;
    margin-bottom: 15px;
}

.contact_text{
    font-size: 1rem;
    line-height: 1.5;
    color:#40196D;
    margin-bottom: 15px;
}

.contact_media{
    display: flex;
    gap:15px;
    margin-top: 15px;
}

.help_link{
    font-size:0.9rem;
    font-weight: 700;
    text-decoration: underline;
    color:#40196D
}

.location_group{
    display: flex;
    align-content: space-between;
    gap: 10%;
}

.location_group h3{
    margin-top: 40px;
    margin-bottom:10px;
}

.location_group p{
    font-size: 0.875rem;

    line-height: 1.5;
}

.det{
    margin-top:50px;
    margin-bottom: 100px;
}

.det p{
    color: #979797;
    margin-bottom: 21px;
    font-size: 0.82rem;
    line-height: 1.5;
}

.kuda_feet{
    background: #EFF1FF;
    display: flex;
    height: 80px;
    justify-content: space-between;
    position: fixed;
    bottom: 0;
    width: 100%;
    left:0;
    padding-left: 20px;
    padding-right: 20px;
}

.kuda_get_App{
    align-self: center;
    text-decoration: none;
    font-weight: 700;
    font-size: 0.9rem;
    line-height: 1;
    display: flex;
    align-items: center;
    padding: 15px;
    border-radius: 4px;
    justify-content: center;
    cursor: pointer;
    background: #40196D;
    border-radius: 10px;
    color: white;
    height: 40px;
    
}
</style>