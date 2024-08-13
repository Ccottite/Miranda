<template>
    <div class="container py-5">
        <div class="row">
            <!-- Sección de Imágenes y Descripción -->
            <div class="col-lg-6 d-flex align-items-center">
                <div id="product-display">
                    <img :src="products[currentProduct].image" alt="Product Image" class="img-fluid mb-4">
                    <h3>{{ products[currentProduct].title }}</h3>
                    <p>{{ products[currentProduct].description }}</p>
                </div>
            </div>

            <!-- Sección de Lista de Puntos -->
            <div class="col-lg-6 d-flex align-items-center">
                <ul id="product-list" class="list-unstyled">
                    <li v-for="(product, id) in products" :key="id" :class="{ active: currentProduct === id }"
                        @click="changeProduct(id)">
                        <i class="bi bi-circle-fill"></i> {{ product.title }}
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MirandaNew',
    data() {
        return {
            currentProduct: '1',
            products: {
                '1': {
                    image: 'product1.jpg',
                    title: 'Product 1 Title',
                    description: 'This is a description of Product 1. It highlights the key features and benefits of this product.'
                },
                '2': {
                    image: 'product2.jpg',
                    title: 'Product 2 Title',
                    description: 'This is a description of Product 2. It highlights the key features and benefits of this product.'
                },
                '3': {
                    image: 'product3.jpg',
                    title: 'Product 3 Title',
                    description: 'This is a description of Product 3. It highlights the key features and benefits of this product.'
                },
                '4': {
                    image: 'product4.jpg',
                    title: 'Product 4 Title',
                    description: 'This is a description of Product 4. It highlights the key features and benefits of this product.'
                }
            }
        }
    },
    methods: {
        changeProduct(productId) {
            this.currentProduct = productId;
        }
    }
}
</script>

<style scoped>
/* Aquí puedes poner los estilos que mencioné anteriormente o cualquier otro estilo que necesites */
#product-display {
    text-align: center;
}

#product-title {
    font-size: 1.5rem;
    margin-top: 20px;
}

#product-description {
    font-size: 1rem;
    color: #666;
}

#product-list li {
    font-size: 1.25rem;
    padding: 10px;
    cursor: pointer;
    transition: color 0.3s;
}

#product-list li.active,
#product-list li:hover {
    color: #28a745;
}

#product-list li i {
    margin-right: 10px;
    color: #28a745;
}
</style>