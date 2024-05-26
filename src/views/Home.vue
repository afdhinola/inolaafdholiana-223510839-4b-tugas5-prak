<template>
  <div class="home">
    <Hero />
    <Tengah />
    <Carousel />
    <Tengah2 />
    <VideoProduct />
    <Kategori />
    <Footer />

    
  </div>
</template>

<script>
import Hero from '../components/Hero.vue';
import Tengah from '../components/Tengah.vue';
import Carousel from '../components/Carousel.vue';
import Tengah2 from '../components/Tengah2.vue';
import VideoProduct from '../components/VideoProduct.vue';
import Kategori from '../components/Kategori.vue';
import Footer from '../components/Footer.vue';



export default {
  name: 'Home',
  components : {
    Hero,
    Tengah,
    Carousel,
    Tengah2,
    VideoProduct,
    Kategori,
    Footer,
  }
}
</script>

