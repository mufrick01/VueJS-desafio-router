<template>
  <div>
    <button class="btn btn-primary m-2">
        <router-link
        to="/"
        >
        <span class="text-white">
            GO HOME
        </span>
        </router-link>
    </button>
  </div>
</template>

<script>
export default {
  name: 'GoHomeButton',
  data() {
    return {
      // Datos aquí
    };
  },
  props:{
      propA:String,
      propB:{
          type:String,
          default:'default-value',
          required: true,
      },
  }
};
</script>

<style scoped>
/* Estilos aquí */
</style>
