<template>
  <NavBar/>
  <AboutComponent/>
  <SkillsComp/>
  <ProjectsComp/>
  <ContactBar/>
  <ContactComp/>
</template>

<script>
import NavBar from './components/NavBar.vue'
import AboutComponent from './components/AboutComp.vue';
import SkillsComp from './components/SkillsComp.vue';
import ProjectsComp from './components/ProjectsComp.vue';
import ContactComp from './components/ContactComp.vue';
import ContactBar from './components/ContactBar.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    AboutComponent,
    SkillsComp,
    ProjectsComp,
    ContactBar,
    ContactComp
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
