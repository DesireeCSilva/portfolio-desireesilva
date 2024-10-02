<template>
  <section id="contacto" class="section-05">
    <div class="text_section-05">
      <h1 class="title_sidebar">¡Hablemos!</h1>
      <p class="text_descriptions">
        ¿Qué te parece si empezamos a construir algo increíble juntos? Estoy
        convencida de que una colaboración puede llevarnos a crear proyectos
        excepcionales y de gran impacto. ¡Espero tu respuesta con mucho
        entusiasmo! 😊
      </p>
    </div>
    <form v-if="!mostrarMensaje" class="form_section-05">
      <div class="top-form">
        <div class="input-container">
          <label for="nombre"></label>
          <input
            required
            minlength="3"
            id="nombre"
            name="nombre"
            type="text"
            class="input-form"
            v-model="nombre"
            placeholder="Nombre"
            :class="{ error: errorNombre }"
          />
          <span class="error-message" v-if="errorNombre">Este campo no puede estar vacío</span>
        </div>
        <div class="input-container">
          <label for="email"></label>
          <input
            required
            id="email"
            name="email"
            type="email"
            class="input-form"
            v-model="email"
            placeholder="Email"
            :class="{ error: errorEmail }"
          />
          <span class="error-message" v-if="errorEmail">Introduce un email correcto</span>
        </div>
      </div>
      <div class="bottom-form">
        <label for="Comentarios"></label>
        <input
          required
          minlength="10"
          id="comentarios"
          type="text"
          name="comentarios"
          class="input-placeholder"
          v-model="comentarios"
          placeholder="Comentarios"
          :class="{ error: errorComentarios }"
        />
        <span class="error-message" v-if="errorComentarios">Este campo no puede estar vacío</span>
      </div>
      <div class="content-button_section-05">
        <button
          type="submit"
          class="button-send_section-05"
          value="Enviar"
          @click="submitForm"
        >
        <img width="40" height="40" src="https://img.icons8.com/color/48/circled-chevron-right--v1.png" alt="circled-chevron-right--v1"/>
        Enviar
        </button>
        <button class="button-whatsapp_section-05" value="WhatsApp">
          <a href="tel:675937952" target="_blank">
            <img width="40" height="40" src="https://img.icons8.com/color/48/whatsapp--v1.png" alt="whatsapp--v1"/>¡WhatsApp!
            </a>
        </button>
        <button class="button-call_section-05">
          <a href="mailto:desiree_cs@hotmail.com" target="_blank">
            <img width="40" height="40" src="https://img.icons8.com/color/96/circled-envelope.png" alt="circled-envelope"/>Contáctame
          </a>
        </button>
      </div>
    </form>
    <div class="sweet-alert" v-else>
      <p>Tu formulario ha sido enviado con éxito. <br>¡Gracias por tu mensaje!</p>
    </div>
  </section>
  <hr class="hr_portfolio hr_last" />
</template>

<script setup>
import { ref } from 'vue'
import emailjs from '@emailjs/browser';

const nombre = ref('')
const errorNombre = ref(false)
const email = ref('')
const errorEmail = ref(false)
const comentarios = ref('')
const errorComentarios = ref(false)
const mostrarMensaje = ref(false)

// Submit form
const submitForm = (e) => {
  e.preventDefault()

  const isValid = validate()
  if (isValid) sendEmail()
}

// Form basic validation 
const validate = () => {
  errorNombre.value = nombre.value === ""
  errorEmail.value = email.value === "" || !emailIsValid(email.value)
  errorComentarios.value = comentarios.value === ""
  if (nombre.value === "") return false
  if (email.value === "" || !emailIsValid(email.value)) return false
  if (comentarios.value === "") return false
  return true
}

// Basic pattern validation for email
const emailIsValid = email => {
  return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
}

