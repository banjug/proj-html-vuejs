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
    }
</style>