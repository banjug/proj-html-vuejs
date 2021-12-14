<template>
    <footer>
        <section class="newsletter">
            <h2>
                Subscribe Newsletters
            </h2>
            <span>Enter your email addres to register to our newsletter subscription delivered on a regular basis!</span>
            <input type="text" placeholder="Enter your email">
            <button>Subscribe</button>
        </section>
        <nav>
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
                    <li>Start Here</li>
                    <li>Blog</li>
                    <li>About Us</li>
                </ul>
                <ul>
                    <li></li>
                    <li>Start Here</li>
                    <li>Blog</li>
                    <li>About Us</li>
                </ul>
                <ul>
                    <li><strong>Explore</strong></li>
                    <li>Start Here</li>
                    <li>Blog</li>
                    <li>About Us</li>
                </ul>
            </div>
        </nav>
        <div class="rights">
            © 2021 Samuele Miotto. All Rights Reserved.
        </div>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter',
}
</script>

<style lang="scss" scoped>
    footer {
        .newsletter {
            margin: 100px auto;
            text-align: center;
            * {
                margin-bottom: 30px;
            }
            span {
                display: block;
            }
        }
        nav {
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
        .rights {
            text-align: center;
        }
    }
</style>