<template>
    <nav :class="{'fixed-navbar': true, 'navbar-hidden': isNavbarHidden, 'navbar-sticky': isSticky}">
      <div class="navbar-container">
        <div class="top-bar">
          <p>FREE SHIPPING ON ORDERS +25€</p>
        </div>
        <div class="promotion-bar">
          <p>A PROFESSIONAL, EFFECTIVE AND NATURAL COSMETICS</p>
        </div>
        <div class="bottom-bar">
          <div class="left-icons">
            <router-link to="/search">
              <img src="@/assets/search.png" alt="Search" class="icon" />
            </router-link>
          </div>
          <div class="logo">
            <router-link to="/">
              <img src="@/assets/logo.png" alt="Logo" class="logo-img" />
            </router-link>
          </div>
          <div class="right-icons">
            <router-link to="/cart">
              <img src="@/assets/cart.png" alt="Cart" class="icon" />
            </router-link>
          </div>
        </div>
        <ul class="nav-links">
          <li><router-link to="/" exact-active-class="active-link">Home</router-link></li>
          <li><router-link to="/products" exact-active-class="active-link">Products</router-link></li>
          <li><router-link to="/about" exact-active-class="active-link">About</router-link></li>
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar',
    data() {
      return {
        lastScrollTop: 0,
        isSticky: false,
        isNavbarHidden: false,
        heroHeight: 0,
      };
    },
    mounted() {
      window.addEventListener('scroll', this.handleScroll);
      this.heroHeight = document.querySelector('.hero').clientHeight;
    },
    beforeDestroy() {
      window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
      handleScroll() {
        const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
  
        if (scrollTop > this.heroHeight) {
          this.isSticky = true;
        } else {
          this.isSticky = false;
        }
  
        if (scrollTop > this.lastScrollTop) {
          // Scroll ke bawah
          this.isNavbarHidden = true;
        } else {
          // Scroll ke atas
          this.isNavbarHidden = false;
        }
  
        this.lastScrollTop = scrollTop <= 0 ? 0 : scrollTop; // Untuk menghindari efek bouncing di iOS
      },
    },
  };
  </script>
  
  <style scoped>
  .fixed-navbar {
    width: 100%;
    background-color: #fff;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    z-index: 1000;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    transition: top 0.3s, background-color 0.3s;
    position: absolute;
    top: 0;
    left: 0;
  }
  
  .navbar-sticky {
    position: fixed;
    top: 0;
  }
  
  .navbar-hidden {
    top: -250px; /* Adjust this value based on the height of your navbar */
  }
  
  .navbar-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }
  
  .top-bar {
    width: 150%;
    background-color: #f7f7f7;
    text-align: center;
    padding: 1px 0;
    font-size: 14px;
    color: #333;
  }
  
  .promotion-bar {
    width: 150%;
    background-color: #d18b79;
    text-align: center;
    padding: 1px 0;
    font-size: 14px;
    color: #fff;
  }
  
  .bottom-bar {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    padding: 10px 0;
  }
  
  .left-icons,
  .right-icons {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
  }
  
  .left-icons {
    left: 20px;
  }
  
  .right-icons {
    right: 20px;
  }
  
  .icon {
    height: 24px;
  }
  
  .logo {
    text-align: center;
  }
  
  .logo-img {
    height: 40px;
  }
  
  .nav-links {
    list-style-type: none;
    margin: 10px 0 0 0;
    padding: 0;
    display: flex;
    justify-content: center;
    width: 100%;
  }
  
  .nav-links li {
    margin: 0 15px;
  }
  
  .nav-links a {
    text-decoration: none;
    color: #333;
    padding: 10px 20px;
    display: block;
    font-weight: bold;
    position: relative;
    transition: color 0.3s;
  }
  
  .nav-links a::after {
    content: '';
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    bottom: -5px;
    width: 0;
    height: 2px;
    background-color: #d18b79;
    transition: width 0.3s;
  }
  
  .nav-links a:hover::after,
  .nav-links a.active-link::after {
    width: 100%;
  }
  
  .nav-links a.active-link {
    color: #d18b79;
  }
  </style>
  