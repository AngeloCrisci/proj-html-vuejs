<script>
import HeaderLinksItems from './HeaderLinksItems.vue';

export default {
    name: 'AppHeader',
    
    data() {
        return {
            navLinks: [
                {
                    label: "HOME",
                    url: "#",
                },
                {
                    label: "FIXTURES & RESULTS",
                    url: "#",
                },
                {
                    label: "LEAGUE TABLE",
                    url: "#",
                },
                {
                    label: "PLAYERS",
                    url: "#",
                },
                {
                    label: "GALLERY",
                    url: "#",
                },
                {
                    label: "BLOG",
                    url: "#",
                },
                {
                    label: "CONTACT",
                    url: "#",
                },
            ]
        }
    },
    components: {
        HeaderLinksItems
    }
}

</script>

<template>
    <header>

        <!-- ! NAVBAR -->
        <div class="position-relative">
            <div class="top-header position-absolute">
                <div class="container">
                    <div class="row pt-2 mb-3">
                        <div class="col text-white d-flex flex-wrap align-items-center">
                            <a href="#"><img src="../assets/sponsor1.png" alt="sponsor-1"></a>
                            <a href="#"><img src="../assets/sponsor2.png" alt="sponsor-2"></a>
                        </div>

                        <div class="col text-center text-white">
                            <a href="#"><img src="../assets/logo-football.png" alt="logo-football"></a>
                        </div>

                        <div class="col text-end text-white mt-4">
                            <i class="bi bi-facebook"></i>
                            <i class="bi bi-instagram"></i>
                            <i class="bi bi-twitter"></i>
                        </div>  
                    </div>

                    <div class="ul-box">
                        <ul class="p-0 justify-content-center gap-5 d-none d-lg-flex">

                            <HeaderLinksItems v-for="(link, index) in navLinks" :key="index"
                            :linkLabel="link.label"
                            :linkUrl="link.url"/>

                        </ul>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- ! CAROUSEL -->
        <section class="header-carousel">
            <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item">
                        <img class="d-block w-100" src="../assets/slider1-1.jpg" alt="slider-img-1">
                        
                        <div class="position-absolute carousel-div-text">
                            <h1 class="text-white fw-bold text-center">Welcome to <br> Football Club</h1>
                            <p class="text-white fw-bold text-center fs-5 mb-4">Live match fix types and results.</p>
                            <div class="d-flex justify-content-center">
                                <a href="#" class="text-white fw-bold fs-5">Learn More &#129050;</a>
                            </div>
                        </div>
                    </div>

                    <div class="carousel-item">
                        <img class="d-block w-100" src="../assets/slider2-1.jpg" alt="slider-img-2">

                        <div class="position-absolute carousel-div-text">
                            <h1 class="text-white fw-bold text-center">Football Club <br> Sport Club</h1>
                            <p class="text-white fw-bold text-center fs-5 mb-4">Private football matches.</p>
                            <div class="d-flex justify-content-center">
                                <a href="#" class="text-white fw-bold fs-5">Learn More &#129050;</a>
                            </div>
                        </div>
                    </div>

                    <div class="carousel-item">
                        <img class="d-block w-100" src="../assets/slider3.jpg" alt="slider-img-3">

                        <div class="position-absolute carousel-div-text">
                            <h1 class="text-white fw-bold text-center">Professional Football Football Club</h1>
                            <p class="text-white fw-bold text-center fs-5 mb-4">Football is the poetry of movement.</p>
                            <div class="d-flex justify-content-center">
                                <a href="#" class="text-white fw-bold fs-5">Learn More &#129050;</a>
                            </div>
                        </div>
                    </div>

                    <div class="carousel-item active">
                        <img class="d-block w-100" src="../assets/slider4.jpg" alt="slider-img-4">

                        <div class="position-absolute carousel-div-text">
                            <h1 class="text-white fw-bold text-center">Football Club <br> Sport Club</h1>
                            <p class="text-white fw-bold text-center fs-5 mb-4">Football is a head game.</p>
                            <div class="d-flex justify-content-center">
                                <a href="#" class="text-white fw-bold fs-5">Learn More &#129050;</a>
                            </div>
                        </div>
                    </div>
                </div>
                <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                </a>
                <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                </a>
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
    .top-header {
        width: 100%;
        min-height: 200px;
        background-color: rgba(0, 0, 0, 0.7);
        z-index: 1;

        i {
            font-size: 1.8rem;
            margin-left: 25px;
        }

        .ul-box {
            margin-bottom: 30px;

            ul {
            list-style-type: none;
            }
        }
    }

    .header-carousel img{
        height: 1140px;
        object-fit: cover;

    }
    .carousel-div-text {
        width: 750px;
        position: absolute;
        z-index: 1;
        top: 57%;
        left: 50%;
        transform: translate(-50%, -50%);

        h1 {
            font-size: 4.6rem;
        }

        a {
            text-decoration: none;
            padding: 20px 40px;
            border: 2px solid white;
            border-radius: 40px;
        }
    }
</style>