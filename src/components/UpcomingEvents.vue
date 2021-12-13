<template>
    <div>
        <div class="video-container">
            <img src="../assets/img/video-bg-3.jpg" alt="">

            <div class="play-button">
                <i class="fas fa-play"></i>
            </div>
        </div>

        <div class="card-container">
            <div class="text-content">
                <div class="title-container">
                    <h3>Upcoming Events</h3>
                </div>
                <div class="description">
                    <div class="offer">
                        <h4>Princeton offers admission information sessions and student-led tours to capus visitors</h4>
                        <a href="#">Learn more<span> > </span></a>
                    </div>
                    <div class="offer">
                        <h4>Admission information sessions and student-led tours to compus visitors</h4>
                        <a href="#">Learn more<span> > </span></a>
                    </div>

                </div>
                    <div class="explore-locations">
                        <i class="far fa-map"></i>
                        <a href="#">Event Locations</a>
                        <span> > </span>
                    </div>
            </div>

            <div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'UpcomingEvents'
}
</script>

<style scoped lang='scss'>

div {
    position: relative;
    .video-container {
        position: relative;
        display: flex;
        width: 55%;
        img {
            width: 100%;
            height: 100%;
        };
        .play-button {
            display: flex;
            align-items: center;
            justify-content: center;
            position: absolute;
            padding: 1.5rem;
            top: 46%;
            left: 46%;
            border-radius: 50%;
            background-color: #fff;
            i {
                font-size: 3rem;
                color: #d74d52;
                &:hover {
                    color: #d74d5240;
                }
            }
        }

    }

    .card-container {
        position: absolute;
        top: 4rem;
        right: 0;
        width: 55%;
        background-color: #fff;
        box-shadow: 10px 10px 30px #ccc;
        .text-content {
            .title-container {
                width: 45%;
                margin: auto;
                padding-bottom: 4rem;
                h3 {
                    font-size: 1.5rem;
                    font-weight: 400;
                    color: #fff;
                    padding: 2rem;
                    text-align: center;
                    background-color: #d74d52;
                }
            }
            .description {
                padding: 0 7.5rem 0 2.5rem;
                .offer {
                    padding-bottom: .8rem;
                    h4 {
                        font-size: 1.2rem;
                        line-height: 2;
                        padding-bottom: 1.5rem;
                        
                    }
                }
            }
            .explore-locations {
                padding: 4rem 0 6rem 0;
                display: flex;
                align-items: center;
                justify-content: center;
                a {
                    padding: 0 .5rem;
                }
            }
        }
    }
}

a {
    text-decoration: none;
    color: black;
    font-weight: bold;
    span {
        font-weight: 400;
    }
}
</style>