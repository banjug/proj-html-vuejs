<template>
    <section>
        <span>MAXCOACH AVAILABLE COURSES</span>
        <h2>Access <span>Smart Tutoring</span> Program For Benefits.</h2>
        <div class="benefit-cont">
            <BenefitCard
            v-for="card, i in benefitCards"
            :key="i"
            :card="card"
            />
        </div>
        <div class="get-started">
            <div class="started-vid">
                    <a href="https://www.youtube.com/" target="_blank" >
                        <div class="thumb-wrapper">
                            <div class="vid-thumbnail"></div>
                        </div>
                        <img src="../assets/images/icon-youtube-play.png" alt="" class="yt-btn">
                    </a>
                    <img class="vid-shape vid-shape-1" src="../assets/images/maxcoach-shape-05.png" alt="">
                    <img class="vid-shape vid-shape-2" src="../assets/images/maxcoach-shape-07.png" alt="">
                    <div class="vid-shape vid-circle"></div>
                    <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg" class="vid-shape vid-blob">
                            <path fill="#ECC5AB" d="M43.6,-65.5C57.9,-58.6,72,-48.9,71.9,-36.5C71.8,-24.1,57.6,-8.9,49.6,3.1C41.6,15.2,40,24.2,37.3,38.7C34.7,53.2,31,73.3,23.2,72.6C15.4,72,3.4,50.6,-13.7,45.9C-30.8,41.2,-53.1,53.2,-63.1,50C-73.2,46.8,-71,28.4,-72.5,11.1C-74,-6.2,-79.1,-22.3,-72.4,-31.5C-65.8,-40.7,-47.5,-43.1,-33.5,-50.1C-19.4,-57.2,-9.7,-68.9,2.4,-72.7C14.6,-76.6,29.2,-72.4,43.6,-65.5Z" transform="translate(100 100)" />
                    </svg>
            </div>
            <div class="started-info">
                <span>GET STARTED <span>EFFORTLESSLY</span></span>
                <h2>Enjoy Our <span>Companionship</span></h2>
                <p>Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird rewards as well.</p>
                <a href="">Download free guidebook <i class="fas fa-arrow-right"></i></a>
            </div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none" class="divider-shape">
            <path d="M 50 0 S75 0 100 100 L100 0"></path>
        </svg>
    </section>
</template>

<script>
import BenefitCard from '@/components/BenefitCard.vue'
export default {
    name: 'CourseBenefits',
    components: {
        BenefitCard,
    },
    data() {
        return {
            benefitCards: [
                {
                    title: 'Customize Preferences',
                    text: 'Learners are given the right to arrange and customize their study schedule and timetable based on preferences.',
                    linkText: 'Start Here',
                    img: 'home-2-image-box-01.png'
                },
                {
                    title: 'Cloud Storage',
                    text: 'You can store online lessons via online cloud or download to your device and revise lessons on the way.',
                    linkText: 'Get Free Quote',
                    img: 'about-us-02-image-box-02.png'
                },
                {
                    title: 'Multimedia Channels',
                    text: 'We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.',
                    linkText: 'Start Now',
                    img: 'home-2-image-box-03.png'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        text-align: center;
        margin: 100px auto 0;
        padding-bottom: 100px;
        position: relative;
        >span {
            color: #918ea6;
            font-size: 1.3rem;
        }
        >h2{
            color: #3f3a64;
            font-size: 3rem;
            >span {
                color: #8c89a2;
                font-weight: 400;
            }
        }
        .benefit-cont {
            display: flex;
            justify-content: space-between;
            width: 65%;
            margin: 100px auto;
        }
        .get-started {
            width: 65%;
            margin: 0 auto;
            padding: 100px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            .started-vid {
                position: relative;
                .thumb-wrapper {
                    width: 670px;
                    height: 450px;
                    overflow: hidden;
                    .vid-thumbnail {
                        background-image: url('../assets/images/home-2-popup-video-poster.jpg');
                        width: 100%;
                        height: 100%;
                        border-radius: 5px;
                        background-size: cover;
                        z-index: 1;
                            transition: all .2s ease;
                        &:hover {
                            transform: scale(1.1);
                        }
                    }
                }
                .yt-btn {
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    z-index: 2;
                    cursor: pointer;
                }                
                .vid-shape {
                position: absolute;
                }
                .vid-shape-1 {
                    top: 15%;
                    left: 0;
                    transform: translate(-50%);
                }
                .vid-shape-2 {
                    bottom: 0;
                    right: 0;
                    transform: translate(30%, 50%);
                }
                .vid-circle {
                    border: 10px solid #ecc5ab;
                    border-radius: 100%;
                    height: 70px;
                    width: 70px;
                    top: 0;
                    right: 0;
                    transform: translate(120%, -50%);
                }
                .vid-blob {
                    height: 200px;
                    top: 0;
                    left: 0;
                    transform: translate(-50%, -50%);
                }
            }
            .started-info {
                text-align: left;
                padding: 0 80px;
                >span {
                    display: block;
                    color: #918ea6;
                    font-size: 1.2rem;
                    >span {
                        display: inline;
                        color: #3f3a64;
                    }
                }
                h2 {
                    color: #3f3a64;
                    font-size: 3rem;
                    >span {
                        color: #8c89a2;
                        font-weight: 400;
                    }
                }
                p {
                    color: #696969;

                }
                a {
                    font-weight: 700;
                    color: #8c89a2;
                    text-decoration-color: transparent;
                    &:hover {
                        transition: all .4s ease;
                        text-decoration-color: #8c89a2;
                    }
                }
                > * {
                    margin-bottom: 30px;
                }
            }
        }
        .divider-shape {
            position: absolute;
            height: 600px;
            right: 0;
            bottom: 0;
            transform:rotate(90deg);
            fill: #f8f8f8;
        }
    }
</style>