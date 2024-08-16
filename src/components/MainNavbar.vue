<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
        <div class="container-fluid px-4 px-md-5">
            <a class="navbar-brand d-flex align-items-center" href="#">
                <img src="@/assets/logo.png" alt="Logo" class="me-2" width="40" height="40">
                <span>Hilos Lobo</span>
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                        <a class="nav-link" href="MirandaHome.vue">Inicio</a>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button"
                            data-bs-toggle="dropdown" aria-expanded="false">
                            Nuestros Productos
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li><a class="dropdown-item" href="MirandaProducts.vue">Hilos</a></li>
                            <li><a class="dropdown-item" href="MirandaProducts.vue">Cierres</a></li>
                            <li><a class="dropdown-item" href="MirandaProducts.vue">Refacciones</a></li>
                            <li><a class="dropdown-item" href="MirandaProducts.vue">Articulos Nuevos</a></li>
                        </ul>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="MirandaUbi.vue">Ubicaciones</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="MirandaContact.vue">Contáctanos</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'MainNavbar'
}
</script>

<style scoped>
.navbar-brand span {
    font-size: 1.25rem;
    font-weight: 600;
}

.navbar-dark .navbar-nav .nav-link {
    color: rgba(255, 255, 255, 0.75);
}

.navbar-dark .navbar-nav .nav-link:hover,
.navbar-dark .navbar-nav .nav-link:focus {
    color: white;
}

.dropdown-menu {
    background-color: #343a40;
    border-color: rgba(0, 0, 0, 0.15);
}

.dropdown-item {
    color: rgba(255, 255, 255, 0.75);
}

.dropdown-item:hover,
.dropdown-item:focus {
    color: white;
    background-color: #495057;
}

.btn-outline-light {
    border-color: rgba(255, 255, 255, 0.75);
}

.btn-outline-light:hover {
    color: white;
    background-color: rgba(255, 255, 255, 0.1);
    border-color: white;
}
</style>