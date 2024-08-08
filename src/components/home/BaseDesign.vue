<script setup></script>

<template>
  <section class="container">
    <h1>BRANDING</h1>
    <div class="one">
      <div class="base">
        <div class="brand"></div>
        <div class="photo"></div>
      </div>
      <div class="base">
        <div class="brand"></div>
        <div class="photo"></div>
      </div>
      <div class="base">
        <div class="brand"></div>
        <div class="photo"></div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.one {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-between;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 24pt;
  font-weight: bold;
  color: black;
  margin: 10px;
}

/* Diseño base de trabajos.*/
.base {
  display: flex;
  margin: 10px;
}

.brand {
  height: 450px;
  width: 100px;
  background-color: rgb(120, 120, 120);
  border-radius: 10px;
  margin: 10px;
}

.photo {
  height: 450px;
  width: 250px;
  background-color: rgb(120, 120, 120);
  border-radius: 10px;
  margin: 10px;
}
</style>
