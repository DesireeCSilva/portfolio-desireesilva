<template>
    <section id="section-04" class="section-04">
        <div class="content_section-04">
            <h1 class="title_sidebar">Tecnologías</h1>
                <div class="icons">
                    <img src="@/assets/icons/Figma.png" alt="icono de Figma" />
                    <img src="@/assets/icons/Html 5.png" alt="icono de HTML" />
                    <img src="@/assets/icons/CSS3.png" alt="icono de CSS" />
                    <img src="@/assets/icons/JavaScript.png" alt="icono de JavaScript" />
                    <img src="@/assets/GitHub-big.png" alt="icono de GitHub" />
                    <img src="@/assets/icons/Jira.png" alt="icono de Jira" />
                    <img src="@/assets/icons/Git.png" alt="icono de Git" />
                    <img src="@/assets/icons/React Native.png" alt="icono de React" />
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
.icons img {
    transition: transform 0.2s ease-in-out;
}

.icons img:hover {
    -webkit-transform: rotateY(180deg);
    -webkit-transform-style: preserve-3d;
    transform: rotateY(180deg);
    transform-style: preserve-3d;
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
</style>
