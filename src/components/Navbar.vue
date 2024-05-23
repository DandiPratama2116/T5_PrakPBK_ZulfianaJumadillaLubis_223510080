<template>
    <nav class="navbar">
      <div class="navbar-brand">Woopy Store</div>
      <ul class="navbar-nav">
        <li class="nav-item">Home</li>
        <li class="nav-item">Albums</li>
        <li class="nav-item">Social Media</li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar'
  };
  </script>
  
  <style>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    background-color: #8f0000;
    color: white;
  }
  
  .navbar-brand {
    font-size: 24px;
  }
  
  .navbar-nav {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
  }
  
  .nav-item {
    margin-left: 20px;
  }
  </style>