<template>
    <div class="container">
        <h1>Our History</h1>
      <p>
        We are a family business, mother and son from the <strong>aesthetics sector</strong> committed to skin care, and with a wonderful team behind us. After years of experience with our clients, we have seen the need to create this project to care for the skin naturally while respecting its balance.
      </p>
      <p>
        Misolo emerged at the beginning of 2020, with the intention of creating a real and effective project, using <strong>exotic active ingredients</strong> that provide great and unknown properties to the skin, such as Baobab oil, Kigelia Africana, bitter orange extract...
      </p>
      <p>
        We also have a <strong>firm commitment to the planet</strong>, having glass containers and bamboo lids, with totally <strong>sustainable and handmade packaging</strong>, and having a connection with humanitarian aid , through our Misolo Project.
      </p>
      <img src="../assets/about.jpg" alt="Productos de Misolo" class="image">
    </div>
  </template>
  
<script>
  import { RouterLink } from 'vue-router';

  export default {
    name: 'History',
    components: {
      RouterLink
    }
  };
</script>
  
  <style scoped>
  .container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    font-family: Arial, sans-serif;
    color: #333;
    line-height: 1.6;
    margin-top: 200px;
  }
  
  h1 {
    font-size: 36px;
    color: #333;
    margin-bottom: 20px;
  }
  
  p {
    font-size: 18px;
    margin-bottom: 20px;
  }
  
  strong {
    font-weight: bold;
  }
  
  .image {
    width: 100%;
    height: 470px;
    border-radius: 8px;
    margin-top: 20px;
  }
  </style>
  