<template>
    <section>
        <span>GRAT WORDS ABOUT MAXCOACH</span>
        <h2>Our <span>top learners'</span> verbatim</h2>
        <div class="card-container">
            <div class="card side">
                <h3>High level of efficiency and scientific teaching methods</h3>
                <p>I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.</p>
                <div>
                    <img src="../assets/images/testimonial-avata-02.jpg" alt="">
                    <div>
                        <h4>MINA HOLLACE</h4>
                        <span>/ Freelancer</span>
                    </div>
                </div>
            </div>
            <div class="card">
                <h3>High level of efficiency and scientific teaching methods</h3>
                <p>I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.</p>
                <div>
                    <img src="../assets/images/testimonial-avata-02.jpg" alt="">
                    <div>
                        <h4>MINA HOLLACE</h4>
                        <span>/ Freelancer</span>
                    </div>
                </div>
            </div>
            <div class="card side">
                <h3>High level of efficiency and scientific teaching methods</h3>
                <p>I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.</p>
                <div>
                    <img src="../assets/images/testimonial-avata-02.jpg" alt="">
                    <div>
                        <h4>MINA HOLLACE</h4>
                        <span>/ Freelancer</span>
                    </div>
                </div>
            </div>            
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
export default {
    name: 'Carousel',
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
        .card {
            width: calc((100% / 3) - 80px);
            margin: 0 40px;
            text-align: left;
            padding: 50px;
            background: #ffffff;
            border-radius: 5px;
            &.side {
                opacity: .5;
            }
            h3, h4 {
                color: #3f3a64;
            }
            p, span {
                color: #696969;
            }
            > * {
                margin-bottom: 50px;
                font-size: 1.3rem;
            }
            > div {
                display: flex;
                align-items: center;
                img {
                    border-radius: 100%;
                    max-height: 100px;
                    margin-right: 30px;
                }
            }
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