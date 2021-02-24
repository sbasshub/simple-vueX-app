<template>
  <div id="app">
    <product-list-one v-bind:products="products"></product-list-one>
    <product-list-two v-bind:products="products"></product-list-two>
  </div>
</template>

<script>
import ProductListOne from './components/ProductListOne.vue';
import ProductListTwo from './components/ProductListTwo.vue';

export default {
  components: {
    'product-list-one': ProductListOne,
    'product-list-two': ProductListTwo
  },
  name: 'app',
  data () {
    return {
      products: [
        {name: 'Pisang skin', price: 20},
        {name: 'Bintang terang', price: 40},
        {name: 'Kerang hijau', price: 60},
        {name: 'Kerang merah', price: 80}
      ]
    }
  }
}
</script>

<style>
</style>
