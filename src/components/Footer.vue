<template>
    <footer>
        <div class="first_cat">
            <logo setheight="22px" setwidth="100px" />
        </div>
        <div class="second_cat">
            <p class="footer-header">Features</p>
            <ul class="kuda-footer">
                <li>
                    <a href="https://kuda.com/cards">Kuda Card</a>
                </li>
                <li>
                    <a href="https://kuda.com/spend">Spend</a>
                </li>
                <li>
                    <a href="https://kuda.com/save">Save</a>
                </li>
                <li>
                    <a href="https://kuda.com/budget">Budget</a>
                </li>
                <li>
                    <a href="https://kuda.com/borrow">Borrow</a>
                </li>
            </ul>
        </div>
        <div class="third_cat">
            <p class="footer-header">Company</p>
            <ul class="kuda-footer">
                <li>
                    <a href="https://kuda.com/cards">Blog</a>
                </li>
                <li>
                    <a href="https://kuda.com/spend">Press</a>
                </li>
                <li>
                    <a href="https://kuda.com/save">Join Our Team</a>
                </li>
                <li>
                    <a href="https://kuda.com/budget">About Us</a>
                </li>
            </ul>
        </div>

        <div class="forth_cat">
            <p class="footer-header">Help</p>
            <ul class="kuda-footer">
                <li>
                    <a href="https://kuda.com/cards">Get Help</a>
                </li>
                <li>
                    <a href="https://kuda.com/spend">FAQS</a>
                </li>
                <li>
                    <a href="https://kuda.com/save">Security</a>
                </li>
                <li>
                    <a href="https://kuda.com/budget">Contact Us</a>
                </li>
            </ul>
        </div>

        <div class="fifth_cat">
            <p class="footer-header">Transparency</p>
            <ul class="kuda-footer">
                <li>
                    <a href="https://kuda.com/cards">Terms &amp; Condition</a>
                </li>
                <li>
                    <a href="https://kuda.com/spend">Privacy Policy</a>
                </li>
                <li>
                    <a href="https://kuda.com/save">Information Security Policy</a>
                </li>
                <li>
                    <a href="https://kuda.com/budget">Cookie Policy</a>
                </li>
            </ul>
        </div>
        <div class="download">
            <downloadApp class="download"/>
        </div>
        <p class="text">Products may vary by country or market</p>
        <contactsec class="con"/>
    </footer>
</template>

<script>
import LogoVue from './Logo.vue';
import Contactsec from './section/contactsec.vue';
import downloadApp from './section/downloadApp.vue';

export default {
    components:{
        "logo":LogoVue,
        "downloadApp":downloadApp,
        "contactsec":Contactsec,
    }
}
</script>

<style scoped>
    footer{
        border-top:1px solid rgba(223,227,255,.5);
        margin-top: 50px;
        display: grid;
        padding-left: 10px;
        padding-right: 10px;
        padding-top: 60px;
        grid-template-columns: repeat(2,1fr);
        grid-template-rows: 50px 1fr 1fr auto;
    }

    .first_cat{
        grid-column: 1/-1;
        grid-row:1/2;
    }

    .second_cat{
        grid-column: 1/2;
        grid-row: 2/3;

    }

    .third_cat{
        grid-column: 2/-1;
        grid-row: 2/3;
    }

    .forth_cat{
        grid-column: 1/2;
        grid-row: 3/4;
    }

    .fifth_cat{
        grid-column: 2/-1;
        grid-row: 3/4;
    }
    
    .footer-header{
        font-size: 1rem;
        line-height: 1.5;
        color:#40196D;
        font-weight: 700;
        margin-bottom: 20px;
        margin-top: 20px;
    }

    .kuda-footer{
        list-style-type: none;
        font-size: 0.8rem;
    }

    .kuda-footer li{
        margin-bottom: 20px;
    }

    .kuda-footer a{
        text-decoration: none;
        color: #000000;
    }

    .download{
        grid-column: 1/-1;
        grid-row:4/-1;
    }


    .text{
        text-align:center;
        grid-column: 1/-1;
        font-size: .9rem;
        color: #979797;
    }

    .con{
        grid-column: 1/-1;
    }
</style>