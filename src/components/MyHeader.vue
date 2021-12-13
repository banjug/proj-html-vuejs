<template>
    <header>
        <nav>
            <div class="nav-wrapper">
                <a href="#" class="logo"><img src="../assets/images/dark-logo.png" alt=""></a>
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
        <section class="hero">

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
        width: 80%;
        margin: 0 auto;
        padding: 20px 0;
        display: flex;
        justify-content: space-between;
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

</style>