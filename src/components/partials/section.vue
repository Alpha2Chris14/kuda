<template>
    <div class="phone_section">
        <h1 class="head">{{title}}</h1>
        
        <p class="desc">
            {{desc}}
        </p>

        <tran v-if="val == 1"/>

        <div class="link" v-if="val == 2 || val==3 || val == 4 || val == 5">
            <a href="">{{link}} </a>
            <span>></span>
        </div>

        <tranii v-if="val == 2"/>
        <traniii v-if="val == 3"/>
        <traniv v-if="val == 4"/>
        <tranv v-if="val == 5"/>

    </div>
</template>

<script>
import tran from '../icons/tran.vue';
import tranii from '../icons/tranii.vue';
import traniii from '../icons/traniii.vue';
import traniv from '../icons/traniv.vue';
import tranv from '../icons/tranv.vue';
export default {
    props:[
        "title",
        "desc",
        "val",
        "link",
    ],
    components:{
        "tran":tran,
        "tranii":tranii,
        "traniii":traniii,
        "traniv":traniv,
        "tranv":tranv,
    }
}
</script>
<style scoped>
    .phone_section{
        margin-top: 150px;
    }
    .head{
        /* margin-left: 9%;
        margin-right: 9%; */
    }

    .desc{
        margin-left: 2%;
        margin-right: 2%;
    }


</style>
