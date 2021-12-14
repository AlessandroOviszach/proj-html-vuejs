<template>
    <div>
        <div v-for="(parameter, index) in ImageList" :key="index">
            <div class="img-container">
                <img :src="require(`@/assets/img/${parameter.img}.jpg`)" alt="img">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'ExampleImages',
    data() {
        return {
            ImageList : [
                {
                    img : 'footer-img-1',
                },
                {
                    img : 'footer-img-2',
                },
                {
                    img : 'footer-img-3',
                },
                {
                    img : 'footer-img-4',
                },
            ]
        }
    }
}
</script>

<style scoped lang='scss'>
div {
    display: flex;
    max-width: 100vw;
    // align-items: center;
    .img-container {
        width: 100%;
        img {
            width: 24.7vw;
            object-fit: fill;
        }
    }
}
</style>