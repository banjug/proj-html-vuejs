<template>
    <section>
        <span>STIMULATED TO LEARN?</span>
        <h2>Featured Online Courses</h2>
        <div class="course-container">
            <CourseCard
            v-for="course, i in courses"
            :key="i"
            :course="course"
            />
        </div>
        <button>View all courses <i class="fas fa-arrow-right"></i></button>
    </section>
</template>

<script>
import CourseCard from '@/components/CourseCard.vue'
export default {
    name: 'FeaturedCourses',
    components: {
        CourseCard
    },
    data() {
        return {
            courses: [
                {
                    title: 'Learning to Write as a Professional Author',
                    lessons: 20,
                    students: 50,
                    price: '$40.00',
                    img: 'course-02-480x298.jpg'
                },
                {
                    title: 'Customer-Centric Info-Tech Strategies',
                    lessons: 24,
                    students: 769,
                    price: 'Free',
                    img: 'stock-full-hd-03-480x298.jpg'
                },
                {
                    title: 'Open Programming Courses for Everyone: Python',
                    lessons: 17,
                    students: 62,
                    price: '$19.00',
                    img: 'stock-full-hd-04-480x298.jpg'
                },
                {
                    title: 'Academic Listening and Note-Taking',
                    lessons: 14,
                    students: 67,
                    price: '$26.00',
                    img: 'stock-full-hd-06-480x298.jpg'
                },
                {
                    title: 'Master jQuery in a Short Period of Time',
                    lessons: 6,
                    students: 51,
                    price: '$39.00',
                    img: 'course-featured-image-01-480x298.jpg'
                },
                {
                    title: 'Instroduction to JavaScript for Beginners',
                    lessons: 14,
                    students: 76,
                    price: '$59.00',
                    img: 'stock-full-hd-05-480x298.jpg'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

section {
    background: #f5f7fa;
    margin: 50px 0;
    text-align: center;
    .course-container {
        width: 65%;
        margin: 50px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;        
    }
}

</style>