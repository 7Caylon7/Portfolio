<template>
  <NavBar/>
  <AboutComponent/>
</template>

<script>
import NavBar from './components/NavBar.vue'
import AboutComponent from './components/AboutComp.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    AboutComponent
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style-type:none
}
</style>
