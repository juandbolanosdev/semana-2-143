<template>

    
                    <div >
                        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
                            <div class="col-lg-6 col-xs-12 border" v-for ="(movie, index) of movies" :key="index">
                
                                <div class="d-flex justify-content-center align-items-center" >
               
                                        <div class="p-3">
                                            <img v-bind:src="movie.Poster" alt="imagen de pelicula">
                
                                        </div>
                                    
                                     
                                    <div class="p-2">
                                        <h2>{{movie.Title}}</h2>
                                        <hr>
                                        <h4>Año de estreno: {{movie.Year}}</h4>
                                         <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                                              
                                            <a :href="'https://www.imdb.com/title/' + movie.imdbID" class="btn btn-outline-info">link</a>
                                        </div>

                                    </div>
                                   
                                </div>
                            </div>

                        </div>
                    </div>
           
               


    
</template>

<script>
import axios from "axios";
export default {
  name: "SectionApi",
  data() {
    return {
      movies: null,
    };
  },

  mounted() {
    axios
      .get("http://www.omdbapi.com/?s=$lord&type=movie&apikey=b4f6d54d")
      .then((response) => (this.movies = response.data.Search.slice(0, 4)))
      .catch((error) => console.log(error));
  },
};
</script>

<style  scoped>
</style>