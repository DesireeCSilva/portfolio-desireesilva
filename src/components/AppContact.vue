<template>
  <section id="section-05" class="section-05">
    <div class="text_section-05">
      <h1 class="title_sidebar">¡Hablemos!</h1>
      <p class="text_sidebar">
        ¿Qué te parece empezar a construir algo increíble juntos? Estoy abierta
        a colaboraciones.
      </p>
    </div>
    <form class="form_section-05" action="" method="get">
      <label for="nombre"></label>
      <input id="nombre" type="text" class="input-form" placeholder="Nombre" />
      <label for="email"></label>
      <input id="email" type="text" class="input-form" placeholder="Email" />
      <label for="Comentarios"></label>
      <input
        id="nombre"
        type="text"
        class="input-placeholder"
        placeholder="Comentarios"
      />

      <div class="content-button_section-05">
        <button
          type="submit"
          class="button-send_section-05"
          value="Enviar"
          onclick=""
        >
          <img
            class="icon_section-05"
            src="@/assets/icons/fa_send.png"
            alt=""
          />Enviar
        </button>
        <button
          type="submit"
          class="button-whatsapp_section-05"
          value="WhatsApp"
        >
          <a href="tel:675937952" target="_blank">
            <img
              class="icon_section-05"
              src="@/assets/icons/ic_twotone-whatsapp.png"
              alt=""
            />¡WhatsApp!</a
          >
        </button>
        <button type="submit" class="button-call_section-05">
          <a href="mailto:desiree_cs@hotmail.com" target="_blank">
            <img
              class="icon_section-05"
              src="@/assets/icons/mdi_email-outline.png"
              alt=""
            />Contáctame
          </a>
        </button>
      </div>
    </form>
  </section>
  <hr class="hr_portfolio">
</template>

<script></script>

<style lang="scss">
.section-05 {
    display: flex;
    justify-content: space-between;
}
.text_section-05{
    width: 25rem;
    height: 20rem;
    background-color: #E1BEE7;
    border-radius: 30px;
    padding: 1rem;
}
.form_section-05 {
    border: solid 2px #FFCCBC;
    border-radius: 30px;
    width: 48rem;
    padding: 1rem;
}
.input-form{
    width: 20rem;
    height: 3rem;
    border: solid 2px #FFCCBC;
    border-radius: 20px;
    margin: 1rem;
    font-size: 1rem;
    font-family: 'Poppins';
    padding-left: 1rem;
}
.input-placeholder {
    width: 43.6rem;
    height: 6rem;
    border: solid 2px #FFCCBC;
    border-radius: 20px;
    margin: 1rem;
    font-size: 1rem;
    font-family: 'Poppins';
    padding-left: 1rem;
}
.content-button_section-05 {
    display: flex;
    justify-content: space-evenly;
}
.icon_section-05 {
    width: fit-content;
    height: fit-content;
    margin-right: 0.3rem;
}
.button-send_section-05 {
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
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); 
    transition: all 0.3s ease; 
}
.button-send_section-05:hover {
    background-color: #CE93D8; 
    transform: scale(0.95); 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
}
.button-send_section-05:active {
    background-color: #bc38d3; 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
    transform: translateY(2px);
}

.button-whatsapp_section-05 {
    background-color: #F8BBD0;
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
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); 
    transition: all 0.3s ease; 
}
.button-whatsapp_section-05:hover {
    background-color: #F8BBD0;
    transform: scale(0.95); 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
}
.button-whatsapp_section-05:active {
    background-color: #ee427e; 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
    transform: translateY(2px); 
}

.button-call_section-05 {
    background-color: #FFCCBC;
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
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); 
    transition: all 0.3s ease; 
}
.button-call_section-05:hover {
    background-color: #FFCCBC;
    transform: scale(0.95); 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
}
.button-call_section-05:active {
    background-color: #fa8662; 
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); 
    transform: translateY(2px); 
}
.button-call_section-05 a, .button-send_section-05 a, .button-whatsapp_section-05 a {
    display: flex;
    text-decoration: none;
    color: #000000;
}
.hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}
</style>
