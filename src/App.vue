<template>
<div id="app">
    <Header />

    <main>
        <Main />
        <MeritCard />
    </main>

</div>
</template>

<script>
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import MeritCard from '@/components/MeritCard.vue'

export default {
    name: 'App',
    components: {
        Header,
        Main,
        MeritCard,
    }
}
</script>

<style lang="scss">
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
}

.container {
    max-width: 1170px;
    margin: auto;
}
</style>
