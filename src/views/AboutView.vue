<template>
  <div class="container mt-4 text-body-secondary">
    <div class="card p-4">
      <h1 class="text-center mt-1">Sobre o Projeto</h1>
      <hr />
      <h3>O que é o PokeVite?</h3>
      <div class="card-body">
        O PokeVite é um projeto desenvolvido durante o curso de
        <a href="https://www.udemy.com/course/curso-front-end-developer-vue/"
          >Vue.js 3</a
        >
        ministrado pelo professor
        <a href="https://link-service.netlify.app/">Yuri Marcon</a>. Nosso
        objetivo é fornecer uma plataforma intuitiva e divertida para que os fãs
        de Pokémon possam explorar e aprender mais sobre seus Pokémons
        favoritos.
      </div>
      <br />
      <h3>Tecnologias Utilizadas</h3>
      <div class="card-body">
        Para o desenvolvimento do PokeVite, foram utilizadas as seguintes
        tecnologias:
        <ul>
          <li>Vue.js 3</li>
          <li>Vite</li>
          <li>PokeAPI</li>
          <li>Bootstrap</li>
          <li>HTML</li>
          <li>CSS</li>
        </ul>
      </div>
      <h3>Principais Funcionalidades</h3>
      <div class="card-body">
        <ul>
          <li>
            Consumo da API PokeAPI para obter informações sobre os pokémons
          </li>
          <li>Exibição de uma lista de pokémons</li>
          <li>Detalhes de cada pokémon, como nome, tipo, habilidades, etc.</li>
          <li>Responsividade para diferentes tamanhos de tela</li>
        </ul>
      </div>
      <section>
        <hr />
        <h5 class="text-center">Obrigado por prestigiar o projeto!</h5>
        <strong>👩🏽‍💻Ana Maria</strong><br />
        <strong>Contato:</strong>
        <p>
          <strong> 📨E-mail:</strong> anamariasouza701@gmail.com<br />
          <img src="@/assets/octocat.png" height="20px" alt="imagem octocat" />
          <a href="https://github.com/souzaana"> /souzaana</a>
        </p>
      </section>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}

a,
h1,
h3,
h5 {
  color: #ec1f90;
  text-decoration: none;
}

body {
  height: 100vh;
}

.container {
  height: 75vh;
  overflow-x: hidden;
  overflow-y: scroll;
}

.card{
  background-color: #ffffffa8;
}
</style>
