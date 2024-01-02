<script setup>
import MainView from "./view/MainView.vue";
</script>

<template>
  <div class="app-container">
    <div class="main-coloured-bg">
      <div class="main-white-section">
      </div>
      <div class="coloured-bg">
        <div class="blue-section"></div>
        <div class="white-section"></div>
      </div>
    </div>
    <MainView></MainView>
  </div>
</template>

<style scoped>
.app-container {
  height: 100vh;
  width: 100vw;
}

.main-white-section {
  width: 50vw;
  height: 100vh;
}

.main-coloured-bg {
  display: flex;
  position: absolute;
  z-index: -1;
  height: 100vh;
}

.blue-section {
  width: 50vw;
  height: 50vh;
  background-color: hsl(207, 33%, 95%);
  border-radius: 0 0 0 100px;
}

.white-section {
  width: 50vw;
  height: 50vh;
}</style>