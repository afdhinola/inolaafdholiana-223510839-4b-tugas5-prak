<template>
    <footer class="footer">
      <div class="footer-content">
        <div class="footer-section">
          <h3>We solve all your doubts</h3>
          <ul>
            <li>Shipping and delivery policy</li>
          </ul>
        </div>
        <div class="footer-section">
          <h3>Quick links</h3>
          <ul>
            <li>Privacy Policy</li>
            <li>Terms and Conditions</li>
            <li>Safe Purchase</li>
          </ul>
        </div>
        <div class="footer-logo">
          <img src="../assets/logo2.png" alt="Misolo Cosmetics" />
        </div>
        <div class="footer-section">
            <h3>Work with us</h3>
          <ul>
            <li>ambassador plan</li>
            <li>Misolo Professional</li>
          </ul>
        </div>
      </div>
      <div class="footer-bottom">
        <div class="footer-locale">
          <div class="locale-item">
            <label for="country-select">País/región</label>
            <select id="country-select">
              <option>Indonesia (EUR €)</option>
            </select>
          </div>
          <div class="locale-item">
            <label for="language-select">Idioma</label>
            <select id="language-select">
              <option>Español</option>
            </select>
          </div>
        </div>
        <p>© 2024, MISOLO COSMETICS - Inola Afdholiana</p>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer',
  };
  </script>
  
  <style scoped>
  .footer {
    background-color: #d18b79;
    color: white;
    padding: 40px 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .footer-content {
    display: flex;
    justify-content: space-between;
    width: 100%;
    max-width: 1200px;
    margin-bottom: 40px;
    align-items: flex-start;
  }
  
  .footer-section {
    flex: 1;
    margin-left: 10px;
  }
  
  .footer-section h3 {
    font-size: 18px;
    margin-bottom: 10px;
    font-weight: bold;
  }
  
  .footer-section ul {
    list-style: none;
    padding: 0;
  }
  
  .footer-section ul li {
    margin-bottom: 5px;
    font-size: 16px;
  }
  
  .footer-logo {
    margin-bottom: 40px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    padding: 20px;
    border-radius: 8px;
    background-color: transparent;
    margin-left: 10px; 
  }
  
  .footer-logo img {
    max-width: 150px;
  }
  
  .footer-bottom {
    width: 100%;
    max-width: 1200px;
    text-align: center;
    border-top: 1px solid rgba(255, 255, 255, 0.3);
    padding-top: 20px;
  }
  
  .footer-locale {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
  }
  
  .locale-item {
    margin-right: 20px;
  }
  
  .locale-item:last-child {
    margin-right: 0;
  }
  
  .locale-item label {
    display: block;
    margin-bottom: 5px;
  }
  
  .locale-item select {
    padding: 5px;
    border: none;
    border-radius: 5px;
  }
  </style>
  