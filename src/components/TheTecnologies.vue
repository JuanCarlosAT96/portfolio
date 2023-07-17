<template>
  <section id="tecnologies" class="tecnologies--info">
    <h2 class="tecnologies--info__h2">Tecnologías</h2>
    <div class="tecnologies--info__img">
      <div class="tecnologies--info__img--info">
        <img src="../assets/tecnologies/Vuejs.png" alt="Vuejs" />
      </div>
      <div class="tecnologies--info__img--info">
        <img src="../assets/tecnologies/Html.png" alt="Html" />
      </div>
      <div class="tecnologies--info__img--info">
        <img src="../assets/tecnologies/Css.png" alt="Css" />
      </div>
      <div class="tecnologies--info__img--info">
        <img src="../assets/tecnologies/JavaScript.png" alt="JavaScript" />
      </div>
      <div class="tecnologies--info__img--info">
        <img src="../assets/tecnologies/Git.png" alt="Git" />
      </div>
      <div class="tecnologies--info__img--info">
        <img src="../assets/tecnologies/Figma.png" alt="Figma" />
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.tecnologies--info__h2 {
  text-align: center;
  margin-top: 1rem;
}
.tecnologies--info__img--info {
  width: 259px;
  margin: 1rem auto;
  height: 294px;
}

@media (min-width: 768px) {
  .tecnologies--info__img {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>