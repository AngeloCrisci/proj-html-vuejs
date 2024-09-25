<script>
export default {
    name: 'MainPlayers',
    props: {

    },
    data() {
        return {
            players: [
                {
                    img: 'player1.jpg',
                    shirtNumber: '07',
                    nameAndRole: 'Adam Brown - Forwander'
                }
            ]
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
                <div class="single-card" v-for="(card, index) in 4" :key="index">
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
    width: 250px;
}

.title {
    color: white;
    font-weight: 500;
    text-align: center;
    padding: 20px;
}

.player-cards {
    display: flex;
    justify-content: space-around;
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
    width: 250px;
    height: 80px;
    border-radius: 20px;
    padding: 10px;
    background-color: black;
    position: absolute;
    bottom: -10px;
    left: 0;
}

</style>
