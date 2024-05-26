<template>
    <div class="collapsible-content__wrapper section-template--15978159669408__1c9f02e4-ca88-4566-8fd6-b4f27106aac8-padding">
      <div class="collapsible-content-wrapper-narrow">
        <div class="collapsible-content__header" style="text-align: center;">
          <p class="caption-with-letter-spacing">REASONS WHY TO BUY MISOLO</p>
          <h2 class="collapsible-content__heading h2">THE KEYS OF MISOLO</h2>
        </div>
        <div class="collapsible-content__grid">
          <div class="accordion">
            <details>
              <summary>
                <div class="summary-content">
                  <img src="../assets/kategori/leaf.png" class="icon-leaf" alt="leaf icon" />
                  <span>VEGAN</span>
                </div>
                <svg class="icon-chevron" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M5 8l5 5 5-5H5z"></path>
                </svg>
              </summary>
              <div class="accordion__content rte">
                <p>Our products are respectful of animals and nature. An ethical alternative to the consumption of products from animal exploitation, this philosophy is applied to all areas of daily life: food, clothing, personal care, etc.</p>
              </div>
            </details>
          </div>
          <div class="accordion">
            <details>
              <summary>
                <div class="summary-content">
                  <img src="../assets/kategori/recycle.png" class="icon-recycle" alt="recycle icon" />
                  <span>SUSTAINABLE</span>
                </div>
                <svg class="icon-chevron" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M5 8l5 5 5-5H5z"></path>
                </svg>
              </summary>
              <div class="accordion__content rte">
                <p>Our products are <em>made in Spain</em> to reduce our carbon footprint. In addition, all our packaging is sustainable and recyclable with materials such as glass, cardboard or sugar cane.</p>
              </div>
            </details>
          </div>
          <div class="accordion">
            <details>
              <summary>
                <div class="summary-content">
                  <img src="../assets/kategori/star.png" class="icon-star" alt="star icon" />
                  <span>PROFESIONALS</span>
                </div>
                <svg class="icon-chevron" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M5 8l5 5 5-5H5z"></path>
                </svg>
              </summary>
              <div class="accordion__content rte">
                <p>Our cosmetics are effective not just because we say so. But because the more than 10,000 clients in our network of centers assure it. Beauty centers, hairdressers and spas throughout Spain already work with misolo products. A guarantee of professionalism and efficiency.</p>
              </div>
            </details>
          </div>
          <div class="accordion">
            <details>
              <summary>
                <div class="summary-content">
                  <img src="../assets/kategori/love.png" class="icon-love" alt="heart icon" />
                  <span>NATURAL AND SAFE</span>
                </div>
                <svg class="icon-chevron" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M5 8l5 5 5-5H5z"></path>
                </svg>
              </summary>
              <div class="accordion__content rte">
                <p>Our ingredients are 99% natural. Our formulas do not include any harmful ingredients.</p>
              </div>
            </details>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Kategori',
  };
  </script>
  
  <style scoped>
  .collapsible-content__wrapper {
    padding: 40px;
    background: #f8f5f1;
  }
  
  .collapsible-content__header {
    margin-bottom: 30px;
  }
  
  .caption-with-letter-spacing {
    letter-spacing: 0.1em;
    font-weight: bold;
    color: #555;
    font-size: 10px;
  }
  
  .h2 {
    font-size: 28px;
    font-weight: bold;
    color: #333;
  }
  
  .collapsible-content__grid {
    display: flex;
    flex-direction: column;
  }
  
  .accordion {
    margin-bottom: 10px;
    border-bottom: 1px solid #e5e5e5;
  }
  
  details {
    padding: 20px;
    cursor: pointer;
  }
  
  summary {
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-weight: bold;
    color: #333;
    list-style: none;
  }
  
  .summary-content {
    display: flex;
    align-items: center;
  }
  
  summary img {
    margin-right: 10px;
    width: 24px;
    height: 24px;
  }
  
  summary span {
    flex-grow: 1;
  }
  
  .accordion__content {
    padding: 10px 0;
    margin-top: 10px;
    color: #666;
  }
  
  .icon-leaf {
    width: 65px;
    height: 65px;
  }

  .icon-recycle {
    width: 55px;
    height: 55px;
  }

  .icon-star {
    width: 40px;
    height: 40px;
  }

  .icon-love {
    width: 38px;
    height: 38px;
  }
  
  .icon-chevron {
    transition: transform 0.3s ease;
  }
  
  details[open] .icon-chevron {
    transform: rotate(180deg);
  }
  </style>
  