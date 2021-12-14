<template>
    <div>
        <div class="footer-1"></div>
        <div class="footer-2"></div>
        <div class="footer-3"></div>
        <div class="footer-4"></div>


        <!-- <img src="../assets/img/footer-img-1.jpg" alt="footer-img-1">
        <img src="../assets/img/footer-img-2.jpg" alt="footer-img-2">
        <img src="../assets/img/footer-img-3.jpg" alt="footer-img-3">
        <img src="../assets/img/footer-img-4.jpg" alt="footer-img-4"> -->
    </div>
</template>

<script>
export default {
    name : 'ExampleImages',
}
</script>

<style scoped lang='scss'>
div {
    display: flex;
    width: 100%;
    div {
        width: 100%;
        height: 400px;
    }

    .footer-1,
    .footer-2,
    .footer-3,
    .footer-4 {
        background-position: center;
        background-size: cover;
    }
    .footer-1 {
        background-image: url('../assets/img/footer-img-1.jpg');
    }
    .footer-2 {
        background-image: url('../assets/img/footer-img-2.jpg');
    }
    .footer-3 {
        background-image: url('../assets/img/footer-img-3.jpg');
    }
    .footer-4 {
        background-image: url('../assets/img/footer-img-4.jpg');
    }
}
</style>