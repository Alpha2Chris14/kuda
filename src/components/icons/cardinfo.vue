<template>
    <div class="card_container">
        <div class="item">
            <freecard/>
            <p>We’ll give you a free debit card. Order it right in the app.</p>
        </div>

        <div class="item">
            <budget/>
            <p>Create smart budgets to help you take control of your spending.</p>
        </div>

        <div class="item">
            <see/>
            <p>See where your money goes without solving equations.</p>
        </div>

        <div class="item">
            <pay/>
            <p>Pay absolutely nothing for sending money.</p>
        </div>

        <div class="item">
            <payabs/>
            <p>Save automatically and we’ll pay you up to 15% interest every year.</p>
        </div>
    </div>
</template>

<style scoped>
.card_container{
    margin-top: 20px;
}
.item{
    color: #40196D;
    display:grid;
    grid-template-columns: 1fr 10fr;
    gap:20px;
    background-color: white;
    height: 80px;
    width: 100%;
    align-content: center;
    text-align:left;
    padding-left:20px;
    padding-right:20px;
    box-shadow: 0 0 25px rgb(0 0 0 / 6%);
    font-size: 0.8rem;
    line-height: 1.5;
    font-weight:900;
    margin-bottom: 20px;
}
.item p{
    align-self: center;
}
</style>
<script>
import freecard from '../icons/freecard.vue';
import budget from '../icons/budgetii.vue';
import see from '../icons/see.vue';
import pay from '../icons/pay.vue';
import payabs from '../icons/payabs.vue';
export default {
    components:{
        'freecard':freecard,
        'budget':budget,
        'see':see,
        'pay':pay,
        'payabs':payabs,
    }
    
}
</script>