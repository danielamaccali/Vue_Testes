<template>
    <div>
        <p v-if="estou_trabalhando">Estou dormindo no momento.</p>
        <p>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>CSS</li>
            <li>Vue</li>
        </ul> 
    </div>
</template>

<script>
    export default {
        name: 'Info',
        data() {
            return {
                estou_trabalhando: true
            }
        }
    }
</script>
