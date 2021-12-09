<template>
    <div class="jumbotron">
        <header>
            <img class="logo" src="../assets/img/Logo.jpg" alt="PICWIK">

            <div class="menu-positioner">
                <div class="menu-container">
                    <ul class="menu">
                        <li>Home</li>
                        <li>About</li>
                        <li>Academics</li>
                        <li>Courses</li>
                        <li>News</li>
                    </ul>
                </div>
            </div>
        </header>
        <div class="jumbo-content container">
            <h1>professional development for <br> coaches and leaders</h1>

            <a href="#">Learn more</a>
        </div>
    </div>

</template>

<script>
export default {
  name: 'Header',

//   props: {
//   },
}
</script>


<style scoped lang="scss">
.jumbotron {
    height: 100vh;
    background-image: url('../assets/img/jumbo-bg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;

    header {
        display: flex;
        justify-content: space-around;
        height: 5rem;
        background-color: #ffffff;

        .logo {
            height: 7.5rem;
        }

        .menu-positioner {
            height: 100%;

            .menu-container {
                height: 100%;
                display: flex;
                align-items: center;

                .menu {
                    display: flex;
                    list-style: none;
                    li {
                        padding-right: 2rem;
                        font-weight: bold;
                        text-transform: capitalize;
                    }
                }
            }
        }
    }

    .jumbo-content {
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4.5rem;
            text-transform: capitalize;
            text-align: center;
            padding-bottom: 2rem;
        }

        a {
            padding: 1rem 3rem;
            border: 1px solid #ccc;

            font-size: 1rem;
            text-transform: capitalize;
            text-decoration: none;
            color: #000;
        }
    }
}
</style>
