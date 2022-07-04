<template>
    <h1>Meu nome é: {{ nome }} </h1>
</template>

<script>
    export default {
        name: 'LyfeCycle',
        data(){
            return{
                nome: 'Ainda não sei'
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Daniela'
            }, 1000)
            
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Luci'
            }, 2000)
            
        }
    }
</script>