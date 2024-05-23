<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <div class="card-container">
      <Card
        v-for="album in albums"
        :key="album.id"
        :title="album.title"
        :description="album.description"
        :image="album.image"
      />
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Carousel from './components/Carousel.vue';
import Card from './components/Card.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    Card,
    Footer
  },
  data() {
    return {
      albums: [
        {
          id: 1,
          title: 'NEW JEANS Album GET UP Bunny Beach Bag Weverse - WEVERSE VER, SEALED',
          description: 'Rp 300.000',
          image: 'https://images.tokopedia.net/img/cache/900/VqbcmM/2023/8/14/daf5e64f-46ad-44e5-9807-dc8409eb658b.jpg'
        },
        {
          id: 2,
          title: 'DOYOUNG NCT The 1st Album YOUTH [FOAM ver / NEW SPRING ver]',
          description: 'Rp 350.000',
          image: 'https://images.tokopedia.net/img/cache/900/VqbcmM/2024/5/14/c32bfbec-5040-449d-87ce-50d766b52eeb.jpg'
        },
        {
          id: 3,
          title: '[Ready SEALED] RED VELVET WENDY 2nd Album WISH YOU HELL [QR Ver] ',
          description: 'Rp 270.000',
          image: 'https://images.tokopedia.net/img/cache/900/VqbcmM/2024/3/30/436a6fc7-6aad-43be-a142-7afa7089c646.jpg'
        }
      ]
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}

.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 20px;
}
</style>