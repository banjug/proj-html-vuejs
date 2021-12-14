<template>
    <main>
        <FeaturedCourses/>
        <CourseBenefits/>
        <Carousel/>
        <Insights/>
    </main>
</template>

<script>
import FeaturedCourses from '@/components/FeaturedCourses.vue'
import CourseBenefits from '@/components/CourseBenefits.vue'
import Carousel from '@/components/Carousel.vue'
import Insights from '@/components/Insights.vue'

export default {
    name: 'MyMain',
    components: {
        FeaturedCourses,
        CourseBenefits,
        Carousel,
        Insights,
    }
}
</script>

<style lang="scss" scoped>

</style>