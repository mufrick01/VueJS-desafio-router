<template>
    <section class="container" id="productos">
    <div class="row">
    <!-- Contenido del componente -->
     <Card v-for="(product) in products" :key="product.id" :product="product"/>
  </div>
  </section>
</template>

<script>
import Card from './Card.vue';

export default {
  name: 'CardList',
  components:{
    Card
  },
  data() {
    return {
    };
  },
  props:{
      products:{
          type:Array,
          default:[],
          required: false,
      },
  },
  created(){
    
  }
};
</script>

<style scoped>
/* Estilos aquí */
</style>
