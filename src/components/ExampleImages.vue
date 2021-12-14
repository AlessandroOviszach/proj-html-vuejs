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
                    img : 'sdfgs',
                }
            ]
        }
    }
}
</script>

<style scoped lang='scss'>
div {
    .img-container {
        width: calc(100% / 4);

        img {
            width: 100%;
        }
    }
}
</style>