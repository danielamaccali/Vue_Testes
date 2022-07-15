<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Sobre</a></li>
        <li><a href="#">Contato</a></li>
    </ul>
</template>

<script>
export default {
    name: 'Header'
    
}
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        background: #cc7f0c;
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: #7e3959;
    }

</style>
