<template>
    <div class="container-fluid py-5 bg-dark text-white">
        <div class="row align-items-center mb-5">
            <div class="col-lg-6 text-center text-lg-left">
                <h2 class="font-weight-bold">100+ Companies trust us</h2>
                <div id="brandCarousel" class="carousel slide" data-ride="carousel">
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <img src="brand1.png" class="d-block w-100" alt="Brand 1">
                        </div>
                        <div class="carousel-item">
                            <img src="brand2.png" class="d-block w-100" alt="Brand 2">
                        </div>
                        <div class="carousel-item">
                            <img src="brand3.png" class="d-block w-100" alt="Brand 3">
                        </div>
                        <!-- Añadir más marcas según sea necesario -->
                    </div>
                    <a class="carousel-control-prev" href="#brandCarousel" role="button" data-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="sr-only">Previous</span>
                    </a>
                    <a class="carousel-control-next" href="#brandCarousel" role="button" data-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="sr-only">Next</span>
                    </a>
                </div>
            </div>
            <div class="col-lg-6 text-center text-lg-left">
                <div class="d-flex justify-content-center justify-content-lg-start align-items-center mb-4">
                    <div class="info-box bg-secondary text-white mr-3 p-4">
                        <h3 class="font-weight-bold">10+</h3>
                        <p>Years of experience</p>
                    </div>
                    <div class="info-box bg-success text-white p-4">
                        <h3 class="font-weight-bold">1.2K</h3>
                        <p>Happy customers</p>
                    </div>
                </div>
                <h2 class="font-weight-bold">Defining the future of online experiences!</h2>
                <p class="lead">Embrace a new era of digital success with our company. Our team combines cutting-edge
                    design with robust development to deliver websites that captivate and convert.</p>
                <ul class="list-unstyled">
                    <li><i class="bi bi-check-circle-fill text-success mr-2"></i>Emphasis on ROI-driven solutions</li>
                    <li><i class="bi bi-check-circle-fill text-success mr-2"></i>Expert team with diverse skill</li>
                    <li><i class="bi bi-check-circle-fill text-success mr-2"></i>Proven track record of delivering
                        results</li>
                </ul>
                <a href="#" class="btn btn-outline-light btn-lg mt-3">Discover more</a>
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