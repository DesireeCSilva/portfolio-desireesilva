<template>
  <section id="section-03" class="section-03">
    <div class="above_section-03">
      <div class="description-above_section-03">
        <h1 class="title_sidebar">Formación</h1>
        <p class="date_sidebar">2024-2023</p>
        <p class="text-sidebar_section-03">
          Recientemente me he graduado del
          <span class="bold">Bootcamp de Desarrollo Web Fullstack (850h)</span>
          en Factoría F5 en colaboración con Google.org.
        </p>
        <p class="text-sidebar_section-03">
          Destacar el aprendizaje de Metodología Scrum, el trabajo en equipo, el
          estudio de UX/UI, la programación Front-end y la maquetación web.
        </p>
      </div>

      <div class="card-01_section-03">
        <p class="date_sidebar">2024</p>
        <p class="text-sidebar_section-03">
          <span class="bold">
            Diseño de Experiencia del Usuario UX de Google (7 cursos)</span
          >
        </p>
        <p class="text-sidebar_section-03">
          Se proponen soluciones de diseño, se crean esquemas y prototipos.
        </p>

        <p class="date_sidebar">2023</p>
        <p class="text-sidebar_section-03">
          <span class="bold"
            >Curso Interfaces y Experiencia de Usuario UI UX </span
          >en Centro de Referencia Nacional Getafe <span class="bold">(CFTIC)</span>
        </p>
        <p class="text-sidebar_section-03">
          Señalar el prototipado de proyectos en Figma, la creación de
          interfaces que maximizan la usabilidad, la creación de User Persona y
          diagramas de flujo.
        </p>
      </div>
        <div class="column-cards_section-03">
          <div class="card-02_section-03">
            <a href="https://github.com/DesireeCSilva" target="_blank">
              <img src="@/assets/icons/GitHub.png" alt="logotipo de GitHub" />
              <h2 class="title_sidebar-card-02">github.com/DesireeCSilva</h2>
            </a>
          </div>

          <div class="card-03_section-03">
            <p class="date_sidebar">2018</p>
            <p class="text-sidebar_section-03">
              Curso
              <span class="bold">ARGN0210 Asistencia a la Edición (490h)</span>
            </p>
            <p class="text-sidebar_section-03">Masercisa Fuenlabrada</p>
              
            
            <p class="date_sidebar">2008-2010</p>
            <p class="text-sidebar_section-03">
              Ciclo de Grado Superior de
              <span class="bold">Diseño y Producción Editorial</span>
              + Ciclo de Grado Superior de
              <span class="bold"
                >Producción en Industrias de Artes Gráficas</span
              >
            </p>
            <p class="text-sidebar_section-03">IES Europa - IES Islas Filipinas</p>
          </div>
        </div>
    </div>
    <div class="below_section-03">
      <div class="description-below_section-03">
        <h1 class="title_sidebar">Experiencia</h1>
          <p class="date_sidebar">2020 - 2018</p>
          <p class="text-sidebar_section-03">
            <span class="bold">
              Maquetadora - correctora ortotipográfica - diseñadora gráfica
            </span>
          </p>
          <p style="margin-top: 1rem; font-size: 1.1rem;">Entrelíneas Editores</p>
      </div>
      <div class="card_certificates">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate00.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate01.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate02.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate03.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate04.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate05.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate06.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate07.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate08.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate09.png" alt="Certificados obtenidos por Desirée Silva">
      </div>
    </div>
  </section>
  <hr class="hr_portfolio" />
</template>

<script setup>
import { onMounted } from "vue"

onMounted(() => {
  document.addEventListener('DOMContentLoaded', function() {
    const images = document.querySelectorAll('.carousel-certificate')
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

.section-03 {
  height: auto;
  width: auto;
  display: flex;
  flex-direction: column;
}

.text-sidebar_section-03 {
  font-size: 1.1rem;
  margin: 0;
  margin-top: 0.2rem;
  display: inline;
}

.above_section-03 {
  width: auto;
  height: auto;
  display: flex;
  gap: 1.5rem;
  align-items: stretch;
  justify-content: space-between;
  margin-bottom: 1.5rem;
}

.description-above_section-03 {
  background-color: #e1bee7;
  border-radius: 30px;
  padding: 1rem;
  width: auto;
  height: auto;
  flex: 0.6;
}

.bold {
  font-weight: 700;
}

.date_sidebar {
  font-family: "Purple Purse", serif;
  font-weight: 400;
  font-size: 1.2rem;
  font-style: normal;
}

.card-01_section-03 {
  display: flex;
  flex-direction: column;
  width: auto;
  height: auto;
  background-color: #ffccbc;
  border-radius: 30px;
  padding: 1rem;
  flex: 1;
}
.card-02_section-03 {
  border: solid 2px #ffccbc;
  border-radius: 30px;
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
  background-image: url("@/assets/avatar.png");
  background-position: right;
  background-repeat: no-repeat;
  width: 100%;
  min-height: 130px;
  padding: 0.2rem;
  flex: 1;

  a {
    display: flex;
    flex-direction: column;
    text-decoration: none;
    color: #000000;

    img {
      width: 4rem;
    }

    h2 {
      padding-left: 8px;
    }
  }
}
.title_sidebar-card-02 {
  margin: 0;
}
.card-02_section-03 h1 {
  z-index: 1;
}
.avatar {
  min-width: 5rem;
  height: 5rem;
  z-index: -1;
  margin-right: 0.5rem;
}

.column-cards_section-03 {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  flex: 1;

}

.card-03_section-03 {
  width: auto;
  height: auto;
  background-color: #f8bbd0;
  border-radius: 30px;
  padding: 1rem;
  padding-bottom: 1.5rem;
}

.below_section-03 {
  display: flex;
  width: auto;
  height: auto;
  justify-content: space-between;
  align-items: center;
}

.description-below_section-03 {
  background-color: #fff9c4;
  border-radius: 30px;
  padding: 1rem;
  min-width: 50%;
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
}

.card_certificates {
  width: auto;
  height: 100%;

  .carousel-certificate {
      display: none;
      width: auto;
      max-width: 100%;
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }

    .carousel-certificate.active {
      display: block;
      opacity: 1;
    }
}

/* Media Queries */

@media only screen and (max-width: 768px) {

  .date_sidebar {
    color: #000000;
    text-decoration: overline dotted 5px #ce93d8;
    width: 100%;
  }

  .description-above_section-03 {
    min-width: 90%;
  }

.text-sidebar_section-03 {
  font-size: 1rem;
  margin: 0;
  display: inline;
}

.card-01_section-03 {
  display: flex;
  flex-direction: column;
  min-width: 90%;
  gap: 1.5rem;
  padding: 2.5rem 1rem;
}

.column-cards_section-03 {
  width: 100%;
}
.card-03_section-03 {
  display: flex;
  flex-direction: column;
  min-width: 90%;
  display: flex;
  flex-direction: column;
  padding: 2.5rem 1rem;
}

  .section-03 {
    display: flex;
    flex-direction: column;
  
    height: auto;
    box-sizing: border-box;
  }
  .above_section-03 {
    flex-direction: column;
    align-items: center;
  }

  .below_section-03 {
    width: auto;
    height: auto;
    flex-direction: column-reverse;
    align-content: center;
    justify-content: center;
  }

  .description-below_section-03 {
    width: 100%;
    padding: 1rem;
    box-sizing: border-box;
  }

  .below_section-03 {
    padding: 0.5rem;
  }
}

@media only screen and (min-width: 1920px) {

  .above_section-03 {
    gap: 2.5rem;
  }
}
</style>
