<template>
    <section id="proyectos" class="section-02">
            <div class="above_section-02">
                <div class="description-above_section-02">
                    <div class="description-above">
                        <h1 class="title_sidebar">Proyectos</h1>
                        <p class="text-cards_section-02">He desarrollado mis diseños partiendo de una sólida investigación previa, aplicando de manera integral mis conocimientos en UX/UI. Me he enfocado en crear interfaces completas tanto para web como para aplicaciones, siempre con el objetivo de garantizar que la experiencia del usuario sea fluida, intuitiva y altamente satisfactoria.
                        </p> 
                    </div>
                        <button class="button_see-more">
                            <img src="https://img.icons8.com/color/48/visible--v2.png" class="icon_see-more" alt="visible--v2"/>
                            <a href="https://www.behance.net/desirecarrizo" target="_blank">
                            Ver más proyectos
                            </a>          
                        </button> 
                </div>

                <div class="card-01_section-02">
                    <a href="https://www.figma.com/proto/yR8KjnndNATFkYYxFBxoUr/Proyecto--Nirname?page-id=1%3A2&node-id=1-2284&viewport=741%2C325%2C0.06&t=lld7nY527ALzDYMo-1&scaling=scale-down&content-scaling=fixed&starting-point-node-id=1%3A2284" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title-sidebar_section-02">Nirname</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha">
                        </div>
                        <p class="text-cards_section-02">Creación de todas las screens, estudio UX y realización de User Personas.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-01-section-02.png" alt="foto del Proyecto Nirname, centro de yoga">
                    </div>
                    </a>
                </div>

                <div class="card-02_section-02">
                    <a href="https://www.figma.com/proto/FviGi5i5nFR2VY8XDGYwlF/Actividades-Desir%C3%A9e?page-id=72%3A2&node-id=87-95&viewport=582%2C85%2C0.08&t=yJM7C3qV5cAIacNL-1&scaling=scale-down&content-scaling=fixed" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title-sidebar_section-02">Constructora Blocka</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha"> 
                        </div>
                    <p class="text-cards_section-02">Diseño responsive en desktop, tablet y mobile de la landing page.</p>
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
                            <h1 class="title-sidebar_section-02">Ecopop: web Hackaton</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha">
                        </div>
                    <p class="text-cards_section-02">Diseño de un e-commerce en pocas horas, quedando en 2º puesto.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-03-section-02.png" alt="foto de Ecopop, una web de muebles de segunda mano">
                    </div>  
                    </a>
                </div>
                <div class="card-04_section-02">
                    <a href="https://www.figma.com/proto/4J8nTOfWZLkGK9tkFnDxex/TechToday?page-id=0%3A1&node-id=42-1501&viewport=865%2C225%2C0.22&t=CMG6Jheigb8PEICS-1&scaling=scale-down&content-scaling=fixed" target="_blank">
                        <div class="title_section-02">
                        <h1 class="title-sidebar_section-02">TechToday</h1>
                        <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha">
                    </div>
                    <p class="text-cards_section-02">Propuesta de desarrollo sostenible de una web de gestión de noticias.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-04-section-02.png" alt="foto del Proyecto Green Newspaper, un periódico digital con diseño sostenible">
                    </div>
                    </a>
                </div>
                <div class="card-05_section-02">
                    <a href="https://harmony-heaven.netlify.app" target="_blank">
                        <div class="title_section-02">
                            <h1 class="title-sidebar_section-02">Harmony Heaven</h1>
                            <img class="arrow" src="@/assets/icons/arrow_in.png" alt="icono de flecha"> 
                        </div>
                    <p class="text-cards_section-02">Diseño responsive para una web de instrumentos interactivos.</p>
                    <div class="mockup-cards_section-02">
                        <img src="@/assets/card-05-section-02.png" alt="foto de Harmony Heaven, una web para tocar instrumentos">
                    </div>
                    </a>
                </div>
            </div>

        </section>
        <hr class="hr_portfolio">
</template>

<script setup>
</script>

<style lang="scss">

.section-02 {
    display: flex;
    flex-direction: column;
}

.above_section-02 {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
}

.below_section-02 {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    margin-top: 1.5rem;
}

.description-above_section-02 {    
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    max-width: 25rem;
    height: auto;   
    background-color: #E1BEE7;
    border-radius: 45px;
    padding: 1rem;
    box-sizing: border-box;
}

.card-01_section-02 p, 
.card-02_section-02 p, 
.card-03_section-02 p, 
.card-04_section-02 p, 
.card-05_section-02 p {
    padding: 0rem 1rem;    
}

.card-01_section-02 a, 
.card-02_section-02 a, 
.card-03_section-02 a, 
.card-04_section-02 a, 
.card-05_section-02 a {
    text-decoration: none;
    color: #000;
}
.card-01_section-02, 
.card-02_section-02, 
.card-03_section-02, 
.card-04_section-02, 
.card-05_section-02 {
    border-radius: 45px;
    width: 100%; 
    max-width: 25rem; 
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    cursor: pointer;
    text-decoration: none;
    box-sizing: border-box;
    overflow: hidden;
    padding: 0;
    gap: 1.5rem;
}

