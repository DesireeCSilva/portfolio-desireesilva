<template>
    <section id="section-02" class="section-02">
            <div class="above_section-02">
                <div class="description-above_section-02">
                    <h1 class="title_sidebar">Proyectos</h1>
                    <p class="text_sidebar">Mis trabajos se han basado en la investigación previa aplicando mis conocimientos UX, y la creación completa de la interfaz de la web/app para que la experiencia de usuario sea óptima.
                    </p>    
                </div>
                <div class="card-01_section-02">
                    <a href="https://www.figma.com/proto/yR8KjnndNATFkYYxFBxoUr/Proyecto--Nirname?page-id=1%3A2&node-id=1-2284&viewport=741%2C325%2C0.06&t=lld7nY527ALzDYMo-1&scaling=scale-down&content-scaling=fixed&starting-point-node-id=1%3A2284" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title_sidebar">Nirname. Centro de Yoga</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha">
                        </div>
                        <p class="text_descriptions">Creación de todas las screens de la web y realización de User Personas.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-01-section-02.png" alt="foto del Proyecto Nirname, centro de yoga">
                    </div>
                    </a>
                </div>

                <div class="card-02_section-02">
                    <a href="https://www.figma.com/proto/FviGi5i5nFR2VY8XDGYwlF/Actividades-Desir%C3%A9e?page-id=72%3A2&node-id=87-95&viewport=582%2C85%2C0.08&t=yJM7C3qV5cAIacNL-1&scaling=scale-down&content-scaling=fixed" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title_sidebar">Constructora Blocka</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha"> 
                        </div>
                    <p class="text_descriptions">Diseño responsive en desktop, tablet y mobile de la landing page.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-02-section-02.png" alt="foto del Proyecto Constructora Blocka">
                    </div>
                    </a>
                </div>
            </div>
            <div class="below_section-02">
                <div class="card-03_section-02">
                    <a href="https://www.figma.com/proto/LKQiFFZSCHntHlIkhviezT/Hackaton-Globant?page-id=0%3A1&node-id=1-2&viewport=313%2C141%2C0.09&t=p53fha0SbWl4NLxz-1&scaling=scale-down&content-scaling=fixed" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title_sidebar">Ecopop: proyecto Hackaton</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha">
                        </div>
                    <p class="text_descriptions">Diseño de un e-commerce en pocas horas, quedando en 2º puesto.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-03-section-02.png" alt="foto de Ecopop, una web de muebles de segunda mano">
                    </div>  
                    </a>
                </div>
                <div class="card-04_section-02">
                    <a href="https://www.figma.com/proto/4J8nTOfWZLkGK9tkFnDxex/TechToday?page-id=0%3A1&node-id=42-1501&viewport=865%2C225%2C0.22&t=CMG6Jheigb8PEICS-1&scaling=scale-down&content-scaling=fixed" target="_blank">
                        <div class="title_section-02">
                        <h1 class="title_sidebar">TechToday: web sostenible</h1>
                        <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha">
                    </div>
                    <p class="text_descriptions">Propuesta de desarrollo sostenible de una web de gestión de noticias.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-04-section-02.png" alt="foto del Proyecto Green Newspaper, un periódico digital con diseño sostenible">
                    </div>
                    </a>
                </div>
                <div class="card-05_section-02">
                    <a href="https://www.figma.com/proto/Q87bkn0d1SZRA2IEiHSqYz/HarmonyHeavenMVP?page-id=0%3A1&node-id=1-867&viewport=1041%2C340%2C0.09&t=pT2HNtwFQ5w3zb2B-1&scaling=scale-down&content-scaling=fixed&starting-point-node-id=1%3A867&show-proto-sidebar=1" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title_sidebar">Harmony Heaven</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha"> 
                        </div>
                    <p class="text_descriptions">Diseño responsive para una web de instrumentos interactivos.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-05-section-02.png" alt="foto de Harmony Heaven, una web para tocar instrumentos">
                    </div>
                    </a>
                </div>
            </div>
        </section>
        <hr class="hr_portfolio">
</template>


<script>
export default {
}
</script>

<style>
.above_section-02 {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 1rem;
}
.description-above_section-02 {
    width: 100%;
    max-width: 23rem;
    max-height: 20rem;
    background-color: #E1BEE7;
    border-radius: 30px;
    padding: 1rem;
    margin-bottom: 1rem; 
}
.title_sidebar {
    font-size: 1.4rem;
    font-style: bold;
    text-decoration: none;
}

.card-01_section-02 p, .card-02_section-02 p, .card-03_section-02 p, .card-04_section-02 p, .card-05_section-02 p {
    padding: 0rem 1rem 0rem 1rem;    
}

.card-01_section-02 a, .card-02_section-02 a, .card-03_section-02 a, .card-04_section-02 a, .card-05_section-02 a {
    text-decoration: none;
    color: #000;
}
.card-01_section-02, .card-02_section-02, .card-03_section-02, .card-04_section-02, .card-05_section-02 {
    border-radius: 40px;
    width: 100%; 
    max-width: 25rem; 
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-bottom: 1.5rem;
    cursor: pointer;
    text-decoration: none;
    box-sizing: border-box;
    overflow: hidden;
    padding: 0;
}
.mockup-cards_section-02 {
    width: 100%; 
    height: auto; 
    overflow: hidden;
    border-radius: 20px;
    margin: 0; 
    padding: 0; 
}
.mockup-cards_section-02 img {
    width: 100%; 
    height: auto;
    display: block; 
    transition: transform 0.3s ease; /* Añade una transición suave al escalado */
}
.mockup-cards_section-02:hover img {
    -webkit-transform: scale(1.3); /* Escala la imagen al pasar el ratón */
    transform: scale(1.3); 
    border-radius: 20px;
}
.arrow {
    width: fit-content;
    height: fit-content;
}
.arrow:hover {
    -webkit-transform: rotate(90deg);
    transform: rotate(180deg);
    transition: transform 0.2s ease-in-out;
}
a .title_section-02 {
    display: flex;
    flex-direction: row ;
    align-items: center;  
    justify-content: space-around;
    text-decoration: none;
    color: #000;
}
.below_section-02 {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}
.card-01_section-02 {
    border: solid 2px #FFCCBC;
}
.card-02_section-02 {
    border: solid 2px #E1BEE7;
}
.card-03_section-02 {
    border: solid 2px #F8BBD0;
}
.card-04_section-02 {
    border: solid 2px #CE93D8;
}
.card-05_section-02 {
    border: solid 2px #F8BBD0;
}
.hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}

/* Media queries */

@media screen and (max-width: 767px) {
    .section-02 {
    padding: 0.5rem; 
    }
    .description-above_section-02 {
    text-align: center; 
    }
    .title_sidebar {
    font-size: 1.1rem; 
    }

    .card-01_section-02,
    .card-02_section-02,
    .card-03_section-02,
    .card-04_section-02,
    .card-05_section-02 {
    width: 100%; 
    }

    .text_sidebar,
    .text_descriptions {
    font-size: 0.95rem; 
    }

    .mockup-cards_section-02 {
    margin: 0 auto; 
    }
}
</style>