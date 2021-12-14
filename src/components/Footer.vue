<template>
<div>
    <ExampleImages />


    <div class="footer-container">
        <div class="container">
        <NewsLetterForm />

        </div>
    </div>
</div>
    
</template>

<script>
import ExampleImages from '@/components/ExampleImages.vue'
import NewsLetterForm from '@/components/NewsLetterForm.vue'


export default {
    name : 'Footer',
    components : {
        ExampleImages,
        NewsLetterForm,
    }
}
</script>

<style scoped lang='scss'>

div {
    .footer-container {
        height: 800px;
        background-color: #192735;
    }
}
</style>