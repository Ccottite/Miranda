<template>
    <div class="contact-container">
        <h2>Contacto</h2>
        <form @submit.prevent="handleSubmit">
            <div class="form-group">
                <label for="name">Nombre:</label>
                <input type="text" id="name" v-model="form.name" required placeholder="Nombre completo" />
            </div>

            <div class="form-group">
                <label for="email">Correo Electrónico:</label>
                <input type="email" id="email" v-model="form.email" required placeholder="Correo electronico" />
            </div>
            <div class="form-group">
                <label for="text">Sujeto</label>
                <input type="text" id="text" v-model="form.text" required placeholder="Indique el motivo" />
            </div>

            <div class="form-group">
                <label for="message">Mensaje:</label>
                <textarea id="message" v-model="form.message" rows="4" required></textarea>
            </div>

            <button type="submit">Enviar</button>

            <div v-if="statusMessage" class="status-message">
                {{ statusMessage }}
            </div>
        </form>
    </div>
</template>

<script>
export default {
    data() {
        return {
            form: {
                name: '',
                email: '',
                message: ''
            },
            statusMessage: ''
        };
    },
    methods: {
        handleSubmit() {
            // Aquí puedes manejar el envío del formulario.
            // Por ejemplo, enviarlo a un servidor o una API.
            // Para este ejemplo, simplemente limpiamos el formulario y mostramos un mensaje de éxito.

            // Simular un envío exitoso
            setTimeout(() => {
                this.statusMessage = '¡Mensaje enviado con éxito!';
                this.form.name = '';
                this.form.email = '';
                this.form.message = '';
            }, 1000);
        }
    }
};
</script>

<style scoped>
.contact-container {
    max-width: 600px;
    margin: 0 auto;
    padding: 1rem;
}

.form-group {
    margin-bottom: 1rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.5rem;
}

.form-group input,
.form-group textarea {
    width: 100%;
    padding: 0.5rem;
    border: 1px solid #ddd;
    border-radius: 4px;
}

button {
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 4px;
    background-color: #007bff;
    color: #fff;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

.status-message {
    margin-top: 1rem;
    color: green;
}
</style>

<style></style>