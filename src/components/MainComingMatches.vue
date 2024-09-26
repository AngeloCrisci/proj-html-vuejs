<script>
import ComingMatchesItems from './ComingMatchesItems.vue';

export default {
    name: 'MainComingMatches',
    components: {
        ComingMatchesItems,
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <section id="coming-matches">
        <div class="container">
            <h3 class="text-center pt-4 text-white">UpComing Matchs</h3>
            <div class="cards-coming-matches">
                <ComingMatchesItems />
                <!-- <div class="mt-5 d-flex justify-content-between card-coming-matches">
                    <div class=" d-flex">
                        <p class="fw-bolder"> TEAM1</p>
                        <p class="fw-bolder"> IMMAGINE</p>
                    </div>
                    <div>
                        <p class="fw-bolder"> VS</p>
                    </div>
                    <div class=" d-flex">
                        <p class="fw-bolder"> IMMAGINE</p>
                        <p class="fw-bolder"> TEAM2</p>
                    </div>
                </div>
                <div class="address">
                    <div class="d-flex justify-content-center align-content-center">
                        <p class="text-end"># May, 21 , 2022 18:05 pm </p>
                        <p># Expert Stadium</p>
                    </div>
                </div>
                <div class="mt-5 d-flex justify-content-between card-coming-matches">
                    <div class=" d-flex">
                        <p class="fw-bolder"> TEAM1</p>
                        <p class="fw-bolder"> IMMAGINE</p>
                    </div>
                    <div>
                        <p class="fw-bolder"> VS</p>
                    </div>
                    <div class=" d-flex">
                        <p class="fw-bolder"> IMMAGINE</p>
                        <p class="fw-bolder"> TEAM2</p>
                    </div>
                </div>
                <div class="address">
                    <div class="d-flex justify-content-center align-content-center">
                        <p class=" text-end"># May, 21 , 2022 18:05 pm </p>
                        <p># Expert Stadium</p>
                    </div>
                </div>
                <div class="mt-5 d-flex justify-content-between card-coming-matches">
                    <div class=" d-flex">
                        <p class="fw-bolder"> TEAM1</p>
                        <p class="fw-bolder"> IMMAGINE</p>
                    </div>
                    <div>
                        <p class="fw-bolder"> VS</p>
                    </div>
                    <div class=" d-flex">
                        <p class="fw-bolder"> IMMAGINE</p>
                        <p class="fw-bolder"> TEAM2</p>
                    </div>
                </div>
                <div class="address">
                    <div class="d-flex justify-content-center align-content-center">
                        <p class="text-end"># May, 21 , 2022 18:05 pm </p>
                        <p># Expert Stadium</p>
                    </div>
                </div>
                <div class="mt-5 d-flex justify-content-between card-coming-matches">
                    <div class=" d-flex">
                        <p class="fw-bolder"> TEAM1</p>
                        <p class="fw-bolder"> IMMAGINE</p>
                    </div>
                    <div>
                        <p class="fw-bolder"> VS</p>
                    </div>
                    <div class=" d-flex">
                        <p class="fw-bolder"> IMMAGINE</p>
                        <p class="fw-bolder"> TEAM2</p>
                    </div>
                </div>
                <div class="address">
                    <div class="d-flex justify-content-center align-content-center">
                        <p class="text-end"># May, 21 , 2022 18:05 pm </p>
                        <p># Expert Stadium</p>
                    </div>
                </div>
                <div class="mt-5 d-flex justify-content-between card-coming-matches">
                    <div class=" d-flex">
                        <p class="fw-bolder"> TEAM1</p>
                        <p class="fw-bolder"> IMMAGINE</p>
                    </div>
                    <div>
                        <p class="fw-bolder"> VS</p>
                    </div>
                    <div class=" d-flex">
                        <p class="fw-bolder"> IMMAGINE</p>
                        <p class="fw-bolder"> TEAM2</p>
                    </div>
                </div>
                <div class="address">
                    <div class="d-flex justify-content-center align-content-center">
                        <p class="text-end"># May, 21 , 2022 18:05 am </p>
                        <p># Expert Stadium</p>
                    </div>
                </div> -->
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
#coming-matches {
    background-image: url(../assets/saha.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

h3 {
    font-weight: 600;
    font-size: 25px;
}
</style>