// Send email
const sendEmail = () => {
  const params = {
    nombre: nombre.value,
    email: email.value,
    comentarios: comentarios.value
  }
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
  gap: 2rem;
  width: auto;
  box-sizing: border-box;

  .text_section-05 {
    width: 50%;
    height: auto;
    background-color: #e1bee7;
    border-radius: 45px;
    padding: 1rem 1.5rem;
    box-sizing: border-box;
  }

  .form_section-05 {
    border: solid 2px #ffccbc;
    border-radius: 45px;
    width: 100%;
    height: auto;
    padding: 1.5rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;

    .top-form {
      display: flex;
      flex-direction: row;
      width: 100%;
      justify-content: space-between;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .bottom-form {
      display: flex;
      flex-direction: column;
      width: 100%;
    }

    .input-container {
      flex: 1;
      display: flex;
      flex-direction: column;
    }

    .input-form {
      width: 100%;
      height: 3rem;
      border: solid 2px #ffccbc;
      border-radius: 20px;
      margin: 0;
      font-size: 1rem;
      font-family: "Poppins";
      padding-left: 1rem;
      box-sizing: border-box;
    }

    .input-placeholder {
      width: 100%;
      min-height: 6rem;
      border: solid 2px #ffccbc;
      border-radius: 20px;
      font-size: 1rem;
      font-family: "Poppins";
      padding-left: 1rem;
      box-sizing: border-box;
    }

    .error {
      border: 1px solid #ff0000 !important;
    }

    .error-message {
      color: #ff0000;
      font-size: 0.9rem;
      margin-top: 0.2rem;
      margin-bottom: 0.2rem;
    }

    .content-button_section-05 {
      display: flex;
      flex-direction: row;
      width: 100%;
      justify-content: space-between;
      align-items: center;
      margin: 0;
      flex-wrap: wrap;
      gap: 2rem;

      .button-send_section-05,
      .button-whatsapp_section-05,
      .button-call_section-05 {
        background-color: #ce93d8;
        color: #000000;
        width: 10em;
        height: fit-content;
        font-size: 1.3rem;
        font-family: "Poppins";
        padding: 0.5rem 0;
        border-radius: 0.5rem;
        border: none;
        cursor: pointer;
        text-decoration: none;
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 0.3rem;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        transition: all 0.3s ease;

        &:hover {
          transform: scale(0.95);
          box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        }

        &:active {
          background-color: #bc38d3;
          box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
          transform: translateY(2px);
        }

        a {
          display: flex;
          text-decoration: none;
          color: #000000;
          justify-content: center;
          align-items: center;
          gap: 0.2rem;
        }
      }
    }
  }

  .sweet-alert {
    background-color: #fa8662;
    border-radius: 30px;
    padding: 1rem;
    width: auto;

    p {
      font-family: 'Poppins';
      font-size: 2.5rem;
      color: #ffffff;
      text-align: center;
    }
  }

  .hr_portfolio {
    color: #ce93d8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;

    &.hr_last {
      margin-bottom: 0;
    }
  }

  .text_descriptions {
    font-size: 1.1rem;
  }
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
  }

  .form_section-05 {
    .input-form,
    .input-placeholder {
      width: 100%;
      margin: 0.5rem 0;
      box-sizing: border-box;
    }

    .error-message {
      margin-top: -0.5rem;
      margin-bottom: 0.5rem;
    }

    .top-form {
      display: flex;
      flex-direction: column;
      justify-content: center;
      gap: 0;
    }

    .content-button_section-05 {
      flex-direction: column;
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
}

@media only screen and (min-width: 1024px) and (max-width: 1240px) {
  .content-button_section-05 {
    justify-content: space-evenly;
    gap: 0.5rem;

    .button-send_section-05,
    .button-whatsapp_section-05,
    .button-call_section-05 {
      width: 80%;
    }
  }
}

@media only screen and (min-width: 1920px) {
  .section-05 {
    gap: 5.5rem;
  }
}


</style>
