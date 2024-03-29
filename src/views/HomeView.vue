<script setup>
import Navegacion from '@/components/Navegacion.vue';
</script>

<template>

  <Navegacion/>

  <section class="banner-1">
    <div class="banner-1__uno">
      <img class="img-1" src="/src/assets/img/banner-1.png" alt="">
    </div>
    <div class="banner-1__dos">
      <img class="img-2" src="/src/assets/img/banner-2.png" alt="">
    </div>
  </section>

  <section class="cards">
    <div></div>
    <div></div>
    <div></div>
    <div></div>
  </section>
</template>

<style scoped>

.banner-1{
  display: flex;
  margin-top: 1rem;
}

.banner-1__uno{
  width: 45%;
}
.banner-1__dos{
  width: 45%;
}

.img-1{
  width: 1300px;
}
.img-2{
  width: 500px;
  margin-left: 10rem;
}
</style>
