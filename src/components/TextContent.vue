<script setup>
import ChallengeInfo from "./ChallengeInfo.vue";
</script>

<template>
    <div class="text-content-main-container">
        <div class="text-content-sub-main-container">
            <div class="new-and-mono">
                <p class="new">New</p>
                <p class="mono">Monograph Dashboard</p>
            </div>
            
            
            <h1 class="h1">  Powerful insights into your team</h1>
            <p style="margin:1vh 0 8vh;color:hsl(231, 7%, 65%);font-family: 'Barlow', sans-serif;">Project planning and time tracking<br> for agile teams</p>
            <div class="btn-container">
                <button class="schedule">Schedule a demo</button>
                <div class="btn-describe">to see a live preview</div>
            </div> 
            <ChallengeInfo></ChallengeInfo>
        </div>

    </div>
</template>
<style scoped>
.h1{
    font-size:3em;
    text-transform:uppercase;
    font-family: 'Barlow', sans-serif;
}
.btn-container{
    display:flex;
    gap:1vw;
    text-transform:uppercase;
}
.schedule{
    background-color:hsl(0, 100%, 68%);
    color:hsl(0, 100%,100%);
    padding:1vh 2vw;
    border:3px solid hsl(0, 100%, 68%);
    text-transform:uppercase;
    font-family: 'Barlow Condensed', sans-serif;
    font-size:900;
    letter-spacing: 2px;
}
.schedule:hover{
    cursor:pointer;
    background-color:hsl(0, 77%, 76%);
    transform: scaleX(0.98);
    transition:all .5s;
}
.btn-describe{
    margin:auto 0;
    color:hsl(231, 7%, 65%);
    font-family: 'Barlow Condensed', sans-serif;
    letter-spacing:3px;
}
.new-and-mono{
    display:flex;
    justify-content:start;
    gap:10px;
}
.mono{
    color:hsl(231, 7%, 65%);
    text-transform:uppercase;
    font-family: 'Barlow Condensed', sans-serif;
    letter-spacing: 3px;
}
.new{
    padding: 0 10px;
    background-color:hsl(0,0%,0%);
    color:hsl(0,100%,100%);
    text-align:center;
    text-transform:uppercase;
    font-weight:400;
    border-radius:50px;
    font-weight:400;
    font-family: 'Barlow Condensed', sans-serif;}
.text-content-main-container{
    display:flex;
    place-items:center;
    justify-content:center;
    width:50vw;
}
.text-content-sub-main-container{
    margin:0 6vw;
}

@media screen and (max-width:960px) and (min-width:851px){
    .btn-container{
        display:block;
    }
    .schedule{
        width:100%;
    }
    .btn-describe{
        width:100%;
        text-align:center;
    }
}
@media screen and (max-width:850px){
    .text-content-main-container{
        width:100vw;
        height:50vh;
    }
    .h1{
        font-size:2em;
    }
}
@media screen and (max-width:400px){
    .btn-container{
        display:block;
    }
    .schedule{
        width:100%;
    }
    .btn-describe{
        width:100%;
        text-align:center;
    }
}

</style>