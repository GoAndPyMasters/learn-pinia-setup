<template>
  <div class="home">
   <Counter/>
      <div class = "buttons">
        <button @click="storeCounter.decreaseCount">-</button>
        <button @click="storeCounter.increaseCount">+</button>
      </div>
      <hr>
      <div>
        The counter is : {{ storeCounter.oddOrEven }}
      </div>
      <hr>
      <h3> Edit Counter: </h3>
      <input type="number" v-model="storeCounter.count"/>
  </div>
</template>


<script setup>

import { useCounterStore } from '@/stores/counter.js';
import Counter from '@/components/Counter.vue';
const storeCounter = useCounterStore();


</script>



<style scoped>
.home{
  text-align: center;
}
.count{
  font-size: 60px;
  margin: 20px;
}
.buttons button{
  font-size: 48px;
  margin: 10px;
  width: 50px;
  height: 50px;
}

</style>