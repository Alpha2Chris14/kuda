<template>
    <div class="free">
        <h1 class="head shrink">Choose the freedom you need.</h1>
        <div class="free_box">
            <div class="col">
                <h2 class="free_bank">Other Banks</h2>
                <logo setwidth="99px" setheight="22px"/>
            </div>
            <div class="col">
                <div class="trans_fee">
                    <p class="title">Transfer Fee</p>
                    <div class="arc">
                        <cir/>
                        <p>Up to ₦50 plus V.A.T</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>25 free transfers every month</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Debit Card</p>
                    <div class="arc">
                        <cir/>
                        <p>₦1,000 plus V.A.T</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>Free</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Card Delivery</p>
                    <div class="arc">
                        <cir class="bles"/>
                        <sad/>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>free</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Card Maintenance Fee</p>
                    <div class="arc">
                        <cir/>
                        <p>Up to ₦50 plus quarter</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>Never</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Alerts</p>
                    <div class="arc">
                        <cir/>
                        <p>Charge for SMS alerts</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>Free instant notifications</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Annual Interest</p>
                    <div class="arc">
                        <cir/>
                        <p>4%</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>Up to 15%</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Bill Payment Fee</p>
                    <div class="arc">
                        <cir/>
                        <p>Up to ₦100 per bill</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>No</p>
                    </div>
                </div>
            </div>

            <div class="col">
                <div class="trans_fee">
                    <p class="title">Instant Reversals</p>
                    <div class="arc">
                        <cir class="bles"/>
                        <p><frown/></p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>Yes</p>
                    </div>
                </div>
            </div>


            <div class="col">
                <div class="trans_fee">
                    <p class="title">Account Maintenance Fee</p>
                    <div class="arc">
                        <cir/>
                        <p>Yes</p>
                    </div>
                </div>
                <div class="trans_fee_kuda">
                    <div class="arc sand">
                        <add/>
                        <p>Never</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import logo from '../Logo.vue';
import circle from '../icons/circle.vue';
import add from '../icons/add.vue';
import sad from '../icons/sad.vue';
import frown from '../icons/frown.vue';
export default {
    components:{
        "logo":logo,
        "cir":circle,
        "add":add,
        "sad":sad,
        "frown":frown,
    }
}
</script>

<style>
    .free{
        display: grid;
        text-align: center;
        justify-content: space-around;
        margin: 20px 0px;
        padding: 50px 20px 63px;
    }

    .shrink{
        margin-left: 5%;
        margin-right: 5%;
    }

    .free_bank{
        font-size: 1rem;
        color: #40196D;
        font-weight: 900;
    }
    .free_box{
        background: #fff;
        justify-content: center;
        border: 1px solid rgba(219,220,224,.5);
        box-shadow: 15px 30px 40px rgb(64 25 109 / 7%);
        border-radius: 5px;
        text-align: left;
    }

    .col{
        display: grid;
        grid-template-columns: repeat(2,1fr);
        border-bottom: 1px solid rgba(219,220,224,.5);
        padding:16px 30px;
    }

    .title{
        font-size: 0.8rem;
        font-weight: 600;
        margin-top: 10px;
    }

    .arc{
        display: flex;
        gap: 7px;
        font-size: 0.8rem;
        margin-top: 13px;
    }

    .sand{
        margin-top:37px;
    }

    .bles{
        justify-self: center;
        align-self: center;
    }


</style>