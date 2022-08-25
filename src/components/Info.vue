
<template>
    <div>
        <p v-if="trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Não estou trabalhando no momento.</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>

        <!-- mostra caso for true -->
        <p v-show="mostrar_email" >Mande uma mensagem para {{email}}</p>
    </div>
</template>

<script>
    export default {
        name: 'Info',
        data() {
            return {
                trabalhando: false,
                mostrar_email: false,
                email: 'rafael@hotmail.com.br.teste'
            }
        }
    }
</script>