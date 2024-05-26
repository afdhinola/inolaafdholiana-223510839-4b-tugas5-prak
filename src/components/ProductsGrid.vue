<template>
  <div class="Products">
    <ProductGrid />,
    <Sponsor />,
    <VideoProduct />,
    <Footer />,
    
  </div>
</template>

<script>
  import ProductGrid from '../components/ProductList.vue';
  import Sponsor from '../components/Sponsor.vue';
  import VideoProduct from '../components/VideoProduct.vue';
  import Footer from '../components/Footer.vue';
  
  export default {
        name : 'Products',
        components: {
          ProductGrid,
          Sponsor,
          VideoProduct,
          Footer,
           
        }
    }

</script>