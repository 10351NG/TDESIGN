<script setup>
const props = defineProps({
  name: String,
});
</script>
<template>
  <div class="name">
    <h1>{{ props.name }}</h1>
  </div>
</template>
<style>
.name {
  display: flex;
  width: 200px;
  height: 100px;
  border: 1px solid rgb(0, 0, 0);
  background-color: bisque;
  justify-content: center;
  align-items: center;
}

h1 {
  display: flex;
  font-family: Helvetica;
  font-size: 14pt;
  font-weight: bold;
}
</style>
