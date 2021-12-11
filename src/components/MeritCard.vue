<template>
    <div class="container">
        <div class="card-container">
            <div class="img-container">
                <img src= '../assets/svg/svg-0.svg' alt="img">
            </div>
            <h3> {{MeritCardList[0].name}} </h3>
            <div class="description-container">
                <p> {{MeritCardList[0].description}} </p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'MeritCard',

    data() {
        return {
            MeritCardList : [
                {
                    name : 'Online coaching',
                    img : '../assets/svg/svg-0.svg',
                    description : 'loerm ipsum is simply dummy text of the print ing and typesetting has been the industrys'
                }
            ]
        }
    }
}

</script>

<style scoped lang='scss'>

    .card-container {
        width: calc(100% / 3);
        height: 100%;
        padding: 2rem 4rem;
        text-align: center;

        .img-container {
            height: 4rem;
            img {
                height: 100%;
            }
        }
        h3 {
            font-weight: 500;
            font-size: 1.2rem;
            padding: 2rem;
        }
        .description-container {
            width: 80%;
            margin: auto;
        }
    }
</style>