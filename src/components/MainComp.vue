<template>
  <main>
    <div class="container">
      <ProductsComp :products="products"/>

      <NumbersComp/>

      <LocationsComp/>
    </div>
  </main>
</template>

<script>
import ProductsComp from './ProductsComp.vue'
import NumbersComp from './NumbersComp.vue'
import LocationsComp from './LocationsComp.vue'

export default {
  name: 'MainComp',
  props: ['products'],
  components: {
    ProductsComp,
    NumbersComp,
    LocationsComp
  }
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

</style>