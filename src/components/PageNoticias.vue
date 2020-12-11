<template>
<!-- inicia seccion noticias -->
    <div>
        <!-- primer container noticias -->
        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
            <div class="col-lg-6 col-xs-12" v-for="(movie,index) of movies" :key="index">
                <div class="alert alert-dark" role="alert">
        <div class="d-flex justify-content-center align-items-center">
            
            <div class="p-3">
                <img :src="movie.Poster" alt="movie poster">
            </div>
    
            <div class="p-2">
                <h2 align="center">{{movie.Title}}</h2>
                <hr>
                <p align="justify">
                ¿Es {{movie.Title}} un ejemplo de que los perros son nuestros<i><strong> "mejores amigos" </strong></i><br> 
                ¡La domesticación pudo haber ocurrido al final de la Edad de hielo!<br><br>
                Pontus Skoglund, coautor del estudio y miembro del Laboratorio de Genomas Antiguos del Instituto Crick de Londres, 
                le dijo a la BBC: <i><strong>"Nuestra relación con los perros es algo único, bastante particular...".</strong></i>
                 </p>
            </div>
            </div>   
            
            <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                <a class="btn btn-outline-info"
                :href="'https://www.imdb.com/title/' + movie.imdbID" target="_blank">Info</a>
            </div>
            </div>
        </div>
    </div>
<!-- segundo container noticias -->
        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
            <div class="col-lg-6 col-xs-12" v-for="(movi,index) of movis" :key="index">
                <div class="alert alert-light" role="alert">
        <div class="d-flex justify-content-center align-items-center">
            
            <div class="p-3">
                <img :src="movi.Poster" alt="movie poster">
            </div>
    
            <div class="p-2">
                <h2 align="center">{{movi.Title}}</h2>
                <hr>
                <p align="justify">
                <i><strong>¡Aprovecha el tiempo con tu mascota!</strong></i> {{movi.Title}} puede enseñarte como hacerlo!<br><br> 
                El aislamiento generado por la Covid-19 no solo ha modificado el diario vivir de los seres humanos, sino 
                también el de las mascotas. En el caso de los perros, aunque tienen la opción de salir a pasear con sus amos...
                 </p>
            </div>
            </div>   
            
            <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                <a class="btn btn-outline-info"
                :href="'https://www.imdb.com/title/' + movi.imdbID" target="_blank">Info</a>
            </div>
            </div>
        </div>
    </div>

</div>
<!-- termina seccion noticias -->
</template>

<script>

import axios from 'axios';

export default {
    // nombrar el componente de noticias
    name: 'PageNoticias',

    data(){
        return{
            //variables de noticias
            movies: null,
            movis: null

        }
    },
    //para consumir a la api en la seccion de noticias con axios
    mounted(){
        axios.get('http://www.omdbapi.com/?s=The+Secret+Life+of+Pets&type=movie&apikey=23daade9')
        .then(response => {
            (this.movies = response.data.Search.slice(0,2))
                console.log(this.movies)
            })
        axios.get('http://www.omdbapi.com/?s=Despicable+Me&type=movie&apikey=23daade9')
        .then(response => {
            (this.movis = response.data.Search.slice(0,2))
                console.log(this.movis)
            })
    }
    
}
</script>

<style scoped>

</style>