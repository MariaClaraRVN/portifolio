<template>
    <section class="home" id="inicio">
      <div class="home-content">
        <h1>Olá, eu sou a <span>Maria Clara</span></h1>
        <h3>Atualmente sou <span>Estagiaria em Front - End</span></h3>
        <p>Desenvolvimento de páginas web responsivas utilizando HTML, CSS (SASS), com integração de Javascript, React e Vue. <br>Além de manipulação de imagens, controle de versão com GIT e integração com backend</p>
        <div class="social-icons">
          <a target="_blank" href="https://github.com/MariaClaraRVN"><i class="bx bxl-github"></i></a>
          <a target="_blank" href="https://www.linkedin.com/in/mariaclaravianna/"><i class="bx bxl-linkedin"></i></a>
          <a target="_blank" href="https://www.instagram.com/why_clarinharv/"><i class="bx bxl-instagram"></i></a>
          <a target="_blank" href="https://sketchfab.com/mariaclararezendeviannaa"><i class="bx bxs-cube"></i></a>
        </div>
        <br>
        <div class="btn-group">
          <a href="/docs/CurriculoMariaClara.pdf" download="Curriculo Maria Clara" class="btn">Download CV</a>
          <a href="#contatos" class="btn">Contato</a>
        </div>
      </div>
      <!-- <div class="home-img">
        <img src="../assets/img/MariaClara.png" alt="Maria Clara">
      </div> -->
    </section>
  </template>
  
  <script>
  export default {
    name: 'HomePorti',
    data(){
      return{
        dow:'@/public/docs/CurriculoMariaClara.pdf' 
      }
    }
  }
  </script>
  
  <style scoped>
/* Estilização do inicio */
.home {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 15rem;
}

span{
  color: var(--main-color);
}
.home-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

/* Estilização do inicio titulo */
.home-content h1 {
    color: var(--text-color);
    font-size: 8rem;
    font-weight: 700;
    margin-top: 1.5rem;
    line-height: 1rem 0;
}

/* Estilização do inicio subtitulo */
.home-content h3 {
    color: var(--text-color);
    font-size: 4rem;
    margin: 1rem 0;
}

/* Estilização do inicio paragrafo*/
.home-content p {
    color: var(--text-color);
    font-size: 1.5rem;
    font-weight: 500;
    line-height: 1.8;
}

/* Estilização do inicio imagem*/
.home-img img {
    transition: 0.3s ease;
    max-width: 100%;
    width: 32vw;
    border-radius: 50%;
    box-shadow: 0 0 25px var(--main-color);
    transition: 0.4s ease-in-out;
}

.home-img img:hover {
    transform: scale(1.3)translateY(-5px);
    box-shadow: 0 0 25px var(--main-color),
        0 0 50px var(--text-color),
        0 0 100px var(--main-color);
}

/* Estilização do inicio icones */
.social-icons a {
    display: inline-flex;
    justify-content: center;
    align-items: flex-end;
    font-size: 3rem;
    padding: 1rem;
    background: transparent;
    border: 2px solid var(--main-color);
    border-radius: 50%;
    color: var(--main-color);
    margin: 3rem 0.5rem;
    transition: 0.3s ease;
}

.social-icons a:hover {
    color: var(--text-color);
    background-color: var(--main-color);
    transform: scale(1.3)translateY(-5px);
    box-shadow: 0 0 25px var(--main-color);
}

/* Estilização do inicio botões */
.btn-group {
    display: flex;
    gap: 5rem;
}

.btn {
    display: inline-block;
    padding: 1rem 3rem;
    background: var(--main-color);
    box-shadow: 0 0 20px var(--main-color);
    border-radius: 3rem;
    font-size: 1.8rem;
    color: var(--bg-color);
    border: 2px solid transparent;
    font-weight: 600;
    transition: 0.3s ease-in-out
}

.btn:hover {
  color: var(--text-color);
    transform: scale(1.05);
    box-shadow: 0 0 45px var(--main-color)
/*         0 0 50px var(--text-color),
        0 0 100px var(--main-color) */;
}

.btn-group a:nth-of-type(2) {
    background-color: black;
    color: var(--main-color);
    border: 2px solid var(--main-color);
    box-shadow: 0 0 25px transparent;
}

.btn-group a:nth-of-type(2):hover {
    box-shadow: 0 0 25px var(--main-color);
    background-color: var(--main-color);
    color: var(--text-color);
}
  </style>
  