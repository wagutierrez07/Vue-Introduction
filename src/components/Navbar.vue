<template>
  <div>
      <b-navbar toggeable="lg" type="light" variant="info">
          <b-navbar-brand href="/Home">Navbar</b-navbar-brand>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
            <b-collapse class="nav-collapse" is-nav>
                <b-navbar-nav>
                <b-nav-item :to="{name: 'Cursos'}" exact>Otros cursos</b-nav-item>
                <b-nav-item :to="{name: 'Biblioteca'}" exact>Biblioteca</b-nav-item>
                </b-navbar-nav>
                <b-navbar-nav class="ml-auto">
    <b-avatar size="36px"></b-avatar>
                <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template #button-content>
            <em>User</em>
          </template>
          
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
                </b-navbar-nav>
            </b-collapse>
      </b-navbar>
          <router-view/>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>