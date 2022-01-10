<template>
  <div >
        <Navbar/>
<div class="container-background bg-dark">
 <b-aspect :aspect="aspect">
<b-row>
  <b-col cols="12" sm="8">
    <div class="component-data p-5">
      <div class="component-links">
        <router-link to="/">Cursos</router-link>
        &nbsp;
         <a>></a>
         &nbsp;
        <a>Desarrollo Frontend</a>
        <div class="container-info">
          <h1> Curso completo de desarrollo Backend  - De cero a experto con ejercicios</h1>
          <h4>El mejor curso para aprender a trabajar con HTML, CSS y JavaScript, tambien aprenderas a manejar frameworks y librerias como React, Angular, Bootstrap, Ember, Vue, y mucho mas!</h4>
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
                <a> Christian Nuñez </a>
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
    title="Curso Frontend"
    img-src="http://www.cursosgis.com/wp-content/uploads/2017/06/lenguajes_1.png"
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
<li class="d-flex">Servidor local</li>
<li class="d-flex">Cómo funciona la web</li>
<li class="d-flex">Introducción a HTML</li>
<li class="d-flex">Introducción a CSS</li>
<li class="d-flex">Practica de diseño I</li>
<li class="d-flex">Etiquetas de diseño</li>
<li class="d-flex">Introduccion a JavaScript</li>
<li class="d-flex">Funciones con JavaScript</li>
<li class="d-flex">Preparar AJAX y formulario JSON</li>
<li class="d-flex">Practica de diseño II</li>
<li class="d-flex">Bootstrap</li>
<li class="d-flex">Ejecucion Offline</li>
<li class="d-flex">Diseño responsive</li>
<li class="d-flex">Practica de diseño III</li>
<li class="d-flex">Introduccion a los Frameworks</li>
<li class="d-flex">Desarrollo de SPA</li>
<li class="d-flex">Proyecto</li>
  </ul>
</div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Frontend',
         created () {
            document.title = "Cursos gratis de desarrollo frontend";
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