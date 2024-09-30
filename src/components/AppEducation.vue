<template>
  <section id="formacion" class="section-03">
    <div class="above_section-03">
      <div class="description-above_section-03">
        <h1 class="title_sidebar">Formación</h1>
        <p class="date_sidebar">2023-2024</p>
        <p class="text-sidebar_section-03">
          Recientemente me he graduado del
          <span class="bold">Bootcamp de Desarrollo Web Fullstack (850h)</span>
          en Factoría F5 en colaboración con <span class="bold">Google.org</span> y Manpower Group.
        </p>
        <p class="text-sidebar_section-03">
          Destacar el trabajo en equipo, la Metodología Scrum, el estudio de Maquetación Web, Diseño UX/UI y programación Front-end, lo que me permite abordar proyectos de manera integral.
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
          Adquisición de habilidades esenciales en Investigaciones UX, confección de User Persona y User Flow. Se proponen soluciones de diseño, se crean esquemas, prototipos e interfaces.
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
          <p class="date_sidebar">2018 - 2020</p>
          <p class="text-sidebar_section-03">
            <b class="bold">
              Maquetadora - correctora ortotipográfica - diseñadora gráfica
            </b>
          </p>
          <p class="text-sidebar_section-03">Entrelíneas Editores</p>
          <p class="date_sidebar">2010 - 2023</p>
          <p class="text-sidebar_section-03">
            <b class="bold">
              Comercial de ventas / Asesora / Promotora
            </b>
          </p>
          <p class="text-sidebar_section-03">Media Markt · El Corte Inglés · Worten · Alcampo</p>
      </div>
      <div class="card-cv_section-03">
        <a href="https://drive.google.com/file/d/1eqcxrCOnaMXNDoOg0VTY0N0z2tiPsSRW/view?usp=drive_link" target="_blank">
          <img width="70" height="70" src="https://img.icons8.com/color/70/parse-from-clipboard.png" alt="parse-from-clipboard"/>
          <h4 class="title_sidebar-card-02">Ver Currículum Vitae de Desirée</h4>
        </a>
      </div>
      
      <div class="card_certificates">
        <a href="https://www.canva.com/design/DAGQ2QPMAXk/cEMOxf2Ff1jZxUueM5p3iw/watch" target="_blank">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate00.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate01.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate02.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate03.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate04.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate05.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate06.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate07.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate08.png" alt="Certificados obtenidos por Desirée Silva">
        <img class="carousel-certificate" src="@/assets/certificates/card-certificate09.png" alt="Certificados obtenidos por Desirée Silva"></a>
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
  margin-top: 1rem;
}

.text-sidebar_section-03 {
  font-size: 1.1rem;
  margin: 0.3rem 0;
}

.date_sidebar {
  font-weight: 800;
  font-size: 1.3rem;
  font-style: normal;
  margin: 0.5rem 0;
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
  border-radius: 45px;
  padding: 0 1.5rem;
  width: auto;
  height: auto;
  flex: 0.6;
}

.bold {
  font-weight: 700;
}

.card-01_section-03 {
  display: flex;
  flex-direction: column;
  width: auto;
  height: auto;
  background-color: #ffccbc;
  border-radius: 45px;
  padding: 1rem 1.5rem;
  flex: 1;
}
.card-02_section-03 {
  border: solid 2px #ffccbc;
  border-radius: 45px;
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
  background-image: url("@/assets/avatar.png");
  background-position: right;
  background-repeat: no-repeat;
  width: 100%;
  min-height: 130px;
  
  flex: 1;

  a {
    display: flex;
    flex-direction: column;
    text-decoration: none;
    color: #000000;
    padding: 0.4rem;

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
.card-02_section-03 h2 {
  z-index: 1;
}

.column-cards_section-03 {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  flex: 1;
  
  .card-03_section-03 {
    width: auto;
    height: auto;
    background-color: #f8bbd0;
    border-radius: 45px;
    padding: 1rem 1.5rem;
    padding-bottom: 1.5rem;
    }
}

.below_section-03 {
  display: flex;
  width: auto;
  height: auto;
  justify-content: stretch;
  align-items: center;
  gap: 1.5rem;
}    

.description-below_section-03 {
    background-color: #fff9c4;
    border-radius: 45px;
    padding: 0 1.5rem 1rem 1.5rem;
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
      height: 100%;
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }

    .carousel-certificate.active {
      display: block;
      opacity: 1;
      height: 100%;
    }
}

.card-cv_section-03 {
  border: solid 2px #ffccbc;
  border-radius: 30px;
  display: flex;
  align-items: center;
  background-image: url("@/assets/avatar-00.png");
  background-position: right;
  background-repeat: no-repeat;
  background-size: 10rem;
  width: 100%;
  height: 100%;
  min-height: 170px;
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

    h4 {
      padding-left: 0.5rem;
    }
  }
}
.card-cv_section-03 h4 {
  z-index: 1;
}

.card-02_section-03:active, .card-cv_section-03:active {
  transform: scale(1.1); 
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3); 
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}


/* Media Queries */

@media only screen and (max-width: 768px) {

  .date_sidebar {
    color: #000000;
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
    align-content: center;
    justify-content: center;
    height: auto;
    box-sizing: border-box;
  }

  .above_section-03 {
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .below_section-03 {
    width: 100%;
    height: auto;
    flex-direction: column-reverse;
    align-content: center;
    justify-content: center;
    padding: 0.5rem;
  }

  .description-below_section-03 {
    width: 100%;
    padding: 1rem;
    box-sizing: border-box;
  }

  .card-02_section-03 h2{
    font-size: 100%;
  }

  .card-cv_section-03 {
    width: 100%;
  }
}



@media only screen and (max-width: 1024px) {
  .section-03 {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    height: auto;
    box-sizing: border-box;
  }

  .above_section-03 {
    display: flex;
    flex-direction: column;
  }

  .below_section-03 {
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .description-below_section-03 {
    width: 100%;
    padding: 1rem;
    box-sizing: border-box;
  }
  .card-02_section-03 , .card-cv_section-03 {
    max-width: 70%;
  }
}

@media only screen and (min-width: 1920px) {

  .above_section-03 {
    gap: 2.5rem;
  }

  .card-cv_section-03 {
    max-width: 25rem;
  }
}
</style>
