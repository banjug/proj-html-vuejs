<template>
    <section>
        <span>GRAT WORDS ABOUT MAXCOACH</span>
        <h2>Our top learners' verbatim</h2>
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
    </section>
</template>

<script>
export default {
    name: 'Carousel',
}
</script>

<style lang="scss" scoped>
section {
    background: #f5f7fa;
    text-align: center;
    .card-container {
        display: flex;
        margin: 50px 0;
        .card {
            width: calc((100% / 3) - 80px);
            margin: 0 40px;
            text-align: left;
            padding: 50px;
            &.side {
                opacity: .5;
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
}
</style>