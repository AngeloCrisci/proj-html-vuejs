<script>
export default {
    name: 'MainSponsor',
    props: {

    },
    data() {
        return {
            sponsors: [
                'client2.png',
                'client3.png',
                'client4.png',
                'client7.png',
                'client9.png',
                'client10.png',
            ]
        }
    },
    methods: {
        getImageUrl(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
<div class="main-sponsors">
        <div class="container container-flex">
            <div class="sponsor" v-for="(sponsor, index) in sponsors" :key="index">
                <img :src="getImageUrl(`../assets/${sponsor}`)" :alt="sponsor">
            </div>
        </div>
</div>
</template>

<style lang="scss" scoped >
.main-sponsors {
    height: 225px;
    background-color: black;
    display: flex;
    align-items: center;
}

.container-flex {
    display: flex;
    height: 60%;
    justify-content: space-around;
}

.sponsor {
    display: flex;
    align-items: center;
    justify-content: space-around;
    gap: 20px;
}

img {
    width: 70%;
    border: 1px solid white;
    border-radius: 30px;
    padding: 20px;
}
</style>