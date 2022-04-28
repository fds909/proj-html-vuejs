<template>
  <div class="products">
    <!-- Slider Large -->
    <div class="slider-large">

      <div class="our-products">
        <div class="upper-text">our products</div>
        <h2>All our delectable pastries are backed Fresh in our Kitchen very morning,
            and are made with all-natural, all organic ingredients
        </h2>
        <a class="btn btn-purple" href="#">Start Shopping</a>
      </div>

      <div class="slider-large-content">
        <div class="arrow-left"><i class="fa-solid fa-angle-left"></i></div>
        <div class="arrow-right"><i class="fa-solid fa-angle-right"></i></div>
        <img src="../assets/img/choco-chip-cookies-400x510.jpg" alt="Choco Chip Coockies">
        <img src="../assets/img/strawberry-jam-cookies-400x510.jpg" alt="Strawberry Jam Cookies">
      </div>
  
    </div>

    <div class="wedding">
      <div class="upper-text">
        corporate & weddings
      </div>
      <h2>Baking Special Moments</h2>
      <div class="wedding-images">
        <div class="img-container">
          <img src="../assets/img/corporate-bg.jpg" alt="Corporate">
        </div>

        <div class="img-container">
          <img src="../assets/img/wedding-bg.jpg" alt="Wedding">
        </div>
      </div>
    </div>

    <div class="slider-small">
      <div class="slider-small-text">
        <h2>Find a freshly baked product perfect for you</h2>
        <p>Integer a nihb vitae ex porttitor rutrum et ut velit.
           Etiam ac felis at leo feugiat placerat. Sed ac nulla id orci
           tempor convallis des.
        </p>
        <a class="btn btn-purple" href="#">Shop All Products</a>
      </div>

      <div class="slider-small-content">
        <div class="card-container">
          <!-- <ProductCard
              v-for="(prod, index) in products"
              :key="index"
              :name="prod.name"
              :image="prod.image"
              :price="prod.price"
          /> -->
          <div class="arrow-left"><i class="fa-solid fa-angle-left"></i></div>
          <div class="arrow-right"><i class="fa-solid fa-angle-right"></i></div>
          <div class="product-card">
            <img src="../assets/img/choco-chip-cookies.jpg" alt="Choco Chip Cookies">
            <h3>Choco Chip Cookies</h3>
            <div class="price">$19.00 - $39.00</div>
          </div>
          <div class="product-card">
            <img src="../assets/img/strawberry-jam-cookies.jpg" alt="Choco Chip Cookies">
            <h3>Strawberry Jam Cookies</h3>
            <div class="price">$24.00 - $62.00</div>
          </div>
          <div class="product-card">
            <img src="../assets/img/strawberry-donut.jpg" alt="Choco Chip Cookies">
            <h3>Strawberry Donut</h3>
            <div class="price">$24.00 - $42.00</div>
          </div>
          <div class="product-card">
            <img src="../assets/img/perfect-macarons.jpg" alt="Choco Chip Cookies">
            <h3>Perfect Macarons</h3>
            <div class="price">$18.00 - $52.00</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import ProductCard from './partials/ProductCard.vue'

export default {
  name: 'ProductsComp',
  props: ['products'],
  // components: {
  //   ProductCard
  // }
}
</script>

<style scoped lang="scss">
  @import '../style/palette.scss';

  .products {
    padding: 100px 0;
  }

  img {
    max-width: 100%;
  }

  // Slider Lanrge
  .slider-large {
    display: flex;
  }

  .our-products {
    width: calc(100% / 2.5);
    margin-right: 10px;
  }

  .upper-text {
    display: block;
    font-size: 12px;
    font-weight: 500;
    text-transform: uppercase;
    color: $mamba;
  }

  h2 {
    font-family: 'Libre Bodoni', serif;
    font-size: 28px;
    font-weight: bold;
    color: $daisy-bush;
    margin: 25px 0;
  }

  .slider-large-content {
    display: flex;
    position: relative;
  }

  .slider-large-content img {
    width: 50%;
  }

  .arrow-left, .arrow-right {
    display: flex;
    align-items: center;
    color: $white;
    background-color: $perfume;
    padding: 0 10px;
    height: 60px;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
  }

  .arrow-left {
    left: 0;
  }

  .arrow-right{
    right: 0;
  }

  // Wedding
  .wedding {
    margin: 120px 0;
  }

  .wedding .upper-text {
    text-align: center;
  }

  .wedding h2 {
    text-align: center;
  }
  
  .wedding-images {
    display: flex;
    justify-content: center;
  }

  .wedding .img-container {
    width: 50%;
    padding: 0 20px;
  }

  //Slider Small
  .slider-small {
    display: flex;
  }

  .slider-small-text {
    display: flex;
    flex-direction: column;
    justify-content: end;
    width: calc(100% / 4);
    text-align: center;
  }

  .slider-small-text h2 {
    font-size: 25px;
  }

  .slider-small-text p {
    font-size: 14px;
    color: $mamba;
    margin-top: 10px;
    margin-bottom: 30px;
  }

  .slider-small-content {
    width: calc(100% / 4) * 3;
    padding: 0 30px;
  }

  .card-container {
    display: flex;
    height: 100%;
    position: relative;
  }

  .product-card {
    display: flex;
    flex-direction: column;
    width: calc(100% / 4);
  }

  .product-card h3 {
    font-family: 'Libre Bodoni', serif;
    font-size: 17px;
    font-weight: bold;
    text-align: center;
    color: $daisy-bush;
    margin: 15px 0;
  }

  .product-card .price {
    color: $daisy-bush;
    font-size: 15px;
    text-align: center;
  }



</style>