<template>
    <header class="header">
      <a href="#inicio" class="logo">Mc<span>rv.</span></a>
      <i class="bx bx-menu" id="menu-icon" @click="toggleMenu"></i>
      <nav class="navbar" :class="{ active: isActive }">
        <a href="#inicio" @click="toggleMenu">Início</a>
        <a href="#sobre" @click="toggleMenu">Sobre</a>
        <a href="#experience" @click="toggleMenu">Experiência</a>
        <a href="#servicos" @click="toggleMenu">Projetos</a>
        <a href="#contatos" @click="toggleMenu">Contatos</a>
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: 'HeaderPorti',
    data() {
      return {
        isActive: false
      }
    },
    methods: {
      toggleMenu() {
        this.isActive = !this.isActive;
      }
    }
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
    transform: scale(1.3) translateY(-5px);
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

/* Media Queries para responsividade */
@media (max-width: 1200px) {
    .header {
        padding: 2rem 5%;
    }

    .navbar a {
        font-size: 1.6rem;
        margin-left: 3rem;
    }
}

@media (max-width: 768px) {
    #menu-icon {
        display: block;
    }

    .navbar {
        position: fixed;
        top: 0;
        left: -100%;
        width: 100%;
        height: 100vh;
        background: rgba(0, 0, 0, 0.9);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        transition: 0.3s;
    }

    .navbar a {
        font-size: 2rem;
        margin: 2rem 0;
    }

    .navbar.active {
        left: 0;
    }
}

@media (max-width: 480px) {
    .logo {
        font-size: 2.5rem;
    }

    .navbar a {
        font-size: 1.8rem;
    }
}
</style>