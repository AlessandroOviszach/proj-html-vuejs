<template>
    <div class="container">
        <div v-for="(item, index) in ParamList" :key="item.index" class="statistic-container">
            <div class="statistic">
                <div class="img-container">
                    <img :src="require(`@/assets/img/${ParamList[index].img}.png`)" alt="img">
                </div>
                <h1>
                    {{ParamList[index].average}} 
                    <span>{{ParamList[index].text}}</span>
                </h1>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'Statistics',

    data() {
        return {
            ParamList : [
                {
                    img : 'counter-shape-1-1-1',
                    average : '6500 +',
                    text : 'Students',
                },
                {
                    img : 'counter-shape-2-1-1',
                    average : '200 +',
                    text : 'Online Courses',
                },
                {
                    img : 'counter-shape-3-1-1',
                    average : '100 %',
                    text : 'Happy Client',
                },
            ]
        }
    }
}
</script>

<style scoped lang='scss'>

.container {
    display: flex;
    align-items: center;
    .statistic-container {
        width: 100%;
        display: flex;
        padding-left: 3rem;
        
        .statistic {
            display: flex;
            align-items: center;
            .img-container {
                position: relative;
            }
    
            h1 {
                display: flex;
                align-items: center;
                position: absolute;
                span {
                    font-size: 1.5rem;
                    font-weight: 500;
                    padding-left: 1rem;
                }
            }
        }
    }
}
</style>