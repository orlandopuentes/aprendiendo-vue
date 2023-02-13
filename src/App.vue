<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>

  <nav class="navbar navbar-dark bg-dark">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/">
        <img src="@/assets/logo.svg" alt="" width="30" height="24" />
        Pokeapi
      </router-link>
      <div>
        <RouterLink to="/" class="btn btn-outline-primary mx-2">Home</RouterLink>
        <RouterLink to="/pokemons" class="btn btn-outline-primary">Pokemons</RouterLink>
      </div>
    </div>
  </nav>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/pokemons">Pokemons</RouterLink>
      </nav>
    </div>
  </header> -->
  <div class="container text-center">
    <RouterView />

  </div>
</template>

<style scoped>

</style>
