<template>
  <div class="about d-flex flex-column">
    <GoHomeButton />
    <h1 class="text-center">Ven a visitarnos</h1>
    <section class="row p-5 mx-auto">
      <article class="col-12 col-lg-8 text-center text-lg-start mb-5">  
        <h4 class="fw-bold">Nos encontramos en: </h4>
        <span>Dirección falsa, calle no existe #i</span>
        <h4 class="fw-bold mt-2">Teléfono : </h4>
        <span>+420 1904 1985</span>
      </article>
      <article class="col-12 col-lg-4 d-flex justify-content-center">  
        <img src="https://i.blogs.es/ade34e/google-maps-portada-trafico/1366_2000.jpg" alt="" class="circle" style="width: 300px; height: 300px;">
      </article>
    </section>
  </div>
</template>

<script>
import GoHomeButton from '@/components/GoHomeButton.vue';

export default {
  components: {
    GoHomeButton
  }
};
</script>

<style scoped>

.circle{
  border-radius: 50%;
  object-fit: cover;
  object-position: center;
}
/* Estilos aquí */
</style>
