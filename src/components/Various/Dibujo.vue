<template>
  <div >
        <Navbar/>
<div class="container-background bg-dark">
 <b-aspect :aspect="aspect">
<b-row>
  <b-col cols="12" sm="8">
    <div class="component-data p-5">
      <div class="component-links">
        <router-link to="/Cursos">Cursos</router-link>
        &nbsp;
         <a>></a>
         &nbsp;
        <a>Curso de dibujo</a>
        <div class="container-info">
          <h1> Curso completo de dibujo - De cero a experto con ejercicios</h1>
          <h4>El mejor curso para aprender a dibujo con tanto a mano como con otros programas como Adobe Ilustrator, Paint Tool Sai, o GIMP</h4>
                  <div class="content-description">
            <span class="udlite-badge udlite-badge-bestseller udlite-heading-xs" data-purpose="badge">Lo más vendido</span>
            &nbsp;
            <span class="udlite-sr-only">Calificación: 4,7 de 5</span>
            &nbsp;
            <span>(35.000 callificaciones)</span>
            &nbsp;
            <span>145.179 estudiantes</span>
            <div class="content-creator">
              <span class="instructor-links">
                <span class="text-sm">Creado por: </span>
                <a> Juana Maria </a>
              </span>
              <div class="content-date">
                <span class="date">
                  <span>Fecha de creacion: 14/08/2021</span>
                </span>
                            &nbsp;
                <span class="language">
                  <span>Curso en español</span>
                </span>
                            &nbsp;
                <span class="subtitle">
                  <span>Español (Automatico)</span>
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </b-col>
  <b-col cols="6" sm="4">
                  <b-card
    title="Curso de dibujo"
    img-src="https://www.uni-ball.es/wp-content/uploads/2019/03/Cursos-dibujo.jpg"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      9,99 US$    </b-card-text>
 <b-card-text>Precio original 19,99 US$    </b-card-text>
 <b-card-text>Descuento 50 % de descuento    </b-card-text>
    <button class="btn btn-primary">Añadir al carrito</button>
    <br>
        <br>
        <button class="btn btn-success">Comprar</button>
  </b-card>
  </b-col>
</b-row>

 </b-aspect>

</div>
<div class="content-course">
  <h2 class="d-flex p-2">Lo que aprenderas</h2>
  <ul>
<li class="d-flex">Historia</li>
<li class="d-flex">Materiales</li>
<li class="d-flex">Postura y habitos</li>
<li class="d-flex">Inicio al dibujo artístico</li>
<li class="d-flex">Empezar a dibujar</li>
<li class="d-flex">Composición y equilibrio del dibujo</li>
<li class="d-flex">Descomposición en volúmenes</li>
<li class="d-flex">Teoría del color</li>
  </ul>
</div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Dibujo',
         created () {
            document.title = "Cursos gratis de dibujo";
        },
  components: {
    Navbar
  }
    
}
</script> 

<style>
img{
    height: 300px;
     width: 500px;
}
div.container-background {
      height: 400px;
  
}
div.component-data{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    text-align: left;
}
div.component-links{
  color: #fff;
  top: .1rem;
margin: .4rem;
}

</style>