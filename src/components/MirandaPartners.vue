<template>
    <div class="container-fluid py-5 bg-dark text-white">
        <div class="row align-items-center mb-5">
            <div class="col-lg-12 text-center text-lg-left">
                <h2 class="font-weight-bold">Marcas que confian en nosotros</h2>
                <div id="brandCarousel" class="carousel slide" data-ride="carousel">
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <img src="../assets/logo.png" class="d-block w-100" alt="Brand 1">
                        </div>
                        <div class="carousel-item">
                            <img src="../assets/logo.png" class="d-block w-100" alt="Brand 2">
                        </div>
                        <div class="carousel-item">
                            <img src="../assets/logo.png" class="d-block w-100" alt="Brand 3">
                        </div>
                        <!-- Añadir más marcas según sea necesario -->
                    </div>
                    <a class="carousel-control-prev" href="#brandCarousel" role="button" data-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="sr-only">Anterior</span>
                    </a>
                    <a class="carousel-control-next" href="#brandCarousel" role="button" data-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="sr-only">Siguiente</span>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MirandaPartners'
}
</script>

<style scoped>
.bg-dark {
    background-color: #181818 !important;
}

.info-box {
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.carousel-item img {
    width: auto;
    height: 50px;
    object-fit: contain;
}

.carousel-control-prev-icon,
.carousel-control-next-icon {
    background-color: #28a745;
    border-radius: 50%;
    padding: 10px;
}
</style>