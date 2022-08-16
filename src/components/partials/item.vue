<template>
    <div class="item">
        <p>{{title}}</p>
        <div class="user_group">
            <img src="https://kuda.com/static/realsok-5d06d4522824d070231e462908be8654.jpg" alt="" srcset="">
            <h3>{{name}}</h3>
        </div>
    </div>
</template>

<script>
export default {
    props:[
        "title",
        "name",
    ]
}
</script>

<style scoped>
    /* .con{
        display: inline-block;
    } */
    .item{
        display:grid;
        width: 350px;
        height: auto;
        gap: 30px;
        box-shadow: 0 0 25px rgb(0 0 0 / 20%);
        border-radius: 10px;
        padding: 20px 20px;

    }
    .item p{
        text-align: left;
        font-size: 12px;
    }
    .user_group{
        display: flex;
        flex-direction: row;
        gap: 3px;
    }

    img{
        width:50px;
        height:50px;
        border-radius: 50%;
        align-self: center;
    }

    .user_group h3{
        font-size: 0.8rem;
        font-weight: bold;
        align-self: center;
    }
</style>