<template>
    <div id="app">
        <Title></Title>
    </div>
<!--    开发人员添加代码-->
</template>

<script>
    import Title from './components/Title.vue'
    export default {
        name: 'App',
        components: {
            Title
        }
    }
</script>

<style>
    #app {
        cursor:pointer;
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
