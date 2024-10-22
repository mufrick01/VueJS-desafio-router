<template>
  <div class="col-sm-4 col-12 px-5 mb-4">
    <div class="card">
      <img :src="this.product.img" class="card-img-top" alt="colaciones" style="height: 250px; object-fit: cover;"/>
      <div class="card-body">
        <!-- titulo -->
        <h5 class="card-title fw-bold text-capitalize">{{ this.product.title }}</h5>
        <!-- texto -->
        <p class="card-text">
          {{ this.product.description }}
        </p>
      </div>
      <ul class="list-group list-group-flush">
        <li class="list-group-item">{{ this.product.subtext1 }}</li>
        <li class="list-group-item">{{ this.product.subtext2 }}</li>
      </ul>
      <div class="card-body">
        <!-- links -->
        <router-link :to="{
          name: 'ProductView',
          query: { product: JSON.stringify(product) }
        }" class="card-link">
          Ver más
        </router-link>
        <router-link to="/" class="card-link">Comprar</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  data() {
    return {
      // Datos aquí
    };
  },
  props: {
    product: {
      type: Object,
      default: {
        title: 'colaciones',
        description: "Some quick example text to build on the card title and make up the bulk of the card's content.",
        subtext1: 'Dapibus ac facilisis in',
        subtext2: 'Vestibulum at eros',
        img: 'https://26f1d75dec.cbaul-cdnwnd.com/84373def39cde354f9449d988cfc9bfb/system_preview_detail_200000006-274a9285e0-public/1290610415_141257511_8-Fastlunch-Delivery-Banqueteria-Colaciones-Almuerzos-Coffee-Breaks--1290610415.jpg',
        id: Date.now(),
      },
      require: false,
    },
  }
};
</script>

<style scoped>
/* Estilos aquí */
</style>
