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
      ></svg-icon>
      <svg-icon
        v-else
        type="mdi"
        :path="mdiClose"
        @click.stop="showMenu = false"
      ></svg-icon>
    </div>

    <nav v-if="showMenu" class="main-menu__mobile">
      <ul>
        <li>
          <a href="/index.html#section-01">Sobre mí</a>
        </li>
        <li>
          <a href="/index.html#section-02">Proyectos</a>
        </li>
        <li>
          <a href="/index.html#section-03">Formación</a>
        </li>
        <li>
          <a href="/index.html#section-05">Contáctame</a>
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
  padding: 1.5rem;

  .menu_toggle {
    display: flex;
    justify-content: space-between;
    align-items: center;

    img.logo_header__mobile {
      width: 3rem;
    }

    @media (min-width: 430px) {
      img.logo_header__mobile {
        width: 4.5rem;
      }
    }

    svg {
      cursor: pointer;
    }
  }

  .main-menu__mobile {
    position: absolute;
    left: 0;
    right: 0;
    widows: 100%;
    z-index: 100;
    background-color: #FFF;

    ul {
      list-style: none;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    a {
      text-decoration: none;
    }
  }
}
</style>
