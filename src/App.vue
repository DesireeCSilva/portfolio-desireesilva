<template>
  <main>
    <AppHeader v-if="!isMobileDevice" />
    <AppHeaderMobile v-else />
    <AppSummaryAlt />
    <AppProjects/>
    <AppEducation />
    <AppTechnologies/>
    <AppContact />
    <AppFooter />
  </main>
</template>

<script setup>
import AppHeader from './components/AppHeader.vue'
import AppHeaderMobile from './components/AppHeaderMobile.vue'
// import AppSummary from './components/AppSummary.vue'
import AppSummaryAlt from './components/AppSummaryAlt.vue'
import AppEducation from './components/AppEducation.vue'
import AppContact from './components/AppContact.vue'
import AppProjects from './components/AppProjects.vue'
import AppTechnologies from './components/AppTechnologies.vue'
import AppFooter from './components/AppFooter.vue'
import { ref, onMounted, onBeforeUnmount } from 'vue'

const isMobileDevice = ref(false)

const setScreenSize = () => isMobileDevice.value = window.innerWidth < 768

onMounted(() => {
  setScreenSize()
  window.addEventListener('resize', setScreenSize)
})
onBeforeUnmount(() => window.removeEventListener('resize', setScreenSize))
</script>

<style lang="scss">
body {
  margin: 0;
  box-sizing: border-box;
  min-height: 100vh;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: normal;
  padding: 2rem;

  .hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
  }

  .text_sidebar {
    font-size: 1.2rem;
  }
}

@media (max-width: 768px) {
  body {
    padding: 0;

    main > :not(header) {
      padding: 2rem;
    }

    .hr_portfolio {
      display: none;
    }
  }
}
</style>
