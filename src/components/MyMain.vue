<template>
    <main>
        <FeaturedCourses/>
        <AvailableCourses/>
        <Carousel/>
        <Insights/>
    </main>
</template>

<script>
import FeaturedCourses from '@/components/FeaturedCourses.vue'
import AvailableCourses from '@/components/AvailableCourses.vue'
import Carousel from '@/components/Carousel.vue'
import Insights from '@/components/Insights.vue'

export default {
    name: 'MyMain',
    components: {
        FeaturedCourses,
        AvailableCourses,
        Carousel,
        Insights,
    }
}
</script>

<style lang="scss" scoped>

</style>