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
                    <a href="#">Course by : {{parameter.credits}} </a>
                </div>
            </div>
        </div>

        <div class="opinion">
            <div>
                <i class="fas fa-quote-right"></i>
            </div>
            <h1>
                "Academics was committed to my success from the moment I attended an Open House. with the support of caring
                <span class="red"> advisor, professors, and staff </span>
                i was able to thrive in courses, gain recognition throught scholarships, and finish
                <span class="bold"> with confidance in my </span>
                <span class="red">@academics </span>
                <span class="bold">abilities.</span>
                "
            </h1>
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
                {
                    img : 'bruce-mars-FWVMhUa_wbY-unsplash',
                    price : 'Free',
                    name : 'UI Animation using Sketch 3, Principle App, and Flinto',
                    description : 'This online photography course will teach you how to take amazing images and even sell...',
                    credits : 'University'
                },
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
        display: flex;
        padding-bottom: 4rem;
        .courses-card {
            width: calc(100% / 3);
            border-radius: 0 0 0.3rem 0.3rem;
            margin: 1rem;
            box-shadow: 10px 10px 30px #ccc;

            .img-container {
                width: 100%;
                img {
                    height: 100%;
                    width: 100%;
                    border-radius: 0.3rem 0.3rem 0 0;
                }
            }
            .course-description {
                padding: 3rem 1.5rem;
                h4 {
                    font-weight: 400;
                }
                h2 {
                    font-size: 1.2rem;
                    padding: 1rem 0 2rem 0;
                }
                p {
                    padding-bottom: 2.5rem;
                }
            }
        }
    }

    .opinion {
        padding: 7rem 0;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        div {
            display: flex;
            align-items: center;
            justify-content: center;
            position: absolute;
            width: 100%;
            height: 100%;
            i {
                font-size: 20rem;
                color: rgba(200, 200, 200, 0.5);
            }
        }
        h1 {
            text-align: center;
            position: absolute;
            font-weight: 400;
        }
    }
}


// styles
.red {
    font-weight: bold;
    color: red;
    text-decoration: underline;
}

.bold {
    font-weight: bold;
}

</style>