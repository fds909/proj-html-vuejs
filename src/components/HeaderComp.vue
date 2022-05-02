<template>
  <header>
    <FloatingButtons/>

    <div class="header-top">
        <img class="logo" src="../assets/img/avada-bakery-logo.png" alt="Bakery Avada Logo">
        <nav>
            <ul>
                <li class="menu-item" v-for="(element, index) in menu" :key="index">
                    <a href="#">{{ element }}</a>
                </li>
                <li>
                    <a href="#">
                        <i class="fa-solid fa-cart-shopping"></i>
                    </a>
                </li>
            </ul>
        </nav>
    </div>
    <div class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="upper-text">fresh & tasty bakery every day</div>
                <h1>The Perfect Fresh Bread</h1>
                <p>Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Aliquam erat volutpat. Nullam quis saggittis nibh nulla is orci tempor.</p>
                <a class="btn btn-white" href="#">Explore our products</a>
            </div>
        </div>
    </div>
  </header>
</template>

<script>
import FloatingButtons from './FloatingButtons.vue';

export default {
  name: 'HeaderComp',
  props: ['menu'],
  components: {
      FloatingButtons
  }
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

    header {
        font-family: 'Open Sans', sans-serif;
        color: $daisy-bush;
        background-image: url('../assets/img/hero-header-bakery.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        height: 100vh;
    }
    
    .logo {
        height: 75px;
    }

    .header-top {
        font-weight: 500;
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 90px;
        padding: 0 20px;
    }

    nav ul {
        list-style-type: none;
    }

    nav li {
        display: inline-block;
        margin: 0 10px;
    }

    nav .menu-item {
        display: inline;
        margin: 0 10px;
        margin-bottom: 20px;
        &:hover {
            border-bottom: 2px solid $daisy-bush;
        }
    }

    nav a {
        color: $daisy-bush !important;
        text-decoration: none;
        font-size: 14px;
    }

    // Hero
    .hero {
        padding: 100px 0;
    }

    .upper-text {
        font-size: 12px;
        font-weight: 500;
        text-transform: uppercase;
        color: $mamba;
    }

    .hero-content {
        width: calc(100% / 3);
    }

    h1 {
        font-family: 'Libre Bodoni', serif;
        font-size: 45px;
        font-weight: bold;
        margin: 15px 0;
    }

    .hero p {
        text-align: justify;
        margin-bottom: 30px;
        color: $mamba;
        font-weight: 500;
    }
</style>