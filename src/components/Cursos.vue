<template>
 
<div>
          <Navbar/>
    <div class="d-flex align-items-center mb-3">
      <b-progress class="w-100" :max="maxLoadingTime" height="1.5rem">
        <b-progress-bar :value="loadingTime" :label="`${((loadingTime / maxLoadingTime) * 100).toFixed(2)}%`"></b-progress-bar>
      </b-progress>

      <b-button class="ml-3" @click="startLoading()">Reload</b-button>
    </div>

    <b-skeleton-wrapper :loading="loading">
      <template #loading>
        <b-card>
          <b-skeleton width="85%"></b-skeleton>
          <b-skeleton width="55%"></b-skeleton>
          <b-skeleton width="70%"></b-skeleton>
        </b-card>
      </template>

      <b-container>
          <h1>Cursos adicionales</h1>
    <b-row>
      <b-col>
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
      En este curso aprenderas conceptos basicos de dibujo y practicas
    </b-card-text>

     <router-link to="/Dibujo">About</router-link>
  </b-card>
</b-col>
      <b-col>
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
      Curso especializado de cocina en el cual aprenderas a hacer diversos platillos
    </b-card-text>
    <router-link to="/Cocina">About</router-link>
  </b-card>
      </b-col>
      <b-col>
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
      Aprende la carpinteria y la ebanistería paso a paso como un profesional
    </b-card-text>

    <router-link to="/Carpinteria">About</router-link>
  </b-card>
      </b-col>
    </b-row>
      </b-container>
      <b-container>

        <b-row>
          <b-col>
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
    Aprende a como reparar y hacer mantenimiento y a a dar soporte técnico a equipos de computo o computadoras
    </b-card-text>

    <router-link to="/Reparacion">About</router-link>
  </b-card>
          </b-col>
          <b-col>
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
 Durante el curso de orientación vocacional podrás decidir la carrera universitaria para ti.
    </b-card-text>

          <router-link to="/Orientacion">About</router-link>
  </b-card>
          </b-col>
          <b-col>
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
      Descubre la comunicación no violenta como nuevo lenguaje de vida. Basada en los conceptos de Marshall Rosenberg
    </b-card-text>

     <router-link to="/CNV">About</router-link>
  </b-card>
          </b-col>
        </b-row>
      </b-container>
    </b-skeleton-wrapper>
  </div>

</template>

<script>
import Navbar from '@/components/Navbar.vue'
export default {
  name: 'Cursos',
  components: {
    Navbar
  },
      data() {
      return {
        loading: false,
        loadingTime: 0,
        maxLoadingTime: 3
      }
    },
    watch: {
      loading(newValue, oldValue) {
        if (newValue !== oldValue) {
          this.clearLoadingTimeInterval()

          if (newValue) {
            this.$_loadingTimeInterval = setInterval(() => {
              this.loadingTime++
            }, 1000)
          }
        }
      },
      loadingTime(newValue, oldValue) {
        if (newValue !== oldValue) {
          if (newValue === this.maxLoadingTime) {
            this.loading = false
          }
        }
      }
    },
    created() {
      this.$_loadingTimeInterval = null,
      document.title = "Cursos adicionales";
    },
    mounted() {
      this.startLoading()
    },
    methods: {
      clearLoadingTimeInterval() {
        clearInterval(this.$_loadingTimeInterval)
        this.$_loadingTimeInterval = null
      },
      startLoading() {
        this.loading = true
        this.loadingTime = 0
      }
    }
}
</script>
<style>
b-img{
      height: 300px;
     width: 400px;
}
</style>