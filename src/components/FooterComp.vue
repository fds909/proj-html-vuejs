<template>
  <footer>
    <div class="container">
      <!-- Top Footer -->
      <div class="top-footer">
        <!-- Left Menu -->
        <div class="left-menu">
          <img class="logo" src="../assets/img/avada-bakery-logo.png" alt="Bakery Avada Logo">
          <nav>
            <ul>
              <li class="menu-item" v-for="(element, index) in menu" :key="index">
                <a href="#">{{ element }}</a>
              </li>
              <li>
                <a href="#">
                  <i class="fa-solid fa-cart-shopping"></i>
                  <span class="cart-number">0</span>
                </a>
              </li>
            </ul>
          </nav>
        </div>

        <!-- Right Subscribe -->
        <div class="right-subscribe">
          <h4>Subscribe to our Newsletter</h4>
          <div>
            <input type="text" placeholder="Enter email address*">
            <a class="btn btn-purple" href="#">Subscribe</a>
          </div>
        </div>
      </div>

      <!-- Bottom Footer -->
      <div class="bottom-footer">
        <div class="copyright">
          &copy; Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Right Reserved | Powered by Wordpress       
        </div>

        <div class="social">
          <i class="fa-brands fa-instagram"></i>
          <i class="fa-brands fa-twitter"></i>
          <i class="fa-brands fa-facebook-f"></i>
          <i class="fa-brands fa-pinterest-p"></i>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp',
  props: ['menu'],
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';
    
    footer {
        background-color: $white;
        padding: 80px 0;
    }

    .logo {
      width: 150px;
      margin-left: 20px;
      margin-bottom: 40px;
    }

    .top-footer {
      display: flex;
      justify-content: space-between;
      margin-bottom: 50px;
    }

    .left-menu {
      display: flex;
      flex-direction: column;
    }

    ul {
      list-style-type: none;
    }

    .left-menu li {
      display: inline-block;
      margin-right: 25px;
    }

    .left-menu li a {
      text-decoration: none;
      color: $daisy-bush;
      font-size: 15px;
    }

    .left-menu i {
      font-size: 14px;
    }

    .cart-number {
      margin-left: 8px;
      background-color: $pearl-bush;
      padding: 3px 8px;
      border-radius: 50%;
    }

    .right-subscribe {
      display: flex;
      flex-direction: column;
    }

    h4 {
      text-align: right;
      font-family: 'Libre Bodoni', serif;
      font-size: 23px;
      font-weight: bold;
      color: $daisy-bush;
      margin-bottom: 40px;
    }

    .right-subscribe input {
      height: 40px;
      width: 250px;
      margin-right: 10px;
      border: 1px solid $manatee;
      border-radius: 5px;
    }

    .right-subscribe input::placeholder {
      font-size: 14px;
      padding-left: 20px;
    }

    // Bottom Footer
    .bottom-footer {
      display: flex;
      justify-content: space-between;
    }

    .copyright {
      font-size: 11px;
      color: $mamba;
    }

    .social {
      color: $daisy-bush;
      font-size: 20px;
    }

    .social i {
      margin: 0 20px;
    }
</style>