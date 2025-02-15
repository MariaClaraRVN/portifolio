<template>
    <section class="contact" id="contatos">
      <h2 class="heading">Contate <span>- Me</span></h2>
      <form action="https://formsubmit.co/mariaclararezendeviannaa@gmail.com" method="POST">
        <input type="hidden" name="_captcha" value="false">
        <input type="hidden" name="_template" value="table">
        <input type="hidden" name="_subject" value="Nova mensagem do seu portfólio!">
        <input type="hidden" name="_next" value="https://github.com/MariaClaraRVN">
        <div class="input-group">
          <div class="input-box">
            <input type="text" name="nome" placeholder="Nome Completo" required>
            <input type="email" name="email" placeholder="Email" required>
          </div>
          <div class="input-box">
            <input type="tel" name="telefone" placeholder="Número de Celular">
            <input type="text" name="assunto" placeholder="Assunto">
          </div>
        </div>
        <div class="input-group-2">
          <textarea name="mensagem" cols="30" rows="10" placeholder="Sua Mensagem" required></textarea>
          <input type="submit" value="Enviar Mensagem" class="btn">
        </div>
      </form>
    </section>
  </template>
  
  <script>
  export default {
    name: 'ConattoPorti'
  }
  </script>
  
  <style scoped>
/* Estilização de contatos*/
.heading {
    text-align: center;
    font-size: 7rem;
    margin: 5rem 0;
}

.contact {
    background-color: var(--bg-color);
}

.contact h2 {
    margin-bottom: 3rem;
    color: var(--text-color);
}

.contact form {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 3rem;
    margin: 5rem 0;
    text-align: center;
}

span {
    color: var(--main-color);
}

span:hover {
    transform: scale(1.3)translateY(-5px);
    text-shadow: 0 0 25px var(--main-color),
        0 0 50px var(--text-color);
}

.contact form .input-box input,
.contact form textarea {
    width: 100%;
    padding: 2.5rem;
    font-size: 1.8rem;
    color: var(--text-color);
    background-color: var(--bg-color);
    border-radius: 2rem;
    border: 2px solid var(--main-color);
    margin: 1.5rem;
    resize: none;
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
    box-shadow: 0 0 25px var(--main-color);
    border-radius: 3rem;
    font-size: 1.8rem;
    color: black;
    border: 2px solid transparent;
    font-weight: 600;
    transition: 0.3s ease-in-out
}

.btn:hover {
    transform: scale(1.05);
    box-shadow: 0 0 25px var(--main-color),
        0 0 50px var(--text-color),
        0 0 100px var(--main-color);
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
    color: black;
}

  </style>
  