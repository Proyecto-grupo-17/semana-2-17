<template>
    <div>
        
            <div class="card text-white bg-dark">
                <div class="d-flex justify-content-center p-2">
                    <img v-bind:src= "member.imagen" class="img-responsive" height="192" width="192" alt="Fotografía del integrante">
                </div>
                <div class="card-body">
                    <h5 class="card-title">{{ member.nombre}}</h5>
                    <p class="card-text"> Edad: {{ member.descripcion.edad}}</p>
                    <p class="card-text"> Profesión: {{ member.descripcion.profesion}}</p>
                    <p class="card-text"> Ciudad Actual: {{ member.descripcion.ciudad}}</p>
                    <p class="card-text"> Pasatiempos: {{ member.descripcion.pasatiempos}}</p>
                    <p class="card-text"> Rol: {{ member.rol}}</p>
                    <p class="card-text"> Código: {{ member.codigo}}</p>
                </div>
                <div class="card-footer">
                    <small class="text-muted">Last updated 3 mins ago</small>
                </div>
            </div>
        
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
