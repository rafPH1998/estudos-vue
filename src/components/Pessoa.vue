<template>
    <div>
        <h1>Esta é a descrição da pessoa: {{nome}}</h1>
        <p>Estou trabalhando no momento</p>
        <button @click="showEmail">{{ textBotao }}</button>
        <p v-show="mostrar_email">Email Rafaelb89.rb@gmail.com.br</p>
        <Form />

        <p>Utilizo as seguintes tecnologias para backend: </p>
        <ul>
            <li v-for="(item, index) in backend_technologies" :key="index">
                {{ item }}
            </li>
        </ul>
        
        <p>Utilizo as seguintes tecnologias para backend: </p>
        <ul>
            <li v-for="(item, index) in frontend_technologies" :key="index">
                {{ item.language }} XP: {{item.xp}}
            </li>
        </ul>

    </div>
</template>

<script>
    import Form from './Form.vue'

    export default {
        name: 'Pessoa',
        components: {
            Form
        },
        data() {
          return {
            nome: "Rafael",
            mostrar_email: false,
            textBotao: 'Mostrar email',
            backend_technologies: [
                'Javascript', 'PHP', 'Python'
            ],
            frontend_technologies: [
                {id: 1, language: 'HTML', xp: 10},
                {id: 2, language: 'CSS', xp: 8},
                {id: 3, language: 'Inertia', xp: 14},
            ],
          }
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email
                if (!this.mostrar_email) {
                    this.textBotao = 'Mostrar email'
                } else {
                    this.textBotao = 'Enconder email'
                }
            }
        },
    }
</script>