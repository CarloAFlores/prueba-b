<script setup>
import Navegacion from '@/components/Navegacion.vue';
import { ref } from 'vue';

const comienzo = ref([]);


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
    <template v-for="index in 4" :key="index">
      <div class="carta-1">
        <div class="cards-1">
          <div class="cards-1__img"><img class="img-card" src="/src/assets/img/banner-3.png" alt=""></div>
          <div class="cards-1__btn">
            <button class="cards-1__btn-1"><i class="fa fa-heart" aria-hidden="true"></i>  22</button>
            <button class="cards-1__btn-1">-30%</button>
          </div>
        </div>

        <div class="cards-2">
          <div class="cards-2__desCan">
            <span class="negrita">Citrate Mag</span>
            <p class="descripcion">240 capsulas || 800mg</p>
          </div>

          <div class="cards-2__Precio">
            <span class="negrita">$273.00</span>
            <span>$134.00</span>
          </div>

          <div class="cards-2__Estrellas">
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa fa-star-half-o" aria-hidden="true"></i>
          </div>
        </div>


        <div class="cards-3">
          <div class="cards-3__comp">
            <span>Comparte</span>
            <div>
              <RouterLink class="router" to="/"><i class="fab fa-facebook" aria-hidden="true"></i></RouterLink>
              <RouterLink class="router" to="/"><i class="fab fa-instagram" aria-hidden="true"></i></RouterLink>
              <RouterLink class="router" to="/"><i class="fab fa-twitter" aria-hidden="true"></i></RouterLink>
            </div>
          </div>

          <div class="cards-3__agg">
            <button class="btn-agg">Agregar</button>
          </div>
        </div>
      </div>
  </template>
    

    


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

.cards{
  display: flex;
  justify-content: space-evenly;
}

.carta-1{
  margin-top: 30px;
  margin-left: 30px;
  width: 20%;
  height: 20rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: all .25s ease-in;
}
.carta-1:hover{
  transform: scale(1.1);
  border: 1px solid blue;
  transition: all .25s ease-in;
  border-radius: 15px;
}
.cards-1{
  display: flex;
  justify-content: center;
  width: 100%;
}
.cards-1__img{
  width: 80%;
}
.img-card{
  width: 100%;
  height: 12rem;
}
.cards-1__btn{
  display: flex;
  flex-direction: column;
}
.cards-1__btn-1{
  margin-top: 5px;
  border: none;
  border-radius: 15px;
  font-weight: bold;
}
.cards-1__btn-1:hover{
  background: #FF8E8E;
  transition: all .25s ease-in;
  color: white;
}

.cards-2 {
  display: flex;
  flex-wrap: wrap;
  width: 80%;
}

.cards-2__desCan,
.cards-2__Precio {
  flex: 1 1 45%; 
  margin-left: 5px;

}
.cards-2__Precio{
  display: flex;
  flex-direction: column;
}
.cards-2__Estrellas {
  width: 100%; 
}

.cards-3{
  display: flex;
  justify-content: space-around;
  width: 80%;
}

.cards-3__agg{
  display: grid;
  place-items: center;
}
.btn-agg{
  width: 6rem;
  height: 1.5rem;
  border-radius: 15px;
  border: 1px solid orange;
  font-weight: bold;
  background: white;
}
.btn-agg:hover{
  background: black;
  color: white;
  transition: all .3s ease-in;
}


.negrita{
  font-weight: bold;
}
.descripcion{
  font-size: 8px;
}
</style>
