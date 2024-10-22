<template>
  <div>
    <h1 class="text-center m-0" style="font-size: 2.5rem">Nuestros producto principales</h1>
    <CardList :products="this.products" />
  </div>
</template>

<script>
import CardList from '@/components/CardList.vue';

// @ is an alias to /src

export default {
  components: {
    CardList
  },

  data() {
    const products = [
      {
        title: 'Bebidas',
        description: "Algunas bebidas refrescantes y deliciosas.",
        subtext1: 'Ideal para cualquier ocasión',
        subtext2: 'Disfruta de una experiencia refrescante',
        img: 'https://www.semana.com/resizer/v2/6CIKIETI2VFNZICHOAXJC7B7TU.jpg?auth=e60e391cd214804d0a36c9d729d19311de6f81ad0aef1c73d1c560f42b6c998d&smart=true&quality=75&width=1280',
        id: Date.now() + 1, // Asignar un ID único
      },
      {
        title: 'Colaciones',
        description: "Alimentos perfectos para picar entre horas.",
        subtext1: 'Rápidas y deliciosas',
        subtext2: 'Satisfacción al instante',
        img: 'https://26f1d75dec.cbaul-cdnwnd.com/84373def39cde354f9449d988cfc9bfb/system_preview_detail_200000006-274a9285e0-public/1290610415_141257511_8-Fastlunch-Delivery-Banqueteria-Colaciones-Almuerzos-Coffee-Breaks--1290610415.jpg',
        id: Date.now() + 2, // Asignar un ID único
      },
      {
        title: 'Desayunos',
        description: "Disfruta de un desayuno completo y nutritivo.",
        subtext1: 'Comienza bien tu día',
        subtext2: 'Energía para toda la mañana',
        img: 'https://www.divinacocina.es/wp-content/uploads/2016/01/huevos-revueltos-desayuno-2.jpg',
        id: Date.now() + 3, // Asignar un ID único
      },
    ];


    return {
      products
    }
  }
}
</script>
