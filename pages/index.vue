<template>
  <v-container> 
    <Carousel>
    </Carousel>
    <ProductsBox>
    </ProductsBox>
    <ProductsBox>
    </ProductsBox>
  </v-container>
</template>

<script>

import Carousel from '../components/Carousel.vue'
import ProductsBox from '../components/ProductsBox.vue'

export default {
  components: {
    Carousel,
    ProductsBox,
  }
}
</script>
