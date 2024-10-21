<template>
  <Navbar />
  <router-view style="margin-top: 100px;"/>
  <medios-pago/>
  <Footer/>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'
import MediosPago from '@/components/MediosPago.vue'

export default {
  name: 'HomeView',
  components: {
    Navbar,
    Footer,
    MediosPago
  }
}
</script>
