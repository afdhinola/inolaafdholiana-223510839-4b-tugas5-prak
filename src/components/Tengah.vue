<template>
    <div class="rich-text__wrapper rich-text__wrapper--center page-width">
      <div class="rich-text__blocks center">
        <div class="rich-text__text rte">
          <p>NATURAL<strong> COSMETIC</strong> , EFFECTIVE, CRUELTY FREE ,<strong> VEGAN</strong> , FOR PEOPLE WHO WORRY ABOUT THEIR SKIN AND THE <strong> PLANET</strong> . FROM MALAGA</p>
        </div>
        <div class="rich-text__buttons">
          <RouterLink to="/products" class="button button--primary">PURCHASE</RouterLink>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { RouterLink } from 'vue-router';
  
  export default {
    name: 'Tengah',
    components: {
      RouterLink
    }
  };
  </script>

<style scoped>
.rich-text__wrapper {
  text-align: center;
  margin: 20px 0;
}

.rich-text__blocks {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.rich-text__text p {
  font-size: 14px;
  line-height: 1.5;
}

.button {
  display: inline-block;
  padding: 10px 20px;
  margin-top: 10px;
  background-color: #6fdc1b;
  color: white;
  text-decoration: none;
  border-radius: 5px;
}

.button--primary {
  background-color: #07270b;
}
</style>
