<script setup>
// import { ref } from 'vue'
import Card from '../components/TheCard.vue'

</script>

<template>
  <main>
    <section class="card">
      <div>
        <h2>Daily</h2>
        <div class="cards">
          <Card hw="일일에포나" />
          <Card hw="가디언 토벌" />
          <Card hw="카오스 던전" />
        </div>
  
      </div>
    
      <div>
        <h2>Weekly</h2>
        <div class="cards">
          <Card hw="일일에포나" />
          <Card hw="가디언 토벌" />
          <Card hw="카오스 던전" />
        </div>
  
      </div>
    </section>
    
    
  </main>
</template>

<style scoped>
  main {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2em;
  }

 
  section.card  {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2em;
    flex: 1;
  }

  section.card div {
    width: 520px;
  }

  h2 {
    text-align: center;
  }
</style>
