<template>
    <header ref="header" id="menu_header">
        <Logo class="logo" setwidth="72" setheight="15"/>
        <nav class="web-view">
            <ul class="nav-left">
                <li>Features</li>
                <li>Business</li>
                <li>Company</li>
                <li>Help</li>
            </ul>
            <ul class="nav-right">
                <li>Sign In</li>
                <li><button>Get Kuda</button></li>
                <li><img src="../assets/icon.svg" alt="" srcset=""></li>
            </ul>
        </nav>
        <div class="last">
            <img src="../assets/icon.svg" class="img" alt="" srcset="">
            <div class="menu-mobile" v-on:click="toggle">
                <div class="bar"></div>
                <div class="bar"></div>
            </div>
        </div>

        <nav class="mobile_view"  id="mob_view" v-if="visible">
                <button class="sign_in">Sign In</button>
                <button class="business">Business</button>
            
                <ul>
                    Features
                    <li class="icon-item"><card style="height:25px; width:25px;"/>Kuda Card</li>
                    <li class="icon-item"><spend style="height:25px; width:25px;"/>Spend</li>
                    <li class="icon-item"><save style="height:25px; width:25px;"/>Save</li>
                    <li class="icon-item"><budget style="height:25px; width:25px;"/>Budget</li>
                    <li class="icon-item"><borrow style="height:25px; width:25px;"/>Borrow</li>
                </ul>
            
                <ul class="right-list">
                    Company
                    <li>Blog</li>
                    <li>Press</li>
                    <li>Join Our Team</li>
                    <li>About Us</li>
                </ul>

                <ul class="left-list">
                    Help
                    <li>Get Help</li>
                    <li>FAQs</li>
                    <li>Security</li>
                    <li>Contact Us</li>
                </ul>
        </nav>
    </header>
</template>

<script>
import Logo from './Logo.vue'
import card from './icons/card.vue';
import spend from './icons/card.vue';
import save from './icons/card.vue';
import budget from './icons/card.vue';
import borrow from './icons/card.vue';
export default {
    components:{
        Logo,
        card,
        spend,
        save,
        budget,
        borrow,
    },
    data() {
        return {
            visible:false,
        }
    },
    methods: {
        toggle: function(){
            var head = this.$refs.header.id;
            var headerMenu = document.getElementById(head);
            // var log = this.$refs.logo.$el;
            if(this.visible){
                headerMenu.style.paddingLeft="30px";
                headerMenu.style.paddingRight="30px";
                headerMenu.style.boxShadow= "0 4px 13px rgb(0 0 0 / 5%)";
                // console.log(log)
            }else{
                headerMenu.style.paddingLeft="15px";
                headerMenu.style.paddingRight="15px";
                headerMenu.style.boxShadow= "none";
            }
            return this.visible =! this.visible;
        }
    },
}
</script>

<style scoped>
    header{
        width: 100vw;
        background:white;
        height: 70px;
        box-shadow: 0 4px 13px rgb(0 0 0 / 5%);
        padding-left: 60px;
        padding-right: 60px;
        display: grid;
        grid-template-columns: repeat(12,1fr);
        align-items: center;
    }

    .menu-mobile,.mobile_view{
        display: none;
    }

    .img{
        display: none;
    }

    .logo{
        grid-column: 1/3;
    }
    .web-view{
        grid-column: 3/-1;
        display: grid;
        grid-template-columns:repeat(12,1fr) ;
    }
    .nav-left,.nav-right{
        list-style-type: none;
        font-weight: 700;
        align-items: center;
        font-size: 14px;
        color: #40196D;
    }

    .nav-left{
        grid-column: 1/6;
        display: flex;
        justify-content: space-between;
    }

    .nav-right{
        grid-column: 9/-1;
        display: flex;
        justify-content: space-between;
        justify-items: center;
    }

    .nav-right>li:nth-child(2){
       flex-grow: 2;
       display: flex;
       justify-content: center;
    }

    .nav-right button{
        background-color: #40196D;
        color: white;
        outline: none;
        border: none;
        border-radius: 10px;
        padding: 15px;
        font-size: 16px;
        font-weight: 700;
        width: 50%;
    }
    
    @media only screen and (max-width:768px) {
        header{
            top:0;
            position:fixed;
            height:64px;
            padding-left: 15px;
            padding-right: 15px;
            background: white;
            z-index: 1;
        }
        .logo{
            height:18px;
        }

        .web-view{
            display: none;
        }

        .last{
            grid-column: 12/-1;
            display:grid;
            grid-template-columns: repeat(2,1fr);
            justify-content: center;
            align-content: center;
            gap:5px;
        }
        
        .menu-mobile{
             width:20px;
             height: 20px;
             display: grid;
             grid-template-rows: repeat(2,1fr);
             align-items: center;
             justify-self: right;
             align-self:center;
        }

        .bar{
            display:block;
            background-color:#40196D;
            width: 100%;
            height:2px;        
        }

        .img{
            display: block;
        }

        .mobile_view{
            background: white;
            z-index: 10;
            position: absolute;
            height: 100vh;
            top:64px;
            display: grid;
            grid-template-columns: 1fr 4fr;
            grid-template-rows: 40px 300px auto;
            grid-auto-rows: 100px;
            gap:10px;
            margin-left: 100px;
            animation: appear .3s;
            padding-top: 20px;
        }

        .mobile_view button{
            border-radius: 10px;
            outline: none;
            border:none;
            font-weight: 500;
        }

        @keyframes appear {
            0%{
                opacity: 0;
            }
            25%{
                opacity: 0.25;
            }
            50%{
                opacity: 0.5;
            }
            75%{
                opacity: 0.75;
            }
            100%{
                opacity: 1;
            }
            
        }

        .sign_in{
            background: #40196D;
            color: white;
            grid-column: 1/2;
            width: 135px;
        }
        .business{
            grid-column: 2/-1;
            width: 135px;
            color:#40196D;
            background: #DFE3FF;
        }

        .left-list{
            grid-row: 3/-1;
        }

        .right-list{
            margin-left: 120px;
        }
        .mobile_view ul{
            color: #40196D;
            font-size: 16px;
            font-weight: 600;
            margin-top: 40px;
        }
        .mobile_view li:nth-child(1){
            margin-top: 20px;
        }
        .mobile_view li{
            color: #000000;
            font-size: 14px;
            margin-bottom: 26px;
            font-weight: 100;
            list-style-type: none;
        }

        .icon-item{
            display:grid;
            grid-template-columns: 1fr 3fr;
            align-items: center;
            justify-items: left;
        }

    }

</style>