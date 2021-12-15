<template>
    <footer>
        <section class="newsletter">
            <h2>
                Subscribe <span>Newsletters</span>
            </h2>
            <span>Enter your email addres to register to our newsletter subscription delivered on a regular basis!</span>
            <input type="text" placeholder="Enter your email">
            <button>Subscribe</button>
            <img class="footer-shape shape-1" src="../assets/images/maxcoach-shape-02.png" alt="">
            <img class="footer-shape shape-2" src="../assets/images/maxcoach-shape-09.png" alt="">
            <div class="footer-shape footer-circle"></div>
        </section>
        <nav>
            <div class="wrapper-nav">
                <div class="wrapper-left">
                    <ul>
                        <li><strong>Address</strong></li>
                        <li>382 NE 191st St # 87394 Miami, FL 33179-3899</li>
                        <li>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</li>
                        <li>support@maxcoach.com</li>
                    </ul>
                        <i class="fab fa-facebook-square"></i>
                        <i class="fab fa-twitter"></i>
                        <i class="fab fa-instagram"></i>
                        <i class="fab fa-linkedin"></i>
                </div>
                <div class="wrapper-right">
                    <ul>
                        <li><strong>Explore</strong></li>
                        <li v-for="link, i in exploreLinks" :key="i"><a :href=link.url>{{link.name}}</a></li>
                    </ul>
                    <ul>
                        <li><strong>Information</strong></li>
                        <li v-for="link, i in informationLinks" :key="i"><a :href=link.url>{{link.name}}</a></li>
                    </ul>
                </div>
            </div>
            <div class="rights">
                © 2021 Samuele Miotto. All Rights Reserved.
            </div>
        </nav>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter',
    props: {
        exploreLinks: Array,
        informationLinks: Array
    }
}
</script>

<style lang="scss" scoped>
    footer {
        .newsletter {
            margin: 100px auto;
            text-align: center;
            position: relative;
            * {
                margin-bottom: 30px;
            }
            h2 {
                font-size: 2rem;
                color: #3f3a64;
                span {
                    color: #20ad96;
                    font-weight: 400;
                }
            }
            >span {
                display: block;
                color: #696969;
                width: 25%;
                margin-left: auto;
                margin-right: auto;
            }
            input {
                padding: 20px;
                width: 20%;
                background: #f5f5f5;
                border: none;
                font-size: 1rem;
                border-top-left-radius: 5px;
                border-bottom-left-radius: 5px;
            }
            button {
                margin: 50px 0 0;
                padding: 20px 40px;
                border: none;
                // border-radius: 5px;
                border-top-right-radius: 5px;
                border-bottom-right-radius: 5px;
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
            .footer-shape {
                position: absolute;
            }
            .footer-circle {
                border: 10px solid #ecc5ab;
                border-radius: 100%;
                height: 70px;
                width: 70px;
                left: 15%;
                top: 50%;
            }
            .shape-1 {
                right: 20%;
            }
            .shape-2 {
                right: 20%;
                top: -10%;
            }
        }
        nav {
            background: #f8f8f8;
            padding: 100px 0;
            .wrapper-nav {
                width: 65%;
                margin: 100px auto;
                display: flex;
                justify-content: space-between;
                
                ul {
                    list-style: none;
                }
                strong {
                    font-size: 1.2rem;
                }
                .wrapper-left {
                    * {
                        margin-bottom: 20px;
                    }
                    i {
                        margin-right: 40px;
                        font-size: 1.5rem;
                    }
                }
                .wrapper-right {
                    display: flex;
                    align-items: flex-end;
                    ul {
                        margin-left: 50px;
                        li {
                            margin-bottom: 20px;
                        }
                    }
                }
            }
        }
        .rights {
            text-align: center;
        }
    }
</style>