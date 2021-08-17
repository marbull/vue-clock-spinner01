<template>
  <div class="circle">
    <div class="spin"></div>
  </div>
</template>

<script setup></script>

<style scoped>
  .circle {
    width: 200px;
    height: 200px;
    border: 20px solid crimson;
    border-radius: 50%;
    position: relative;
    top: 200px;
    bottom: 0;
    right: 0;
    left: 0;
    margin: auto;
  }
  .spin {
    width: 20px;
    height: 90px;
    background: crimson;
    border-radius: 10px;
    position: absolute;
    top: 50%;
    bottom: 0;
    right: 0;
    left: 0;
    margin: auto;
    animation: clock 2s linear infinite;
    transform-origin: top;
  }
  @keyframes clock {
    from {
      transform: rotateZ(0deg);
    }
    to {
      transform: rotateZ(360deg);
    }
  }
</style>
