<template>
    <div class="container py-5">
        <div class="row">
            <div class="col-md-4">
                <div class="card h-100 text-center bg-dark text-white p-3">
                    <div class="card-body">
                        <div class="icon mb-4">
                            <i class="bi bi-ui-checks-grid display-4 text-success"></i>
                        </div>
                        <h5 class="card-title">UI/UX Design</h5>
                        <p class="card-text">Creating user interfaces that are both efficient and enjoyable.</p>
                        <a href="#" class="text-success">Know more →</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card h-100 text-center bg-dark text-white p-3">
                    <div class="card-body">
                        <div class="icon mb-4">
                            <i class="bi bi-briefcase display-4 text-success"></i>
                        </div>
                        <h5 class="card-title">Business Strategy</h5>
                        <p class="card-text">Developing and executing plans to achieve business goals.</p>
                        <a href="#" class="text-success">Know more →</a>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card h-100 text-center bg-dark text-white p-3">
                    <div class="card-body">
                        <div class="icon mb-4">
                            <i class="bi bi-bar-chart display-4 text-success"></i>
                        </div>
                        <h5 class="card-title">Research</h5>
                        <p class="card-text">Gathering and analyzing data to inform decision-making.</p>
                        <a href="#" class="text-success">Know more →</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MirandaProducts'
}
</script>

<style scoped>
.card {
    border: none;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
    transform: translateY(-10px);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
}

.icon {
    font-size: 3rem;
}
</style>