<template>
    <div>
 <h1>Products</h1> 
    <div class="products">
      <div v-for= "(product, index) in products" :key="index">{{ product.name }}<img class="productImg" :src="product.img">
      <div>{{ product.cost }}</div>
      <button @click="addItemToCart(product)">Add to Cart</button>
  </div>
</div>
</div>
</template>

<script>
export default{}
</script>

<style>

</style>