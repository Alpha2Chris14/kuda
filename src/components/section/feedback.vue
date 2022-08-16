<template>
    <div class="phone_section less">
        <h1 class="head">{{title}}</h1>
        <div class="list_con">
            <div class="list">
            <item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="Onyeka Christian"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="Ifeayi Paul"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="James Isreal"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Doe"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="Peter Doe"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Paul"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Paul"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Paul"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Paul"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Paul"/>

<item title="Never thought an app would stylish become my everyday way to bank and have access to physical cash.
@kudabank is sleek" name="John Paul"/>

        </div>
        </div>
    </div>
</template>

<script>
import item from "../partials/item.vue"
export default {
    components:{
        "item":item,
    },
    data() {
        return {
            title:"Don’t just take our word for it"
        }
    },
}
</script>
<style scoped>
    .less{
        margin-top: 120px;
    }

    .list_con{
        overflow-x: hidden;
        padding-left: 1vh;
        padding-right: 1vh;
        padding-bottom: 20px;
        margin-bottom: 20px;
    }
    .list{
        display:flex;
        flex-direction: row;
        margin-top: 25px;
        width: 3650px;
        gap: 15px;
        animation: ints 55s  infinite linear;
        animation: name duration timing-function delay iteration-count direction fill-mode;
    }

    @keyframes ints {
        0%{
            /* transform: translateX("350px"); */
            transform: translateX(-350px);
        }

        25%{
            transform: translateX(-700px);
        }

        50%{
            transform: translateX(-1050px);
        }

        75%{
            transform: translateX(-1400px);
        }

        100%{
            transform: translateX(-350px);
        }

        
    }
    
</style>