<template>
  <div class="home">
    <!--img alt="Vue logo" src="../assets/logo.png"-->
    <Navbar/>
    <Contenido/>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Contenido from '../components/Contenido.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Contenido
  }
}
</script>