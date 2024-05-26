<template>
    <div class="hero-container">
      <div class="hero-content">
        <h1>TRY IT</h1>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HeroSection',
  };
  </script>
  
  <style scoped>
  .hero-container {
    position: relative;
    width: 100%;
    height: 600px;
    background-image: url('/assets/sponsor.jpg'); 
    background-size: cover;
    background-position: center;
  }
  
  .hero-content {
    position: absolute;
    bottom: 50px;
    left: 50px;
    color: white;
    font-size: 48px;
    font-weight: bold;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.6);
  }
  </style>
  