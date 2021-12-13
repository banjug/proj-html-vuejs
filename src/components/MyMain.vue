<template>
    <main>
        <FeaturedCourses/>
        <AvailableCourses/>
    </main>
</template>

<script>
import FeaturedCourses from '@/components/FeaturedCourses.vue'
import AvailableCourses from '@/components/AvailableCourses.vue'

export default {
    name: 'MyMain',
    components: {
        FeaturedCourses,
        AvailableCourses,
    }
}
</script>

<style lang="scss" scoped>

</style>