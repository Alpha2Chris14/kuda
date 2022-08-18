<template>
    <div class="download_con">
        <img src="https://kuda.com/static/app-store-9df3d746121bcf93fcdce6bff77758b5.svg" alt="Kuda App Store" class="available">
        <img src="https://kuda.com//static/google-play-61cb4b62e2b04e3c1c5e6908b4cc7f6a.svg" alt="Kuda Google Play" class="available">
        <img src="https://kuda.com//static/kuda-web-77bc3dc525d8fc20bddde7f8195a4c17.svg" alt="Kuda Web Icon" class="available">
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.download_con{
    display: flex;
    flex-direction:row;
    justify-content: space-between;
    margin-bottom: 21px;
}

img{
    width: 33.33%;
}
</style>