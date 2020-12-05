<template>
  
  <div id="app">
    <!-- Header con carrusel -->
    <header class="page-header">
      <seccion-header></seccion-header>
    </header>
    
    <footer id="contact" class="page-footer font-small text-white" style="background-color: #662d80">
      <seccion-footer></seccion-footer>
    </footer>
    <!-- Footer -->
  </div>
</template>

<script>

import SeccionHeader from './components/SeccionHeader.vue'
import SeccionFooter from './components/SeccionFooter.vue'

export default {
  name: 'App',
  components:{
    SeccionHeader,
    SeccionFooter
  }
}
</script>

