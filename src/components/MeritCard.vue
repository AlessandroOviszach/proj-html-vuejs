<template>
    <div class="container">
        <div 
        v-for="(item, index) in MeritCardList" :key="item.index"
        class="card-formatter"
        >
            <div class="card-container">
                <div class="img-container">
                    <img :src="require(`@/assets/svg/${MeritCardList[index].img}.svg`)" alt="img">
                </div>
                <h3> {{MeritCardList[index].name}} </h3>
                <div class="description-container">
                    <p> {{MeritCardList[index].description}} </p>
                </div>
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
                    name : 'Online Coaching',
                    img : 'svg-0',
                    description : 'loerm ipsum is simply dummy text of the print ing and typesetting has been the industrys'
                },
                {
                    name : 'Consultation',
                    img : 'svg-1',
                    description : 'loerm ipsum is simply dummy text of the print ing and typesetting has been the industrys'
                },
                {
                    name : 'Life Programs',
                    img : 'svg-2',
                    description : 'loerm ipsum is simply dummy text of the print ing and typesetting has been the industrys'
                },
            ]
        }
    }
}

</script>

<style scoped lang='scss'>

.container {
    width: 60%;
    display: flex;
    justify-content: center;
    padding-bottom: 4rem;
    .card-formatter {
        display: flex;
        justify-content: center;
        width: calc(100% / 3);
        .card-container {
            width: 90%;
            height: 100%;
            padding: 4rem 0rem;
            text-align: center;
            box-shadow: 10px 10px 30px #ccc;
            border-radius: 0.3rem;
    
            .img-container {
                height: 4rem;
                img {
                    height: 100%;
                }
            }
            h3 {
                font-weight: 500;
                font-size: 1.2rem;
                text-transform: capitalize;
                padding: 1.5rem;
            }
            .description-container {
                width: 80%;
                margin: auto;
            }
        }
    }
}
</style>