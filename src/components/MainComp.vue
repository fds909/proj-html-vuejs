<template>
  <main>
    <div class="container">
      <ProductsComp :products="products"/>

      <NumbersComp/>
    </div>
  </main>
</template>

<script>
import ProductsComp from './ProductsComp.vue'
import NumbersComp from './NumbersComp.vue'

export default {
  name: 'MainComp',
  props: ['products'],
  components: {
    ProductsComp,
    NumbersComp
  }
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

</style>