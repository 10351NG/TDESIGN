<script setup>
import TheWelcome from "./../components/home/TheWelcome.vue";
import BaseDesign from "@/components/home/BaseDesign.vue";
import Papa from "papaparse";

import { ref, onMounted } from "vue";

const proyects = ref([]);

onMounted(() => {
  Papa.parse(
    "https://docs.google.com/spreadsheets/d/e/2PACX-1vT4e41o-maN_CVA6cNkH9QybuEYBmiw9d8PApD_B9whN5Xacg1sq2BpC6HiMdHYx84monUFTqBb6k8U/pub?gid=0&single=true&output=csv",
    {
      download: true,
      header: true,
      complete: (results) => {
        proyects.value = results.data;
        console.log(results.data);
      },
    }
  );
});

function getProyectByTitle(title) {
  return proyects.value.find((proyect) => proyect.TITULO === title);
}
</script>

<template>
  <TheWelcome />
  <BaseDesign
    title="FOTOGRAFÍA / EDICIÓN"
    :p1="getProyectByTitle('WHITE')"
    :p2="getProyectByTitle('CLAUDIA HERRERA')"
    :p3="getProyectByTitle('ISISPHARMA')"
  />
  <BaseDesign
    title="BRANDING"
    :p1="getProyectByTitle('ASTER')"
    :p2="getProyectByTitle('ASTER')"
    :p3="getProyectByTitle('ASTER')"
  />
</template>

<style scoped></style>
