<template>
    <section class="container" id="productos">
    <h1 class=" text-center">Nuestros Productos</h1>
    <div class="row">
    <!-- Contenido del componente -->
     <Card/>
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
