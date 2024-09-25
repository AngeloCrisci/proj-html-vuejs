<script>
export default {
    name: 'AppHeader',
    props: {

    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <header>
        <div class="position-relative">
            <div class="top-header position-absolute">
                <div class="container">
                    <div class="row pt-2">
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

                    <div>
                        <ul class="d-flex p-0 justify-content-center">
                            <li>
                                <a href="#">CIAO</a>
                            </li>
                            
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        
        <section class="header-carousel">
            <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img class="d-block w-100" src="../assets/slider1-1.jpg" alt="slider-img-1">
                        <div>
                            <h1 text-white>Welcome to Football Club</h1>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img class="d-block w-100" src="../assets/slider2-1.jpg" alt="slider-img-2">
                    </div>
                    <div class="carousel-item">
                        <img class="d-block w-100" src="../assets/slider3.jpg" alt="slider-img-3">
                    </div>
                    <div class="carousel-item">
                        <img class="d-block w-100" src="../assets/slider4.jpg" alt="slider-img-4">
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
        background-color: rgba(0, 0, 0, 0.5);
        z-index: 1;

        i {
            font-size: 1.8rem;
            margin-left: 25px;
        }

        ul {
            list-style-type: none;

            a {
                text-decoration: none;
                color: white;
                font-weight: bold;
            }
        }

    }

    .header-carousel img{
        height: 1140px;
        object-fit: cover;

    }
</style>