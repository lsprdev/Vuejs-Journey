<script setup lang="ts">
import { ref, onMounted } from 'vue';

const count = ref(0);

function increment() {
  count.value++;
}

function decrement() {
  count.value--;
}

</script>

<template>
  <div class="counter-area">
    <button @click="increment">Increment</button>
    <span>{{ count }}</span>
    <button @click="decrement">Decrement</button>
  </div>
</template>

<style scoped>
.counter-area {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  margin-top: 20px;
}

.counter-area button {
  padding: 10px 20px;
  font-size: 16px;
  border: none;
  border-radius: 5px;
  background-color: #42b883;
  color: #fff;
  cursor: pointer;
}

.counter-area span {
  font-size: 30px;
}
</style>
