<template>
  <div>
    <MultiplosEventos/>
    <Reutilizacao/>
  </div>
</template>

<script>
  import MultiplosEventos from './MultiplosEventos.vue';
  import Reutilizacao from './Reutilizacao.vue';

    export default {
        name: 'PrimeiroComponente',
        components: {
          MultiplosEventos,
          Reutilizacao,
        },
    }

</script>