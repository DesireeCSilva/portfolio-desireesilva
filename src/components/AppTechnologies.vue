<template>
    <section id="section-04" class="section-04">
        <div class="content_section-04">
            <h1 class="title_sidebar">Tecnologías</h1>
            <div class="icons">
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/figma.png" alt="figma"/>
                    <p class="icon-label">Figma</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/html-5.png" alt="html-5"/>    
                    <p class="icon-label">HTML5</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/css3.png" alt="css3"/>
                    <p class="icon-label">CSS3</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/javascript.png" alt="javascript"/>
                    <p class="icon-label">JavaScript</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/github.png" alt="github"/>
                    <p class="icon-label">GitHub</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-filled/100/git.png" alt="git"/>
                    <p class="icon-label">Git</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/react.png" alt="react"/> 
                    <p class="icon-label">React</p>
                </div>
                <div class="icon-wrapper">
                    <img width="100" height="100" src="https://img.icons8.com/ios-glyphs/100/vuejs.png" alt="vuejs"/>
                    <p class="icon-label">Vue.js</p>
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

        .iconify {
            font-size: 50px; /* Tamaño uniforme para los íconos */
            color: #333;     /* Color de los íconos */
            transition: transform 0.3s ease-in-out;
        }

        .iconify:hover {
            transform: rotate(360deg); /* Animación al pasar el cursor */
        }
.content_section-04 {
    display: flex;
    flex-direction: row;
    background-color: #f8bbd0;
    border-radius: 30px;
    padding: 1rem;
    align-items: center;
    justify-content: space-between;
}

.icons {
    display: flex;
    padding: 1rem;
    justify-content: center;
    align-items: center;
    gap: 3rem;
    cursor: pointer;
    flex-wrap: wrap; 
}

.icon-wrapper {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
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
    bottom: -2rem;
}

.icon-wrapper:hover .icon-label {
    opacity: 1;
}

.icons img:hover {
    -webkit-transform: rotateY(180deg);
    -webkit-transform-style: preserve-3d;
    transform: rotateY(180deg);
    transform-style: preserve-3d;
    transition: transform 0.4s ease-in-out;
}

.icons i {
    font-size: 50px; /* Ajusta el tamaño del icono según sea necesario */
    transition: transform 0.2s ease-in-out;
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

@media only screen and (min-width: 1920px) {
    .content_section-04 {
        padding: 1rem 5rem 2rem 1rem;
        align-items: center;
        justify-content: space-between;
    }
}
</style>
