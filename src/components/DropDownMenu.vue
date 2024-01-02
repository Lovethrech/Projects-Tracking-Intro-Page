<template>
    <div class="dropdown-main-container">
        <ul class="main-header-nav-list">
            <li class="main-header-nav">products</li>
            <li class="main-header-nav">features</li>
            <li class="main-header-nav">pricing</li>
            <li class="main-header-dot"><i class='bx bxs-circle'></i></li>
            <li class="main-header-login">login</li>
        </ul>
    </div>
</template>

<style scoped>
.main-header-nav-list{
    background-color: hsl(0, 100%, 100%);
    padding:6vh 0;
    margin: 0;
    list-style: none;
    color:hsl(212, 27%, 19%);
    display:flex;
    flex-direction:column;
    text-align:center;
    padding:30px 100px;
}
.main-header-nav{
    margin:0 auto;
    font-family: 'Barlow Condensed', sans-serif;
    text-transform: uppercase;
    margin:2vh 0;
}
.main-header-login{
    margin:0 auto;
    font-family: 'Barlow Condensed', sans-serif;
    text-transform: uppercase;
    margin:6vh 0 0;
}
.main-header-dot{
    display:none;
}
.main-header-nav:hover{
    cursor: pointer;
    text-decoration:underline;
    transform:scaleX(0.98);
    transition:all .5s;
}
.main-header-login:hover{
    cursor: pointer;
    text-decoration:underline;
    transform:scaleX(0.98);
    transition:all .5s;
}
@media screen and (max-width:350px) {
    .main-header-nav-list{
        padding:3vh 10vw;
        max-width:200px;
    }
}
</style>