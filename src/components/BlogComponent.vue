<template>
    <div class="blog d-flex flex-column align-items-center">
        <h2 class="blog-headline">Blog</h2>
        <div class="news row">

            <div class="news-card col d-flex flex-column">
                <img class="news-card-img" src="../assets/images/blog/2438389 1.png" />
                <span class="news-card-date">02.06.20</span>
                <p class="news-card-text">In expression an solicitude principles in do. Small for ask shade water manor think men begin. At principle perfectly by sweetness do.</p>
            </div>

            <div class="news-card col d-flex flex-column">
                <img class="news-card-img" src="../assets/images/blog/download 1.png" />
                <span class="news-card-date">02.06.20</span>
                <p class="news-card-text">In expression an solicitude principles in do. Small for ask shade water manor think men begin. At principle perfectly by sweetness do.</p>
            </div>

            <div class="news-card col d-flex flex-column">
                <img class="news-card-img" src="../assets/images/blog/bangkok_d_850 1.png" />
                <span class="news-card-date">02.06.20</span>
                <p class="news-card-text">In expression an solicitude principles in do. Small for ask shade water manor think men begin. At principle perfectly by sweetness do.</p>
            </div>

        </div>
        <button class="news-btn btn btn-success" @click="modalChange">View all news</button>
    </div>
</template>

<script>
    export default {
        name: 'BlogComponent',
        methods: {
            modalChange() {
                this.$emit('modalChange', {isModal: true, success: true, form: false})
            },
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.blog-headline{
    text-align: center;
    font-size: 2.8125rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin-bottom: 1.75rem;
}
.news{
    margin-bottom: 1.87rem;
}
.news-card-img{
    width: 25.2rem;
}
.news-card-date{
    font-size: 1.25rem;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    margin: 0.87rem 0 0.31rem 0;
}
.news-card-text{
    font-size: 1.25rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}
.news-btn{
    margin-bottom: 2.12rem;
    width: 16rem;
    border: 3px solid #2DC66E !important;
    background-color: #2DC66E;
}
.news-btn:hover{
    background-color: transparent !important;
    color: #2DC66E;
}
@media (min-width: 361px) and (max-width: 1366px){
    .news-card-img{
        width: 21.2rem;
    }
}
@media screen and (max-width: 361px){
    .news-card-img{
        width: 20rem;
    }
}
</style>