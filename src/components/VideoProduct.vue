<template>
    <div class="video-wrapper">
      <div class="product-video-container">
        <video src="/assets/skincare.mp4" autoplay muted loop class="product-video"></video>
      </div>
    </div>
  </template>
  
  <script>
  import { RouterLink } from 'vue-router';
  
  export default {
    name: 'VideoProduct',
    components: {
      RouterLink
    }
  };
  </script>
  
  <style scoped>
  .video-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0;
    background-color: #f9f9f9;
    height: 100vh;
    box-sizing: border-box;
    margin-top: 55px;
    margin-bottom: 60px;
  }
  
  .product-video-container {
    width: 100%;
    height: auto;
    overflow: hidden;
  }
  
  .product-video {
    width: 100%;
    height: auto;
    border-radius: 0;
    object-fit: cover;
  }
  </style>
  