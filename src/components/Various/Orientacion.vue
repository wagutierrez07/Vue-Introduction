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
        <a>Orientacion vocacional</a>
        <div class="container-info">
          <h1> Orientación vocacional: elegir a conciencia </h1>
          <h4>El curso que ha ayudado a más de 1,000 jóvenes a tener claridad sobre su elección de carrera universitaria</h4>
                  <div class="content-description">
            <span class="udlite-badge udlite-badge-bestseller udlite-heading-xs" data-purpose="badge">Lo más vendido</span>
            &nbsp;
            <span class="udlite-sr-only">Calificación: 4,7 de 5</span>
            &nbsp;
            <span>(35.000 callificaciones)</span>
            &nbsp;
            <span>145.179 estudiantes</span>
            iv class="content-creator">
              <span class="instructor-links">
                <span class="text-sm">Creado por: </span>
                <a> Walter gutierrez </a>
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
  </b-col>
  <b-col cols="6" sm="4">
             <b-card
    title="Orientacion vocacional"
    img-src="https://logrosperu.com/files/articulos/medianas/test_vocacional.png"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      9,99 US$    </b-card-text>
 <b-card-text>Precio original 19,99 US$    </b-card-text>
 <b-card-text>Descuento50 % de descuento    </b-card-text>
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
<li class="d-flex">¿Qué es el proceso de Orientación Vocacional?</li>
<li class="d-flex">Obstáculos que dificultan el proceso de elección a la hora de elaborar proyectos no solo a nivel educativo o laboral</li>
<li class="d-flex">Análisis FODA</li>
<li class="d-flex">El proceso de elección basado en la práctica del Mindfulness</li>
<li class="d-flex">Aspectos teóricos de la Orientación Vocacional</li>
<li class="d-flex">Interrogantes para reflexionar sobre la actual relación con los proyectos actuales y futuros</li>
<li class="d-flex">Elegir una profesión</li>
<li class="d-flex">Hacer una planeación de vida y carrera</li>
<li class="d-flex">Elegir una ocupación</li>
  </ul>
</div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'SQL',
         created () {
            document.title = "Cursos gratis de orientacion vocacional";
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