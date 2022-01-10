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
        <a>Reparacion de equipos informaticos</a>
        <div class="container-info">
          <h1> Curso completo de Reparacion de equipos informaticos</h1>
          <h4>Soporte Técnico a nuestro computador, PC, ordenador. Armado y Desarme. Laptops, Notebook, Ordenador Portátil. Hardware y Software. Instalación Windows 10, 8.1 y 7 y mucho mas</h4>
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
    title="Curso de reparacion de equipos informaticos"
    img-src="https://x3jme3vmctf3dmlkql5tzx17-wpengine.netdna-ssl.com/wp-content/uploads/2020/10/reparaciones-electronicas.jpg"
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
<li class="d-flex">Funcionamiento del Computador</li>
<li class="d-flex">Desarmar y Armar Computadoras</li>
<li class="d-flex">Como ingresar al BIOS, modificar valores y eliminar contraseña.</li>
<li class="d-flex">Instalación de Windows 7, 8.1 y 10</li>
<li class="d-flex">Descargar imágenes ISO Windows y Office</li>
<li class="d-flex">Instalación y actualización de Drivers o Controladores</li>
<li class="d-flex">Eliminación de Virus y otras amenazas</li>
<li class="d-flex">Mantenimiento Preventivo y Correctivo</li>
<li class="d-flex">Partes de un Computador Portátil</li>
<li class="d-flex">Consejos antes de Desarmar un Computador Portátil</li>
<li class="d-flex">Desarme de Computadoras Portátiles</li>
<li class="d-flex">Reemplazar Pantallas</li>
<li class="d-flex">Descargar Imágenes ISO</li>
<li class="d-flex">Programas Esenciales para un Computador Portátil</li>
<li class="d-flex">Java EE (Enterprise Edition)</li>
<li class="d-flex">Optimizar un Computador Portátil</li>
<li class="d-flex">Ampliar la Memoria RAM a un Computador Portátil</li>
<li class="d-flex">Cuidados del Disco Duro</li>
<li class="d-flex">Herramientas de Particiones</li>
<li class="d-flex">Reparación de Fallas Físicas en Discos Duros</li>
<li class="d-flex">Formateo de Bajo Nivel</li>
<li class="d-flex">Recuperación de Archivos</li>
<li class="d-flex">Creación de Pendrive MultiBoot</li>
<li class="d-flex">Copias de Seguridad de Windows, Particiones y Archivos</li>
<li class="d-flex">Partición de Discos Duros</li>
<li class="d-flex">Herramientas para Diagnóstico de Discos Duros</li>
<li class="d-flex">Reparación de Fallas Lógicas en Discos Duros</li>
  </ul>
</div>

  </div>
</template>

<script>

import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Reparacion',
         created () {
            document.title = "Cursos gratis de reparacion de equipos";
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