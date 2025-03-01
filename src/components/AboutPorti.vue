<template>
    <section class="about" id="sobre">
        <div class="about-img">
            <img src="../assets/img/MariaClara.png" alt="Maria Clara">
        </div>
        <div class="about-content">
            <h2 class="heading">Sobre <span>Mim!</span></h2>
            <div class="sobre-mim">
                <div class="caixa">
                    <h2 class="titulo-caixa">Quem Sou Eu</h2>
                    <p class="text-about">Sou Maria Clara, estudante de Jogos Digitais e estagiária de Front-End na Webcore Interactive,
                        com foco em criar experiências digitais inovadoras e acessíveis.</p>
                </div>

                <div class="caixa">
                    <h2 class="titulo-caixa">Experiência</h2>
                    <p class="text-about">Trabalhei como instrutora de Metaverso e desenvolvi o jogo "Eco Resgate" no meu TCC, abordando o
                        resgate de animais em risco. Tenho experiência em game design, arte de cenários e programação.
                    </p>
                </div>

                <div class="caixa">
                    <h2 class="titulo-caixa">Objetivos</h2>
                    <p class="text-about">Busco sempre expandir minhas habilidades para impactar positivamente o público. Acredito na união
                        de criatividade, tecnologia e propósito em todos os projetos que participo.</p>
                </div>
                <!-- <a href="#" class="btn">Saiba Mais</a> -->
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AboutPorti'
}
</script>

<style scoped>
/* Estilização sobre mim */
.about {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 10rem;
    background-color: var(--second-bg-color);
}

.heading {
    text-align: center;
    font-size: 7rem;
    color: var(--text-color);
    margin-bottom: 3rem;
}

.about-img img {
    width: 40rem;
    border-radius: 50%;
    box-shadow: 0 0 15px var(--main-color);
    transition: 0.4s ease-in-out;
}

.about-img img:hover {
    box-shadow: 0 0 25px var(--main-color),
        0 0 45px var(--main-color),
        0 0 100px var(--main-color);
}

.about-content {
    margin-left: 5%;
}

.about-content .btn {
    margin: 3rem 0;
}

.text-about {
    text-align: justify;
}

.caixa {
  background-color: var(--box-color);
  width: 100%;
  border-radius: 8px;
  border: 1px solid var(--main-color);
  padding: 20px;
  margin-bottom: 6%; 
  box-shadow: 0 4px 6px var(--main-color);
}

.caixa:hover{
    transform: scale(1.02);
    border: 1px solid var(--text-color);
    box-shadow: 0 9px 18px var(--text-color);
}

.titulo-caixa{
  font-size: 2rem;
  color:var(--text-color);
  margin-bottom: 10px;
}

.text-about {
  font-size: 1.5rem;
  color:var(--text-color);
  text-align: left;
}

/* Media Queries para responsividade */
@media (max-width: 1200px) {
    .about {
        gap: 5rem;
    }

    .heading {
        font-size: 5rem;
    }

    .about-img img {
        width: 30rem;
    }
}

@media (max-width: 768px) {
    .about {
        flex-direction: column;
        align-items: center;
        gap: 3rem;
    }

    .about-content {
        margin-left: 0;
        text-align: center;
    }

    .heading {
        font-size: 4rem;
    }

    .about-img img {
        width: 25rem;
    }

    .titulo-caixa {
        font-size: 1.8rem;
    }

    .text-about {
        font-size: 1.2rem;
    }
}

@media (max-width: 480px) {
    .heading {
        font-size: 3rem;
    }

    .about-img img {
        width: 20rem;
    }

    .titulo-caixa {
        font-size: 1.5rem;
    }

    .text-about {
        font-size: 1rem;
    }
}
</style>