
<template>
  <div>
    <PrimeiroComponente />
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'

  export default {
    components: {
      PrimeiroComponente,
      LifeCycle,
      Pessoa
    }
  }
</script>

<style>
  body {
    background-color: #333;
    color: #fff;
  }
</style>