<script setup>
import TheCard from "./TheCard.vue";
</script>

<template>
  <div class="square">
    <TheCard name="Juan" />
    <TheCard name="Pedro" />
    <TheCard name="Sebastian" />
    <TheCard name="Santiago" />
    <TheCard name="Salim" />
    <TheCard name="Nowo" />
    <TheCard name="Zapingsong" />
    <TheCard name="Mateo" />
  </div>
</template>

<style scoped>
.square {
  width: 500px;
  height: 500px;
  border: 2px solid white;
  display: grid;
  gap: 1rem;
  grid-template-columns: 1fr 1fr;
  justify-content: center;
  justify-items: center;
  align-content: center;
}
</style>
