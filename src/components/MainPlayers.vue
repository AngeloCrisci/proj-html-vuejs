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
                    nameAndRole: 'Adam Brown - Forwarder'
                },
                {
                    img: 'player2.jpg',
                    shirtNumber: '09',
                    nameAndRole: 'Michael Kayn - Forwarder'
                },
                {
                    img: 'player3.jpg',
                    shirtNumber: '11',
                    nameAndRole: 'Michael Lee - Forwarder'
                },
                {
                    img: 'player4.jpg',
                    shirtNumber: '15',
                    nameAndRole: 'Ethan Smith - Midfielder'
                }
            ],
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
<div class="main-players">
        <div class="container">
            <div class="title">
                <h3>Players</h3>
            </div>
            <ul class="player-cards">
                <li class="single-card" v-for="(player, index) in players" :key="index">
                    <div class="card-image">
                        <img :src='getImageUrl(`../assets/${player.img}`)' alt="player-img">
                    </div>
                    <div class="player-description">
                        <div class="number">
                            {{ player.shirtNumber }}
                        </div>
                        <div class="name-role">
                            {{ player.nameAndRole }}
                        </div>
                    </div>
                </li>
            </ul>
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

li {
    list-style-type: none;
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
