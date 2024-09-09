<template>
    <section id="section-04" class="section-04">
        <div class="content_section-04">
            <h1 class="title_sidebar">Tecnologías</h1>
            <div class="icons">
                <div class="icon-wrapper">
                    <img src="@/assets/icons/Figma.png" alt="icono de Figma" />
                    <p class="icon-label">Figma</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/icons/Html 5.png" alt="icono de HTML" />
                    <p class="icon-label">HTML</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/icons/CSS3.png" alt="icono de CSS" />
                    <p class="icon-label">CSS</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/icons/JavaScript.png" alt="icono de JavaScript" />
                    <p class="icon-label">JavaScript</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/GitHub-big.png" alt="icono de GitHub" />
                    <p class="icon-label">GitHub</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/icons/Git.png" alt="icono de Git" />
                    <p class="icon-label">Git</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/icons/React Native.png" alt="icono de React" />
                    <p class="icon-label">React</p>
                </div>
                <div class="icon-wrapper">
                    <img src="@/assets/icons/vue.png" alt="icono de Vue" />
                    <p class="icon-label">Vue</p>
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
    bottom: -2rem;
    font-size: 0.9rem;
    font-weight: bold;
    color: #333;
}

.icon-wrapper:hover .icon-label {
    opacity: 1;
}

.icons img {
    transition: transform 0.2s ease-in-out;
    width: 50px; /* Ajusta el tamaño según lo necesites */
}

.icons img:hover {
    -webkit-transform: rotateY(180deg);
    -webkit-transform-style: preserve-3d;
    transform: rotateY(180deg);
    transform-style: preserve-3d;
    transition: transform 0.4s ease-in-out;
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
        padding: 1rem 5rem 0rem 1rem;
        align-items: center;
        justify-content: space-between;
    }
}
</style>
