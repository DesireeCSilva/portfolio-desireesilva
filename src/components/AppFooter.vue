<template>
  <footer>
    <nav class="footer_portfolio">
      <img
        class="logo_footer"
        src="../assets/icons/logo_gimp.webp"
        alt="logotipo de Desirée Silva"
      />

      <ul id="main-menu" class="main-menu">
        <div class="footer_icons">
          <li class="main-menu_item">
            <a href="/index.html#section-01" class="main-menu_link">Sobre mí</a>
          </li>
          <li class="main-menu_item">
            <a href="/index.html#section-02" class="main-menu_link"
              >Proyectos</a
            >
          </li>
          <li class="main-menu_item">
            <a href="/index.html#section-03" class="main-menu_link"
              >Formación</a
            >
          </li>
        </div>
        <div class="footer_icons">
          <li class="main-menu_item">
            <a
              href="https://www.linkedin.com/in/desiree-carrizosa/"
              target="blank"
            >
              <img
                src="../assets/icons/fa_linkedin-square.png"
                alt="logotipo de Linkedin"
              />
            </a>
          </li>
          <li class="main-menu_item">
            <a href="https://www.behance.net/desirecarrizo" target="blank">
              <img
                src="../assets/icons/mage_behance.png"
                alt="logotipo de Behance"
              />
            </a>
          </li>
        </div>
      </ul>
      <button class="button_header">
        <svg-icon type="mdi" :path="mdiPhone" class="icon_header"></svg-icon
        ><a href="tel:675937952">¡Contáctame!</a>
      </button>
    </nav>

    <p style="display: flex; justify-content: center; margin-bottom: 2rem">
      © 2024 Nuria Martínez y Desirée Carrizosa Silva. Todos los derechos
      reservados
    </p>
    <div class="bg_heart">
      <!-- Aquí es donde los bubbles animados serán añadidos dinámicamente -->
    </div>
  </footer>
</template>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const bgBubble = document.querySelector(".bg_heart");

  function createBubble() {
    const bubble = document.createElement("div");
    bubble.className = "bubble";

    const size = Math.random() * 40 + 20; // Tamaño entre 20px y 60px
    bubble.style.width = `${size}px`;
    bubble.style.height = `${size}px`;

    const leftPosition = Math.random() * (bgBubble.clientWidth - size); // Evita que la burbuja se salga del contenedor
    bubble.style.left = `${leftPosition}px`;

    // Generar un color aleatorio
    const r = Math.floor(Math.random() * 256);
    const g = Math.floor(Math.random() * 256);
    const b = Math.floor(Math.random() * 256);
    bubble.style.backgroundColor = `rgba(${r}, ${g}, ${b}, 0.6)`;

    const duration = Math.random() * 5 + 5; // Duración entre 5s y 10s
    bubble.style.animation = `float ${duration}s ease-out`;

    bgBubble.appendChild(bubble);

    // Eliminar la burbuja después de que la animación haya terminado
    setTimeout(() => {
      bubble.remove();
    }, duration * 1000);
  }

  // Crear una burbuja cada 500ms
  setInterval(createBubble, 500);
});
</script>
<script setup>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiPhone } from "@mdi/js";
</script>

<style>
footer {
  padding-top: 2rem;
  position: relative;
  height: auto;
  background: #ffffff;
  overflow: hidden;
  z-index: 1;
  box-sizing: border-box;
}

.footer_icons {
  display: flex;
  align-items: center;
  justify-content: space-between;
  box-sizing: border-box;
}

.bg_heart {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  z-index: 0;
}

.bubble {
  position: absolute;
  border-radius: 50%;
  background: rgba(206, 147, 216, 0.6);
  opacity: 0.7;
  pointer-events: none;
}

@keyframes float {
  0% {
    bottom: -10%;
    opacity: 0.8;
  }
  50% {
    opacity: 1;
  }
  100% {
    bottom: 110%;
    opacity: 0;
  }
}
.footer_portfolio,
.button_header,
.main-menu,
.main-menu_item,
.main-menu_link, 
.footer_icons {
  position: relative;
  z-index: 2;
}

.footer_portfolio {
  display: flex;
  height: auto;
  align-items: center;
  justify-content: center;
}

.logo_footer {
  max-width: 15rem;
  height: fit-content;
}

.main-menu {
  width: 100%;
  padding: 3em;
  list-style: none;
  display: flex;
  align-content: center;
  justify-content: space-between;
  text-decoration: none;
  cursor: pointer;
}

.main-menu_item {
  font-size: 1rem;
  padding: 3em;
  font-weight: 500;
  cursor: pointer;
  border: none;
}
.main-menu_link {
  text-decoration: none;
  color: #000000;
}
.main-menu_link::before {
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
.main-menu_link:hover::before {
  transform: scaleX(1);
}
.button_header {
  background-color: #ce93d8;
  width: 10em;
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
}
.button_header:hover {
  background-color: #ce93d8;
  transform: scale(0.95);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}
.icon_header {
  display: flex;
  flex-direction: row;
  align-self: center;
  width: 1.2rem;
  height: 1.2rem;
}
.button_header a {
  text-decoration: none;
  color: #000000;
}

/* Media query */

@media only screen and (max-width: 768px) {
  .footer_portfolio {
    flex-direction: column;
    align-items: center;
    height: auto;
  }

  .logo_footer {
    width: 40%;
    margin-bottom: 0.6rem;
  }

  .main-menu {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    margin: 0;
  }

  .main-menu_item {
    padding: 1em;
    width: 100%;
  }

  .button_header {
    width: 100%;
    text-align: center;
    margin-top: 1rem;
  }

  .footer_icons {
    display: flex;
    align-content: center;
    justify-content: center;
  }

  footer p {
    text-align: center;
    width: 100%;
    margin-top: 1rem;
    margin-bottom: 2rem;
    box-sizing: border-box;
  }
}
</style>
