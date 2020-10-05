<template>
  <div id="app">
    <img alt="Pokemon logo" src="./assets/Pokemon.png">
    <PokeApi msg="Bienvenido a tu Guía Pokemon"/>
  </div>
</template>

<script>
import PokeApi from './components/PokeApi'

export default {
  name: 'App',
  components: {
    PokeApi
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
