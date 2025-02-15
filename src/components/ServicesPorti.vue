<template>
<section class="services" id="servicos">
        <h2 class="heading">Projetos</h2>

        <div class="services-container">

            <!-- Card 1 -->
            <div class="service-box">
                <div class="service-info">
                    <i class='bx bxs-cube'></i>
                    <a target="_blank" href="https://sketchfab.com/mariaclararezendeviannaa"></a>

                    <h4>Scketchfab</h4>
                </div>
            </div>

            <!-- Card 2 -->
            <div class="service-box">
                <div class="service-info">
                    <i class='bx bxs-joystick'></i>

                    <a target="_blank" href="https://sketchfab.com/mariaclararezendeviannaa"></a>
                    <h4>Itch.io</h4>
                </div>
            </div>

            <!-- Card 3 -->
            <div class="service-box">
                <div class="service-info">
                    <i class='bx bxl-html5'></i>
                      
                    <a target="_blank" href="https://github.com/MariaClaraRVN"></a>

                    <h4>Git Hub</h4>
                </div>
            </div>
        </div>

    </section>
  </template>
  
  <script>
  export default {
    name: 'ServicesPorti',
    data() {
      return {
      
      }
    }
  }
  </script>
  
  <style scoped>
/* Estilização de serviços */
.heading {
    text-align: center;
    font-size: 7rem;
    margin: 5rem 0;
}

.services {
    background-color: var(--second-bg-color);
    backdrop-filter: blur(10px);
    color:var(--text-color);
    margin-top: -2%;
}

/* Estilização de serviços subtitulo*/
.services h2 {
    color: var(--text-color);
}

/* Estilização de serviços conteudo todo*/
.services-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    align-items: center;
    gap: 2.5rem;
}

.service-box {
  background-color: var(--bg-color);
  backdrop-filter: blur(10px);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 400px;
    border-radius: 3rem;
    cursor: pointer;
    border: 5px solid var(--main-color);
    transition: 0.4s ease-in-out;
}

.service-box:hover {
    background-color: var(--bg-color);
    color: var(--main-color);
    border: 5px solid var(--main-color);
    transform: scale(1.03);
    text-shadow: 0 3px 18px var(--text-color);
}

.service-info {
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    align-items: center;
    padding: 5rem;
}

.service-info i {
    font-size: 8rem;
}

.service-info h4 {
    font-size: 4rem;
    margin: 2rem 0;
    font-weight: 800;
}
</style>
  