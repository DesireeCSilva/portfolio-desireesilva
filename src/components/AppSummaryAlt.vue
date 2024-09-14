<template>
  <section id="about-me" class="about-me">
    <div class="about-me_left">
      <h1 class="gradient">DISEÑADORA UX/UI<br />MAQUETADORA WEB</h1>
      <p class="text_sidebar-section-01">
        ¡Hola! Soy Desirée y vivo en Madrid. Estudié Diseño Gráfico porque
        siempre he sido una apasionada del arte y la tecnología. Acabo de
        graduarme en un Bootcamp de Desarrollo Web, y me he formado en Diseño
        UX/UI realizando cursos y aplicando la pedagogía activa.
      </p>
    </div>
    <div class="about-me_center">
      <img class="carousel-image" src="@/assets/pic-01.png" alt="Imagen 1">
      <img class="carousel-image" src="@/assets/pic-02.png" alt="Imagen 2">
      <img class="carousel-image" src="@/assets/pic-03.png" alt="Imagen 3">
      <img class="carousel-image" src="@/assets/pic-04.png" alt="Imagen 4">
      <img class="carousel-image" src="@/assets/pic-05.png" alt="Imagen 5">
      <img class="carousel-image" src="@/assets/pic-06.png" alt="Imagen 6">
      <img class="carousel-image" src="@/assets/pic-07.png" alt="Imagen 7">
      <img class="carousel-image" src="@/assets/pic-08.png" alt="Imagen 8">
      <img class="carousel-image" src="@/assets/pic-09.png" alt="Imagen 9">
    </div>
    <div class="about-me_right">
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

.about-me {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 1.5rem;


  &_left {
    border: solid 2px #e1bee7;
    border-radius: 30px;
    padding: 1rem;
    flex: 0.6;

    .gradient {
      font-size: 1.3rem;
      font-weight: 800;
      background-image: linear-gradient(260deg, var(--purple), var(--green));
      background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .text_sidebar-section-01 {
      font-size: 1.1rem;
    }
  }

  &_center {
    flex: 1;
    align-self: flex-start;
    display: flex;
    justify-content: center;
    align-items: center;

    .carousel-image {
      display: none;
      width: auto;
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
    justify-content: space-between;
    flex: 1;

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
      margin-bottom: 1rem;
    }
  }
}

// Media Queries

@media screen and (max-width: 768px) {

  .about-me {
    flex-direction: column;

    &_left {
      order: 2;
      
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

    .text_sidebar-section-01,
    .text_descriptions {
      font-size: 1rem; 
    }

    .item-text_descriptions {
      font-size: 0.85rem; 
    }
  }
}

@media only screen and (max-width: 1024px) {
    .about-me {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
    }

    .about-me_left,
    .about-me_center,
    .about-me_right {
      flex-basis: 100%; /* Asegura que los elementos ocupen todo el ancho disponible */
}
}

@media only screen and (min-width: 1920px) {
  .about-me {
  display: flex;
  justify-content: space-between;
  gap: 1.5rem;

  &_center {
    flex: 1;
  }
  &_right {
    flex: 1; 
  } 
  }

.about-me {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 1.5rem;


  &_left {
    flex: 1.1;

    .text_sidebar-section-01 {
      font-size: 1.5rem;
    }
  }
}                 
}
</style>
