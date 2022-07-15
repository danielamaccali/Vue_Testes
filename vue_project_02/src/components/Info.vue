<template>
    <div>
        <p v-if="estou_trabalhando">Estou dormindo no momento.</p>
        <p v-else>Estou em busca de oportunidades. </p>
        <p>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>CSS</li>
            <li>Vue</li>
        </ul> 
        <div>
            <button @click="showEmail"> {{ textoBotao }} </button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar o emu portólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>
    import Picture from './Picture.vue'
    export default {
        name: 'Info',
        components: {
            Picture
        },
        data() {
            return {
                estou_trabalhando: true,
                mostrar_email: false,
                email: 'luciogato@email.com',
                meu_link: 'https://google.com',
                textoBotao: 'Mostrar e-mail'
            }
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email) {
                    this.textoBotao = 'Mostrar e-mail'
                }
                else {
                    this.textoBotao = 'Esconder e-mail'
                }
                
            }
        }
    }
</script>
