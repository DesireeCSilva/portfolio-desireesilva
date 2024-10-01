<template>
    <section id="tecnologias" class="section-04">
        <div class="content_section-04">
            <h1 class="title_sidebar">Tecnologías</h1>
            <div class="icons">
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/figma--v1.png" alt="figma--v1"/>
                    <p class="icon-label">Figma</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/html-5--v1.png" alt="html-5--v1"/>  
                    <p class="icon-label">HTML5</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/css3.png" alt="css3"/>
                    <p class="icon-label">CSS3</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/javascript--v1.png" alt="javascript--v1"/>
                    <p class="icon-label">JavaScript</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/github--v1.png" alt="github--v1"/>
                    <p class="icon-label">GitHub</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/officexs/react.png" alt="react"/>
                    <p class="icon-label">React</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/vue-js.png" alt="vue-js"/>
                    <p class="icon-label">Vue.js</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/bootstrap--v2.png" alt="bootstrap--v2"/>
                    <p class="icon-label">Bootstrap</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/sass.png" alt="sass"/>
                    <p class="icon-label">Sass</p>
                </div>
                <div class="icon-wrapper">
                    <img class="icon-img" src="https://img.icons8.com/color/70/nodejs.png" alt="nodejs"/>
                    <p class="icon-label">Node.js</p>
                </div>
            </div>

        </div>
    </section>
    <hr class="hr_portfolio" />
</template>


<script>
export default {};
</script>

<style>

.content_section-04 {
    display: flex;
    flex-direction: row;
    background-color: #f8bbd0;
    border-radius: 45px;
    padding: 1rem 1.5rem;
    align-items: center;
    justify-content: space-between;
}

.icons {
    display: flex;
    padding: 1rem;
    justify-content: center;
    align-items: center;
    gap: 2.5rem;
    cursor: pointer;
    flex-wrap: wrap; 
}

.icon-wrapper {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.icon-img {
    width: 3.5rem;
    height: 3.5rem;
}

.icon-label {
    margin-top: 0.5rem;
    opacity: 0;
    transition: opacity 0.3s ease-in-out;
    position: absolute;
    bottom: 2rem;
    font-size: 0.9rem;
    font-weight: bold;
    color: #000000;
    bottom: -2.2rem;
}

.icon-wrapper:hover .icon-label {
    opacity: 1;
}

.icons img:hover {
    animation: beat 0.6s infinite; 
    transition: transform 0.4s ease-in-out; 
}

@keyframes beat {
    0%, 100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.2); /* Aumenta el tamaño al 120% en el medio de la animación */
    }
}


/*Media Queries */
@media screen and (max-width: 768px) {
    .content_section-04 {
        display: flex;
        flex-direction: column;
        padding: 0.5rem;
    }

    .icons {
        gap: 1.5rem; 
    }

    .icons img {
        width: 3rem; 
        height: auto; 
    }
}
@media only screen and (min-width: 1024px) and (max-width: 1280px) {
        .content_section-04 {
        display: flex;
        flex-direction: column;
        padding: 0.5rem;
    }
}

@media only screen and (min-width: 1920px) {
    .content_section-04 {
        padding: 2rem 5rem 2rem 1rem;
        align-items: center;
        justify-content: space-between;
    }
}
</style>
