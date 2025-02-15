<template>
   <div id="app">
    <HeaderPorti />
    <HomePorti />
    <AboutPorti />
    <ExperincePorti/>
    <ProjetosSitePorti/>
    <!-- <ServicesPorti /> -->
    <ContatoPorti />
    <FooterPorti />

  </div>
</template>

<script>
import HeaderPorti from './components/HeaderPorti.vue';
import HomePorti from './components/HomePorti.vue';
import AboutPorti from './components/AboutPorti.vue';
import ContatoPorti from './components/ContatoPorti.vue';
/* import ServicesPorti from './components/ServicesPorti.vue'; */
import FooterPorti from './components/FooterPorti.vue';
import ExperincePorti from './components/ExperincePorti.vue';
import ProjetosSitePorti from './components/ProjetosSitePorti.vue';


export default {
  name: 'App',
  components: {
    HeaderPorti,
    HomePorti,
    AboutPorti,
    ExperincePorti,
/*     ServicesPorti, */
    ContatoPorti,
    FooterPorti,
    ProjetosSitePorti,

  }
}
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    scroll-behavior: smooth;
    font-family: "Varela Round", serif;
}

html {
    font-size: 60%;
    overflow-x: hidden;
}

/* Variaveis */

:root {
    --bg-color: #0f0f0f;
    --second-bg-color: #1d251a;
    --text-color: #fff;
    --main-color: #FF8C42;
    --box-color: #32442d;
}

/* Estilização do 'Corpo' */
body {
    background-color: var(--bg-color);
    color: var(--main-color);
}


/* Estilização de seções */
section {
    min-height: 100vh;
    padding: 10rem 12%;
}
/* Estilização barra de scroll lateral*/
::-webkit-scrollbar {
    width: 10px;
}

::-webkit-scrollbar-thumb {
    background-color: var(--main-color);
}

::-webkit-scrollbar-track {
    background-color: var(--text-color);
}
</style>
