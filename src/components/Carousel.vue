<template>
    <section>
        <span>GRAT WORDS ABOUT MAXCOACH</span>
        <h2>Our <span>top learners'</span> verbatim</h2>
        <div class="card-container">
            <CarouselCard
            v-for="review, i in reviews"
            :key="i"
            :review="review"
            />
        </div>
        <div class="page-selector">
            <div class="dot active"></div>
            <div class="dot"></div>
            <div class="dot"></div>
            <div class="dot"></div>
        </div>
        <div class="carouserl-foot">
            <h3>Start today for getting <span>Online Certification</span></h3>
            <h2>You can be your own guiding star with our help!</h2>
            <button>Get started now</button>
            <img class="carousel-shape shape-1" src="../assets/images/maxcoach-shape-01.png" alt="">
            <img class="carousel-shape shape-2" src="../assets/images/maxcoach-shape-02.png" alt="">
            <div class="carousel-shape carousel-circle"></div>
        </div>
    </section>
</template>

<script>
import CarouselCard from '@/components/CarouselCard.vue'
export default {
    name: 'Carousel',
    components: {
        CarouselCard
    },
    data() {
        return {
            reviews:[
                {
                    name: "Florence Themes",
                    job: "Multimedia Admin",
                    title: "It's a coiche of quality for people with special needs",
                    text: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
                    img: "testimonial-avata-03.jpg"
                },
                {
                    name: "Mina Hollace",
                    job: "Freelancer",
                    title: "High level of efficiency and scientific teaching methods",
                    text: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                    img: "testimonial-avata-02.jpg"
                },
                {
                    name: "Madley Pondor",
                    job: "IT Specialist",
                    title: "Professional team of specialists and passionate mentors at reach",
                    text: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
                    img: "testimonial-avata-04.jpg"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
section {
    background: #f8f8f8;
    text-align: center;
    padding: 100px;
    >span {
        color: #8c89a2;
        font-size: 1.3rem;
    }
    h2 {
        color: #3f3a64;
        font-size: 3rem;
        >span {
            color: #8c89a2;
            font-weight: 400;
        }
    }
    h3 {
        color: #3f3a64;
        font-size: 2rem;
        >span {
            color: #8c89a2;
            font-weight: 400;
        }
    }
    .card-container {
        display: flex;
        margin: 50px 0;
        >div:first-child, >div:last-child {
            opacity: .5;
        }
    }
    .page-selector {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 50px;
        .dot{
            height: 10px;
            aspect-ratio: 1;
            border-radius: 100%;
            background: #b7b5c4;
            margin: 0 10px;
            cursor: pointer;
            &.active {
                background: #3f3a64;
                height: 15px;
            }
        }
    }
    .carouserl-foot {
        position: relative;
        .carousel-shape {
            position: absolute;
        }
        .carousel-circle {
            border: 10px solid #ecc5ab;
            border-radius: 100%;
            height: 70px;
            width: 70px;
            left: 15%;
            top: 0;
        }
        .shape-1 {
            left: 20%;
        }
        .shape-2 {
            right: 20%;
        }
        button {
            margin: 50px 0 0;
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
}
</style>