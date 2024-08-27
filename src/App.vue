<template>
  <main>
    <AppHeader/>
    <AppSummary />
    <AppProjects/>
    <AppEducation />
    <AppTechnologies/>
    <AppContact />
    <AppFooter />
  </main>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppSummary from './components/AppSummary.vue'
import AppEducation from './components/AppEducation.vue'
import AppContact from './components/AppContact.vue'
import AppProjects from './components/AppProjects.vue'
import AppTechnologies from './components/AppTechnologies.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  name: 'index_page',
  components: {
    AppHeader,
    AppSummary,
    AppEducation,
    AppContact,
    AppProjects,
    AppTechnologies,
    AppFooter
  }
}
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
}
</style>
