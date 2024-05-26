<template>
    <div class="product-grid">
      <div class="filter-sort">
        <div class="filter">
          <span>Filter:</span>
          <select>
            <option>Availability</option>
          </select>
          <select>
            <option>Price</option>
          </select>
        </div>
        <div class="sort">
          <span>Sort by:</span>
          <select>
            <option>Characteristics</option>
          </select>
        </div>
        <div class="product-count">
          <span>12 products</span>
        </div>
      </div>
      <div class="products">
        <div class="product" v-for="product in products" :key="product.id" @mouseover="changeImage(product.id, true)" @mouseleave="changeImage(product.id, false)" @mousedown="removeShadow" @mouseup="addShadow">
          <div class="product-image-container">
            <img :src="product.currentImage" :alt="product.name" class="product-image" />
          </div>
          <h3>{{ product.name }}</h3>
          <p>{{ product.price }}</p>
          <button>Buy Now</button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProductGrid',
    data() {
      return {
        products: [
          {
            id: 1,
            name: 'PINK PURIFYING MASK',
            price: '€25,00 EUR',
            image: '/assets/mask1.jpg',
            hoverImage: '/assets/mask2.jpg',
            currentImage: '/assets/mask1.jpg',
          },
          {
            id: 2,
            name: 'VITAMIN ADVANCE SERUM',
            price: '€42,00 EUR',
            image: '/assets/serum1.jpg',
            hoverImage: '/assets/serum2.jpg',
            currentImage: '/assets/serum1.jpg',
          },
          {
            id: 3,
            name: 'VITAMIN C CREAM REPAIR',
            price: '€45,00 EUR',
            image: '/assets/cremaC1.png',
            hoverImage: '/assets/cremaC2.png',
            currentImage: '/assets/cremaC1.png',
          },
          {
            id: 4,
            name: 'BOTOX TOTALIFT SERUM',
            price: '€42,00 EUR',
            image: '/assets/serumC1.png',
            hoverImage: '/assets/serumC2.png',
            currentImage: '/assets/serumC1.png',
          },
          {
            id: 5,
            name: 'LIFTING MASK',
            price: '€47,00 EUR',
            image: '/assets/liftingmask1.jpg',
            hoverImage: '/assets/liftingmask2.jpg',
            currentImage: '/assets/liftingmask1.jpg',
          },
          {
            id: 6,
            name: 'BODY CREAM',
            price: '€49,00 EUR',
            image: '/assets/body1.jpg',
            hoverImage: '/assets/body2.jpg',
            currentImage: '/assets/body1.jpg',
          },
          {
            id: 7,
            name: 'CONTOUR',
            price: '€43,00 EUR',
            image: '/assets/contorno2.jpg',
            hoverImage: '/assets/contorno1.jpg',
            currentImage: '/assets/contorno2.jpg',
          },
          {
            id: 8,
            name: 'REGENERATING FIRMING CREAM',
            price: '€50,00 EUR',
            image: '/assets/crema2.jpg',
            hoverImage: '/assets/crema1.jpg',
            currentImage: '/assets/crema2.jpg',
          },
          {
            id: 9,
            name: 'PEELING',
            price: '€41,00 EUR',
            image: '/assets/peeling1.jpg',
            hoverImage: '/assets/peeling2.jpg',
            currentImage: '/assets/peeling1.jpg',
          },
          {
            id: 10,
            name: 'BASIC REMOVER',
            price: '€42,00 EUR',
            image: '/assets/remover2.jpg',
            hoverImage: '/assets/remover1.jpg',
            currentImage: '/assets/remover2.jpg',
          },
          {
            id: 11,
            name: 'TONIC',
            price: '€46,00 EUR',
            image: '/assets/tonico1.jpg',
            hoverImage: '/assets/tonico2.jpg',
            currentImage: '/assets/tonico1.jpg',
          },
          {
            id: 12,
            name: 'FACIAL WASH',
            price: '€40,00 EUR',
            image: '/assets/wash1.jpg',
            hoverImage: '/assets/wash2.jpg',
            currentImage: '/assets/wash1.jpg',
          },
        ],
      };
    },
    methods: {
      changeImage(productId, isHovering) {
        const product = this.products.find(product => product.id === productId);
        product.currentImage = isHovering ? product.hoverImage : product.image;
      },
      removeShadow(event) {
        event.currentTarget.style.boxShadow = 'none';
      },
      addShadow(event) {
        event.currentTarget.style.boxShadow = '0 4px 8px rgba(0, 0, 0, 0.1)';
      },
    },
  };
  </script>
  
  <style scoped>
  .product-grid {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    margin-top: 200px;
  }
  
  .filter-sort {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
  }
  
  .filter-sort .filter,
  .filter-sort .sort,
  .filter-sort .product-count {
    display: flex;
    align-items: center;
  }
  
  .filter-sort span {
    margin-right: 10px;
    font-weight: bold;
  }
  
  .filter-sort select {
    padding: 5px;
    border: 1px solid #ccc;
    border-radius: 4px;
    margin-right: 10px;
  }
  
  .products {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  
  .product {
    width: calc(25% - 20px);
    border-radius: 16px;
    padding: 0;
    text-align: center;
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: box-shadow 0.2s;
    position: relative;
    overflow: hidden;
  }
  
  .product:hover h3 {
    text-decoration: underline;
  }
  
  .product-image-container {
    position: relative;
    width: 100%;
    padding-top: 100%;
    border-radius: 16px 16px 0 0;
    overflow: hidden;
  }
  
  .product-image {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.8s cubic-bezier(0.25, 0.1, 0.25, 1), opacity 0.8s ease-in-out;
  }
  
  .product:hover .product-image {
    transform: scale(1.1);
  }
  
  .product h3 {
    font-size: 16px;
    margin: 15px 0 5px;
    color: #333;
    font-weight: bold;
    transition: text-decoration 0.3s;
  }
  
  .product p {
    font-size: 14px;
    color: #777;
    margin-bottom: 15px;
  }
  
  .product button {
    padding: 10px 20px;
    border: 1px solid #d18b79;
    border-radius: 24px;
    background-color: #fff;
    color: #d18b79;
    cursor: pointer;
    font-weight: bold;
    transition: background-color 0.4s, color 0.4s;
    margin-bottom: 15px;
  }
  
  .product button:hover {
    background-color: #d18b79;
    color: #fff;
  }
  </style>
  