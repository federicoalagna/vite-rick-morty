<script>
import axios from 'axios';
import CardsFound from './components/CardsFound.vue'
import CardsList from './components/CardsList.vue'
import MainComponent from './components/Main.vue'
import HeaderComponent from './components/Header.vue'
export default {
  name: 'AppRickMorty',
    components: {
      CardsList,
      CardsFound,
      MainComponent,
      HeaderComponent,
    },
  };

</script>

<template>


<MainComponent></MainComponent>
<HeaderComponent></HeaderComponent>
<CardsList></CardsList>
<CardsFound></CardsFound>

</template>

<style>
</style>
