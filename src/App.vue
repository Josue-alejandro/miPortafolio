<template>
    <navigation-bar></navigation-bar>
  <header-section></header-section>
  <proyectos-section></proyectos-section>
  <know-section></know-section>
  <contact-section></contact-section>
</template>

<script>
import NavigationBar from './components/layout/NavigationBar.vue';
import HeaderSection from './components/layout/HeaderSection.vue';
import ProyectosSection from './components/layout/ProyectosSection.vue';
import KnowSection from './components/layout/KnowSection.vue';
import ContactSection from './components/layout/ContactSection.vue';

export default {
  components: {
    NavigationBar,
    HeaderSection,
    ProyectosSection,
    KnowSection,
    ContactSection
  }
}
</script>

<style>
* {
  scroll-behavior: smooth;
}

@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');

body {
  font-family: 'Open Sans', sans-serif;
  padding: 0px;
  margin: 0px;
  display: flex;
  flex-direction: column;
}

nav {
  display: absolute;
}

* {
  padding: 0px;
  margin: 0px;
}

@media (max-width: 991.98px) {}

/*Pantallas pequeñas (móviles en landscape de menos de 768px)*/
@media (max-width: 767.98px) {}

</style>