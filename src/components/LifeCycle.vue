<template>
    <div>
        <p>Meu nome é: {{nome}}</p>
    </div>
</template>

<script>
    export default {
        name: 'LifiCycle',
        data() {
          return {
            nome: "Ainda nao sei"
          }
        },
        created() {
            setTimeout(() => {  
                this.nome = 'Ciclanooooo'
            }, 2000);
        },
        mounted() {
            this.nome = 'Ciclano'
        },
    }

</script>

