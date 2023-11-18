<script setup>
import { ref } from 'vue'

defineProps({
  hw: {
    type: String,
    required: true
  },
})

const number = ref(0)

</script>

<template>
  <div class="card">
   
    <!-- <font-awesome-icon icon="['fas', 'bars']" /> -->
    <img src="" alt="" class="avatar">
    <p>{{ hw }}</p>
    <div class="score">
      <button class="icon" @click="number--"></button>
      <p>{{ number }}</p>
      <button class="icon" @click="number++"></button>
    </div>

  </div>
  
</template>

<style scoped>
  img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    border: none;
    /* background-color: aliceblue; */
  }
  .card {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-top: 1px solid white;
    flex: 1;
    text-align: center;
  }

  .score {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 1.2em;
  }


</style>
