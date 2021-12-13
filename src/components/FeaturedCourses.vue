<template>
    <section>
        <span>STIMULATED TO LEARN?</span>
        <h2>Featured Online Courses</h2>
        <div class="course-container">
            <div class="course-card">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="card-data">
                    <h3>$40.00</h3>
                    <h4>Learning to Write as a Professional Author</h4>
                    <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                    <span><i class="far fa-user"></i> 50 Students</span>
                </div>
            </div>
            <div class="course-card">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="card-data">
                    <h3>$40.00</h3>
                    <h4>Learning to Write as a Professional Author</h4>
                    <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                    <span><i class="far fa-user"></i> 50 Students</span>
                </div>
            </div>
            <div class="course-card">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="card-data">
                    <h3>$40.00</h3>
                    <h4>Learning to Write as a Professional Author</h4>
                    <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                    <span><i class="far fa-user"></i> 50 Students</span>
                </div>
            </div>
            <div class="course-card">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="card-data">
                    <h3>$40.00</h3>
                    <h4>Learning to Write as a Professional Author</h4>
                    <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                    <span><i class="far fa-user"></i> 50 Students</span>
                </div>
            </div>
            <div class="course-card">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="card-data">
                    <h3>$40.00</h3>
                    <h4>Learning to Write as a Professional Author</h4>
                    <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                    <span><i class="far fa-user"></i> 50 Students</span>
                </div>
            </div>
            <div class="course-card">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="card-data">
                    <h3>$40.00</h3>
                    <h4>Learning to Write as a Professional Author</h4>
                    <span><i class="far fa-file-alt"></i> 20 Lessons</span>
                    <span><i class="far fa-user"></i> 50 Students</span>
                </div>
            </div>
            
            
        </div>
        <button>View all courses <i class="fas fa-arrow-right"></i></button>
    </section>
</template>

<script>
export default {
    name: 'FeaturedCourses',
}
</script>

<style lang="scss" scoped>

section {
    margin: 50px 0;
    text-align: center;
    .course-container {
        width: 65%;
        margin: 50px auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
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
    }
}

</style>