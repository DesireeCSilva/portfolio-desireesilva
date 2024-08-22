<template>
  <main>
    <AppHeader/>
    <AppFooter />
  </main>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  name: 'index_page',
  components: {
    AppHeader,
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

  .hr_portfolio {
    color: #CE93D8;
    width: 100%;
    margin-top: 2rem;
    margin-bottom: 2rem;
}
}
</style>