.mockup-cards_section-02 {
    width: 100%; 
    height: auto; 
    overflow: hidden;
    border-radius: 20px;
    margin: 0; 
    padding: 0; 
    img {
        width: 100%; 
        height: auto;
        display: block; 
        transition: transform 0.3s ease; // Añade una transición suave al escalado
    }
    &:hover img {
        -webkit-transform: scale(1.3); // Escala la imagen al pasar el ratón
        transform: scale(1.3); 
        border-radius: 20px;
    }
}

.arrow {
    width: fit-content;
    height: fit-content;
    &:hover {
        -webkit-transform: rotate(90deg);
        transform: rotate(180deg);
        transition: transform 0.2s ease-in-out;
    }
}

a .title_section-02 {
    display: flex;
    flex-direction: row ;
    align-items: center;  
    justify-content: space-between;
    text-decoration: none;
    color: #000;
    padding: 0 1rem;
}


//Borders de las cards
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

.button_see-more {
    background-color: #CE93D8;
    width: 14em;
    height: fit-content;
    font-size: 1.3rem;
    font-family: 'Poppins';
    border-radius: 0.5rem;
    border-style: none;
    cursor: pointer;
    text-decoration: none;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0.5rem 0;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: all 0.3s ease;
    margin-bottom: 2rem;

    &:hover {
    background-color: #ce93d8;
    transform: scale(0.95);
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    }

    &:active {
    background-color: #bc38d3;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    transform: translateY(2px);
    }

    .icon_see-more {
    display: flex;
    flex-direction: row;
    align-self: center;
    width: auto;
    height: auto;
    margin-right: 0.5rem;
    }

    a {
    text-decoration: none;
    color: #000;
    }
}

.text-sidebar {
    display: flex;
    font-size: 1.1rem;
    margin: 0;
}

.text-cards_section-02 { 
    font-size: 1.1rem;
    margin-top: -1rem;
}


/* Media queries */

@media screen and (max-width: 768px) {
    .above_section-02 {
        justify-content: center;
    }
    .description-above_section-02 {    
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        text-align: left; 
        margin-bottom: 1.5rem;
        width: 100%;
    }

    .below_section-02 {
        margin-top: 0;
        flex-direction: column-reverse;
    }

    .title-sidebar_section-02 {
        font-size: 1.2em; 
    }

    .card-01_section-02,
    .card-02_section-02,
    .card-03_section-02,
    .card-04_section-02,
    .card-05_section-02 {
        width: 100%; 
        margin-top: 1rem;
        margin-bottom: 1rem;
    }

    .mockup-cards_section-02 {
    margin: 0 auto; 
    }

    /* Efecto de "tap" en dispositivos móviles */
    .card-01_section-02:active,
    .card-02_section-02:active,
    .card-03_section-02:active,
    .card-04_section-02:active,
    .card-05_section-02:active {
        transform: scale(1.1); 
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3); 
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    /* Efecto de tap para el mockup dentro de la tarjeta */
    .card-01_section-02:active .mockup-cards_section-02 img,
    .card-02_section-02:active .mockup-cards_section-02 img,
    .card-03_section-02:active .mockup-cards_section-02 img,
    .card-04_section-02:active .mockup-cards_section-02 img,
    .card-05_section-02:active .mockup-cards_section-02 img {
        transform: scale(1.3);  
        transition: transform 0.3s ease;
}


@media only screen and (min-width: 1024px) and (max-width: 1240px){
    .section-02 {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }

    .description-above_section-02 {
        width: auto;
    }

    .card-01_section-02,
    .card-02_section-02,
    .card-03_section-02,
    .card-04_section-02,
    .card-05_section-02 {
        margin-top: 1rem;
        margin-bottom: 1rem;
    }

    .above_section-02 {
        flex-direction: column;
        flex-wrap: wrap;
        align-content: center;
        justify-content: center;
    }
    .below_section-02 {
        flex-direction: column;
        flex-wrap: wrap;
        justify-content: center;
    }
}

@media only screen and (min-width: 1920px) {

    .description-above {
        min-width: 100%;
        margin-bottom: 3.5rem;
    }

    .description-above_section-02 {
        display: flex;
        justify-items: space-between;
    }
    
    .above_section-02 {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
    }
    
    .description-above_section-02,
    .card-01_section-02,
    .card-02_section-02,
    .card-03_section-02,
    .card-04_section-02,
    .card-05_section-02 {
        width: 100%; 
        flex: 1;
        flex-grow: 1;
        flex-shrink: 1;
        max-width: 35rem;
        border-radius: 60px;
    }

    .card-01_section-02 p, 
    .card-02_section-02 p, 
    .card-03_section-02 p, 
    .card-04_section-02 p, 
    .card-05_section-02 p {
        padding: 0rem 3rem 0rem 3rem;    
    }
    .description-above_section-02 {    
        max-width: 33rem;
        height: 23rem;
        border-radius: 30px;
        padding: 1rem;
    }

    .title_section-02 {
        padding-top: 1rem;
    }
}
}
</style>