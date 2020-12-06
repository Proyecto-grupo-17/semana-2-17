<template>
  
  <div id="app">

    <!-- Header con carrusel -->
    <header class="page-header">
      <seccion-header></seccion-header>
    </header>
        <div class="container-fluid">
<!-- se llama a la seccion noticias -->
          <page-noticias></page-noticias>
      </div>   
    
    <div> 
           <h5 class="text-center font-weight-bold font-xl">EQUIPO DE TRABAJO</h5> 
           <hr width="200" size="2" noshade="noshade" color=#ffa600>   
      </div>
    <div class="container-fluid">      
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
        descripcion: {
          edad: "24 años",
          profesion: "Ingeniero Físico - Universidad Nacional de Colombia",
          ciudad: "Bogotá D.C.",
          pasatiempos: "ver series o películas, jugar fútbol y estudiar programación"
          },
        rol: "Desarrollador backend",
        imagen: require(`@/assets/Daniel.jpeg`)
      },
      {
        codigo:2,
        nombre: "Stefannie Julieth Morales Plazas",
        descripcion: {
          edad: "22 años",
          profesion: "Técnica en Sistemas y Tecnóloga en Análisis y Desarrollo de Sistemas De Información - SENA",
          ciudad: "Bogotá D.C.",
          pasatiempos: "Leer"
          },
        rol: "Desarrollador backend",
        imagen: require(`@/assets/Stefannie.jpg`)
      },
      {
        codigo:3,
        nombre: "Mayra Alejandra Velásquez Ramos",
        descripcion: {
          edad: "33 años",
          profesion: "Ingeniera Catastral y Geodesta - Universidad Distrital Francisco José de Caldas",
          ciudad: "Bogotá D.C.",
          pasatiempos: "Leer, pasear con sus perros"
          },
        rol: "Desarrollador backend",
        imagen: require(`@/assets/Mayra.jpg`)
      },
      {
        codigo:4,
        nombre: "Héctor Leonardo Sosa Pinto",
        descripcion: {
          edad: "46 años",
          profesion: "Ingeniero Mecánico - Universidad Nacional de Colombia",
          ciudad: "Cali",
          pasatiempos: "Leer, escuchar música, ver series o películas"
          },
        rol: "Desarrollador backend",
        imagen: require(`@/assets/Hector.jpg`)
      },
      {
        codigo:5,
        nombre: "Andrés Miguel Ramírez Palacio",
        descripcion: {
          edad: "24 años",
          profesion: "Ingeniero Biomédico / Investigador - Universidad EIA",
          ciudad: "Medellin",
          pasatiempos: "Hacer deporte y salir a comer con mis amigos"
          },
        rol: "Desarrollador backend",
        imagen: require(`@/assets/Andres.png`)
      }]
    }
  }
</script>

