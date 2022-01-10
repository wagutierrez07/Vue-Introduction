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
          <h4>El mejor curso de carpinteria. Aprende la carpinteria y la ebanistería paso a paso como un profesional </h4>
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
    title="Curso de carpinteria"
    img-src="https://www.majofesa.com/wp-content/uploads/2017/03/muebles-de-madera-carpinteria-de-madera-maderas-valencia.jpg"
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
<li class="d-flex">Presentacion</li>
<li class="d-flex">Manejo de herramientas</li>
<li class="d-flex">Maquinaria adecuada</li>
<li class="d-flex">Ebanistería</li>
<li class="d-flex">Practica I: Afilado de herramientas</li>
<li class="d-flex">Practica II: Trabajar con madera</li>
<li class="d-flex">Practica III: Manejo del cepillo en la carpinteria</li>
<li class="d-flex">Conclusion</li>
  </ul>
</div>
  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Carpinteria',
         created () {
            document.title = "Cursos gratis de carpinteria";
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