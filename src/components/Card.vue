<template>
    <div class="card">
      <img :src="image" alt="album image" class="card-img">
      <div class="card-content">
        <h3>{{ title }}</h3>
        <p>{{ description }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Card',
    props: {
      title: String,
      description: String,
      image: String
    }
  };
  </script>
  
  <style>
  .card {
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    margin: 10px;
    width: 300px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  }
  
  .card-img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  
  .card-content {
    padding: 15px;
    text-align: left;
  }
  </style>