<template>
  <section id="sobremi" class="sobremi">
    <div class="sobremi_left">
      <h1 class="gradient">DISEÑADORA UX/UI<br />MAQUETADORA WEB</h1>
      <p class="text_sidebar">
        ¡Hola! Soy Desirée y vivo en Madrid. Estudié Diseño Gráfico porque
        siempre he sido una apasionada del arte y la tecnología. Acabo de
        graduarme en un Bootcamp de Desarrollo Web, y me he formado en Diseño
        UX/UI realizando cursos y aplicando la pedagogía activa.
      </p>
    </div>
    <div class="sobremi_center">
      <img class="carousel-image" src="@/assets/pic-01.png" alt="Imagen 1">
      <img class="carousel-image" src="@/assets/pic-02.png" alt="Imagen 2">
      <img class="carousel-image" src="@/assets/pic-03.png" alt="Imagen 3">
    </div>
    <div class="sobremi_right">
      <div class="above-right_section-01">
        <p class="text_descriptions">
          Actualmente estoy inmersa en formaciones continuas de UX/UI, para
          conseguir soluciones innovadoras y funcionales que respondan a las
          necesidades de los usuarios.
        </p>
      </div>
      <div class="below-right_descriptions">
        <div class="title_below-right_descriptions">
          <p class="text_descriptions">Mis palabras clave</p>
        </div>
        <div class="items_below-right_descriptions">
          <p class="item-text_descriptions">Figma</p>
          <p class="item-text_descriptions">HTML</p>
          <p class="item-text_descriptions">CSS</p>
          <p class="item-text_descriptions">Web Design</p>
          <p class="item-text_descriptions">UX/UI</p>
          <p class="item-text_descriptions">Lean UX</p>
          <p class="item-text_descriptions">Responsive</p>
          <p class="item-text_descriptions">Happy Path</p>
        </div>
      </div>
    </div>
  </section>
  <hr class="hr_portfolio"> 
</template>

<script setup>
import { onMounted } from "vue"

onMounted(() => {
  document.addEventListener('DOMContentLoaded', function() {
    const images = document.querySelectorAll('.carousel-image')
    let currentIndex = 0
    
    function showImage(index) {
      images.forEach((img) => img.classList.remove('active'))
      images[index].classList.add('active')
    }

    function nextImage() {
      currentIndex = (currentIndex + 1) % images.length
      showImage(currentIndex)
    }

    // Show the first image initially
    showImage(currentIndex)

    // Change the image every 3 seconds
    setInterval(nextImage, 4000)
})
})
</script>

<style lang="scss">
:root {
  --white: #ffffff;
  --blue: #e1bee7;
  --purple: #7026f4;
  --yellow: #fff9c4;
  --pink: #ce93d8;
  --green: #fa8662;
  --green-light: #ffccbc;
}

.sobremi {
  display: flex;
  justify-content: space-between;
  gap: 1.5rem;

  &_left, &_center, &_right {
    flex: 1;
  }

  &_left {
    border: solid 2px #e1bee7;
    border-radius: 30px;
    padding: 1rem;

    .gradient {
      font-size: 1.3rem;
      font-weight: 800;
      background-image: linear-gradient(260deg, var(--purple), var(--green));
      background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .text_sidebar {
      font-size: 1.1rem;
    }
  }

  &_center {
    flex: 0.8;
    align-self: flex-start;
    display: flex;
    justify-content: center;
    align-items: center;

    .carousel-image {
      display: none;
      width: 100%;
      max-width: 100%;
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }

    .carousel-image.active {
      display: block;
      opacity: 1;
    }
  }

  &_right {
    display: flex;
    flex-direction: column;

    .above-right_section-01 {
      background-color: #fff9c4;
      border-radius: 30px;
      padding: 1rem 1.2rem;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .text_descriptions {
      font-size: 1.1rem;
    }

    .below-right_descriptions {
      flex: 1;
      display: flex;
      flex-direction: column;
      justify-content: center;
      border: solid 2px #ffccbc;
      border-radius: 30px;
      padding: 1rem;
      margin-top: 1rem;
    }

    .title_below-right_descriptions {
      font-size: 1.2rem;
      color: #000000;
      opacity: 0.5;
      margin-bottom: 0.5rem;
    }
    .items_below-right_descriptions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem; 
    }

    .item-text_descriptions {
      outline: solid 2px #ffccbc;
      border-radius: 20px;
      padding: 0.5rem 1rem; 
      margin: 0; 
      font-size: 0.9rem; 
    }
  }
}

// Media Queries

@media screen and (max-width: 768px) {
  .sobremi {
    flex-direction: column;

    &_left {
      order: 2;
      padding: 1rem ;
    }

    &_center {
      order: 1;
      width: 100%;
    }

    &_right {
      order: 3;
    }

    .gradient {
      font-size: 1.2rem; 
    }

    .text_sidebar,
    .text_descriptions {
      font-size: 1rem; 
    }

    .item-text_descriptions {
      font-size: 0.85rem; 
    }
  }
}
</style>
