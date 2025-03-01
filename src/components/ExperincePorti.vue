<template>
    <section class="about" id="experience">
        <div class="container">
            <h2 class="heading">Minha Experiência</h2>
            <div class="timeline">
                <div class="experience">
                    <div class="experiencia-empresa">
                        <p class="empresaD">WEBCORE INTERACTIVE</p>
                        <div class="experience-box direita">
                            <div class="date">01/2025 - ATUAL</div>
                            <div>
                                <p class="title">Estágio em Front-End</p>
                            </div>
                            <p>
                                - Montagem de páginas em HTML com CSS (em formato SASS); <br>
                                - Utilização de programas de edição de imagem para export das imagens; <br>
                                - Desenvolvimento de Javascript / React / Vue; <br>
                                - Integração com backend; <br>
                                - Controle de código por GIT;
                            </p>
                        </div>
                    </div>
                </div>
                <div class="experience">
                    <div class="experiencia-empresa esquerda">
                        <p class="empresaE">ASSINCO CURSOS - NÚCLEO WIT</p>
                        <div class="experience-box">
                            <div class="date">06/2024 - 01/2025</div>
                            <div>
                                <p class="title">Instrutora de Metaverso</p>
                            </div>
                            <p>
                                - Modelagem de objetos no Tinkercad e Vectary 3D; <br>
                                - Experiência em realidade virtual com Oculus Meta Quest 2; <br>
                                - Exploração do ambiente virtual no Spatial; <br>
                                - Registro das aulas com câmera profissional Canon; <br>
                                - Uso de celulares e tablets como suporte durante as aulas.
                            </p>
                        </div>
                    </div>
                </div>
                <div class="experience">
                    <div class="experiencia-empresa">
                        <p class="empresaD">SALA MAKER - FATEC CARAPICUÍBA</p>
                        <div class="experience-box direita">
                            <div class="date">08/2023 - 07/2024</div>
                            <div>
                                <p class="title">Estagiária Sala Maker</p>
                            </div>
                            <p>
                                - Desenvolvimento de jogos no Ren'Py; <br>
                                - Criação de documentos de game design (GDD); <br>
                                - Produção de vídeos para pitching de jogos; <br>
                                - Experimentação e prototipação na Sala Maker; <br>
                                - Uso de ferramentas para narrativa interativa e mecânicas de jogo. <br>
                            </p>
                        </div>
                    </div>
                </div>
                <!--                 <div class="experience">
                    <div class="experiencia-empresa">
                        <p class="empresaE">Nome da empresa</p>
                        <div class="experience-box">
                            <div class="date">2023-Presente</div>
                            <div class="title">Empreendedora - Projeto 100K</div>
                            <p>Desenvolvimento de um negócio de baixo custo visando alcançar R$100 mil em receita até o
                                final de 2025. Exploração de oportunidades no setor de jogos, tecnologia e educação.</p>
                        </div>
                    </div>
                </div> -->
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ExperiencePorti'
}
</script>

<style scoped>
.container {
    max-width: 800px;
    margin: auto;
    padding: 50px 20px;
    position: relative;
}

.heading {
    text-align: center;
    font-size: 7rem;
    color: var(--text-color);
    margin-bottom: 3rem;
}

.timeline {
    position: relative;
    padding: 20px 0;
}

.timeline::after {
    content: '';
    position: absolute;
    width: 2px;
    background-color: white;
    top: 0;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
}

.experience {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin-bottom: 20px;
    position: relative;
}

.title {
    font-weight: 600;
    color: var(--main-color);
}

.experience:nth-child(odd) {
    flex-direction: row-reverse;
}

.experiencia-empresa {
    width: 50%;
}

.empresaD {
    margin-left: 4%;
    margin-bottom: 1%;
    color: var(--text-color);
    font-size: 1.9rem;
}

.empresaE {
    margin-left: 3%;
    margin-bottom: 1%;
    color: var(--text-color);
    font-size: 1.9rem;
}

.experience-box {
    border: 1px solid var(--main-color);
    background-color: var(--second-bg-color);
    padding: 15px;
    border-radius: 10px;
    max-width: 100%;
    text-align: left;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
    font-size: 11px;
}

.date {
    font-weight: bold;
    margin-bottom: 5px;
    color: var(--main-color);
}

p {
    color: var(--text-color);
}

/* Media Queries para responsividade */
@media (max-width: 1200px) {
    .heading {
        font-size: 5rem;
    }

    .experience {
        flex-direction: column;
        align-items: flex-start;
    }

    .timeline::after {
        display: none;
    }

    .experiencia-empresa {
        width: 100%;
    }
}

@media (max-width: 768px) {
    .heading {
        font-size: 4rem;
    }

    .experience-box {
        padding: 10px;
        font-size: 1rem;
    }

    .empresaD, .empresaE {
        font-size: 1.5rem;
    }
}

@media (max-width: 480px) {
    .heading {
        font-size: 3rem;
    }

    .experience-box {
        padding: 8px;
        font-size: 0.9rem;
    }

    .empresaD, .empresaE {
        font-size: 1.2rem;
    }
}
</style>