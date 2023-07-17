<template>
  <header class="header">
    <a href="#inicio">
      <h1 class="header__h1">Juan Carlos Alvarez</h1>
    </a>
    <nav class="header__nav">
      <a href="#tecnologies" class="header__nav--option">Tecnologias</a>
      <a href="#proyects" class="header__nav--option">Mis proyectos</a>
    </nav>
  </header>
</template>

<script>
export default {
  name: "TheHeader",
};
</script>

<style scoped>
/* Header */
.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: rgba(52, 64, 85, 1);
  height: 6rem;
  text-align: center;
  z-index: 9999; 
}

.header__h1 {
  color: var(--blanco);
}
.header__nav {
  margin-top: 0.5rem;
}
.header__nav--option {
  color: var(--blanco);
  text-decoration: none;
  margin-right: 2rem;
}

@media (min-width: 768px) {
  .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .header__h1 {
    margin-left: 3rem;
  }

  .header__nav {
    margin: 13rem;
  }

  .header__nav--option {
    margin-right: 2rem;
  }
}
</style>