<template>
    <div class="container">
        <div class="opening-sentence">
            <h1>Recent Courses</h1>
            <p class="section-description">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo tenetur incidunt, laboriosam vero voluptas ipsum dignissimos similique sunt, totam animi vitae quidem.
            </p>
        </div>

        <div class="card-container">
            <div v-for="(parameter, index) in CoursesList" :key="index" class="courses-card">
                <div class="img-container">
                    <img :src="require(`@/assets/img/${parameter.img}.jpg`)" alt="img">
                </div>
                <div class="course-description">
                    <h4> {{parameter.price}} </h4>
                    <h2> {{parameter.name}} </h2>
                    <p> {{parameter.description}} </p>
                    <a href="#"></a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'RecentCourses',
    data() {
        return {
            CoursesList : [
                {
                    img : 'bruce-mars-FWVMhUa_wbY-unsplash',
                    price : 'Free',
                    name : 'UI Animation using Sketch 3, Principle App, and Flinto',
                    description : 'This online photography course will teach you how to take amazing images and even sell...',
                    credits : 'University'
                },
            ]
        }
    }
}
</script>

<style scoped lang='scss'>

.container {
    padding-top: 3rem;
    background-color: #ffffff7a;
    .opening-sentence {
        text-align: center;
        width: 70%;
        margin: auto;
        p {
            padding: 2rem 0;
        }
    }

    .card-container {
        .courses-card {
            width: calc(100% / 3);
            display: flex;
            flex-direction: column;

            .img-container {
                width: 100%;
                img {
                    height: 100%;
                    width: 100%;
                }
            }
        }
    }
}
</style>