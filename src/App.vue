<script setup>

import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <h1>Mokoko Station</h1>
    </div>
  </header>
  <div class="characters">
    <nav>
      <RouterLink to="/">character 1</RouterLink>
      <RouterLink to="/character2">character 2</RouterLink>
    </nav>
    <RouterView />
  </div>
  
  
</template>

<style scoped>
  * {
    color: white;
    
  }

  .wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .characters nav {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 2em;
  }
</style>
