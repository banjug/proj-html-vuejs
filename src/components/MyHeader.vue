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
                        <input type="text" placeholder="Search">
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
        padding: 20px 0;
        display: flex;
        justify-content: space-between;
        .logo {
            height: 25px;
        }
        .nav-right {
            display: flex;
            align-items: center;
            ul {
                display: flex;
                list-style: none;
                li {
                    margin-right: 50px;
                    .fa-user {
                        border: 2px solid black;
                        border-radius: 100%;
                        padding: 2px 3px;
                    }
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
        }
        p {
            line-height: 200%;
            margin-bottom: 15px;
        }
        button {
            display: block;
            margin-bottom: 15px;
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

</style>