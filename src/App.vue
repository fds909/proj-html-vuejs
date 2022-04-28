<template>
  <div id="app">
    <Header :menu="headerMenu"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  },
  data() {
    return {
      headerMenu: ['HOME', 'SHOP', 'ABOUT', 'GALLERY', 'LOCATIONS', 'JOURNAL', 'CONTACT', 'MY ACCOUNT'],
    }
  }
}
</script>

<style lang="scss">
  @import 'style/palette.scss';

  // Reset
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Libre Bodoni', serif;
  }

  // Commons
  .container {
    width: 85%;
    margin: 0 auto;
  }

  .btn {
    text-decoration: none;
    padding: 10px 30px;
    text-align: center;
    font-size: 14px;
    font-weight: 500;
    border-radius: 5px;
  }

  .btn-white {
    background-color: white;
    color: $daisy-bush;
  }
</style>
