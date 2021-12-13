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
            <div class="bullet-points">
                <span>ENJOYABLE INSIGHTS</span>
                <h2>Most Viewed Best Blogs</h2>
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
                <span>ARTIST</span>
                <h3>
                    Brush Strokes Energize Trees in Paintings
                </h3>
                <span><i class="far fa-calendar"></i> May 15, 2020</span>
                <span><i class="far fa-eye"></i> 688 Views</span>
            </div>
            <div class="blog-post">
                <img src="../assets/images/artist-blog-01-480x352.jpg" alt="">
                <span>ARTIST</span>
                <h3>
                    Pocket-Sized Notebooks Hold Miniature Paintings
                </h3>
                <span><i class="far fa-calendar"></i> May 15, 2020</span>
                <span><i class="far fa-eye"></i> 603 Views</span>
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
        width: 65%;
        margin: 0 auto;
        .numbers-section {
            display: flex;
            justify-content: space-between;
            text-align: center;
             div {
                 width: 100%;
                 padding: 100px 50px;
                 border-left: 1px solid gray;
                 * {
                     margin-bottom: 40px;
                 }
                 h2 {
                     font-size: 3.5rem;
                 }
                 h3 {
                     font-size: 1.7rem;
                 }
            }
            > :last-child {
                border-right: 1px solid gray;
            }
        }
        .blog-section {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            .bullet-points {
                width: 40%;
            }
            .blog-post {
                width: calc(25% - 50px);
                margin-left: 50px;
                img {
                    width: 100%;
                }
            }
        }
    }
</style>