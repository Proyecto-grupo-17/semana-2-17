<template>
  
  <div id="app">

    <!-- Header con carrusel -->
    <header class="page-header">
      <seccion-header></seccion-header>
    </header>
<!-- seccion de noticias -->
      <div id="news" class="container-fluid">
        <page-noticias></page-noticias>
      </div>   
    
    <div class="container-fluid" id="team">      
      <div class="row justify-content-center mb-5" >
        
        <div class="col md-5"  v-for="(member, index) of team" :key="index" >
          <TeamCard :member = "member"></TeamCard>
        </div>
      </div>
    </div>

    
    <footer id="contact" class="page-footer font-small text-white" style="background-color: #662d80">
      <seccion-footer></seccion-footer>
    </footer>
    <!-- Footer -->
  </div>
</template>
<script>
// se importa el componente de noticias
import PageNoticias from './components/PageNoticias.vue'
import SeccionHeader from './components/SeccionHeader.vue'
import SeccionFooter from './components/SeccionFooter.vue'
import TeamCard from './components/TeamCard.vue'

export default {
  name: 'App',
  components:{
    PageNoticias,
    SeccionHeader,
    SeccionFooter,
    TeamCard
    },
  data(){
    return{
      title: 'Vivo dentro del VUE',
      team: [
      {
        codigo:1,
        nombre: "Daniel Felipe Martínez Vizcaino",
        descripcion: "24 años, Ingeniero Físico - Universidad Nacional de Colombia, Bogotá D.C., ver series o películas, jugar fútbol y estudiar programación",
        rol: "Desarrollador backend",
        image: require(`@/assets/Daniel.jpeg`)
      },
      {
        codigo:2,
        nombre: "Stefannie Julieth Morales Plazas",
        descripcion: "22 años, Técnica en Sistemas y Tecnóloga en Análisis y Desarrollo de Sistemas De Información - SENA, Bogotá D.C., Leer",
        rol: "Desarrollador backend",
        image: require(`@/assets/Stefannie.jpg`)
      },
      {
        codigo:3,
        nombre: "Mayra Alejandra Velásquez Ramos",
        descripcion: "33 años, Ingeniera Catastral y Geodesta - Universidad Distrital Francisco José de Caldas, Bogotá D.C., Leer, pasear con sus perros",
        rol: "Desarrollador backend",
        image: require(`@/assets/Mayra.jpg`)
      },
      {
        codigo:4,
        nombre: "Héctor Leonardo Sosa Pinto",
        descripcion: "46 años, Ingeniero Mecánico - Universidad Nacional de Colombia, Cali, Leer, escuchar música, ver series o películas",
        rol: "Desarrollador backend",
        image: require(`@/assets/Hector.jpg`)
      },
      {
        codigo:5,
        nombre: "Andrés Miguel Ramírez Palacio",
        descripcion: "24 años, Ingeniero Biomédico / Investigador - Universidad EIA, Medellin,Hacer deporte y salir a comer con mis amigos",
        rol: "Desarrollador backend",
        image: require(`@/assets/Andres.png`)
      }]
    }
  }
}
</script>

