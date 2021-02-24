<template>
  <div id="product-list-two">
    <h2>List produk dua</h2>
    <ul>
        <li v-for="(product, index) in products" :key="index">
          <span class="name"> {{ product.name }}, </span>
          <span class="price">${{ product.price }} </span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ['products'],
  data () {
    return {
      
    }
  }
}
</script>

<style scopeed>
#product-list-two{
    background: #D1E4FF;
    box-shadow: 1px 2px 3px rgba(0,0,0,0.2);
    margin-bottom: 30px;
    padding: 10px 20px;
}
#product-list-two ul{
    padding: 0;
    list-style-type: none;
}
#product-list-two li{
    margin-right: 10px;
    margin-top: 10px;
    padding: 20px;
    background: rgba(255,255,255,0.7);
}

#product-list-two li:hover{
    margin-right: 10px;
    margin-top: 10px;
    padding: 20px;
    color: #ffffff;
    background: rgba(0,0,0,0.7);
}

.price{
    font-weight: bold;
    color: #ab77d4;
    display: block;
}
</style>
