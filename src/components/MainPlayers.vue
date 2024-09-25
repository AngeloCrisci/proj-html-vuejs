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
                <div class="single-card">
                    <div class="card-image">
                        <img src="../assets/player1.jpg" alt="player 1">
                    </div>
                    <div class="player-description">
                        <div class="number">
                            07
                        </div>
                        <div class="name-role">
                            Adam Brown - Forwander
                        </div>
                    </div>
                </div>
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

img {
    width: 200px;
}

.title {
    color: white;
    font-weight: 500;
}

.single-card {
    position: relative;
}

.card-image img {
        border-radius: 20px;
}

.player-description {
    text-align: center;
    color: white;
    width: 200px;
    border-radius: 20px;
    padding: 10px;
    background-color: black;
    position: absolute;
    bottom: 0;
    left: 0;
}

</style>
