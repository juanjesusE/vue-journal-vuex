<template>

<div class="entry-container mb-3 pointer p-2" @click="$router.push({ name: 'entry', params:{ id: 10} })">
  <div class="entry-title d-flex">
    <span class="text-success fs-5 fw-bold">04</span>
    <span class="mx-1 fs-5">Septiembre</span>
    <span class="mx-2 fw-light">2021, jueves</span>
  </div>
  <div class="entry-description">
    Lorem ipsum es el texto que se usa habitualmente en diseño gráfico en demostraciones de tipografías o de borradores de diseño para probar el diseño visual antes de insertar el texto final.
  </div>

</div>

</template>

<script>
export default {
  name: "Entry"
}
</script>

<style lang="scss" scoped>
.entry-container{
  border-bottom: 1px solid #2c3e50;
  transition: 0.2s all ease-in;

  &:hover{
    background-color: lighten($color: grey, $amount: 45);
    transition: 0.2s all ease-in;
  }

  .entry-description{
    font-size: 13px;
  }
}
</style>