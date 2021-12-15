<template>
    <section>
        <div class="numbers-section">
            <div>
                <h3>Successfully trained</h3>
                <h2>1790</h2>
                <span>ENROLLED LEARNERS</span>
            </div>
            <div>
                <h3>Proudly received</h3>
                <h2>19</h2>
                <span>COUNTRYWIDE AWARDS</span>
            </div>
            <div>
                <h3>Firmly Enstablished</h3>
                <h2>24</h2>
                <span>LOCAL BRANCHES</span>
            </div>
            <div>
                <h3>Getting Featured on</h3>
                <h2>1090</h2>
                <span>BLOG POSTS</span>
            </div>
        </div>
        <div class="blog-section">
            <div class="blog-wrapper">
                <div class="bullet-points">
                    <span>ENJOYABLE INSIGHTS</span>
                    <h2>Most Viewed <span>Best Blogs</span></h2>
                    <ul class="fa-ul">
                        <li><span class="fa-li"><i class="fas fa-arrow-right"></i></span> Become a Better Blogger: Content Planning</li>
                        <li><span class="fa-li"><i class="fas fa-arrow-right"></i></span> Promoting Your Online Business on Pinterest</li>
                        <li><span class="fa-li"><i class="fas fa-arrow-right"></i></span> Gamification and Game-Based Learning</li>
                        <li><span class="fa-li"><i class="fas fa-arrow-right"></i></span> Designin an Online Course from Expert's Perspective</li>
                        <li><span class="fa-li"><i class="fas fa-arrow-right"></i></span> Why Online Courses Are the Future of Education</li>
                    </ul>
                </div>
                <div class="blog-post">
                    <img src="../assets/images/artist-blog-03-480x352.jpeg" alt="">
                    <div class="blog-text">
                        <span class="blog-category">ARTIST</span>
                        <h3>
                            Brush Strokes Energize Trees in Paintings
                        </h3>
                        <span class="blog-data"><i class="far fa-calendar"></i> May 15, 2020</span>
                        <span class="blog-data"><i class="far fa-eye"></i> 688 Views</span>
                    </div>
                </div>
                <div class="blog-post">
                    <img src="../assets/images/artist-blog-01-480x352.jpg" alt="">
                    <div class="blog-text">
                        <span class="blog-category">ARTIST</span>
                        <h3>
                            Pocket-Sized Notebooks Hold Miniature Paintings
                        </h3>
                        <span class="blog-data"><i class="far fa-calendar"></i> May 15, 2020</span>
                        <span class="blog-data"><i class="far fa-eye"></i> 603 Views</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Insights',
}
</script>

<style lang="scss" scoped>
    section {
        .numbers-section {
            width: 65%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            text-align: center;
             div {
                width: 100%;
                padding: 100px 50px;
                border-left: 2px solid #f5f1ed;
                * {
                    margin-bottom: 40px;
                }
                h2 {
                    font-size: 4rem;
                    color: #20ad96;
                }
                h3 {
                    font-size: 1.7rem;
                    color: #3f3a64;
                }
                span {
                    color: #20ad96;
                    font-weight: 700;
                    font-size: 1.2rem;
                }
            }
            > :last-child {
                border-right: 2px solid #f5f1ed;
            }
        }
        .blog-section {
            background: #f5f1ed;
            padding: 100px 0;
            .blog-wrapper {
                display: flex;
                justify-content: space-between;
                align-items: center;
                width: 65%;
                margin: 0 auto;
                .bullet-points {
                    width: 40%;
                    * {
                        margin-bottom: 50px;
                    }
                    >span {
                        color: #918ea6;
                        font-size: 1.3rem;
                    }
                    h2 {
                        color: #3f3a64;
                        font-size: 3rem;
                        margin-top: 50px;
                        >span {
                            color: #8c89a2;
                            font-weight: 400;
                        }
                    }
                    li {
                        color: #3f3a64;
                        font-weight: 700;
                    }
                }
                .blog-post {
                    width: calc(30% - 50px);
                    margin-left: 50px;
                    background: #ffffff;
                    border-radius: 5px;
                    &:hover {
                        transition: all .4s ease;
                        box-shadow: 0px 0px 15px 0px rgba(0,0,0,0.1);
                        transform: scale(1.03);

                    }
                    img {
                        width: 100%;
                        border-top-right-radius: 5px;
                        border-top-left-radius: 5px;
                    }
                    .blog-text {
                        padding: 10px 30px 30px;
                        .blog-category {
                            color: #918ea6;
                        }
                        h3 {
                            color: #3f3a64;
                            margin: 20px 0;
                            font-size: 1.2rem;
                            cursor: pointer;
                        }
                        .blog-data {
                            color: #7e7e7e;
                            margin-right: 20px;
                        }
                    }
                }
            }
        }
    }
</style>