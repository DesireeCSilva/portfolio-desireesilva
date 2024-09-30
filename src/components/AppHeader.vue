<template>
  <header>
    <nav class="header_portfolio">
      <img
        class="logo_header"
        src="../assets/icons/logo_gimp.webp"
        alt="logotipo de Desirée Silva"
      />
      <ul id="main-menu" class="main-menu">
        <li class="main-menu_item">
          <a href="#proyectos" class="main-menu_link">Proyectos</a>
        </li>
        <li class="main-menu_item">
          <a href="#formacion" class="main-menu_link">Formación</a>
        </li>
        <li class="main-menu_item">
          <a
            href="https://drive.google.com/file/d/1eqcxrCOnaMXNDoOg0VTY0N0z2tiPsSRW/view?usp=drive_link"
            class="main-menu_link"
            target="_blank"
            >Ver Currículum Vitae</a
          >
        </li>
        <div class="header_icons">
          <li class="main-menu_item">
            <a href="https://www.linkedin.com/in/desiree-carrizosa/"
              target="blank">
              <img src="https://img.icons8.com/color/70/linkedin.png" alt="linkedin"/>
            </a>
          </li>
          <li class="main-menu_item">
            <a href="https://www.behance.net/desirecarrizo" target="blank">
            <img src="https://img.icons8.com/color/70/behance.png" alt="behance"/>
            </a>
          </li>
        </div>
      </ul>
      <button class="button_header">
        <img width="40" height="40" src="https://img.icons8.com/color/48/smartphone.png" alt="smartphone"/><a href="tel:675937952">¡Contáctame!</a>
      </button>
    </nav>
  </header>
  <hr class="hr_portfolio" />
</template>

<script setup>
</script>

<style lang="scss">
.logo_header {
  width: 15rem;
  height: auto;
}
.header_portfolio {
  display: flex;
  flex-direction: row;
  width: 100%;
  height: 10rem;
  align-items: center;
  justify-content: space-between;

  .main-menu {
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    text-decoration: none;
    cursor: pointer;

    &_item {
      padding: 2em;
      font-size: 1rem;
      font-weight: 500;
      cursor: pointer;
      border: none;
    }

    &_link {
      text-decoration: none;
      color: #000000;
      position: relative;
      color: inherit;
    }

    &_link::before {
      content: "";
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 2px;
      background: linear-gradient(to right, #ce93d8, #e878a2, #eb85ab);
      z-index: 1;
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.5s ease-in-out;
    }

    &_link:hover::before {
      transform: scaleX(1);
    }
  }

  .button_header {
  background-color: #ce93d8;
  width: 14em;
  height: fit-content;
  font-size: 1.3rem;
  font-family: "Poppins";
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  border-radius: 0.5rem;
  border-style: none;
  cursor: pointer;
  text-decoration: none;
  text-align: center;
  justify-content: center;
  display: flex;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transition: all 0.3s ease;

  a {
    text-decoration: none;
    color: #000000;
  }

  &:hover {
    background-color: #ce93d8;
    transform: scale(0.95);
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  }
}

.header_icons {
  display: flex;
  width: 5rem;

}
}
</style>
