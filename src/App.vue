<template>
  <div id="app">
    <HeaderComp :menu="headerMenu"/>

    <MainComp :products="products"/>

    <FooterComp :menu="footerMenu"/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

import "bootstrap";

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  },
  data() {
    return {
      headerMenu: ['HOME', 'SHOP', 'ABOUT', 'GALLERY', 'LOCATIONS', 'JOURNAL', 'CONTACT', 'MY ACCOUNT'],
      footerMenu: ['Shop', 'About', 'Gallery', 'Locations', 'Journal', 'Contact', 'Orders'],
      products: [
        {
          'name': 'Choco Chip Cookies',
          'image': 'choco-chip-cookies.jpg',
          'priceRange': '$19.00 - $39.00'
        },
        {
          'name': 'Strawberry Jam Cookies',
          'image': 'strawberry-jam-cookies.jpg',
          'priceRange': '$24.00 - $62.00'
        },
        {
          'name': 'Strawberry Donut',
          'image': 'strawberry-donut.jpg',
          'priceRange': '$24.00 - $42.00'
        },
        {
          'name': 'Perfect Macarons',
          'image': 'perfect-macarons.jpg',
          'priceRange': '$18.00 - $52.00'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
  @import 'style/palette.scss';
  @import "bootstrap/dist/css/bootstrap.min.css";

  // Reset
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Open Sans', sans-serif;
  }

  // Commons
  .container {
    width: 85%;
    margin: 0 auto;
  }

  img {
    max-width: 100%;
  }

  // Buttons
  .btn {
    text-decoration: none;
    padding: 10px 30px;
    text-align: center;
    font-size: 14px;
    font-weight: 500;
    border-radius: 5px;
  }

  .btn-white {
    background-color: $white;
    color: $daisy-bush;
  }

  .btn-purple {
    background-color: $daisy-bush;
    color: $white;
  }

  .btn-white:hover {
    background-color: $daisy-bush;
    color: $white;
  }

  .btn-purple:hover {
    background-color: $white;
    color: $daisy-bush;
  }
</style>
