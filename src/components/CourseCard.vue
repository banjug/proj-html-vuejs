<template>
    <div class="course-card">
                <img :src="require('../assets/images/' + course.img)" alt="">
                <div class="card-data">
                    <h3 v-if="course.price !== 0">${{course.price}}<span>.00</span></h3>
                    <h3 v-else>Free</h3>
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
            padding: 30px;
            height: 200px;
            width: 50%;
            display: flex;
            align-items: center;
            transition: all .3s ease;
            border-radius: 5px;
            img {
                height: 100%;
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
                h3 {
                    color: #20ad96;
                    font-size: 2rem;
                    > span {
                        font-size: 1.6rem;
                    }
                }
                h4 {
                    color: #3f3a64;
                }
                > span {
                    margin-right: 20px;
                    color: #a09eb2;
                }
            }
            &:hover {
                box-shadow: 0px 0px 15px 0px rgba(0,0,0,0.1);
                cursor: pointer;
                transform: scale(1.02);
            }
        }
</style>