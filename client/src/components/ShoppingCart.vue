<script setup lang="ts">
import { refCart, count, total } from '@/models/shoppingCart'
import { ref } from 'vue'

const cart = refCart()
</script>

<template>
  <div class="cart">
    <h1 class="title">Shopping Cart</h1>
    <h2 class="subtitle">This is the shopping cart page</h2>
    <p>Here is a list of items in your cart</p>
    <div v-for="item in cart" :key="item.product.id">
      <p>{{ item.product.title }}</p>
      <p>{{ item.product.price }}</p>
    </div>
    <p>Total: {{ count }} items = ${{ total }}</p>
  </div>
</template>

<style scoped>
.cart {
  padding: 1rem;
}
</style>
