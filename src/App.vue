<template>
  <NavBar/>
  <AboutComponent/>
  <SkillsComp/>
  <ProjectsComp/>
</template>

<script>
import NavBar from './components/NavBar.vue'
import AboutComponent from './components/AboutComp.vue';
import SkillsComp from './components/SkillsComp.vue';
import ProjectsComp from './components/ProjectsComp.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    AboutComponent,
    SkillsComp,
    ProjectsComp
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
