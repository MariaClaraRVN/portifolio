<template>
  <section class="services" id="servicos">
    <h2 class="heading">Projetos</h2>

    <div class="container">
      <div class="projects">
        <div class="project-card">
          <div class="project-image">
            <img src="../assets/img/EcoResgate.png" alt="Eco Resgate">
          </div>
          <div class="project-title">ECO RESGATE</div><br><br>
          <p class="project-description">Eco Resgate é um jogo de ação e aventura onde Zadok, um estudante de
            veterinária, resgata animais em perigo enquanto enfrenta desafios ambientais e decisões morais.</p> <br>
          <div class="botoes">
            <div class="service-info">
              <i class='bx bxs-joystick'></i>
            </div>
            <div class="btn-group">
              <a href="https://alp4ca.itch.io/eco-resgate" target="_blank" class="btn">Jogue Agora</a>
            </div>
          </div>
        </div>

        <div class="project-card">
          <div class="project-image">
            <img src="../assets/img/Portal_D_Triunfo.png" alt="Portal do Triunfo">
          </div>
          <div class="project-title">PORAL DO TRIUNFO</div> <br><br>
          <p class="project-description">Uma visual novel que auxilia na escolha do curso na Fatec Carapicuíba,
            apresentando desafios de 7 protagonistas que representam os perfis dos estudantes da instituição.</p> <br>

          <div class="botoes">
            <div class="service-info">
              <i class='bx bxs-joystick'></i>
            </div>
            <div class="btn-group">
              <a href="https://salamaker.itch.io/portaldotriunfo" target="_blank" class="btn">Jogue Agora</a>
            </div>
          </div>
        </div>

        <div class="project-card">
          <div class="project-image">
            <img src="../assets/img/Capa_Do_Jogo-export2.png" alt="Crossed Ways">
          </div>
          <div class="project-title">CROSSED WAYS</div><br><br>
          <p class="project-description">Crossed Ways é um jogo narrativo onde o jogador escolhe entre seguir a vida de
            um ladrão ou de um pianista renomado, com mecânica rítmica envolvente.</p> <br> <br>
          <div class="botoes">
            <div class="service-info">
              <i class='bx bxs-joystick'></i>
            </div>
            <div class="btn-group">
              <a href="https://alp4ca.itch.io/crossed-ways" target="_blank" class="btn">Jogue Agora</a>
            </div>
          </div>
        </div>

        <div class="project-card">
          <div class="project-image">
            <img src="../assets/img/Ricake.png" alt="Ricake Linktree">
          </div>
          <div class="project-title">Linktree Ricake</div>
          <p class="project-description">Uma landing page moderna e responsiva, criada com Vue 3 e CSS scoped, que
            funciona como um Linktree personalizado para uma confeitaria, reunindo links para redes sociais e
            informações essenciais em um único lugar</p> <br> <br>
          <div class="botoes">
            <div class="service-info">
              <i class='bx bxs-window-alt'></i>
            </div>
            <div class="btn-group">
              <a href="https://ricake-oficial-redes-sociais-7dp09bro8-mariaclararvns-projects.vercel.app/"
                target="_blank" class="btn">Veja Agora</a>
            </div>
          </div>
        </div>


        <div class="project-card">
          <div class="project-image">
            <img src="../assets/img/iptvoz.png" alt="IPTVOz" style="width: 100%;">
          </div>
          <div class="project-title">IPTVOz</div>
          <p class="project-description">IPTVOz é uma aplicação Vue.js para IPTV, oferecendo diversos planos e suporte
            ao cliente, com foco em responsividade e usabilidade, utilizando tecnologias modernas como Vue.js, Font
            Awesome, Google Fonts e CSS3.</p> <br> <br>
          <div class="botoes">
            <div class="service-info">
              <i class='bx bxs-window-alt'></i>
            </div>
            <div class="btn-group">
              <a href="https://iptvoz.com.br" target="_blank" class="btn">Veja Agora</a>
            </div>
          </div>
        </div>

        <!-- 
      <div class="project-card">
        <div class="project-image"></div>
        <div class="project-title">Projeto 6</div>
        <p class="project-description">Descrição breve do projeto.</p>
      </div> -->
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProjetosSitePorti',
  data() {
    return {
    }
  }
}
</script>

<style scoped>
.services {
    background-color: var(--second-bg-color);
    backdrop-filter: blur(10px);
    color:var(--text-color);
    margin-top: -2%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

}

.container {
  padding: 50px 20px;
  max-width: 70%;
}

.heading {
    text-align: center;
    font-size: 7rem;
    margin: 5rem 0;
}

h2 {
  font-size: 2em;
  margin-bottom: 20px;
}

.projects {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
  justify-content: center;
}

.project-card {
  background-color: var(--main-color);
  border: 1px solid var(--bg-color);
  box-shadow: 0 4px 12px var(--bg-color);
  padding: 20px;
  border-radius: 10px;
  transition: transform 0.3s;
}

.project-card:hover{
  transform: scale(1.05);
  border: 1px solid var(--text-color);
  box-shadow: 0 0 25px var(--text-color)
}

.project-image img {
  width: 100%;
  height: 150px;
  background-color: #3c5c57;
  border-radius: 8px;
}

.project-title {
  text-align: center;
  font-size: 1.5rem;
  margin-top: 10px;
  font-weight: 600;
}

.project-title, .project-description{
  color: var(--bg-color);
}
.project-description {
  text-transform: uppercase;
  text-align: justify;
  font-size: 1.3rem;
  opacity: 0.8;
}

.project-description:hover {
  opacity: 0.8;
}

.botoes{
  display: flex;
  gap: 7%;
}

.service-info i {
  color: var(--bg-color);
    font-size: 3rem;
}

/* Estilização do inicio botões */
.btn-group {
    display: flex;
    gap: 5rem;
}

.btn {
    display: inline-block;
    padding: 1rem 3rem;
    background: var(--bg-color);
    box-shadow: 0 0 10px var(--text-color);
    border-radius: 3rem;
    font-size: 1.3rem;
    color: var(--text-color);
    border: 2px solid transparent;
    font-weight: 600;
    transition: 0.3s ease-in-out
}

.btn:hover {
    transform: scale(1.03);
    box-shadow: 0 0 12px var(--bg-color);
}

/* Media Queries para responsividade */
@media (max-width: 1200px) {
    .heading {
        font-size: 5rem;
    }

    .project-description {
        font-size: 1.2rem;
    }

    .btn {
        padding: 0.8rem 2.5rem;
        font-size: 1.2rem;
    }
}

@media (max-width: 768px) {
    .heading {
        font-size: 4rem;
    }

    .project-description {
        font-size: 1rem;
    }

    .btn {
        padding: 0.6rem 2rem;
        font-size: 1rem;
    }
}

@media (max-width: 480px) {
    .heading {
        font-size: 3rem;
    }

    .project-description {
        font-size: 0.9rem;
    }

    .btn {
        padding: 0.4rem 1.5rem;
        font-size: 0.9rem;
    }
}
</style>