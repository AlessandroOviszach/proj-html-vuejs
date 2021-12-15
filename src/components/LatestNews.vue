<template>
    <div class="container">
        <div class="opening-sentence">
            <h1>Latest from our blogs</h1>
            <p class="section-description">
                Whether you're considering a foundation course or an undergraduate degree master's or a PhD, academics is a place where students thrive.
            </p>
        </div>

        <div class="card-container">
            <div v-for="(parameter, index) in CoursesList" :key="index" class="courses-card">
                <div class="img-container">
                    <img :src="require(`@/assets/img/${parameter.img}.jpg`)" alt="img">
                </div>
                <div class="course-description">
                    <div class="poperty-container">
                        <div class="poperty">
                            <i :class="`${parameter.gradeIcon}`"></i>
                            <h4> {{ parameter.grade }} </h4>
                        </div>

                        <div class="poperty">
                            <i :class="`${parameter.typeIcon}`"></i>
                            <h4> {{ parameter.type }} </h4>
                        </div>
                    </div>

                    <h2> {{ parameter.title }} </h2>

                    <div class="separator-container">
                        <hr class="separator">
                    </div>

                    <div class="cta">
                        <a href="#">Read more</a>
                        <i class="fas fa-chevron-right"></i>
                    </div>
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
                    img : 'news-3-2',

                    gradeIcon : 'far fa-user',
                    grade : 'Admin',
                    typeIcon : 'far fa-folder',
                    type : 'University',

                    title : 'Peer pressure changes how teens tackle inequality',
                },
                {
                    img : 'news-2-2',

                    gradeIcon : 'far fa-user',
                    grade : 'Admin',
                    typeIcon : 'far fa-folder',
                    type : 'University',

                    title : 'Lewisham Live Mixtape celebrates boroughs',
                    // TODO chiedere come inserire l'apostrofo
                },
                {
                    img : 'news-1-2',

                    gradeIcon : 'far fa-user',
                    grade : 'Admin',
                    typeIcon : 'far fa-folder',
                    type : 'University',

                    title : 'Turner Prize winners work to open Gold on Film festival',
                },
            ]
        }
    },
}
</script>

<style scoped lang='scss'>
.container {
    padding-top: 15rem;
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
                    width: 100%;
                    height: 200px;
                    object-fit: cover;
                    border-radius: 0.3rem 0.3rem 0 0;
                }
            }
            .course-description {
                padding: 3rem 1.5rem;
                h2 {
                    font-size: 1.2rem;
                }

                .separator-container {
                    width: 4rem;
                    padding-top: 1.5rem;
                    .separator {
                        color: #d74d52;
                    }
                }

                .cta {
                    padding-top: 3rem;
                    display: flex;
                    align-items: center;
                    a {
                        text-decoration: none;
                        color: #000;
                        padding-right: .5rem;
                    }
                }
                .poperty-container {
                    display: flex;
                    align-items: center;
                    padding-bottom: 1.5rem;
                    .poperty {
                        display: flex;
                        align-items: center;
                        padding-right: 2rem;
                        i {
                            padding-right: .5rem;
                        }
                    }
                }
            }
        }
    }
}
</style>