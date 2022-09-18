<template>
    <div>
        <button @click="primeiro(txt), segundo(txt2)">Ativar</button>
        <p> {{ multiplos_ventos }}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data() {
          return {
            multiplos_ventos: 'opa',
            txt: 'Primeiro teste',
            txt2: 'segundo teste',
          }
        },
        methods: {
            primeiro(txt) {
                this.multiplos_ventos = txt;
            },
            segundo(txt2) {
                setTimeout(() => this.multiplos_ventos = txt2, 1500);
            }
        }
    }
</script>

<style scoped>
    div {
        margin: 100px
    }
</style>

