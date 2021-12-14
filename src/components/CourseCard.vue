<template>
    <div class="course-card">
                <img :src="require('../assets/images/' + course.img)" alt="">
                <div class="card-data">
                    <h3>{{course.price}}</h3>
                    <h4>{{course.title}}</h4>
                    <span><i class="far fa-file-alt"></i> {{course.lessons}} Lessons</span>
                    <span><i class="far fa-user"></i> {{course.students}} Students</span>
                </div>
            </div>
</template>

<script>
export default {
    name: 'CourseCard',
    props: {
        course: Object
    }
}
</script>

<style lang="scss" scoped>
.course-card {
            margin: 30px 0;
            height: 200px;
            width: 50%;
            display: flex;
            align-items: center;
            img {
                height: 90%;
                aspect-ratio: 1;
                object-fit: cover;
                border-radius: 100%;
            }
            .card-data {
                padding-left: 50px;
                text-align: left;
                > * {
                    margin-bottom: 30px;
                }
                span {
                    margin-right: 20px;
                }
            }
        }
</style>