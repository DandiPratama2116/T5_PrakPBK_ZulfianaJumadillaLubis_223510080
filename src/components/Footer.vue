<template>
    <footer class="footer">
      <div class="footer-content">
        <div class="footer-section about">
          <h2 class="logo-text">K-Pop Album Store</h2>
          <p>
            Toko online terbaik untuk penggemar K-pop. Temukan berbagai album K-pop terbaru dan terpopuler di sini.
          </p>
        </div>
  
        <div class="footer-section links">
          <h3>Quick Links</h3>
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Albums</a></li>
            <li><a href="#">Contact</a></li>
            <li><a href="#">About Us</a></li>
          </ul>
        </div>
  
        <div class="footer-section social">
          <h3>Follow Us</h3>
          <div class="social-links">
            <a href="#"><i class="fab fa-facebook"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
          </div>
        </div>
      </div>
      <div class="footer-bottom">
        <p>&copy; 2024 K-Pop Album Store. All rights reserved.</p>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  };
  </script>
  
  <style>
  .footer {
    background-color: #333;
    color: white;
    padding: 40px 0;
    position: relative;
    bottom: 0;
    width: 100%;
    text-align: center;
  }
  
  .footer-content {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    padding: 20px;
  }
  
  .footer-section {
    flex: 1;
    margin: 10px;
  }
  
  .logo-text {
    font-size: 24px;
    font-weight: bold;
  }
  
  .footer-section h3 {
    margin-bottom: 10px;
  }
  
  .footer-section p, .footer-section a {
    color: white;
    text-decoration: none;
  }
  
  .footer-section a:hover {
    text-decoration: underline;
  }
  
  .footer-section ul {
    list-style: none;
    padding: 0;
  }
  
  .footer-section ul li {
    margin-bottom: 10px;
  }
  
  .social-links a {
    font-size: 24px;
    margin: 0 10px;
    color: white;
    text-decoration: none;
  }
  
  .social-links a:hover {
    color: #1da1f2;
  }
  
  .footer-bottom {
    margin-top: 20px;
    border-top: 1px solid #444;
    padding-top: 10px;
  }
  </style>
  
  <!-- Add Font Awesome for social media icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">