<template>
  <header class="header_portfolio__mobile">
    <div class="menu_toggle">
      <img
        class="logo_header__mobile"
        src="../assets/icons/logo_gimp.webp"
        alt="logotipo de Desirée Silva"
      />
      <svg-icon
        v-if="!showMenu"
        type="mdi"
        :path="mdiMenu"
        @click.stop="showMenu = true"
        class="icon-hamburger"
      ></svg-icon>
      <svg-icon
        v-else
        type="mdi"
        :path="mdiClose"
        @click.stop="showMenu = false"
        class="icon-hamburger"
      ></svg-icon>
    </div>

    <nav v-if="showMenu" class="main-menu__mobile">
      <ul>
        <li>
          <a href="https://drive.google.com/file/d/1BUolDxQYZECSIflSKSMSiepAN9UMRVkw/view?usp=sharing" target="_blank">Ver CV de Desirée</a>
        </li>
        <li>
          <a href="#proyectos">Proyectos</a>
        </li>
        <li>
          <a href="#formacion">Formación</a>
        </li>
        <li>
          <a href="#contacto">Contáctame</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiMenu, mdiClose } from "@mdi/js";
import { ref } from "vue";

const showMenu = ref(false);
</script>

<style lang="scss">
.header_portfolio__mobile {
  position: relative;
  height: auto;
  padding: 2rem;

  .menu_toggle {
    display: flex;
    justify-content: space-between;
    align-items: center;

    img.logo_header__mobile {
      width: 35%;
    }

  @media only screen and (min-width: 320px) and (max-width: 768px){
      img.logo_header__mobile {
        width: 40%;
      }
    }

    .icon-hamburger {
      width: 3rem; 
      height: 3rem; 
      cursor: pointer;
    }

    svg {
      cursor: pointer;
    }
  }

  .main-menu__mobile {
    position: absolute;
    left: 0;
    right: 0;
    width: 100%;
    z-index: 100;
    background-color: #ffccbc;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 1rem 0;

    ul {
      list-style: none;
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;
      margin: 0;
      padding: 0;
    }
    li {
      width: 100%;
      text-align: center;
    }

    a {
      color: #000000;
      text-decoration: none;
      width: 100%;
      text-align: center;
      padding: 0.5rem 0;
      display: block;
      transition: background-color 0.3s, color 0.3s;

      &:hover {
        background-color: #e1bee7; 
      }

      &:active {
        background-color: #ce93d8;
        color: #ffffff;
      }
    }
  }
}

</style>
