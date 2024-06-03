<script>
import axios from 'axios';
import Card from './components/Card.vue'
import MainComponent from './components/Main.vue'
export default {
  components: {
    CharacterCard
  },
  data() {
    return {
      characters: [] 
    };
  },
  mounted() {
    axios.get('https://rickandmortyapi.com/api/character')
      .then(response => {
        this.characters = response.data.results; 
      })
      .catch(error => {
        console.error('Error fetching data:', error);
      });
  }
}
</script>

<template>
  <div>
    <CharacterCard :characters="characters" />
  </div>
</template>

<style>
</style>
