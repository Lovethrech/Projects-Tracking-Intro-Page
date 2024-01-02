<script setup>
import { ref } from "vue";
import DropDownMenu from "./DropDownMenu.vue";

const showMenuBar = ref(false);
const showMenu = ref(false);
const showDropDown = () => {
    if (showMenuBar.value == false) {
        showMenu.value = true;
        showMenuBar.value = true;
    }
    else {
        showMenu.value = false;
        showMenuBar.value = false;
    }
}
</script>
<template>
    <div class="main-header-container">
        <div class="main-header-logo-container">
            <img src="../assets/images/logo.svg" alt="page logo" class="main-header-logo">
        </div>
        <div class="main-header-nav-container">
            <ul class="main-header-nav-list">
                <li class="main-header-nav">products</li>
                <li class="main-header-nav">features</li>
                <li class="main-header-nav">pricing</li>
                <li class="main-header-nav" style="color:hsl(231, 7%, 65%);font-size:10px;margin:auto 0;"><i class='bx bxs-circle'></i></li>
                <li class="main-header-nav">login</li>
            </ul>
        </div>
        <div @click="showDropDown()"  class="menu-bar">
            <i v-if="!showMenuBar" class='bx bx-menu'></i>
            <i v-else  class='bx bx-x'></i>
        </div>
        <div class="dropdown">
            <DropDownMenu v-if="showMenu"></DropDownMenu>
        </div>
    </div>
</template>
<style scoped>
.main-header-container{
    padding:6vh 6vw;
    display:flex;
    justify-content: space-between;
}
.main-header-logo-container{
    margin:auto 0;
}
.main-header-nav-list{
    list-style:none;
    display:flex;
    gap:2vw;
    text-transform: uppercase;
    font-family: 'Barlow Condensed', sans-serif;
}
.main-header-nav:hover{
    cursor: pointer;
    text-decoration:underline;
    transform:scaleX(0.98);
    transition:all .5s;
}
.menu-bar {
    font-size:30px;
    display: none;
    color:hsl(0, 0%, 0%);
    
}
.menu-bar:hover{
    transform:scale(0.9);
    transition: all .5s;
}
.dropdown{
    position: absolute;
    top:12vh;
    right:0;
    margin:0 8vw 0 0;
}
.dropdown{
    display:none;
}

@media screen and (max-width:850px){
    .main-header-nav-container{
        display:none;
    }
    .menu-bar{
        display:block;
    }
    .dropdown{
        display: block;
    }
}
</style>