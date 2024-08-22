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
}
</style>
