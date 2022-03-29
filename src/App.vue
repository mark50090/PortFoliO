<template>
  <v-app>
    <v-app-bar app flat max-height="75" color="#0e141b">
      <Header />
    </v-app-bar>
    <v-content>
    <Home />
    </v-content>
    <About />
    <Resume />
    <Skill />
    <Project />
    <Contact />
    <Footer />
    <!-- <v-content>
    <router-view/>
  </v-content> -->
  <router-view/>
  </v-app>
</template>

<script>
import Header from './components/Header'
import Home from './components/Home'
import About from './components/About'
import Resume from './components/Resume'
import Skill from './components/Skill'
import Project from './components/Project'
import Contact from './components/contect.vue'
import Footer from './components/Footer.vue'
export default {
  components: { Header, Home, About, Resume, Skill, Project, Contact, Footer },
  name: 'App',
  data () {
    return {
    //
    }
  }
}
</script>

<style>
</style>
