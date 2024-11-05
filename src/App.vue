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
  list-style-type:none;
}

html{
  scroll-behavior: smooth;
}


/* Estilos para o Chrome, Safari e Edge */
::-webkit-scrollbar {
  width: .6vw;
}

::-webkit-scrollbar-thumb {
  background-color: #000;
  border-radius: 10px;
}

::-webkit-scrollbar-track {
  background: #787676;
}

/* Estilos para o Firefox */
scrollbar {
  width: .6vw;
}

scrollbar-thumb {
  background-color: #000;
  border-radius: 10px;
}

scrollbar-track {
  background: #787676;
}
</style>
