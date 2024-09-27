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
        <div class="container container-flex">
            <div class="title-section">
                <h3>Players</h3>
            </div>
            <ul class="player-cards-section">
                <li class="single-card" v-for="(player, index) in players" :key="index">
                    <div class="card-image-container">
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
                    </div>
                </li>
            </ul>
            <div class="player-button-section">
                <div class="player-button">
                    <p>View All Players</p>
                </div>
            </div>
        </div>
</div>
</template>

<style lang="scss" scoped>
.main-players {
    height: 550px;
    background-image: url(../assets/player.jpg);
    background-position: center;
}

.container-flex {
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 30px;
}

img {
    width: 225px;
}

p {
    margin: 0;
}

li {
    list-style-type: none;
}

.title-section {
    color: white;
    font-weight: 500;
    text-align: center;

}

.player-cards-section {
    display: flex;
    justify-content: space-around;
}

.card-image-container {
    width: 250px;
    height: 280px;
    background-color: black;
    border-radius: 20px;
    display: flex;
    justify-content: center;
    align-items: flex-end;
}

li:last-child .card-image-container {
    background-color: #1B1B19;
}

.card-image:hover {
    scale: 1.1;
}

.card-image:hover + .player-description{
    bottom: -20px;
    left: 0;
}

.single-card {
    position: relative;
}

.card-image img {
    border-radius: 20px;
}

.player-description {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
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

.name-role {
    font-size: 0.9rem;
    opacity: 0.8;
}

.player-button-section {
    display: flex;
    justify-content: center;
}

.player-button {
    padding: 18px 20px;
    background-color: black;
    color: white;
    width: 200px;
    border-radius: 25px;
    text-align: center;
    border: 1px solid white;
    font-weight: 500;
    cursor: pointer;
}

</style>
