
  <script>
  import { store } from '../store';

export default {
    name: 'CardsFound',
    data() {
        return {
            store,
        };
    },
};
  </script>
  
  <template>
<h4 class="center m-top grey">
  {{ store.meta.total_rows }} Risultati trovati
</h4>
  </template>
  