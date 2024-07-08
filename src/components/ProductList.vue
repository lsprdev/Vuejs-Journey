<script setup lang="ts">
import { ref, onMounted } from 'vue';

const props = defineProps(['products']);

</script>

<template>
    <main>
        <h1>Products</h1>
        <ul>
            <li v-for="product in props.products" :key="product.id">
                <h2>{{ product.nome }}</h2>
            </li>
        </ul>
    </main>
</template>