<template>
 
  
<div>
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
          <h1>Bienvenido a mi sitio</h1>
    <b-row>
      <b-col>
        <b-card
    title="Curso C++"
    img-src="https://i.ytimg.com/vi/dJzLmjSJc2c/maxresdefault.jpg"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      Aqui te mostraremos como funciona el famoso lenguaje C++
    </b-card-text>

     <router-link to="/C++">About</router-link>
  </b-card>
</b-col>
      <b-col>
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
      Aqui te mostraremos como funciona el famoso lenguaje Java
    </b-card-text>

    <router-link to="/Java">About</router-link>
  </b-card>
      </b-col>
      <b-col>
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
      Aqui te mostraremos como funciona el famoso lenguaje Python
    </b-card-text>

    <router-link to="/Python">About</router-link>
  </b-card>
      </b-col>
    </b-row>
      </b-container>
      <b-container>
        <h2>Estudios Web</h2>
        <b-row>
          <b-col>
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
      Aqui te mostraremos como funciona el desarrollo frontend, con HTML, CSS y JavaScript, junto a frameworks y librerias para trabajar
    </b-card-text>

    <router-link to="/Frontend">About</router-link>
  </b-card>
          </b-col>
          <b-col>
             <b-card
    title="Curso Backend"
    img-src="https://www.campusmvp.es/recursos/image.axd?picture=/2021/1T/lenguajes-programacion-back-end.png"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      Aqui te mostraremos como funciona el desarrollo frontend, principalmente con PHP, junto a frameworks y librerias para trabajar
    </b-card-text>

          <router-link to="/Backend">About</router-link>
  </b-card>
          </b-col>
          <b-col>
             <b-card
    title="Curso de base de datos"
    img-src="https://revistadigital.inesem.es/informatica-y-tics/files/2016/01/portada.jpg"
    img-alt="Image"
    img-top
    tag="article"
    style="max-width: 20rem;"
    class="mb-2"
  >
    <b-card-text>
      Aqui te mostraremos como funcionan los distintos gestores de bases de datos
    </b-card-text>

     <router-link to="/SQL">About</router-link>
  </b-card>
          </b-col>
        </b-row>
      </b-container>
    </b-skeleton-wrapper>
  </div>

</template>

<script>
export default {
     name: 'Contenido',
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
      this.$_loadingTimeInterval = null
            document.title = "Cursos principales";
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
