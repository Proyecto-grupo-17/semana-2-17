<template>
  <div>
      <!-- Footer Text -->
      <div class="container-fluid text-center text-md-left">
        <!-- Grid row -->
        <div class="row">
          <!-- Grid column -->
          <div class="col-md-6 mt-md-0 mt-3">
            <!-- Content -->
            <h5 class="text-uppercase font-weight-bold">Motivación</h5>
            <br />
            <p>
              La siguiente pagina web es desarrollada por el equipo 17 de MINTIC
              2020, trata de una plantilla de una clínica veterinaria. La pagina
              se divide en 5 secciones: La sección superior, la sección de
              servicios, la sección de noticias, la sección del equipo y la
              sección footer. Cada sección fue desarrollada por un integrante
              del grupo. Todo esto con el objetivo de cumplir con el reto 1 del
              ciclo 3.
            </p>
            <span> Repositorio: </span>
            <br />
            <a
              class="badge badge-light"
              href="https://github.com/Proyecto-grupo-17/semana-1-17"
              >https://github.com/Proyecto-grupo-17/semana-1-17</a
            >
          </div>
          <!-- Grid column -->

          <hr class="clearfix w-100 d-md-none pb-3" />

          <!-- Grid column -->
          <div class="col-md-6 mb-md-0 mb-3">
            <!-- Content -->
            <h5 class="text-uppercase font-weight-bold">Contacto</h5>
            <!-- Form -->
            <form>
              <div class="form-group d-flex align-items-center">
                <label for="nombre" class="col-sm-2 col-form-label"
                  >Nombre</label
                >
                <div class="col-sm-10">
                  <input
                    type="text"
                    class="form-control form-control-sm w-75"
                    id="nombre"
                  />
                </div>
              </div>
              <div class="form-group d-flex align-items-center">
                <label for="correo" class="col-sm-2 col-form-label"
                  >Correo</label
                >
                <div class="col-sm-10">
                  <input
                    type="email"
                    class="form-control form-control-sm w-75"
                    id="correo"
                    placeholder="username@domain.com"
                  />
                </div>
              </div>
              <div class="form-group d-flex align-items-start">
                <label for="Mensaje" class="col-sm-2 col-form-label"
                  >Mensaje</label
                >
                <div class="col-sm-10">
                  <textarea
                    class="form-control form-control-sm w-75"
                    id="Mensaje"
                    rows="5"
                  ></textarea>
                </div>
              </div>
              <div class="form-group d-flex align-items-center">
                <div class="col-sm-10">
                  <button class="btn btn-light" type="submit">Submit</button>
                </div>
              </div>
            </form>
          </div>
          <!-- Grid column -->
        </div>
        <!-- Grid row -->
      </div>
      <!-- Footer Text -->

      <!-- Copyright -->
      <div class="footer-copyright text-center py-3">
        © 2020 Copyright: Equipo 17
      </div>
      <!-- Copyright -->
  </div>
</template>

<script>
export default {
  name: "SeccionFooter",
  props: {},
};
</script>

<style scoped>
</style>