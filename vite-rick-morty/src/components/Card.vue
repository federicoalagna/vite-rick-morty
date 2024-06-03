<template>
    <div>
      <div v-for="character in characters" :key="character.id">
        <div class="card">
          <img :src="character.image" alt="Character Image">
          <h3>{{ character.name }}</h3>
          <p>{{ character.species }}</p>
        </div>
      </div>
    </div>
    
  </template>
  
  <script>
  export default {
    props: {
      characters: Array 
    }
  }
  </script>
  
  <style>
  .card {
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 10px;
    margin: 10px;
    width: 200px;
  }
  </style>