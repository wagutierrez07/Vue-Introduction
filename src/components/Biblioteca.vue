<template>
    <div>
    <Navbar/>
    <h4>"Sólo el conocimiento que llega desde dentro es el verdadero conocimiento."</h4>
    <h4>Sócrates (470 AC-399 AC) Filósofo griego.</h4>
      <div class="content-library">
        <div class="content-library-information">
          <h2>Catalogo de libros</h2>
          <b-row>
            <b-col>
              <div class="image">
                  <img src="https://www.lawebdelprogramador.com/pdf/files/1499030563_programacion.jpg">
                </div>
                <div class="title">
                  <a>Introduccion a la programacion</a>
                </div>
                </b-col>
            <b-col>
              <div class="image">
                  <img src="https://www.pdf-manual.es/documents/covers/0150-introduccion-a-la-programacion-web.pdf.png">
                </div>
                <div class="title">
                  <a>Introduccion a la programacion web</a>
                </div>
                </b-col>
            <b-col>
              <div class="image">
                  <img src="https://olcovers2.blob.core.windows.net/coverswp/2015/12/Introduccion-a-la-programacion-en-C-OpenLibra.png">
                </div>
                <div class="title">
                  <a>Introduccion a la programacion en C</a>
                </div>
                </b-col>
            <b-col>
              <div class="image">
                  <img src="https://www.lawebdelprogramador.com/pdf/files/1540560278_1NTR0DUCC10N%204%20L4%209R06R4M4C10N%20C0N%20J4V4-97.jpg">
                </div>
                <div class="title">
                  <a>Introduccion a la programacion Java</a>
                </div>
                </b-col>
          </b-row>
          &nbsp;
          <b-row>
            <b-col>
              <div class="image">
                  <img src="https://olcovers2.blob.core.windows.net/coverswp/2016/06/introduccion-programacion-python-3-OpenLibra.gif">
                </div>
                <div class="title">
                  <a>Introduccion a la programacion Python</a>
                </div>
            </b-col>
            <b-col>
                <div class="image">
                  <img src="https://www.lawebdelprogramador.com/pdf/files/1622984517_Curso_SQL-84.jpg">
                </div>
                <div class="title">
                  <a>Introduccion a SQL</a>
                </div>
            </b-col>
            <b-col>
                  <div class="image">
                  <img src="https://imgv2-2-f.scribdassets.com/img/document/438020882/original/8e331c1455/1619543810?v=1">
                </div>
                <div class="title">
                  <a>Introduccion al frontend y el backend</a>
                </div>
            </b-col>
            <b-col>
                                <div class="image">
                  <img src="https://image.isu.pub/140512182124-1ad6ec26980ed165609b205f3ecc804d/jpg/page_1.jpg">
                </div>
                <div class="title">
                  <a>Introduccion a las redes y servidores</a>
                </div>
            </b-col>
          </b-row>
        </div>
      </div>
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
      document.title = "Biblioteca";
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

img{
  width: 180px;
}
</style>