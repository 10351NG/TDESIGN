<script setup>
import CardContainer from "./../components/CardContainer.vue";
import TheWelcome from "./../components/home/TheWelcome.vue";
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
</script>

<template>
  <TheWelcome />
  <CardContainer />
</template>

<style scoped></style>
