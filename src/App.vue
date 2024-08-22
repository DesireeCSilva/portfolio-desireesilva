<template>
  <main>
    <AppHeader/>
    <AppSummary />
    <AppFooter />
  </main>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppSummary from './components/AppSummary.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  name: 'index_page',
  components: {
    AppHeader,
    AppSummary,
    AppFooter
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
  min-height: 100vh;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: normal;
  padding: 2rem;
}
</style>
