<template>
    <section id="profil" class="profil">
        <Title title="A PROPOS"/>
        <div class="profil-text">
            <p class="profil-sentences">Je suis Leslie et je suis développeuse Web junior.</p>
            <p class="profil-sentences">En 2022, j'ai entamé une reconversion professionnelle via une formation Bac +2 de développeur Web qui m'a permis d'acquérir de nombreuses compétences en réalisant de nombreux projets dans différents langages de programmation.</p>
            <p class="profil-sentences">Etant consciente que ce domaine est vaste et en perpetuelle évolution, je poursuis mon apprentissage en préparant un Bachelor concepteur développeur d'applications en alternance auprès de MyDigitalSchool et de l'entreprise parisienne Ownest.</p>
            <p class="profil-sentences profil-sentences__last">Pour plus d'informations sur mon profil, vous pouvez télécharger mon CV ci-dessous</p>
        </div>
        <div class="button-container">
            <a :href="pdfUrl" target="_blank">
                <Button button-text="Télécharger le CV"/>
            </a>
        </div>
    </section>
</template>

<script setup>
    import Button from "./button/Button.vue";
    import Title from "./title/Title.vue";

    const pdfUrl = `${import.meta.env.VITE_APP_URL}/leslie_el_kattoussi_cv.pdf`;
</script>

<style lang="scss" scoped>
    .button-container {
        margin: 50px;
        text-align: center;
    }

    .profil {
        margin: auto;
    }

    .profil-sentences {
        font-weight: bold;
        padding-bottom: 45px;
        &__last {
            padding-bottom: 0;
        }
    }

    .profil-text {
        margin: auto;
        max-width: 900px;
        display: flex;
        flex-direction: column;
        text-align: center;
    }
    
    @media only screen and (min-width: 768px) {
        .picture {
            max-width: 60%;
        }

    }

    @media only screen and (min-width: 998px) {

    } 

</style>
