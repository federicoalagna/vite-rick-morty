
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
<div class="center m-top grey">
  {{ store.meta.total_rows }} Risultati trovati
</div>
  </template>
  