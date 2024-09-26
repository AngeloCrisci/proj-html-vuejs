<script>
export default {
    name: 'MainArticles',
    props: {

    },
    data() {
        return {
            articles: [
                {name: 'What is Football', img: 'news1-1-300x300.png', description:'Football is a sport known as a ball game and is loved by[...]'},
                {name: 'Football Rules', img: 'news3-1-300x300.png', description:'GOLDEN GOAL: In a football match, the goal scored by one of the teams in […]'},
                {name: 'Football Features', img: 'news2-1-300x300.png', description:'Football: It is an aerobic-based anaerobic sport in which jumps, kicks, turns, running with changing […]'},
                {name: 'Football Terms', img: 'news4-1-300x300.png', description:'GOLDEN GOAL: In a football match, the goal scored by one of the teams in […]'},
                {name: 'How many football players are there in the world?', img: 'news6-1-300x300.png', description:'According to this report, there are more than 301 thousand football clubs, over 1.752 million […]'}
            ]
        }
    },
    methods: {
        getImageUrl(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        },

        getActiveIndex () {
            return this.activeIndex;
        }
    }

    created(getActiveIndex) [
        getActiveIndex;
    ]
}
</script>

<template>
<div class="container d-flex flex-column justify-content-center align-items-center mt-5">
    <div class="text-center">
        <i class="bi bi-hand-thumbs-up-fill h1"></i>
        <p class="h2"><strong>Resent New & Articles</strong></p>
        <p>Be aware of the football world.</p>
    </div>
    <div class="container text-center">
        <div class="row align-items-center">

            <div class="col-3 card-layout" :class="this.activeIndex ? 'active' : 'd-none'" v-for="(article, activeIndex) in articles" :key="activeIndex" >
                <div class="card">
                    <div class="card-body text-card-field text-center p-4">
                        <img :src="getImageUrl(`../assets/${article[activeIndex].img}`)" class="card-img-top" alt="...">
                        <p class="h4">29.05.2022-Football</p>
                        <p class="h3"><strong>{{ article[activeIndex].name }}</strong></p>
                        <p>{{ article[activeIndex].description }}</p>
                        <button type="button" class="btn btn-dark button-card"><strong>More</strong></button>
                    </div>
                </div>    
            </div>

            <div class="thumbnails d-flex justify-content-center gap-1">
                <div class="thumb" v-for="(article, index) in articles" :key="index" @click="getActiveIndex">
                </div>
            </div>

        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
.card-layout {
    width: 19.5rem;
    img{
        height: 230px;
        width: 220px;
    }
    .button-card {
        padding: 20px 50px;
        border-radius: 30px;
    }
}

.card-layout:active {
    display: block;
}

.thumb {
    width: 70px;
    height: 10px;
    background-color: grey;
    border-radius: 20px;
}

.thumb:active {
    background-color: black;
}
</style>