<template>
  <div class ="resume" id="resume">
    <v-container>
      <v-row align="center" style="margin-top: 150px;">
        <v-col class="resume-top">
            <div class="resume-top-section-title">
              <h1>Resume.</h1>
            </div>
        </v-col>
      </v-row>
      <!-- แก้ไขใหม่ -->
      <v-row>
        <v-col class="resume-mid">
          <div class="page-one">
            <h3 class="heading">Education</h3>
            <v-card shaped class="resume-wrap d-flex" >
              <div class="icon d-flex align-items-center justify-content-center" style="width: 50px; background-color: #fff; height: 50px; border-radius: 50%;
                justify-content: center;" >
                <v-icon>mdi-school</v-icon>
              </div>
              <div class="text pl-3">
                <span class="data">2017-2021</span>
                <h3 style="color: #fff; font-size: 24px; font-weight: 700;">Bachelor in Information Engineering</h3>
                <span class="position">King Mongkut's Institute of Technology Ladkrabang</span>
                <p>Information Technology Engineering (ITE)  is a software engineering approach to designing and developing information systems.
                   information technology engineering background and are proficient in class is iot, database, network, web service and programming languages </p>
              </div>
            </v-card>
          </div>
          <div class="page-two">
            <h3 class="heading">Experience</h3>
            <v-card shaped class="resume-wrap d-flex">
              <div class="icon d-flex align-center justify-content-center" style="width: 50px; background-color: #fff; height: 50px; border-radius: 50%;
                justify-content: center;" >
                <v-icon>mdi-briefcase</v-icon>
              </div>
              <div class="text pl-3">
                <span class="data">2021-2022</span>
                <h3 style="color: #fff; font-size: 24px; font-weight: 700;">Software Engineering</h3>
                <span class="position">Backend Developer</span>
                <p>My back-end development  is Paperless Teams  refers to the development of server-side logic,
                   It includes to build out the database, server, and API </p>
              </div>
            </v-card>
          </div>
        </v-col>
      </v-row>
      <!-- <v-row class="py-8">
        <v-col class="resume-mid" style="display: grid; justify-content: center;align-items: center;">
          <div class="page-one">
            <h3 class="subtitle">Education</h3>
            <v-card class="edu-one d-flex rounded-xl" max-width="870">
              <div class="icon d-flex align-center justify-content-center">
                <v-icon>mdi-school</v-icon>
              </div>
              <div class="text pl-3">
                <span class="data">2017-2021</span>
                <h3 style="color: #fff; font-size: 24px; font-weight: 700;">Bachelor in Information Engineering</h3>
                <span class="position">King Mongkut's Institute of Technology Ladkrabang</span>
                <p>Information Technology Engineering (ITE)  is a software engineering approach to designing and developing information systems.
                   information technology engineering background and are proficient in class is iot, database, network, web service and programming languages </p>
              </div>
            </v-card>
          </div>
          <div class="page-two">
            <h3 class="subtitle">Experience</h3>
            <v-card class="edu-two d-flex rounded-xl" max-width="870">
              <div class="icon d-flex align-center justify-content-center">
                <v-icon>mdi-briefcase</v-icon>
              </div>
              <div class="text pl-3">
                <span class="data">2021-2022</span>
                <h3 style="color: #fff; font-size: 24px; font-weight: 700;">Software Engineering</h3>
                <span class="position">Backend Developer</span>
                <p>My back-end development  is Paperless Teams  refers to the development of server-side logic,
                   It includes to build out the database, server, and API </p>
              </div>
            </v-card>
          </div>
        </v-col>
      </v-row> -->
    </v-container>
  </div>
</template>
<script>
export default {
  name: 'Resume',
  data () {
    return {
      count: 0
    }
  }
}
</script>

<style>
.resume{
  background-color:rgb(31,31,31);  /*#0d1117;*/
  font-family:"Montserrat",sans-serif;
  color:hsla(0,0%,82.7%,.774);
}
.resume-top-section-title h1{
  color:#F9F9F9;
  font-size: 45px;
  font-weight: 700;
  position: relative;
  margin-bottom: 15px;
  line-height: 44px;
  text-align:center;
  text-decoration: underline;
}

/* .resume .resume-mid .page-one {
  width: 100%;
  margin-bottom: 3em;
} */

.heading{
  color:#fff;
  font-size: 24px;
  font-weight: 700;
  line-height: 44px;
  margin-bottom: 30px;
}

/* แก้ */
.resume .page-one .resume-wrap{
  width:100%;
  padding: 40px 30px;
  margin-bottom: 30px;
  background-color: rgb(42,42,42)
}

.resume .page-one .resume-wrap .text{
  width: calc(100% - 100px);
}

.resume .page-one .data{
  font-weight: 700;
  font-size: 16px;
  color:rgb(255, 255, 255);
}

.resume .page-one .position{
  font-weight: 700;
  font-size: 16px;
  color:hsla(0,0%,82.7%,.774);
  display:inline-block;
  margin-bottom:15px;
}
p{
  color:hsla(0,0%,82.7%,.774);
}

.resume  .page-two .resume-wrap{
  width:100%;
  padding: 40px 30px;
  margin-bottom: 30px;
  background-color: rgb(42,42,42)
}

.resume  .page-two  .icon{
  width: 55px;
  height: 39px;
  background: #fff;
  border-radius: 15px;
  justify-content: center;
}

.resume  .page-two  .data{
  font-weight: 700;
  font-size: 16px;
  color:rgb(255, 255, 255);
}

.resume  .page-two  .position{
  font-weight: 700;
  font-size: 16px;
  color:hsla(0,0%,82.7%,.774);
  display:inline-block;
  margin-bottom:15px;
}

.resume .page-two .resume-wrap .text{
  width: calc(100% - 100px);
}

@media (max-width:959px){
  .resume  .resume-mid{
  margin:0px 50px;
  }
}

@media (max-width:600px){
  .resume  .resume-mid{
  margin:0px 10px;
  }
}
</style>
