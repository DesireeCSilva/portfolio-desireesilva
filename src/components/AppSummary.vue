<template>
  <section id="section-01" class="section-01">
    <div class="section-01_left">
      <h1 class="gradient">DISEÑADORA UX/UI<br />MAQUETADORA WEB</h1>
      <p class="text_sidebar">
        ¡Hola! Soy Desirée y vivo en Madrid. Estudié Diseño Gráfico porque
        siempre he sido una apasionada del arte y la tecnología. Acabo de
        graduarme en un Bootcamp de Desarrollo Web, y me he formado en Diseño
        UX/UI realizando cursos y aplicando la pedagogía activa.
      </p>
    </div>
    <div class="section-01_center">
      <img
        src="@/assets/pic-01.png"
        alt="imágenes del Portfolio en after delay"
        class="section-01_after-delay"
      />
    </div>
    <div class="section-01_right">
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

<script>
export default {};
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

.section-01 {
  display: flex;
  flex-direction: row;
  align-items: center;  
  justify-content: space-between;
  gap: 1rem;
  width: auto;
  height: auto; 

  &_left,
  &_right {
    flex: 1; 
    display: flex;
    flex-direction: column;
    justify-content: center;
    
  }
    &_center {
    flex: 1.2; 
    display: flex;
    justify-content: center;
    align-items: center;
  }

  &_left {
    border: solid 2px #e1bee7;
    border-radius: 30px;
    width: auto;
    height: fit-content;
    padding: 1rem;
    margin: 1rem 0; 

    .gradient {
      font-size: 1.3rem;
      font-weight: 800;
      background-image: linear-gradient(260deg, var(--purple), var(--green));
      background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .text_sidebar {
      font-size: 1.2rem;
    }
  }

  &_right {
    display: flex;
    flex-direction: column; 
    justify-content: center; 
    width: auto;
    height: auto;

    .above-right_section-01 {
      background-color: #fff9c4;
      border-radius: 30px;
      padding: 1rem;
      width: auto;
      height: auto;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .text_descriptions {
      font-size: 1.1rem;
    }
    .below-right_descriptions {
      border: solid 2px #ffccbc;
      border-radius: 30px;
      padding: 1rem;
      width: auto;
      height: fit-content;
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
      font-size: 0.72rem; 
    }
  }
}
.section-01_after-delay {
  max-width: 25rem; 
  width: 100%; 
  height: auto; 
}

.hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}

// Media Queries

@media only screen and (max-width: 768px) {
  .section-01 {
    flex-direction: column;
    gap: 1rem; 
    padding: 1rem;
    align-items: center;
    margin: 1rem 0;

    &_left,
    &_center,
    &_right {
      width: 100%; 
      align-items: center;

    }
    &_left {
      margin: 1rem;
      box-sizing: border-box;
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

  .section-01_after-delay { 
  width: 100%; 
  height: auto; 
}

  .hr_portfolio {
    display: none;
  }
}
</style>
