<template>
    <footer class="footer">
      <div class="container">
        <div class="footer-content">
          <p class="copyright">&copy; {{ currentYear }} Estate Angela. copyright. </p>
          <nav class="footer-nav">
            <ul>
              <li><NuxtLink to="/">home</NuxtLink></li>
              <li><NuxtLink to="/about">about</NuxtLink></li>
              <li><NuxtLink to="/services">services</NuxtLink></li>
              <li><NuxtLink to="/contact">contact</NuxtLink></li>
            </ul>
          </nav>
        </div>
      </div>
    </footer>
</template>
  
  <script setup>
  const currentYear = computed(() => new Date().getFullYear())
  </script>
  
  <style scoped>
  .footer {
    background-color: #f8f9fa;
    padding: 2rem 0;
    margin-top: 2rem;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
  }
  
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
  }
  
  .copyright {
    margin: 0;
  }
  
  .footer-nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    gap: 1rem;
  }
  
  .footer-nav a {
    color: #333;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  .footer-nav a:hover {
    color: #007bff;
  }
  
  @media (max-width: 768px) {
    .footer-content {
      flex-direction: column;
      text-align: center;
    }
  
    .footer-nav {
      margin-top: 1rem;
    }
  
    .footer-nav ul {
      justify-content: center;
    }
  }
  </style>