<script setup lang="ts">
import ButtonLinks from '@/components/ButtonLinks.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <img alt="Main Picture" class="logo" src="./assets/main-picture.png" />

      <h1>Escandalosa Graça</h1>
      <h3>Bárbara Morgana</h3>
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
  line-height: 1.4;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 1rem;
}

header h3 {
  color: var(--color-h3);
}

.wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  max-width: 250px;
  border-radius: 15%;
  border: #1f150d 3px solid;
}

h1 {
  color: #cb835f;
  font-weight: 500;
  font-size: clamp(1.5rem, 6vw, 2.6rem);
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 100%;
  padding-top: 7px;
}
</style>
