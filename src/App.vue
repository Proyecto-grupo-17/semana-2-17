<template>
  <div id="app">

    <div class="container-fluid">
<!-- se llama a la seccion noticias -->
          <page-noticias></page-noticias>
      </div>
     

  </div>
</template>

<script>
// se importa el componente de noticias
import PageNoticias from './components/PageNoticias.vue'

export default {
  name: 'App',
  components:{
//se agrega el componente de noticias
    PageNoticias
  },
  data(){

  }
}
</script>

