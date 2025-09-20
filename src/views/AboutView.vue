<template>
  <div class="about">
    <h1>About</h1>
    <button @click="storeCounter.increaseCount">
      
      {{ storeCounter.count }}
    </button>
  </div>
</template>



<script setup>

import { useCounterStore } from '@/stores/counter.js';
const storeCounter = useCounterStore();


</script>


<style scoped>
.about{
  text-align: center;
}
</style>

