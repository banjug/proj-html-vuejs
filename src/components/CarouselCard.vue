<template>
    <div class="card">
        <h3>{{review.title}}</h3>
        <p>{{review.text}}</p>
        <div>
            <img :src="require('../assets/images/' + review.img)" alt="">
            <div>
                <h4>{{review.name.toUpperCase()}}</h4>
                <span>/ {{review.job}}</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CarouselCard',
    props: {
        review: Object
    }
}
</script>

<style lang="scss" scoped>
    .card {
        width: calc((100% / 3) - 80px);
        margin: 0 40px;
        text-align: left;
        padding: 50px;
        background: #ffffff;
        border-radius: 5px;
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
</style>