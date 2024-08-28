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
  gap: 1.5rem;

  &_left {
    border: solid 2px #e1bee7;
    border-radius: 30px;
    padding: 1rem;
    width: 70rem;

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

  &_center {
    width: fit-content;
    height: fit-content;
  }

  &_right {
    display: flex;
    flex-direction: column;  

    .above-right_section-01 {
      background-color: #fff9c4;
      border-radius: 30px;
      padding: 1rem;
      margin-bottom: 1rem;
    }
    .text_descriptions {
      font-size: 1.1rem;
    }
    .below-right_descriptions {
      border: solid 2px #ffccbc;
      border-radius: 30px;
      padding: 1rem;
      height: fit-content;
    }
    .title_below-right_descriptions {
      font-size: 1.2rem;
      color: #000000;
      opacity: 50%;
    }
    .items_below-right_descriptions {
      display: flex;
      flex-wrap: wrap;
    }
    .item-text_descriptions {
      outline: solid 2px #ffccbc;
      border-radius: 20px;
      padding: 0.6rem;
      margin-bottom: 0.7rem;
    }
  }
}
.hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}
</style>
