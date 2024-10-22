<template>
    <div class="container d-flex flex-column">
        <h1>Product View</h1>
        <div class="card mx-auto my-5" style="width: 50%;">
            <img :src="this.product.img" class="card-img-top" alt="...">
            <div class="card-body">
                <h5 class="card-title text-capitalize">{{ this.product.title }}</h5>
                <p class="card-text">{{ this.product.description }}</p>
            </div>
            <ul class="list-group list-group-flush">
                <li class="list-group-item">{{ this.product.subtext1 }}</li>
                <li class="list-group-item">{{ this.product.subtext2 }}</li>
            </ul>
            <div class="card-body">
                <a href="#" class="card-link">Comprar</a>
            </div>
        </div>
    </div>
</template>

<script>
import { useRoute } from 'vue-router';

export default {
    components: {
    },
    data() {
        const route = useRoute();
        const product = JSON.parse(route.query.product);

        return { product };
    }
};
</script>

<style scoped>
/* Estilos aquí */
</style>