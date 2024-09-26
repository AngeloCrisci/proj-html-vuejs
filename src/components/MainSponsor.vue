<script>
export default {
    name: 'MainSponsor',
    props: {

    },
    data() {
        return {
            sponsor: [
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
        <div class="container">
            <div class="sponsor">

            </div>
        </div>
</div>
</template>

<style lang="scss">

.main-sponsors {
    height: 250px;
    background-color: black;
}
</style>