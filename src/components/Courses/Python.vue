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
        <a>Python</a>
        <div class="container-info">
          <h1> Curso completo de Python - De cero a experto con ejercicios</h1>
          <h4>El mejor curso de Python, aquí aprenderas POO, Web con Django, Flask, Jinja, SQL Alchemy, Postgresql, PyCharm! </h4>
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
                <a> Johana Martiñon </a>
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
    title="Curso Python"
    img-src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQvrs2uOMOO0j9CL69OFbToc0K4o4PaZAoxogixiPYHYV7ZCKCNqdSYOFgpCggbGFSg7VI&usqp=CAU"
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
<li class="d-flex">Fundamentos de programacion</li>
<li class="d-flex">Sintaxis</li>
<li class="d-flex">Estructuras basicas</li>
<li class="d-flex">Estructuras de control</li>
<li class="d-flex">Condicionales</li>
<li class="d-flex">Bucles</li>
<li class="d-flex">Arrays</li>
<li class="d-flex">Funciones</li>
<li class="d-flex">Archivos secuenciales</li>
<li class="d-flex">POO</li>
<li class="d-flex">Clases</li>
<li class="d-flex">Herencia</li>
<li class="d-flex">Polimorfismo</li>
<li class="d-flex">Librerias</li>
<li class="d-flex">Plantillas</li>
<li class="d-flex">Grafos</li>
  </ul>
</div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Python',
         created () {
            document.title = "Cursos gratis de Python";
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