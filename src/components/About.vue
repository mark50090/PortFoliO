<template>
<div id="mark" class ="about">
<v-container>
  <v-row align="center" style="margin-top: 50px;">
    <v-col class="about-left" cols="12" lg="6" md="6">
      <div class="about-img">
        <img class="img-about" src="./../assets/about.jpg">
      </div>
    </v-col>
    <v-col class="about-right"  cols="12" lg="6" md="6" >
    <div class="about-details">
      <h2 class="title-about">About Me.</h2>
      <p> I'm passionate about using latest Technology. now I do Back End Development also known as server-side development.
          It focuses primarily on databases, backend logic, APIs, and Servers.
          but in near future I want to learn Front End Developer</p>
      <ul class="about-info mt-4">
        <li>
          <span class="span-1">Name:</span>
          <span>Krittapas Kaewmit</span>
        </li>
        <li>
          <span class="span-1">Date of birth:</span>
          <span>January 30, 1998</span>
        </li>
        <li>
          <span class="span-1">Address:</span>
          <span>Mueang Lampang, Thailand</span>
        </li>
        <li>
          <span class="span-1">Zip code:</span>
          <span>52100</span>
        </li>
        <li>
          <span class="span-1">Email:</span>
          <span>mark50090@gmail.com</span>
        </li>
        <li>
          <span class="span-1">Phone:</span>
          <span>083-5154687</span>
        </li>
      </ul>
      <v-btn elevation="5" rounded x-large>Download CV<v-icon right>mdi-download</v-icon>
      </v-btn>
    </div>
    </v-col>
  </v-row>
</v-container>
</div>
</template>
<script>
export default {
  name: 'About',
  data () {
    return {
      count: 0
    }
  }
}
</script>
<style>
.about{
  background-color:rgb(31,31,31);  /*#0d1117;*/
  font-family:"Montserrat",sans-serif;
  color:hsla(0,0%,82.7%,.774);
  min-height:650px
}
.about .img-about{
  outline: 10px solid #f8f9fa;
  outline-offset: -54px;
  border-radius:50px;
  border: 44px solid transparent;
  border-width: 0px 10px 0px 85px;
}
.about .title-about{
  font-size: 45px;
  font-weight: 700;
  color:#F9F9F9;
  position: relative;
  margin-bottom: 30px;
  line-height: 44px;
  text-decoration: underline;
}
.about p{
  font-size: 16px;
  font-weight: 500;
  margin-bottom:10px
}
.about ul{
  margin-bottom:30px;
}

.about ul, ol {
  list-style: none;
}
.about li {
  margin-bottom: 10px;
  display:flex;
}
.about .span-1{
  color:#F9F9F9;
  width:130px;
  font-size: 16px;
  font-weight: 600;
}
.about .about-details{
  display:block;
  margin:0px auto;
}

.v-application ul, .v-application ol {
    padding-left: 0px;
}

.about span.v-btn__content {
  color: #000
}

.about span.v-btn__content:hover{
  color: #fff
}
.about .theme--light.v-btn.v-btn--has-bg {
  background-color: rgb(24, 144, 255);
}

@media (max-width:1263px){
  .about .img-about{
  max-width:100%;
  }
}

@media (max-width:959px){
  .about .about-img{
    display:flex;
    justify-content: center;
  }
  .about .title-about{
    text-align:center;
  }
  .about .about-details{
  margin:0px 50px;
  }
}
@media (max-width:600px){
  .about .about-details{
  margin:0px 10px;
  }
}
</style>
