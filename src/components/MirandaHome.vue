<template>
    <div class="container-fluid vh-100 d-flex flex-column">
        <div class="row flex-grow-1">
            <!-- Sección de Texto -->
            <div class="col-lg-6 d-flex flex-column justify-content-center text-white p-5">
                <div>
                    <h1 class="display-4 fw-bold">Creative studio focused on <span class="text-success">Web
                            Development</span></h1>
                    <p class="lead my-4">From concept to execution, we deliver web designs that make an impact. Let your
                        brand shine with our innovative and visually stunning websites.</p>
                    <form class="d-flex mb-4">
                        <input type="email" class="form-control form-control-lg me-2"
                            placeholder="Enter your email address">
                        <button class="btn btn-lg btn-success" type="submit">Start trial!</button>
                    </form>
                    <div class="d-flex">
                        <div class="me-4 text-center">
                            <i class="bi bi-24-hour-fill text-success fs-2"></i>
                            <p class="mt-2">24/7 Support</p>
                        </div>
                        <div class="text-center">
                            <i class="bi bi-award-fill text-success fs-2"></i>
                            <p class="mt-2">Award Winning Agency</p>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Sección de Imagen -->

        </div>
    </div>
</template>

<script>
export default {
    name: 'MirandaHome'
}
</script>

<style scoped>
.container-fluid {
    background-color: #181818;
    /* Fondo oscuro para la página principal */
}

.form-control-lg {
    max-width: 400px;
    /* Ancho máximo del input */
}

.btn-success {
    min-width: 150px;
    /* Ancho mínimo del botón */
}

.text-success {
    color: #28a745 !important;
}

h1 {
    color: white;
}

.lead {
    color: #d1d1d1;
}

.position-absolute {
    right: 20px;
    top: 20px;
}
</style>