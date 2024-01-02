<script setup>
import Header from "../components/Header.vue";
import TextContent from "../components/TextContent.vue";
import ImageContent from "../components/ImageContent.vue";
</script>

<template>
    <div class="main-view-main-container">
        <Header></Header>
        <div class="main-view-content-container">
            <TextContent></TextContent>
            <ImageContent></ImageContent>
        </div>
    </div>
</template>

<style scoped>
.main-view-content-container{
    display:flex;
    position:absolute;
    z-index:-1;
    top:0;
}
@media screen and (max-width:850px){
    .main-view-content-container{
        flex-direction:column-reverse;
        width:100vw;
        height:100vh;
        margin:2vh 0 0;
    }
}
</style>