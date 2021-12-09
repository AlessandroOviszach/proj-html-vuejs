<template>
    <div class="jumbotron">
        <header>
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
    background-image: url('../assets/img/course-1-2.jpg');
    background-position: center;

    header {
        display: flex;
        justify-content: flex-end;

        height: 4.5rem;
        background-color: #ffffff;

        .menu-positioner {
            height: 100%;
            margin-right: 25rem;

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

                    }
                }
            }
        }
    }
}
</style>
