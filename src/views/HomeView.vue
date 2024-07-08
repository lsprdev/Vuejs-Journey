<script setup lang="ts">
import ProductList from '../components/ProductList.vue';
import { useProductsStore } from '../stores/products';
const productStore = useProductsStore();

</script>

<template>
  <main>
    <product-list :products="productStore.products" />
  </main>
</template>
