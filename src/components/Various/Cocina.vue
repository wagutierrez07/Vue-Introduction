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
        <a>Cocina</a>
        <div class="container-info">
          <h1> Curso completo de Cocina</h1>
          <h4>Aquí aprenderas a cocinar diferentes platillos, postres y comidas gourmet paso a paso</h4>
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
                <a> Esteban Segundo </a>
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
    title="Curso de cocina"
    img-src="https://corbuse.edu.mx/blog/wp-content/uploads/2016/09/CORBUSE-Cursos-de-cocina-basica-en-mexico.jpg"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      9,99 US$    </b-card-text>
 <b-card-text>Precio original19,99 US$    </b-card-text>
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
<li class="d-flex">Higiene alimentaria, análisis de riesgos y puntos críticos de control</li>
<li class="d-flex">Introducción a la cocina “la cocina moderna”</li>
<li class="d-flex">Operaciones preliminares</li>
<li class="d-flex">Las entradas</li>
<li class="d-flex">Los huevos</li>
<li class="d-flex">Las sopas y potajes “legumbres secas”</li>
<li class="d-flex">El arroz</li>
<li class="d-flex">Las pastas alimenticias</li>
<li class="d-flex">Las verduras y hortalizas</li>
<li class="d-flex">Las patatas</li>
<li class="d-flex">Las salsas y mantequillas</li>
<li class="d-flex">Los pescados</li>
<li class="d-flex">Los mariscos “moluscos, crustáceos y caracoles”</li>
<li class="d-flex">Las carnes de matadero</li>
<li class="d-flex">Los despojos</li>
<li class="d-flex">La caza</li>
<li class="d-flex">Canapés, sándwiches y platos combinados</li>
<li class="d-flex">Los quesos</li>
<li class="d-flex">Dirección y organización del departamento de cocina</li>
<li class="d-flex">Estudio y logística sobre menús y cartas</li>
<li class="d-flex">Regeneración y emplatado</li>
  </ul>
</div>

  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Cocina',
         created () {
            document.title = "Cursos gratis de cocina";
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
ul{
  margin-bottom: 1rem;
}
ul li{
  margin-bottom: 1rem;
}
</style>