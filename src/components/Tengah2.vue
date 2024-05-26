<template>
    <div class="rich-text__wrapper rich-text__wrapper--center page-width">
      <div class="rich-text__blocks center">
        <h2 class="rich-text__heading rte h2">
          <span>RESULTS VISIBLE FROM THE FIRST APPLICATION</span>
        </h2>
        <div class="rich-text__text rte">
          <p>LA <strong>CONSTANCE</strong> IS THE KEY TO SKIN CARE, APPLY YOUR PRODUCTS EVEN DAY BY DAY AND YOU WILL HAVE IDEAL SKIN </p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { RouterLink } from 'vue-router';
  
  export default {
    name: 'Tengah2',
    components: {
      RouterLink
    }
  };
  </script>

<style scoped>
.rich-text__wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
  text-align: center;
  background-color: #356234;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px auto;
}

.rich-text__blocks {
  max-width: 600px;
}

.rich-text__heading {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 20px;
  color: #000000;
}

.rich-text__text p {
  font-size: 18px;
  line-height: 1.5;
  color: #000000;
  margin-bottom: 20px;
}

</style>
