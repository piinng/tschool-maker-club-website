<template>
  <HeaderPage/>
  <AboutPage/>
  <ProjectPage/>
  <ContactPage/>
</template>

<script>
import HeaderPage from './components/HeaderPage.vue'
import AboutPage from './components/AboutPage.vue'
import ProjectPage from './components/ProjectPage.vue'
import ContactPage from './components/ContactPage.vue'

export default {
  name: 'App',
  components: {
    HeaderPage,
    AboutPage,
    ProjectPage,
    ContactPage
  }
}
</script>

<style>
</style>
