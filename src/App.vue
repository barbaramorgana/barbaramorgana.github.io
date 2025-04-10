<script setup lang="ts">
import ButtonLinks from '@/components/ButtonLinks.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <img alt="Main Picture" class="logo" src="./assets/main-picture.jpg" />

      <h1 class="green">Bárbara Morgana</h1>
      <h3>A música do céu no ar!</h3>
    </div>
  </header>

  <main>
    <div class="wrapper">
      <h3>Escolha seu serviço de música preferido</h3>
      <ButtonLinks />
    </div>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 1rem;
}

.wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  max-width: 300px;
  border-radius: 15%;
  border: #2c3e50 3px solid;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
}
</style>
