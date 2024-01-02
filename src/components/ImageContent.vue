<template>
    <div class="image-content-main-container">
    </div>
</template>
<style scoped>
.image-content-main-container{
    background: url("../assets/images/illustration-devices.svg") left center/auto no-repeat;
    width:50vw;
    height:100vh;
}

@media screen and (max-width:850px){
    .image-content-main-container{
        width:100vw;
        height:40vh;
        background: url("../assets/images/illustration-devices.svg") left top/auto 100vh  no-repeat;
        background-size: cover;
    }
}
</style>