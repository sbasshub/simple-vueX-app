<template>
  <div id="app">
    <product-list-one></product-list-one>
    <product-list-two></product-list-two>
  </div>
</template>

<script>
export default {
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
