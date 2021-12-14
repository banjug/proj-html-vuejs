<template>
    <header>
        <!-- nav section  -->
        <nav>
            <div class="nav-wrapper">
                <a href="#" class="logo"><img class="logo" src="../assets/images/dark-logo.png" alt=""></a>
                <div class="nav-right">
                    <ul>
                        <li>Home <i class="fas fa-chevron-down"></i></li>
                        <li>Home <i class="fas fa-chevron-down"></i></li>
                        <li>Home <i class="fas fa-chevron-down"></i></li>
                        <li>Home <i class="fas fa-chevron-down"></i></li>
                        <li>Home <i class="fas fa-chevron-down"></i></li>
                        <li>Home <i class="fas fa-chevron-down"></i></li>
                        <li><i class="far fa-user"></i></li>
                    </ul>
                    <div class="input-wrapper">
                        <input type="text" placeholder="Search...">
                        <i class="fas fa-search"></i>
                    </div>
                </div>
            </div>
        </nav>
        <!-- hero/jumbotron section  -->
        <section class="hero">
            <div class="hero-left">
                <h1>
                    Distant learning for further expansion
                </h1>
                <p>
                    Learning is a life-long journey that in fact we never find the terminate stop. Stop searching, enjoy the process.
                </p>
                <button>
                    <i class="fas fa-download"></i>
                    Download free guide
                </button>
                <span>Have questions? <a href="#">Get Free Sample <i class="fas fa-arrow-right"></i></a></span>
            </div>
            <div class="hero-right">
                <img class="portrait" src="../assets/images/hero-img-portrait.jpg" alt="">
                <img class="hero-shape shape-1" src="../assets/images/maxcoach-shape-07.png" alt="">
                <img class="hero-shape shape-2" src="../assets/images/maxcoach-shape-08.png" alt="">
                <img class="hero-shape shape-3" src="../assets/images/maxcoach-shape-08.png" alt="">
                <img class="hero-shape shape-4" src="../assets/images/maxcoach-shape-02.png" alt="">
                <div class="hero-shape hero-circle"></div>
            </div>
        </section>
        <section class="hero-clients">
            <ul>
                <li><img src="../assets/images/client-logo-01.png" alt=""></li>
                <li><img src="../assets/images/client-logo-02.png" alt=""></li>
                <li><img src="../assets/images/client-logo-03.png" alt=""></li>
                <li><img src="../assets/images/client-logo-04.png" alt=""></li>
                <li><img src="../assets/images/client-logo-05.png" alt=""></li>
                <li><img src="../assets/images/client-logo-06.png" alt=""></li>
            </ul>
        </section>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
}
</script>

<style lang="scss" scoped>
nav {
    box-shadow: 0px 0px 15px 0px rgba(0,0,0,0.1);
    .nav-wrapper {
        width: 65%;
        margin: 0 auto;
        padding: 30px 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
        .logo {
            height: 30px;
        }
        .nav-right {
            display: flex;
            align-items: center;
            ul {
                display: flex;
                list-style: none;
                li {
                    margin-right: 50px;
                    .fa-chevron-down {
                        font-size: .6rem;
                        margin-left: 10px;
                    }
                    .fa-user {
                        font-size: .9rem;
                        border: 2px solid black;
                        border-radius: 100%;
                        padding: 3px 3px;
                    }
                }
            }
            .input-wrapper {
                position: relative;
                input {
                    padding: 20px 40px 20px 20px;
                    border: none;
                    border-radius: 5px;
                    background: #f5f5f5;
                }
                .fa-search {
                    color: #20ad96;
                    position: absolute;
                    right: 10px;
                    top: 50%;
                    transform: translate(0, -50%);
                }
            }
        }
    }
}
.hero {
    width: 65%;
    margin: 0 auto;
    padding: 50px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .hero-left {
        width: 40%;
        h1 {
            font-size: 3rem;
            margin-bottom: 15px;
            font-weight: 700;
            color: #3f3a64;
        }
        p {
            font-size: 1.2rem;
            line-height: 200%;
            margin-bottom: 35px;
            color: #8c89a2;
        }
        button {
            display: block;
            margin-bottom: 35px;
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
        span {
            color: #20ad96;
            font-size: 1rem;
            a {
                color: #20ad96;
                font-weight: 700;
            }
        }
    }
    .hero-right {
        padding: 0 100px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        .portrait {
            border-radius: 100%;
            transform: scale(95%);
            z-index: 1;
        }
        .hero-shape {
            position: absolute;
        }
        .hero-circle {
            border: 10px solid #ecc5ab;
            border-radius: 100%;
            height: 70px;
            width: 70px;
            left: 7%;
            top: 60%;
        }
        .shape-1 {
            bottom: 0;
            right: 20%;
        }
        .shape-2 {
            left: 0;
            top: 25%;
        }
        .shape-3 {
            left: 0;
            top: 50%;
        }
        .shape-4 {
            right: 0;
            top: 20%;
        }
    }
}
.hero-clients {
    width: 65%;
    margin: 0 auto;
    ul {
        list-style: none;
        display: flex;
        justify-content: space-between;
        opacity: .5;
    }
}

</style>