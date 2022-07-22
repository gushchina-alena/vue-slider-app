<template>
  <Header></Header>
  <Carousel :slides="slides"></Carousel>
  <Cards></Cards>
  <Footer></Footer>
</template>

<script>
import Header from "./components/Header";
import Carousel from "./components/Carousel/Carousel.vue";
import Cards from "./components/Services/Cards.vue";
import Footer from "./components/Footer.vue";
import pic1 from "./assets/slider-pic1.jpg";
import pic2 from "./assets/slider-pic2.jpg";
import pic3 from "./assets/slider-pic3.jpg";
import pic4 from "./assets/slider-pic4.jpg";

export default {
  components: { Header, Carousel, Cards, Footer },
  data: () => ({
    slides: [pic1, pic2, pic3, pic4],
    visibleSlide: 0,
  })
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');

html, body, #app {
  box-sizing: border-box;
  height: 100%;
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Open Sans', sans-serif;
  color: #0E0E0F;
}
</style>
