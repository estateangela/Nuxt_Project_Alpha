<template>
    <footer class="footer">
      <div class="container">
        <p>&copy; {{ currentYear }} ESTATE ANGEL. All rights reserved.</p>
        <nav>
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
            <li><a href="#">Privacy Policy</a></li>
          </ul>
        </nav>
      </div>
    </footer>
</template>
  
  <script setup>
  const currentYear = new Date().getFullYear()
  </script>
  
  <style scoped>
  .footer {
    background-color: #f8f9fa;
    padding: 20px 0;
    margin-top: 40px;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 15px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  ul {
    list-style: none;
    padding: 0;
    display: flex;
  }
  
  li {
    margin-left: 20px;
  }
  
  a {
    color: #333;
    text-decoration: none;
  }
  
  a:hover {
    text-decoration: underline;
  }
  </style>