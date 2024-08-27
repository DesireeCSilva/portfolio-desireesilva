<template>
  <header>
    <nav class="header_portfolio">
      <ul id="main-menu" class="main-menu">
        <li class="main-menu_item">
          <img class="logo_footer" 
            src="../assets/icons/logo_gimp.webp"
            alt="logotipo de Desirée Silva"
          />
        </li>
        <li class="main-menu_item">
          <a href="/index.html#section-01" class="main-menu_link">Sobre mí</a>
        </li>
        <li class="main-menu_item">
          <a href="/index.html#section-02" class="main-menu_link">Proyectos</a>
        </li>
        <li class="main-menu_item">
          <a href="/index.html#section-03" class="main-menu_link">Formación</a>
        </li>
        <li class="main-menu_item">
          <a href="/index.html#section-04" class="main-menu_link">Tecnologías</a>
        </li>
        <button class="button_header">
          <img class="icon_header" src="@/assets/icons/call.png" alt="" /><a
            href="tel:675937952"
            >¡Contáctame!</a
          >
        </button>
      </ul>
    </nav>
  </header>
  <hr class="hr_portfolio">
</template>

<script>
</script>

<style lang="scss">
.header_portfolio {
  display: flex;
  flex-direction: row;
  width: 100vw;
  height: 10rem;
  align-items: center;
  justify-content: space-around;
  
  .main-menu {
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: space-between;
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
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 2px;
      background: linear-gradient(to right, #CE93D8, #e878a2, #eb85ab);
      z-index: 1;
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.5s ease-in-out;
    }

    &_link:hover::before {
      transform: scaleX(1);
    }

    .button_header {
      background-color: #CE93D8;
      width: 10em;
      height: fit-content;
      font-size: 1.3rem;
      font-family: 'Poppins';
      padding-top: 0.5rem;
      padding-bottom: 0.5rem;
      border-radius: 0.50rem;
      border-style: none;
      cursor: pointer; 
      text-decoration: none;
      text-align: center;
      justify-content: center;
      display: flex;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); 
      transition: all 0.3s ease; 

      .icon_header {
        display: flex;
        flex-direction: row;
        align-self: center;
        width: 1.2rem;
        height: 1.2rem;
      }

      a {
        text-decoration: none;
        color: #000000;
      }
    }

    .button_header:hover {
      background-color: #CE93D8;
      transform: scale(0.95); 
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
    }
  }
}
.hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}
</style>
