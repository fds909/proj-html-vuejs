<template>
  <div id="call-to-action">
      <div class="container-narrow">
        <div class="upper-text">Try our seasonal products</div>
        <h2>Order for pick-up or delivery to your home</h2>
        <a class="btn btn-white" href="#">Shop Now</a>
      </div>
  </div>
</template>

<script>
export default {
  name: 'CallToActionComp',
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

    #call-to-action {
        background-image: url('../assets/img/call-to-action-bg.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        height: 60vh;
    }

    .upper-text {
        display: block;
        font-size: 12px;
        font-weight: 500;
        text-transform: uppercase;
        color: $mamba;
        margin-bottom: 20px;
    }

    .container-narrow {
        width: 60%;
        margin: 0 auto;
        padding: 100px 0;
    }

    h2 {
        font-family: 'Libre Bodoni', serif;
        font-size: 36px;
        font-weight: bold;
        color: $white;
        width: 70%;
        margin-bottom: 60px;
    }
</style>