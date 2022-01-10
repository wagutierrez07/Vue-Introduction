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
        <a>Java</a>
        <div class="container-info">
          <h1> Curso completo de Java - De cero a experto con ejercicios</h1>
          <h4>El mejor curso de Java, aquí aprenderas POO, JDBC, Servlets, JavaEE, Web Services, JSF, EJB, JPA, PrimeFaces, Hibernate, Spring, Struts y mucho mas!</h4>
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
                <a> Adriana Castillo </a>
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
    title="Curso Java"
    img-src="https://i.blogs.es/53044d/java/1366_521.jpg"
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
<li class="d-flex">Fundamentos de programacion</li>
<li class="d-flex">Estructuras basicas</li>
<li class="d-flex">Condicionales</li>
<li class="d-flex">Bucles</li>
<li class="d-flex">Arrays</li>
<li class="d-flex">Funciones</li>
<li class="d-flex">POO</li>
<li class="d-flex">Clases</li>
<li class="d-flex">Herencia</li>
<li class="d-flex">Polimorfismo</li>
<li class="d-flex">Java Swing</li>
<li class="d-flex">Interfaces Graficas</li>
<li class="d-flex">Despliegue de archivos .Jar</li>
<li class="d-flex">Threads</li>
<li class="d-flex">Java EE (Enterprise Edition)</li>
<li class="d-flex">Threads</li>
<li class="d-flex">JDBC</li>
<li class="d-flex">JSP (Java Server Pages)</li>
  </ul>
</div>

  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Java',
         created () {
            document.title = "Cursos gratis de Java";
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