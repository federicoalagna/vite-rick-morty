<template>
    <div class="card-container">
      <div v-for="card in store.data" :key="card.id" class="card">
        <img :src="card.image" :alt="card.name" class="card-image"/>
        <h2>{{ card.name }}</h2>
        <p>Status: {{ card.status }}</p>
        <p>Species: {{ card.species }}</p>

      </div>
    </div>
  </template>
  
  <script>
  import { store } from '../store';
  
  export default {
    name: 'CardsList',
    data() {
      return {
        store,
      };
    },
  };
  </script>
  
  <style scoped>
  .card-container {
    display: flex;
    flex-wrap: wrap; 
    justify-content: space-between;
  }
  
  .card {
    flex-basis: calc(25% - 10px);
   
background-color: rgba(255, 255, 255, 0.703);
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 20px;
    box-sizing: border-box;
    margin-top: 20px;
    text-align: center;
  }
  
  .card-image {
    width: 70%;
    border-radius: 5px;
    margin-bottom: 10px;
  }
  
  h2 {
    margin: 3px 0px 27px 0px;
    font-size: 18px;
  }
  
  p {
    margin: 5px 0;
    font-size: 14px;

  }
  </style>
  