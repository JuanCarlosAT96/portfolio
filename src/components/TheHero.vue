<template>
  <div class="container">
    <section class="main--info">
      <h2 class="main--info__h2">Bienvenid@s</h2>
      <p class="main--info__p">
        ¡Hola! Soy Juan Carlos, un apasionado por la programación y tengo
        experiencia en Vue.js, HTML, CSS, JavaScript y Figma. Como
        desarrollador, doy mi mejor esfuerzo y me encanta ser autocrítico. Me
        encanta traducir ideas en código y trabajar en equipo para lograr
        resultados excepcionales. Siempre estoy buscando aprender nuevas
        tecnologías y enfrentar desafíos emocionantes.
      </p>
    </section>
    <section class="main--links">
      <div class="main-img">
        <img
          class="main-links__img"
          src="../assets/pro.jpg"
          alt="Visual Studio"
        />
      </div>
      <div class="main--links__soc">
        <div class="main--links__social">
          <a href="https://github.com/JuanCarlosAT96" target="blanck_"
            ><img src="../assets/github.png" alt=""
          /></a>
        </div>
        <div class="main--links__social">
          <a href="https://www.linkedin.com/in/juan-carlos-alvarez-tovilla/" target="blanck_"
            ><img src="../assets/linkedin.png" alt=""
          /></a>
        </div>
        <div class="main--links__social">
          <a href="https://www.youtube.com/@deprogramacion1585" target="blanck_"
            ><img src="../assets/youtube.png" alt=""
          /></a>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "TheHero",
};
</script>

<style>
/* Main info */

.main--info__h2 {
  margin-bottom: 1rem;
}

.main-img {
  width: 100%;
  height: 300px; /* Ajusta la altura según tus necesidades */
  object-fit: cover; /* Ajusta el recorte de la imagen */
}

.main--info__p {
  margin-bottom: 1rem;
  text-align: justify;
  padding: 1rem;
}

.main--info__btn {
  width: 6rem;
  height: 3rem;
  margin-bottom: 1rem;
  background-color: rgba(48, 41, 47, 1);
  border: none;
  border-radius: 0.2rem;
  color: var(--blanco);
}

.container {
  text-align: center;
  margin-top: 6rem;
}

.main-links__img {
  margin-bottom: 1rem;
  margin-top: 1rem;
  width: 90%;
  height: 90%;
  object-fit: fill;
}

.main--links__soc {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
}

.main--links__social {
  width: 40px;
  height: 50px;
  border-radius: 50%;
  text-decoration: none;
  overflow: hidden;
  margin-right: 1rem;
  margin-bottom: 1rem;
}

.main--links__social img {
  width: 100%;
  height: 100%;
  object-fit: fill;
}

@media (min-width: 768px) {
  .container {
    display: flex;
    text-align: center;
  }

  .main--info,
  .main--links {
    flex-basis: 50%; /* Ambos ocupan el 50% del ancho */
  }

  .main--info {
    margin: auto;
  }

  .main-img {
    height: auto; /* Restaurar la altura automática para que la imagen se ajuste correctamente */
  }

  .main--links {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
}
</style>