<script>
export default {
    name: 'MainEvent',
    props: {

    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <section id="main-event">
        <div class="container">
            <div class="row mt-5">
                <div class="col-5 d-flex text-end">
                    <p class="fw-bolder"> TEAM1</p>
                    <p class="fw-bolder"> IMMAGINE</p>
                </div>
                <div class="col">
                    <p class="fw-bolder"> VS</p>
                </div>
                <div class="col-5 d-flex">
                    <p class="fw-bolder"> IMMAGINE</p>
                    <p class="fw-bolder"> TEAM2</p>
                </div>
            </div>
            <div class="address">
                <div class="row justify-content-center align-content-center">
                    <p class="col text-end"># May, 21 , 2022 18:05 pm </p>
                    <p class="col "># Expert Stadium</p>
                </div>
            </div>
            <div class="d-flex justify-content-center align-content-center">
                <button type="button" class="btn btn-dark text-center p-2">View Match Details</button>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.btn {}
</style>