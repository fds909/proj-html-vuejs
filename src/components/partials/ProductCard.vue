<template>
    <div class="product-card">
        <img :src="`../assets/img/${image}`" alt="">
        <h4>{{name}}</h4>
    </div>
</template>

<script>
export default {
  name: 'ProductCard',
  props: {
      name: String,
      image: String,
      price: String
  },
}
</script>

<style scoped lang="scss">
    @import '../../style/palette.scss';

    .product-card {
        display: flex;
        flex-direction: column;
        width: calc(100% / 4);
        color: $daisy-bush;
        height: 100%;
        border: 1px solid red;
    }
</style>