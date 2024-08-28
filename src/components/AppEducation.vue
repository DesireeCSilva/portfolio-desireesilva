<template>
  <section id="section-03" class="section-03">
    <div class="above_section-03">
      <div class="description-above_section-03">
        <h1 class="title_sidebar">Formación</h1>
        <div class="text_sidebar">
          <p class="date_sidebar">2024- 2023</p>
          <p class="text_sidebar">
            Recientemente me he graduado del
            <span class="bold"
              >Bootcamp de Desarrollo Web Fullstack (850h)</span
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
          <span class="bold"
            >Diseño de Experiencia del Usuario UX de Google (7 cursos)</span
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
      <img
        class="card-below_section-03"
        src="@/assets/card-06.png"
        alt="card con imagen de Harmony Heaven"
      />
      <img
        class="card-below_section-03"
        src="@/assets/card-07.png"
        alt="card con imagen de Tech Today"
      />
    </div>
  </section>
  <hr class="hr_portfolio">
</template>

<script></script>

<style lang="scss">
.above_section-03 {
  display: grid;
  grid-template-columns: 33% 33% 30%;
  margin-bottom: 1rem;
  gap: 1.5rem;
  justify-content: space-between;
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
  width: 25rem;
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
  background-color: #f8bbd0;
  border-radius: 30px;
  padding: 1rem;
}
.below_section-03 {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.card-below_section-03:hover {
  -webkit-transform: rotate(360deg);
  transform: rotate(360deg);
  transition: transform 0.5s ease-in-out;
}

.description-below_section-03 {
  background-color: #fff9c4;
  border-radius: 30px;
  padding: 1rem;
  width: 50rem;
}

.hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}
</style>
