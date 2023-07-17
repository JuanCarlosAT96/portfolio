<template>
  <main id="inicio" class="animate__animated animate__fadeIn">
    <the-header />
    <hr />
    <the-hero />
    <hr />
    <the-tecnologies />
    <hr />
    <h2 id="proyects" class="proyects__h2">Proyectos</h2>
    <section class="proyects">
      <div class="proyects__card">
        <div class="proyects__img--info">
          <img src="./assets/Proyects/ConoceTepexi.png" alt="Conoce Tepexi" />
        </div>
        <h2 class="proyect__title">Conoce Tepexi</h2>
        <p class="proyect__description">
          Plataforma Web para dar a conocer la ciudad de Tepexi de Rodirguez,
          Puebla, Mexico, usando Vuejs, Quasar y Figma para diseno y
          programación
        </p>
        <div class="proyects__buttons">
          <a
            class="proyects__button"
            href="https://conocetepexi.netlify.app/#/"
            target="blanck_"
            >DEMO</a
          >
          <a class="proyects__button" href="#">CÓDIGO</a>
        </div>
      </div>
      <div class="proyects__card">
        <div class="proyects__img--info">
          <img src="./assets/Proyects/unsplashapi.png" alt="Unsplash Api" />
        </div>
        <h2 class="proyect__title">Unsplash API</h2>
        <p>
          Plataforma Web usando la API de Unsplash para imaganes, usando React para su programación
        </p>
        <div class="proyects__buttons">
          <a
            class="proyects__button"
            href="https://unsplashapi-programacionweb-equipo22.netlify.app/"
            target="blanck_"
            >DEMO</a
          >
          <a class="proyects__button" href="#">CÓDIGO</a>
        </div>
      </div>
      <div class="proyects__card">
        <div class="proyects__img--info">
          <img src="./assets/Proyects/TruthFly.png" alt="" />
        </div>
        <h2 class="proyect__title">Truthfly</h2>
        <p>
          Plataforma Web para informar sobre las noticias falsas, usando Vuejs para su programación y Firebase como Base de datos
        </p>
        <div class="proyects__buttons">
          <a class="proyects__button" href="https://truthfly.netlify.app/#/"
            >DEMO</a
          >
          <a class="proyects__button" href="#">CÓDIGO</a>
        </div>
      </div>
      <div class="proyects__card">
        <div class="proyects__img--info">
          <img src="./assets/Proyects/portfolio.png" alt="" />
        </div>
        <h2 class="proyect__title">Portfolio</h2>
        <p>
          Portfolio Web para dar a conocer mis conocimientos y proyectos realizados
        </p>
        <div class="proyects__buttons">
          <a class="proyects__button" href="#">DEMO</a>
          <a class="proyects__button" href="#">CÓDIGO</a>
        </div>
      </div>
    </section>
  </main>
  <footer class="footer">
    <p class="footer__p">Todos los derechos reservados @2023 Juan Alvarez</p>
  </footer>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import TheHero from "./components/TheHero.vue";
import TheTecnologies from "./components/TheTecnologies.vue";

export default {
  name: "App",
  components: {
    TheHeader,
    TheHero,
    TheTecnologies,
  },
};
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css");
.proyects__h2 {
  text-align: center;
  margin: 1rem;
}
@media (min-width: 768px) {
  .proyects {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}

.proyects__card {
  width: 500px;
  height: 520px;
  margin: auto;
}
.proyects__img--info {
  width: 100%;
  height: 294px;
  overflow: hidden;
}

.proyects__img--info img {
  width: 100%;
  height: 100%;
  object-fit: fill;
}

.proyect__title {
  font-size: 24px;
  margin-bottom: 10px;
  text-align: center;
  color: #333;
  text-transform: uppercase;
  letter-spacing: 1px;
  opacity: 0;
  animation: fade-in 1s ease-in-out forwards;
}

.card h2::after {
  content: "";
  display: block;
  width: 40%;
  height: 3px;
  background-color: #333;
  margin: 8px auto;
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

.proyect__description {
  text-align: justify;
  font-size: 16px;
}

/* Footer */
.footer {
  background-color: rgba(52, 64, 85, 1);
  height: 4rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.proyects__button {
  width: 6rem;
  height: 3rem;
  margin-bottom: 1rem;
  background-color: rgba(48, 41, 47, 1);
  border: none;
  border-radius: 0.2rem;
  color: var(--blanco);
}

.proyects__buttons {
  display: flex;
  justify-content: center;
}

.proyects__button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 10px 20px;
  background-color: #333;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
  margin: 0.5rem;
}

.proyects__button:hover {
  background-color: #555;
}
</style>
