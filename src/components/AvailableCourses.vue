<template>
    <section>
        <span>MAXCOACH AVAILABLE COURSES</span>
        <h2>Access Smart Tutoring Program For Benefits.</h2>
        <div class="benefit-cont">
            <div class="benefit-card">
                <img src="../assets/images/home-2-image-box-01.png" alt="">
                <h3>Customize Preferences</h3>
                <p>Learners are given the right to arrange and customize their study schedule and timetable based on preferences.</p>
                <a href="">Start Here <i class="fas fa-arrow-right"></i></a>
            </div>
            <div class="benefit-card">
                <img src="../assets/images/about-us-02-image-box-02.png" alt="">
                <h3>Cloud Storage</h3>
                <p>You can store online lessons via online cloud or download to your device and revise lessons on the way.</p>
                <a href="">Start Here <i class="fas fa-arrow-right"></i></a>
            </div>
            <div class="benefit-card">
                <img src="../assets/images/home-2-image-box-03.png" alt="">
                <h3>Multimedia Channels</h3>
                <p>We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.</p>
                <a href="">Start Here <i class="fas fa-arrow-right"></i></a>
            </div>
        </div>
        <div class="get-started">
            <div class="started-img">
            <img src="../assets/images/home-2-popup-video-poster.jpg" alt="">
            <img src="../assets/images/icon-youtube-play.png" alt="">
            </div>
            <div class="started-info">
                <span>GET STARTED EFFORTLESSLY</span>
                <h2>Enjoy Our Companionship</h2>
                <p>Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird rewards as well.</p>
                <a href="">Download free guidebook <i class="fas fa-arrow-right"></i></a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AvailableCourses',
}
</script>

<style lang="scss" scoped>
    section {
        text-align: center;
        margin: 100px auto;
        .benefit-cont {
            display: flex;
            justify-content: space-between;
            width: 65%;
            margin: 100px auto;
            .benefit-card {
                padding: 0 50px 0 0;
                text-align: left;
                > * {
                    margin-bottom: 10px;
                }
                &:last-child {
                    padding: 0;
                }
            }
        }
        .get-started {
            width: 65%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            .started-img {
                position: relative;
                img:first-child {
                    border-radius: 5px;
                }
                img:last-child {
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                }
            }
            .started-info {
                text-align: left;
                padding: 0 80px;
                span {
                    display: block;
                }
                > * {
                    margin-bottom: 30px;
                }
            }
        }
    }
</style>