<template>
  <section id="section-03" class="section-03">
    <div class="above_section-03">
      <div class="description-above_section-03">
        <h1 class="title_sidebar">Formación</h1>
        <div class="text_sidebar">
          <p class="date_sidebar">2024- 2023</p>
          <p class="text_sidebar">
            Recientemente me he graduado del
            <spannp class="bold"
              >Bootcamp de Desarrollo Web Fullstack (850h)</spannp
            >
            en Factoría F5 en colaboración con Google.org.
          </p>
          <p class="text_sidebar">
            Destacar el aprendizaje de Metodología Scrum, el trabajo en equipo,
            el estudio de UX/UI, la programación Front-end y la maquetación web.
          </p>
        </div>
      </div>

      <div class="card-01_section-03">
        <p class="date_sidebar">2024</p>
        <p class="text_sidebar">
          <span class="bold" > Diseño de Experiencia del Usuario UX de Google (7 cursos)</span
          >
        </p>
        <p class="text_sidebar">
          Se proponen soluciones de diseño, se crean esquemas y prototipos.
        </p>
        <p class="date_sidebar">2023</p>
        <p class="text_sidebar">
          <span class="bold"
            >Curso Interfaces y Experiencia de Usuario UI UX </span
          >en Centro de Referencia Nacional Getafe (CFTIC)
        </p>
        <p class="text_sidebar">
          Señalar el prototipado de proyectos en Figma, la creación de
          interfaces que maximizan la usabilidad, la creación de User Persona y
          diagramas de flujo.
        </p>
      </div>
      <div>
      <div class="column-cards_section-03">
        <div class="card-02_section-03">
          <a href="https://github.com/DesireeCSilva" target="_blank">
            <img src="@/assets/icons/GitHub.png" alt="logotipo de GitHub" />
            <h2 class="title_sidebar-card-02">github.com/DesireeCSilva</h2>
          </a>
        </div>

        <div class="card-03_section-03">
          <p class="date_sidebar">2018</p>
          <p class="text_sidebar">
            Curso
            <span class="bold">ARGN0210 Asistencia a la Edición (490h)</span>
          </p>
          <p class="text_sidebar">Masercisa Fuenlabrada</p>
          <p class="date_sidebar">2008-2010</p>
          <p class="text_sidebar">
            Ciclo de Grado Superior de
            <span class="bold">Diseño y Producción Editorial</span> 
            + Ciclo de Grado Superior de
            <span class="bold">Producción en Industrias de Artes Gráficas</span>
          </p>
          <p class="text_sidebar">IES Europa - IES Islas Filipinas</p>
        </div>
      </div>
      </div>
    </div>
    <div class="below_section-03">
      <div class="description-below_section-03">
        <h1 class="title_sidebar">Experiencia</h1>
        <div class="text_sidebar">
          <p class="date_sidebar">2020 - 2018</p>
          <p class="text_sidebar">
            <span class="bold">
              Maquetadora - correctora ortotipográfica - diseñadora gráfica
            </span>
          </p>
          <p class="text_sidebar">Entrelíneas Editores</p>
        </div>
      </div>
      <div class="card_certificates">
        <img src="@/assets/certificates/card-certificate.png" alt="">
      </div>
    </div>
  </section>
  <hr class="hr_portfolio">
</template>

<script>
</script>

<style lang="scss">

.section-03 {
  padding: 1rem;
  height: auto;
  width: 100%;
}
.above_section-03 {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: row;
  gap: 1.5rem;
  justify-content: space-between;
  margin-bottom: 1.5rem;
  padding-right: 1rem;
  > div {
    flex: 1; 
  }
} 

.description-above_section-03,
.card-01_section-03,
.card-03_section-03 {
  background-color: #e1bee7;
  border-radius: 30px;
  padding: 1rem;
  width: auto;
  width: 30%; 
  flex: 1; 
}

.description-above_section-03 {
  background-color: #e1bee7;
  border-radius: 30px;
  padding: 1rem;
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
  width: auto;
  background-color: #ffccbc;
  border-radius: 30px;
  padding: 1rem;
}
.card-02_section-03 {
  border: solid 2px #ffccbc;
  border-radius: 30px;
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
  background-image: url('@/assets/avatar.png'); 
  background-position: right; 
  background-repeat: no-repeat; 
  width: 100%; 
  min-height: 130px;
  padding: 0.2rem;

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
  width: 5rem;
  height: 5rem;
  z-index: -1;
  margin-right: 0.5rem;
}

.card-03_section-03 {
  width: auto;
  height: auto;
  background-color: #f8bbd0;
  border-radius: 30px;
  padding: 1rem;
}
.below_section-03 {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
.description-below_section-03 {
  background-color: #fff9c4;
  border-radius: 30px;
  padding: 1rem;
  min-width: 50rem;
  height: auto;
}

.column-cards_section-03 {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
}

/* Media Queries */

@media only screen and (max-width: 768px) {

  .section-03 {
  display: flex;
  flex-direction: column;
  padding: 1rem;
  height: auto;
}
  .above_section-03 {
    flex-direction: column;
    align-items: center;
    
    > div {
      width: 100%; 
      max-width: 100%; 
      margin-bottom: 1rem; 
    }
  }

  .below_section-03 {
    flex-direction: column-reverse;
    align-items: center;
    justify-content: center;
  }

  .description-below_section-03 {
    width: 100%; 
  }

  
}


</style>
