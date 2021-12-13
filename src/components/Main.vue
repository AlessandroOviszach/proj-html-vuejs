<template>
    <div class="container">
        <div class="catchphrase">
            <h1>
                Since 2000, weve been partnering with aducation leaders to
                <span>
                    increase equity and achievement
                </span>
                for all students.
            </h1>
        </div>

        <MeritCard />
        <Statistics />
        <RecentCourses />
        <UpcomingEvents />
    </div>
</template>

<script>
import MeritCard from '@/components/MeritCard.vue'
import Statistics from '@/components/Statistics.vue'
import RecentCourses from '@/components/RecentCourses.vue'
import UpcomingEvents from '@/components/UpcomingEvents.vue'

export default {
    name: 'Main',
    components: {
        MeritCard,
        Statistics,
        RecentCourses,
        UpcomingEvents,
    }
}
</script>

<style scoped lang='scss'>

.container{
    color: #192836;
    .catchphrase {
        width: 80%;
        margin: auto;
        text-align: center;
        padding: 4rem 0;
        span {
            color: #d74d52;
        }
    }

}
</style>