<template>
  <section id="section-05" class="section-05">
    <div class="text_section-05">
      <h1 class="title_sidebar">¡Hablemos!</h1>
      <p class="text_sidebar">
        ¿Qué te parece si empezamos a construir algo increíble juntos? Estoy
        convencida de que una colaboración puede llevarnos a crear proyectos
        excepcionales y de gran impacto. ¡Espero tu respuesta con mucho
        entusiasmo! 😊
      </p>
    </div>
    <form v-if="!mostrarMensaje" class="form_section-05">
      <div class="top-form">
        <label for="nombre"></label>
        <input
          id="nombre"
          name="nombre"
          type="text"
          class="input-form"
          v-model="nombre"
          placeholder="Nombre"
        />
        <label for="email"></label>
        <input
          id="email"
          name="email"
          type="text"
          class="input-form"
          v-model="email"
          placeholder="Email"
        />
      </div>
      <div>
      <label for="Comentarios"></label>
      <input
        id="comentarios"
        type="text"
        name="comentarios"
        class="input-placeholder"
        v-model="comentarios"
        placeholder="Comentarios"
      /></div>
      <div class="content-button_section-05">
        <button
          type="submit"
          class="button-send_section-05"
          value="Enviar"
          @click="sendEmail"
        >
          <img
            class="icon_section-05"
            src="@/assets/icons/fa_send.png"
            alt=""
          />Enviar
        </button>
        <button class="button-whatsapp_section-05" value="WhatsApp">
          <a href="tel:675937952" target="_blank">
            <img
              class="icon_section-05"
              src="@/assets/icons/ic_twotone-whatsapp.png"
              alt=""
            />¡WhatsApp!</a
          >
        </button>
        <button class="button-call_section-05">
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
    <div v-else>
      Tu formulario ha sido enviado con éxito. Gracias por tu mensaje
    </div>
  </section>
  <hr class="hr_portfolio hr_last" />
</template>

<script setup>
import { ref } from 'vue'
import emailjs from '@emailjs/browser';

const nombre = ref(undefined)
const email = ref(undefined)
const comentarios = ref(undefined)
const mostrarMensaje = ref(false)

const sendEmail = (e) => {
  const params = {
    nombre: nombre.value,
    email: email.value,
    comentarios: comentarios.value
  }
  e.preventDefault()
  emailjs
  .send('service_weteccf', 'template_5zps12h', params, {
    publicKey: 'L7sGgET0IWB0NrLB9',
  })
  .then(
    () => {
      mostrarMensaje.value = true
      setTimeout(() => mostrarMensaje.value = false, 4000)
    },
    (err) => console.log('FAILED...', err)
  )
}

</script>

<style lang="scss">
.section-05 {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-content: center;
  gap: 1rem;
  width: 100%;
  box-sizing: border-box;
}

.text_section-05 {
  width: 30rem;
  height: auto;
  background-color: #e1bee7;
  border-radius: 30px;
  padding: 1rem;
  box-sizing: border-box;
}

.form_section-05 {
  border: solid 2px #ffccbc;
  border-radius: 30px;
  max-width: 48rem;
  height: auto;
  padding: 1rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  box-sizing: border-box;
}
.top-form {
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-between;  
  gap: .5rem;
}
.input-form {
  width: 100%;
  height: 3rem;
  border: solid 2px #ffccbc;
  border-radius: 20px;
  margin: 1rem 0; 
  font-size: 1rem;
  font-family: "Poppins";
  padding-left: 1rem;
  box-sizing: border-box;
}

.input-placeholder {
  width: 43.6rem;
  height: 6rem;
  border: solid 2px #ffccbc;
  border-radius: 20px;
  font-size: 1rem;
  font-family: "Poppins";
  padding-left: 1rem;
  box-sizing: border-box; 
}

.content-button_section-05 {
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-between;
  margin-top: 1rem;
  margin-bottom: 1rem;
  align-items: center;
  gap: 0.5rem; 
}

.icon_section-05 {
  width: fit-content;
  height: fit-content;
  margin-right: 0.3rem;
}

.button-send_section-05 {
  background-color: #ce93d8;
  width: 10em;
  height: fit-content;
  font-size: 1.3rem;
  font-family: "Poppins";
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  border-radius: 0.5rem;
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
  background-color: #ce93d8;
  transform: scale(0.95);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}
.button-send_section-05:active {
  background-color: #bc38d3;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  transform: translateY(2px);
}

.button-whatsapp_section-05 {
  background-color: #f8bbd0;
  width: 10em;
  height: fit-content;
  font-size: 1.3rem;
  font-family: "Poppins";
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  border-radius: 0.5rem;
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
  background-color: #f8bbd0;
  transform: scale(0.95);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}
.button-whatsapp_section-05:active {
  background-color: #ee427e;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  transform: translateY(2px);
}

.button-call_section-05 {
  background-color: #ffccbc;
  width: 10em;
  height: fit-content;
  font-size: 1.3rem;
  font-family: "Poppins";
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  border-radius: 0.5rem;
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
  background-color: #ffccbc;
  transform: scale(0.95);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}
.button-call_section-05:active {
  background-color: #fa8662;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  transform: translateY(2px);
}

.button-call_section-05 a,
.button-send_section-05 a,
.button-whatsapp_section-05 a {
  display: flex;
  text-decoration: none;
  color: #000000;
}
.hr_portfolio {
  color: #ce93d8;
  width: 100%;
  margin-top: 2rem;
  margin-bottom: 2rem;
}

.hr_portfolio.hr_last {
  margin-bottom: 0;
}

// Medias Queries

@media only screen and (max-width: 768px) {
  .section-05 {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  
  }

  .text_section-05 {
    width: 100%;
    height: auto;
    background-color: #e1bee7;
    border-radius: 30px;
    padding: 1rem;
  }

  .form_section-05 {
    border: solid 2px #ffccbc;
    border-radius: 30px;
    width: 100%;
    height: auto;
    padding: 1rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }

  .input-form,
  .input-placeholder {
    width: 100%;
    margin: 0.5rem 0; 
    min-width: 20rem;
    box-sizing: border-box;
  }

  .top-form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 0;
  }

  .input-placeholder {
    width: 100%;
  }

  .content-button_section-05 {
    display: flex;
    flex-direction: column;
    width: 100%;
    align-items: center;
    gap: 0.5rem;
  }

  .button-send_section-05,
  .button-whatsapp_section-05,
  .button-call_section-05 {
    width: 100%;
    margin: 0.5rem 0;
  }
}
</style>
