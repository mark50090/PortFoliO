<template>
<div class ="home" id="home">
<v-container>
  <v-row align="center" style="margin-top: 50px;">
    <v-col class="home-left" lg="6" md="6">
    <div class="home-left-caption">
      <h2>HEY! I AM</h2>
      <h1><vue-typer :text='["Krittapas Kaewmit.","Software Engineer."]' erase-style='backspace'></vue-typer>|</h1>
      <p>I am a developer who has passion for building web applications with intuitive functionality and<br>
         I am always curious about learning new skills, tools, and concepts.</p>
      <v-btn elevation="5" rounded x-large>Download CV<v-icon right>mdi-download</v-icon>
      </v-btn>
    </div>
    </v-col>
    <v-col class="home-right d-none d-md-block" lg="6" md="6" d-lg-none>
    <div class="home-img">
      <img src="./../assets/profile.jpg" alt ="">
    </div>
    </v-col>
  </v-row>
</v-container>
</div>
</template>
<script>
export default {
  name: 'Home',
  data () {
    return {
      count: 0
    }
  }
}
</script>

<style>
.home{
  background-color:rgb(31,31,31);   /*#0e141b;*/
  font-family:"Montserrat",sans-serif;
  color:hsla(0,0%,82.7%,.774);
  min-height:850px
}

.home p{
  margin:15px auto;
}

.home h1{
  font-size: 55px;
  font-weight: 600;
  line-height: 60px;
}
.home span.v-btn__content {
  color: #000
}

.home span.v-btn__content:hover{
  color: #fff
}
.home .theme--light.v-btn.v-btn--has-bg {
  background-color: rgb(24, 144, 255);
}
.vue-typer .custom.char.typed {
  color:rgb(24, 144, 255);
}

.home .home-img img {
  border-radius: 50px;
  display: block;
  margin: 0px auto
}

@media (min-width:1904px){
  .container {
  max-width: 1400px;
  }
}
@media (max-width:959px){
  .home{
    min-height:450px
  }
  .home-left-caption{
    margin:50px
  }
}

@media (max-width:600px){
  .home-left-caption{
    margin:10px
  }
  .home h2{
    font-size:16px;
    font-weight: 700;
    letter-spacing: 4px;
  }
  .home h1{
    font-size: 35px;
    font-weight: 600;
    line-height: 60px;
  }
}
</style>
