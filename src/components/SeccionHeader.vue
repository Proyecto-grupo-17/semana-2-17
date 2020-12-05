<template>
  <div>
      <nav class="navbar navbar-expand-lg sticky-top"
        style="background-color: #662d80">
        <a class="navbar-brand text-light" href="#navBarNav ">
          <h3>
            <b> MINTIC Pets</b>
          </h3>
        </a>
        <div
          class="navbar-collapse navbar-fixed-top justify-content-end"
          id="navbarNav ">
          <ul class="navbar-nav">
            <li class="nav-item active">
              <a class="nav-link text-light" href="# "
                >Inicio <span class="sr-only">(current)</span></a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link text-light" href="#news ">Noticias</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-light" href="#team ">Miembros</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-light" href="#contact ">Contacto</a>
            </li>
          </ul>
        </div>
      </nav>
      <!-- Carrousel -->
    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
      <ol class="carousel-indicators">
        <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="3" class=""></li>
      </ol>
      <div class="carousel-inner">
        <div class="carousel-item active" >
          <img src="../assets/pets.jpg" class="img-responsive" alt="" height="400" width="100%">
          <div class="carousel-caption d-md-block">
              <h2 style="opacity: 100%;">Nuestros servicios</h2>
          </div>
        </div>
        <div class="carousel-item">
          <img src="../assets/consulta.jpg" class="img-responsive" alt="" height="400" width="100%">
          <div class="carousel-caption d-md-block " style="background-color:#662d80; opacity: 0.8;">
            <h5>Consulta Médica</h5>
            <p>¡Te brindamos un diagnóstico claro y el tratamiento ideal para tu mascota! En nuestra red de clínicas
              veterinarias contamos con médicos expertos en diferentes disciplinas y equipos de última tecnología que
              nos permiten explicarte de una manera clara qué sucede con la salud de tu mascota y cómo la podemos
              mejorar!</p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="../assets/labclinic.jpg" class="img-responsive" alt="" height="400" width="100%">
          <div class="carousel-caption d-md-block" style="background-color:#662d80; opacity: 0.8;">
            <h5>Laboratorio Clínico</h5>
            <p>¡Aquí no tienes de qué preocuparte! En nuestro hospital contamos con equipos de laboratorio de última
              generación que nos permiten desarrollar pruebas y obtener resultados en minutos, así logramos un
              diagnóstico eficaz y un tratamiento oportuno para tu mascota!</p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="../assets/hospitalizacióncvz.jpg" class="img-responsive" alt="" height="400" width="100%">
          <div class="carousel-caption d-md-block" style="background-color:#662d80; opacity: 0.8;">
            <h5>Hospitalización y Clínica</h5>
            <p>¡Contamos con todo lo necesario para la recuperación de tu mascota: fluidos por vía intravenosa,
              monitoreo profesional, nutrición y administración de los fármacos. Cirugías básicas y procedimientos
              avanzados como cardiovasculares y ortopédicos. Así tu mascota podrá estar en un ambiente tranquilo y
              seguro durante su recuperación.!</p>
          </div>
        </div>
      </div>
      <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "SeccionHeader",
  props: {
      imagen : Image
  }
};
</script>

<style scoped>
</style>
