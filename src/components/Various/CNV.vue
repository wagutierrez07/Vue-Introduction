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
        <a>Comunicación No Violenta</a>
        <div class="container-info">
          <h1> Comunicación No Violenta - CNV</h1>
          <h4>Mejora tu comunicación, resuelve conflictos difíciles, ten relaciones de alta calidad, vive más plenitud en tu vida</h4>
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
    </div>
  </b-col>
  <b-col cols="6" sm="4">
             <b-card
    title="Curso de CNV"
    img-src="https://i.ytimg.com/vi/7yumreeVr-s/maxresdefault.jpg"
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
<li class="d-flex">A desarrollar tu inteligencia emocional y sus habilidades de comunicación interpersonal e intrapersonal</li>
<li class="d-flex">A resolver conflictos</li>
<li class="d-flex">A desarrollar tu capacidad de escucha y empatía</li>
<li class="d-flex">A transformar tus enojos en algo positivo y productivo</li>
<li class="d-flex">A cambiar patrones reactivos a patrones creativos</li>
<li class="d-flex">Las bases de la Comunicación No Violenta</li>
<li class="d-flex">A conocerte mejor a tí mismo y a los demás</li>
<li class="d-flex">A expresarte con claridad y asertividad</li>
<li class="d-flex">A entender de dónde surgen sentimientos negativos como la rabia y la culpabilidad y la frustración para salir de ellos</li>
<li class="d-flex">A pedir lo que necesitas de manera clara y asertiva</li>
<li class="d-flex">Estimular un nuevo lenguaje de vida por medio del proceso de Comunicación No Violenta del autor Marshall Rosenberg.</li>
<li class="d-flex">Obtener herramientas de autoconocimiento para reconocer su estilo comunicacional y el potencial de sus habilidades comunicativas.</li>
<li class="d-flex">Promover destrezas personales para aprovechar la capacidad de escucha activa, comunicación asertiva y empática.</li>
  </ul>
</div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Frontend',
         created () {
            document.title = "Curso gratis de Comunicacion no violenta";
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