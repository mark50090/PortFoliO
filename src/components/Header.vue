<template>
  <v-container>
    <v-toolbar  flat class="mainHeader md">
      <v-toolbar-title class="toolbar-logo-block">
      <h4>Mark<span style="color: rgb(24, 144, 255);">krittapas</span></h4>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-only hidden-xs-only">
        <v-btn text @click="scroll('home')">Home</v-btn>
        <v-btn text @click="scroll('mark')">About</v-btn>
        <v-btn text @click="scroll('resume')">Resume</v-btn>
        <v-btn text @click="scroll('skills')">Skill</v-btn>
        <v-btn text @click="scroll('project')">Work</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
      </v-toolbar-items>
      <div class="hidden-md-and-up">
        <v-menu offset-y>
          <template v-slot:activator="{ on }">
            <v-app-bar-nav-icon v-on="on"></v-app-bar-nav-icon>
          </template>
          <v-list class="responsiveMenu">
            <v-list-item>
              <v-list-item-title  @click="scroll('home')">Home</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title @click="scroll('mark')">About</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title @click="scroll('resume')">Resume</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title @click="scroll('skills')">Skill</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title @click="scroll('project')">Work</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title @click="scroll('contact')">contact</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
      </div>
    </v-toolbar>
  </v-container>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
      menus: [
        { title: 'Home', route: 'home' },
        { title: 'About', route: 'about' },
        { title: 'Resume', route: 'resume' },
        { title: 'Work', route: 'work' },
        { title: 'Contact', route: 'contact' }
      ]
    }
  },
  methods: {
    scroll (refName) {
      const element = document.getElementById(refName)
      element.scrollIntoView({ behavior: 'smooth' })
    }
  }
}
</script>

<style>
.v-toolbar__content{
  background-color:rgb(48,48,48)   /*#0e141b;*/
}
span.v-btn__content {
    color: hsla(0,0%,82.7%,.774);
}
a {
    color: #1976d2;
    font-size: 16px;
    color: #a6a8a9;
    font-weight: 600;
    text-decoration: none;
}
span.v-btn__content:hover{
  color: rgb(24, 144, 255);
}
h4{
  cursor: pointer;
  font-size: 35px;
  font-weight: 800;
  text-transform: capitalize;
  color: hsla(0,0%,82.7%,.774);
}
</style>
