<template>
    <footer class="footer">
      <div class="social-icons">
        <a target="_blank" href="https://github.com/MariaClaraRVN"><i class="bx bxl-github"></i></a>
        <a target="_blank" href="https://www.linkedin.com/in/mariaclaravianna/"><i class="bx bxl-linkedin"></i></a>
        <a target="_blank" href="https://www.instagram.com/why_clarinharv/"><i class="bx bxl-instagram"></i></a>
        <a target="_blank" href="https://sketchfab.com/mariaclararezendeviannaa"><i class="bx bxs-cube"></i></a>
      </div>
      <ul class="list">
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#sobre">Sobre</a></li>
        <li><a href="#experience">Experiência</a></li>
        <li><a href="#servicos">Projetos</a></li>
        <li><a href="#contatos">Contatos</a></li>
      </ul>
      <p class="copyright">© Maria Clara R. Vianna | Todos os direitos reservados</p>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterPorti'
  }
  </script>
  
  <style scoped>
.footer{
    background-color: var(--second-bg-color);
    padding: 50px 0;
}

.footer .social-icons{
    text-align: center;
}

.footer ul{
    text-align: center;
    font-size: 1.8rem;
}

.footer ul li{
    display: inline-block;
    margin-left: 20px;
}

.footer ul li a{
    color: white;
    border-bottom:  3px solid transparent;
    transition: 0.3s ease-in-out;
}

.footer ul li a:hover{
    border-bottom: 3px solid var(--main-color);
}

.footer .copyright{
    text-align: center;
    margin-top: 40px;
    font-size: 16px;
}

/* Estilização do inicio icones */
.social-icons a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
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
  </style>
  