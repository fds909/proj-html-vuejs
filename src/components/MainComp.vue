<template>
  <main>
    <div class="container">
      <ProductsComp :products="products"/>

      <NumbersComp/>

      <LocationsComp/>

      <SocialComp/>
    </div>
      <CallToActionComp/>
  </main>
</template>

<script>
import ProductsComp from './ProductsComp.vue'
import NumbersComp from './NumbersComp.vue'
import LocationsComp from './LocationsComp.vue'
import SocialComp from './SocialComp.vue'
import CallToActionComp from './CallToActionComp.vue'

export default {
  name: 'MainComp',
  props: ['products'],
  components: {
    ProductsComp,
    NumbersComp,
    LocationsComp,
    SocialComp,
    CallToActionComp
  }
}
</script>

<style scoped lang="scss">
    @import '../style/palette.scss';

</style>