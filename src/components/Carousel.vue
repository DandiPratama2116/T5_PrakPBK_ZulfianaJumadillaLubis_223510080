<template>
    <div class="carousel">
      <div
        class="carousel-item"
        v-for="(image, index) in images"
        :key="index"
        :style="{ backgroundImage: 'url(' + image + ')' }"
      ></div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Carousel',
    data() {
      return {
        images: [
          'https://images.tokopedia.net/img/cache/900/VqbcmM/2024/5/4/12a06625-4212-44c6-bd0a-9b9ddb4a227f.jpg',
          'https://images.tokopedia.net/img/cache/900/VqbcmM/2024/3/11/5fa8c19e-1712-4b2b-bccc-fef0d2fba91a.jpg',
          'https://images.tokopedia.net/img/cache/900/VqbcmM/2024/2/28/2c6d18d6-2bd5-41ca-9f01-135d8eb3cf6c.jpg',
          'https://images.tokopedia.net/img/cache/900/VqbcmM/2024/4/8/7ab2f1bf-9a6f-4bc2-a786-4c92ea9f4481.jpg'
        ]
      };
    }
  };
  </script>
  
  <style>
  .carousel {
    display: flex;
    overflow-x: scroll;
    scroll-snap-type: x mandatory;
    gap: 10px;
    padding: 20px;
  }
  
  .carousel-item {
    min-width: 300px;
    height: 200px;
    background-size: cover;
    background-position: center;
    scroll-snap-align: start;
  }
  </style>
  