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

<template>
<div>
    <ul>
        <li v-for="card in store.data" :key="card.id"> <!-- Aggiunto key per una migliore gestione di v-for -->
            {{ card.name }}
        </li>
    </ul>
</div>
</template>
