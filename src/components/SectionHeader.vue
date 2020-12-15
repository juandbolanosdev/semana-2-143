<template>
    <div>
        <header class ="header">
        <!-- menu -->
        <section class="barra-superior">
           
            <nav class="navbar navbar-expand-lg sticky-top navbar-dark bg-dark">
                <a class="navbar-brand" href="#">Sprint 2</a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                  <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
                  <ul class="navbar-nav">
                    <li class="nav-item active">
                      <a class="nav-link" href="#">Inicio <span class="sr-only">(current)</span></a>
                    </li>
                    <li class="nav-item">
                      <a class="nav-link" href="#services">Servicios</a>
                    </li>
                    <li class="nav-item">
                      <a class="nav-link" href="#news">Noticias</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#team">Equipo</a>
                      </li>
                    
                  </ul>
                </div>
              </nav>

        <!-- Carousel -->

        <section class ="banner">

        <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
            <ol class="carousel-indicators">
              <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
              <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
              <li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
            </ol>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="imagen_principal.jpg" class="d-block w-100" alt="Baner_imagen_1">
                <div class="carousel-caption d-none d-md-block">
                  <h5 class="text-body" >Biblioteca pública MAD</h5>
                  <p class="text-muted">Bibloteca pública para todos los colombianos.</p>
                </div>
              </div>
              <div class="carousel-item">
                <img src="imagen_banner2.jpg" class="d-block w-100" alt="Baner_imagen_2">
                <div class="carousel-caption d-none d-md-block">
                  <h5>Libros</h5>
                  <p>La mejor selección de libros, para todas las edades.</p>
                </div>
              </div>
              <div class="carousel-item">
                <img src="banner_3.png" class="d-block w-100" alt="Baner_imagen_3">
                <div class="carousel-caption d-none d-md-block">
                  <h5>Comunidad</h5>
                  <p>Estamos para servir a la comunidad de lectores.</p>
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

        </section>
        
        </section>

    </header>
    </div>
</template>
<script>
export default {
    name:'SectionHeader'
    
}
</script>
<style lang="stylus" scoped>

</style>