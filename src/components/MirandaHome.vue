<template>
    <div class="container-fluid vh-100 d-flex flex-column">
        <div class="row flex-grow-1">
            <!-- Sección de Texto -->
            <div class="col-lg-6 d-flex flex-column justify-content-center text-white p-5">
                <div>
                    <h1 class="display-4 fw-bold">Nosotros somos <div class="text-animated"><span>Hilos Lobo</span>
                        </div>
                    </h1>
                    <p class="lead my-4"> Somos una empresa dedicada a la distribución y al comercio de productos para
                        la
                        industria textil, preocupada por establecer políticas de competencia cuyo principal objetivo es
                        ofrecer artículos de calidad con los mejores precios</p>
                    <form class="d-flex mb-4">
                        <input type="email" class="form-control form-control-lg me-2"
                            placeholder="¿Quieres más información?">
                        <button class="btn btn-lg btn-success" type="submit">Contactanos</button>
                    </form>
                </div>
            </div>
            <div class="col-lg-6 d-flex flex-column justify-content-center p-5">
                <img src="../assets/logo.png" alt="logo_hiloslobo">
            </div>
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

.text-animated {
    color: #fa0404 !important;
}

h1 {
    color: white;
}

.text-animated span {
    position: relative;
}

.text-animated span::before {
    content: 'Familia';
    color: #fa0404;
    animation: words 60s infinite;
}

.text-animated span::after {
    content: '';
    background-color: #181818;
    position: absolute;
    width: calc(100% + 14px);
    height: 100%;
    border-left: 2px solid #fa0404;
    right: -10px;
    animation: cursor .6s infinite, typing 20s steps(14);
}

@keyframes cursor {
    to {
        border-left: 2px solid #181818;
    }
}

@keyframes words {

    0%,
    20% {
        content: 'Familia';
    }

    21%,
    40% {
        content: 'Calidad';
    }

    41%,
    60% {
        content: '100% Mexicanos';
    }

    61%,
    80% {
        content: 'Coloridos';
    }

    81%,
    100% {
        content: 'Autenticos';
    }
}

@keyframes typing {

    10%,
    15%,
    30%,
    35%,
    50%,
    55%,
    70%,
    75%,
    90%,
    95% {
        width: 0;
    }

    5%,
    20%,
    25%,
    40%,
    45%,
    60%,
    65%,
    80%,
    85% {
        width: calc(100% +14px);
    }
}

.lead {
    color: #d1d1d1;
}

.position-absolute {
    right: 20px;
    top: 20px;
}
</style>