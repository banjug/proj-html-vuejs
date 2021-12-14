<template>
    <div class="benefit-card">
        <img :src="require('../assets/images/' + card.img)" alt="">
        <h3>{{card.title}}</h3>
        <p>{{card.text}}</p>
        <a href="">{{card.linkText}} <i class="fas fa-arrow-right"></i></a>
    </div>
</template>

<script>
export default {
    name: 'BenefitCard',
    props: {
        card: Object
    }
}
</script>

<style lang="scss" scoped>
    .benefit-card {
        padding: 0 50px 0 0;
        text-align: left;
        > * {
            margin-bottom: 10px;
        }
        &:last-child {
            padding: 0;
        }
        h3 {
            color: #3f3a64;
            font-size: 1.3rem;
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
    }
</style>