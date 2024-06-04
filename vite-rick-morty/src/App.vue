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

<HeaderComponent></HeaderComponent>
<CardsFound></CardsFound>
<MainComponent></MainComponent>



</template>

<style>
</style>
