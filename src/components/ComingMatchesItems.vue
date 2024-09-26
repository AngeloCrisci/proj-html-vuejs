<script>
export default {
    data() {
        return {
            teamsMatches: [
                { name: store.teams[1].name, image: store.teams[1].img, nameTwo: store.teams[2].name, imageTwo: store.teams[2].image }
            ]
        }

    }

}
</script>

<template>
    <div class="container">
        <div class="cards-coming-matches">
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
        </div>
    </div>
</template>