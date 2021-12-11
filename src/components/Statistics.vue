<template>
    <div class="container">
        <div v-for="(parameter, index) in ParamList" :key="index" class="statistic-container">
            <div class="statistic">
                <div class="img-container">
                    <img :src="require(`@/assets/img/${parameter.img}.png`)" alt="img">
                </div>
                <h1 :class="parameter.color">
                    {{parameter.average}} 
                    <span>{{parameter.text}}</span>
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
                    color : 'orange',
                },
                {
                    img : 'counter-shape-2-1-1',
                    average : '200 +',
                    text : 'Online Courses',
                    color : 'red',
                },
                {
                    img : 'counter-shape-3-1-1',
                    average : '100 %',
                    text : 'Happy Client',
                    color : 'green',
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
                font-size: 2.5rem;
                font-weight: 700;
                display: flex;
                align-items: center;
                position: absolute;
                // color: red;
                
                span {
                    color: #192836;
                    font-size: 1.5rem;
                    font-weight: 500;
                    padding-left: 1rem;
                }
            }
        }
    }
}

// colors
.orange {
    color: #f28202;
}
.red {
    color: #d74d52;
}
.green {
    color: #3adc79;
}
</style>