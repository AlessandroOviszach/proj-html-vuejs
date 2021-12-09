<template>
    <Header />
</template>

<script>
import Header from './components/Header.vue'

export default {
    name: 'App',
    components: {
        Header,
    }
}
</script>

<style lang="scss">
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: sans-serif;
}

.container {
    max-width: 80vw;
    margin: auto;
}

</style>
