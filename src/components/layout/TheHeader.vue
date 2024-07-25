<script setup>
import { useRouter } from "vue-router";
const router = useRouter();
</script>

<template>
  <header>
    <h1 @click="router.push({ name: 'home' })">TD DESIGN</h1>
    <div class="options">
      <p @click="router.push({ name: 'about' })">ABOUT</p>
      <p @click="router.push({ name: 'work' })">WORK</p>
      <p @click="router.push({ name: 'contact' })">CONTACT</p>
    </div>
  </header>
</template>

<style>
header {
  background-color: black;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  align-content: flex-end;
  padding: 0px 20px;
}

h1 {
  font-family: helvetica;
  color: white;
  font-size: 30px;
}

p {
  font-size: 15px;
  font-family: helvetica;
  font-weight: lighter;
  color: white;
}

.options {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  gap: 25px;
}
</style>
