<template>
    <div id="portfolio">
      <section class="parallax-section" ref="parallaxSection">
        <h1>Meu Portfólio</h1>
      </section>
  
      <section class="content-section">
        <p>Conteúdo do portfólio...</p>
      </section>
    </div>
  </template>
  
  <script>
  import ScrollMagic from "scrollmagic";
  import gsap from "gsap";
  import { ScrollMagicPluginGsap } from "scrollmagic-plugin-gsap";
  
  ScrollMagicPluginGsap(ScrollMagic, gsap);
  
  export default {
    name: 'Parallax',
  
    mounted() {
      const controller = new ScrollMagic.Controller();
  
      new ScrollMagic.Scene({
        triggerElement: this.$refs.parallaxSection,
        triggerHook: 0.5,
        duration: '200%',
      })
        .setTween(gsap.fromTo(this.$refs.parallaxSection, { y: '50%' }, { y: '0%' })) // Usando GSAP para animar
        .addTo(controller);
    },
  }
  </script>
  
  
  <style scoped>
  .parallax-section {
    height: 100vh;
    background-image: url('../assets/ilustracao.webp');
    background-size: cover;
    background-position: center top; /* Fundo começa no topo */
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .parallax-content {
    z-index: 1; /* Garante que o conteúdo não seja afetado */
  }
  
  .content-section {
    height: 100vh;
    background-color: #fff;
    padding: 20px;
  }
  
  </style>
  