<script setup></script>

<template>
  <section class="container">
    <h1>FOTOGRAFÍA / EDICIÓN</h1>
    <div class="one">
      <div class="base">
        <div class="brand">
          <img
            src="https://firebasestorage.googleapis.com/v0/b/portafolio-web-end.appspot.com/o/fotografía%20y%20edición%20de%20moda%2FWHITE%20TXT.png?alt=media&token=31a70f78-53c4-40a9-9982-e5900b0e34e6"
            alt=""
          />
        </div>
        <div class="photo">
          <img
            src="https://firebasestorage.googleapis.com/v0/b/portafolio-web-end.appspot.com/o/fotografía%20y%20edición%20de%20moda%2FWHITE%201.png?alt=media&token=8a9f9d62-000c-4b6d-b1e7-e3a2639d37d8"
            alt=""
          />
        </div>
      </div>
      <div class="base">
        <div class="brand">
          <img
            src="https://firebasestorage.googleapis.com/v0/b/portafolio-web-end.appspot.com/o/fotografía%20y%20edición%20de%20moda%2FTXT%20II.png?alt=media&token=97af3911-18f9-4f57-a32f-17281deceda3"
            alt=""
          />
        </div>
        <div class="photo">
          <img
            src="https://firebasestorage.googleapis.com/v0/b/portafolio-web-end.appspot.com/o/fotografía%20y%20edición%20de%20moda%2FCLAUDIA%20HERRERA%205.png?alt=media&token=b1d20f31-faf0-493a-b0fb-0cf45a1daab3"
            alt=""
          />
        </div>
      </div>
      <div class="base">
        <div class="brand">
          <img
            src="https://firebasestorage.googleapis.com/v0/b/portafolio-web-end.appspot.com/o/fotografía%20y%20edición%20de%20moda%2FTXT%20III_ISIS.png?alt=media&token=d0f01fcf-627e-4bb3-b323-39ac62f10699"
            alt=""
          />
        </div>
        <div class="photo">
          <img
            src="https://firebasestorage.googleapis.com/v0/b/portafolio-web-end.appspot.com/o/fotografía%20y%20edición%20de%20moda%2FISAPHARMA%201.png?alt=media&token=6a6dbd43-0fa4-4508-8d38-93e327f5d9b3"
            alt=""
          />
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
