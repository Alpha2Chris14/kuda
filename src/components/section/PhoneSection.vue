<template>
   <div class="phone_section">
        <div class="head">
            <p>Your phone +</p>
            <p>our app +</p>
            <p>a debit card =</p>
            <p>a simpler life</p>
        </div>
        <p class="desc">
            We designed a banking app for your busy lifestyle, and we’ll give you a free debit card to go with it. That’s all you need to make the right moves with your money, no sweat.
        </p>
        <div class="link">
            <a href="">Open An Account in  Minute </a>
            <span>></span>
        </div>
        <ill/>
        <sec title="It's your money, we just help you manage it." desc="Save it, spend it, send it. It’s up to you. Whatever you choose to do with your money, we’ll make sure it’s done better and free of charge. We take responsibility for that." val="1"/>
        <sec title="Save money as you spend it, seriously." desc="You can’t avoid spending. That’s how you pay for your needs. But we can help you put money away every time you pay for something. Just set a percentage to save and watch your money grow." val="2" link="See all our Savings"/>
        <sec title="Turn off access, turn on safety." desc="Life happens. Milk spills. Debit cards go missing. If that ever happens, you can block your missing card on the app so no one can use it. We’d like to see them try." val="3" link="Learn more about Cards "/>
        <sec title="We’re always happy to help you." desc="You can chat with us on the app, slide into our DMs, tweet, leave an Instagram comment, send an email or call. However you choose to reach out, there’ll always be a friendly person there to make your life easy." val="4" link="Get Help "/>
        <sec title="Fees as clear as glass." desc="We’re serious about free banking, and we will never, ever charge you for anything without your consent." val="5" link="See all our fees "/>
        
        <feedback/>
        <sponsor/>
        <partners/>
        <freedom />
        <getapp/>



   </div>
   
</template>

<script>
import ill from '../icons/ill.vue';
import section from '../partials/section.vue';
import feedback from './feedback.vue';
import sponsor from './sponsor.vue';
import partners from './partners.vue';
import freedom from './freedom.vue';
import getapp from './getapp.vue';
export default {
    components:{
        "ill":ill,
        "sec":section,
        "feedback":feedback,
        "sponsor":sponsor, 
        "partners":partners,       
        "freedom":freedom,
        "getapp":getapp,
    }
}
</script>
<style>
.phone_section{
        display:grid;
        text-align:center;
        margin-top:70px;
}
.phone_section .head{
    color:#40196D;
    font-size:1.68rem;
    font-weight: 900;
    margin-bottom: 20px;
}

.desc{
    font-size: 0.97rem;
    line-height: 1.5;
    font-weight: 400;
    margin-left: 15%;
    margin-right: 15%;
    color: #6c6c6c;
}

.link{
    margin-top: 26px;
    font-weight: bold;
    color: #40196D;
    font-size: 14px;
}
.link span{
    font-weight: bolder;
}

</style>