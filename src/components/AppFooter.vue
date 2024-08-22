<template>
  <footer>
    <nav class="footer_portfolio">
      <ul id="main-menu" class="main-menu">
        <img src="../assets/logo_desiree.png" alt="logotipo de Desirée Silva" />
        <li class="main-menu_item">
          <a href="/index.html#section-01" class="main-menu_link">Sobre mí</a>
        </li>
        <li class="main-menu_item">
          <a href="/index.html#section-02" class="main-menu_link">Proyectos</a>
        </li>
        <li class="main-menu_item">
          <a href="/index.html#section-03" class="main-menu_link">Formación</a>
        </li>
      </ul>
      <button class="button_header">
        <img class="icon_header" src="@/assets/icons/call.png" alt="" /><a
          href="tel:675937952"
          >¡Contáctame!</a
        >
      </button>
    </nav>

    <p style="display: flex; justify-content: center; margin-bottom: 2rem">
      © 2024 Desirée Carrizosa Silva. Todos los derechos reservados
    </p>
    <div class="bg_heart">
      <!-- Aquí es donde los corazones animados serán añadidos dinámicamente -->
    </div>
  </footer>
</template>

<script>
document.addEventListener("DOMContentLoaded", function () {
    const bgBubble = document.querySelector('.bg_heart');

    function createBubble() {
        const bubble = document.createElement('div');
        bubble.className = 'bubble';

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

<style>
🔔/* footer */

footer {
    position: relative;
    height: 18rem;
    background: #FFFFFF;
    overflow: hidden;
    z-index: 1; 
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
.main-menu_link {
    position: relative;
    z-index: 2;
}

.footer_portfolio {
    display: flex;
    height: 10rem;
    align-items: center;
    justify-content: space-around; 
    }

.main-menu {
    list-style: none;
    display: flex;
    text-align: center;
    align-items: center;
    align-content: center;
    justify-content: space-between;
    text-decoration: none;
    cursor: pointer;
}

.main-menu_item {
    padding: 3em;
    font-size: 1rem;
    font-weight: 500;
    cursor: pointer;
    border: none;
}
.main-menu_link {
    text-decoration: none;
    color: #000000;    
    position: relative;
    color: inherit;
}
.main-menu_link::before {
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
.main-menu_link:hover::before {
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
}
.button_header:hover {
    background-color: #CE93D8;
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
</style>
