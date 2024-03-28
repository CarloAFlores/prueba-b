<script setup>
import { RouterLink } from 'vue-router';

</script>
<template>
<header class="cabeza">
    <div class="cabeza__logo">B LIFE</div>

    <div class="cabeza__navegacion">
        <nav class="navegacion">
            <RouterLink to="/">PRODUCTO</RouterLink>
            <RouterLink to="/">PROMOCIONES</RouterLink>
            <RouterLink to="/">NOSOTROS</RouterLink>
        </nav>
    </div>


    <div class="cabeza__iconos">
        <nav>
            <RouterLink to="/">PRODUCTO</RouterLink>
            <RouterLink to="/">PROMOCIONES</RouterLink>
            <RouterLink to="/">NOSOTROS</RouterLink>
        </nav>
    </div>
    
</header>
    
</template>

<style scoped>
.cabeza{
    background: red;
    display: flex;
    justify-content: space-between;
    width: 100%;
}

.cabeza__navegacion{
    background: greenyellow;
    width: 40%;
}
.navegacion{
    background: olive;
    display: flex;
    justify-content: space-between;
}

</style>