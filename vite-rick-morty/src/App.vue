<script>
import axios from 'axios';
import Card from './components/Card.vue'
import MainComponent from './components/Main.vue'

export default {
  name: 'AppRickMorty',
    components: {
      Card,
      MainComponent,
    },
  };

</script>

<template>

<Card></Card>
<MainComponent></MainComponent>

</template>

<style>
</style>
