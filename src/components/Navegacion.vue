<script setup>
import { RouterLink } from 'vue-router';

</script>
<template>
<header class="cabeza">
    <div class="cabeza__logo">
        <RouterLink class="router-prin" to="/">
            <img class="logo" src="/src/assets/img/blifelogo-1.png" alt="">
        </RouterLink>
    </div>

    <div class="cabeza__navegacion">
        <nav class="navegacion">
            <RouterLink class="router" to="/">Productos</RouterLink>
            <RouterLink class="router" to="/">Promociones</RouterLink>
            <RouterLink class="router" to="/">Nosotros</RouterLink>
        </nav>
    </div>


    <div class="cabeza__iconos">
        <nav class="navegacion-iconos">
            <RouterLink class="router-icon"  to="/"><img class="icon" src="/src/assets/img/search.png" alt=""></RouterLink>
            <RouterLink class="router-icon" to="/"><img class="icon" src="/src/assets/img/user.png" alt=""></RouterLink>
            <RouterLink class="router-icon" to="/"><img class="icon" src="/src/assets/img/shop.png" alt=""></RouterLink>
        </nav>
    </div>
    
</header>
    
</template>

<style scoped>
.cabeza{
    display: flex;
    justify-content: space-between;
    width: 100%;
    height: 3rem;
}
.cabeza__navegacion{
    width: 40%;
    display: grid;
    place-items: center;
}
.navegacion{
    display: flex;
    justify-content: space-between;
    width: 90%;
}
.router{
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: "Kumbh Sans", sans-serif;
    font-weight: bold;
    color: black;
}
.router:hover{
    background: orange;
    border-radius: 20px;
}
.cabeza__logo{
    width: 20%;
    height: 100%;
    display: flex;
    align-items: center;
}
.router-prin{
    display: flex;
    align-items: center;
}
.router-prin:hover{
    background: none;
    transform: scale(1.05);
}
.logo{
    width: 60%;
}


.cabeza__iconos{
    width: 15%;
    display: grid;
    place-items: center;
}
.navegacion-iconos{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.router-icon{
    display: flex;
    justify-content: center;
    align-items: center;
}
.icon{
    width: 30%;
}
</style>