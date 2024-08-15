<script setup>
import { defineProps } from "vue";

// Define the props
const props = defineProps({
  title: {
    type: String,
    required: true,
  },
  p1: {
    type: Object,
    required: true,
    default: () => ({ IMG1: "", IMG_TXT: "" }),
  },
  p2: {
    type: Object,
    required: true,
    default: () => ({ IMG1: "", IMG_TXT: "" }),
  },
  p3: {
    type: Object,
    required: true,
    default: () => ({ IMG1: "", IMG_TXT: "" }),
  },
});
</script>

<template>
  <section class="container">
    <h1>{{ title }}</h1>

    <div class="one">
      <div class="base">
        <div class="brand">
          <img :src="p1.IMG_TXT" alt="texture image" />
        </div>
        <div class="photo">
          <img :src="p1.IMG1" alt="proyect photo" />
        </div>
      </div>
      <div class="base">
        <div class="brand">
          <img :src="p2.IMG_TXT" alt="texture image" />
        </div>
        <div class="photo">
          <img :src="p2.IMG1" alt="proyect photo" />
        </div>
      </div>
      <div class="base">
        <div class="brand">
          <img :src="p3.IMG_TXT" alt="texture image" />
        </div>
        <div class="photo">
          <img :src="p3.IMG1" alt="proyect photo" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

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
  margin: 20px;
  gap: 12px;
}

.brand {
  height: 450px;
  width: 100px;
  background-color: rgb(120, 120, 120);
  border-radius: 10px;
  overflow: hidden;
}

.photo {
  height: 450px;
  width: 250px;
  background-color: rgb(120, 120, 120);
  border-radius: 10px;
  overflow: hidden;
}
</style>
