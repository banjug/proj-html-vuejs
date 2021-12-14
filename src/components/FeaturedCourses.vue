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
                    price: 40,
                    img: 'course-02-480x298.jpg'
                },
                {
                    title: 'Customer-Centric Info-Tech Strategies',
                    lessons: 24,
                    students: 769,
                    price: 0,
                    img: 'stock-full-hd-03-480x298.jpg'
                },
                {
                    title: 'Open Programming Courses for Everyone: Python',
                    lessons: 17,
                    students: 62,
                    price: 19,
                    img: 'stock-full-hd-04-480x298.jpg'
                },
                {
                    title: 'Academic Listening and Note-Taking',
                    lessons: 14,
                    students: 67,
                    price: 26,
                    img: 'stock-full-hd-06-480x298.jpg'
                },
                {
                    title: 'Master jQuery in a Short Period of Time',
                    lessons: 6,
                    students: 51,
                    price: 39,
                    img: 'course-featured-image-01-480x298.jpg'
                },
                {
                    title: 'Instroduction to JavaScript for Beginners',
                    lessons: 14,
                    students: 76,
                    price: 59,
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
    padding: 100px 0;
    text-align: center;
    > span {
        color: #8c89a2;
        font-size: 1.3rem;
    }
    > h2 {
        color: #3f3a64;
        font-size: 3rem;
    }
    .course-container {
        width: 65%;
        margin: 50px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;        
    }
    button {
            margin-bottom: 35px;
            padding: 20px 40px;
            border: none;
            border-radius: 5px;
            background: #20ad96;
            color: #ffffff;
            font-weight: 500;
            font-size: 1rem;
            cursor: pointer;
            transition: all .2s ease;
            &:hover {
                background: #3f3a64;
            }
        }
}

</style>