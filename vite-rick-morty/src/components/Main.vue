<script>
import axios from 'axios';
import CardsFound from './CardsFound.vue';
import CardsList from './CardsList.vue';
import { store } from '../store';

export default {
    name: 'MainComponent',
    components: {
        CardsFound,
        CardsList,
    },
    data() {
        return {
            store,
        };
    },
    created() {
        axios.get(this.store.apiUrl).then((response) => {
            this.store.data = response.data.results; // Accesso corretto ai dati
            this.store.meta = response.data.info; // Separazione dei meta-dati

            console.log(this.store.data);
        });
    },
};
</script>

<template>
    <div class="container">
        <CardsList></CardsList>
    </div>
</template>

<style>
</style>
