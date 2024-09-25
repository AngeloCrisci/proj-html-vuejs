<script>
export default {
    name: 'MainPlayers',
    props: {

    },
    data() {
        return {

        }
    }
}
</script>

<template>
<div class="main-players">
        <div class="container">
            <div class="title">
                <h3>Players</h3>
            </div>
            <div class="player-cards">
                <div class="card"></div>
            </div>
            <div class="player-button">

            </div>
        </div>
</div>
</template>

<style lang="scss">
.main-players {
    height: 500px;
    background-image: url(../assets/player.jpg);
    background-position: center;
}
</style>
