<template>
    <div>
        <button @click="ativa()">Clique aqui!</button>
        <p v-show="ativado">Ativado!</p>
    </div>
</template>

<script>
    export default {
    name: 'Reutilizacao',
    data() {
        return {
            ativado: false
        }
    },
    methods: {
        ativa() {
            this.ativado = !this.ativado 
        }
    },
}
</script>

