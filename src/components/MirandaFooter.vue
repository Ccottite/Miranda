<template>
    <footer class="footer">
      <div class="container">
        <p>&copy; 2024 Mi Sitio Web. Todos los derechos reservados.</p>
        <nav>
          <ul>
            <li><a href="/about">Sobre nosotros</a></li>
            <li><a href="/contact">Contacto</a></li>
            <li><a href="/privacy">Política de privacidad</a></li>
          </ul>
        </nav>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'MirandaFooter'
  }
  </script>
  
  <style scoped>
  .footer {
    background-color: #333;
    color: #fff;
    padding: 20px 0;
    text-align: center;
  }
  
  .footer .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }
  
  .footer p {
    margin: 0;
  }
  
  .footer nav ul {
    list-style: none;
    padding: 0;
  }
  
  .footer nav ul li {
    display: inline;
    margin: 0 10px;
  }
  
  .footer nav ul li a {
    color: #fff;
    text-decoration: none;
  }
  
  .footer nav ul li a:hover {
    text-decoration: underline;
  }
  </style>
  
