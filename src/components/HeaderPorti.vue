<template>
    <header class="header">
      <a href="#inicio" class="logo">Mc<span>rv.</span></a>
      <i class="bx bx-menu" id="menu-icon"></i>
      <nav class="navbar">
        <a href="#inicio">Início</a>
        <a href="#sobre">Sobre</a>
        <a href="#experience">Experiência</a>
        <a href="#servicos">Projetos</a>
        <a href="#contatos">Contatos</a>
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: 'HeaderPorti'
  }
  </script>
  
  <style scoped>
/* Estilização do header */
.header {
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    padding: 2rem 12%;
    background: rgba(0, 0, 0, 0.3);
    backdrop-filter: blur(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

/* Estilização do menu icone */
#menu-icon {
    font-size: 3.6rem;
    color: var(--main-color);
    display: none;
}

/* Estilização da logo */
.logo {
    font-size: 3rem;
    color: var(--text-color);
    font-weight: 800;
    cursor: pointer;
    transition: 0.3s ease;
}

.logo:hover {
    transform: scale(1.1);
    box-shadow: 2rem solid var(--text-color);
}

span {
    color: var(--main-color);
}

span:hover {
    transform: scale(1.3)translateY(-5px);
    text-shadow: 0 0 25px var(--main-color),
        0 0 50px var(--text-color);
}

/* Estilização do menu de navegação */
.navbar a {
    font-size: 1.8rem;
    color: var(--text-color);
    margin-left: 4rem;
    font-weight: 500;
    border-bottom: 3px solid transparent;
    transition: 0.3s ease;
}

.navbar a:hover {
    border-bottom: 3px solid var(--main-color);
    color: var(--main-color);
}
  </style>
  