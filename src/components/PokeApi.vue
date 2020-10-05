<template>
  <div id="app">
    <h1>Poke Guía</h1>
   <p>Nombre</p> 
   <input :v-model="pokemonName"   type="text" placeholder="Busca un Pokemon">
   <button @click="searchPokemon">Buscar</button>
  </div>
</template>

<script>
export default {
  data(){
    return {
      currentPokemon: {},
      pokemonName: ""
    }
  },
  created(){
    ""
  },
  methods:{
    searchPokemon(){
      fetch(`https://pokeapi.co/api/v2/pokemon/${this.pokemonName}`)
      .then(data => data.json())
      .then(response => this.currentPokemon = response);
      //this.pokemonName
    }
  }
}
</script>

<style>

</style>