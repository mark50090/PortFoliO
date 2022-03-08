<template>
  <div class ="skill" id="skills">
    <v-container>
      <v-row align="center" style="margin-top: 90px;">
        <v-col class="skill-left" cols="12" md="6" lg="6">
          <div class="text-box-inline">
            <h2>My Programming <span>Skills.</span></h2>
            <p>I develop simple, intuitive and responsive user interface that helps users get things done with less effort and time with those technologies.</p>
          </div>
        </v-col>
        <v-col class="skill-right" cols="12" md="6" lg="6">
          <div class="skill-right-icon">
            <div class="skill-icon">
              <v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="https://nafie.webrouk.com/html/assets/images/skills/html5.png" alt="HTML5">
                </template>
                <span>HTML5</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="https://nafie.webrouk.com/html/assets/images/skills/css3.png" alt="CSS3">
                </template>
                <span>CSS3</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="https://nafie.webrouk.com/html/assets/images/skills/javascript.png" alt="JavaScript">
                </template>
                <span>JavaScript</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="https://nafie.webrouk.com/html/assets/images/skills/vue.png" alt="Vue">
                </template>
                <span>Vue</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" :src="require('../assets/logo.svg')" alt="Vuetify" style="width: 48px; height: 48px;">
                </template>
                <span>Vuetify</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="../assets/python.png" alt="python">
                </template>
                <span>Python</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="../assets/nodejs.png" alt="nodejs">
                </template>
                <span>Nodejs</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="../assets/mongodb_original.png" alt="mongodb">
                </template>
                <span>Mongodb</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="../assets/mysql.png" alt="mysql">
                </template>
                <span>Mysql</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="../assets/gitlab.png" alt="gitlab">
                </template>
                <span>Gitlab</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="https://nafie.webrouk.com/html/assets/images/skills/vs-code.png" alt="vscode">
                </template>
                <span>VS Code</span>
              </v-tooltip>
            </div>
            <div class="skill-icon"><v-tooltip top>
                <template v-slot:activator="{ on, attrs }">
                  <img v-bind="attrs" v-on="on" src="https://nafie.webrouk.com/html/assets/images/skills/git.png" alt="git">
                </template>
                <span>Git(GitHub)</span>
              </v-tooltip>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  name: 'Skill',
  data () {
    return {
      count: 0
    }
  }
}
</script>

<style>
.skill{
  background-color:rgb(31,31,31);
  font-family:"Montserrat",sans-serif;
  color:hsla(0,0%,82.7%,.774);
  min-height:500px
}

.text-box-inline h2{
  color:#fff;
  font-size:35px;
  font-weight:700;
  margin-bottom:20px;
}

.text-box-inline span{
  text-decoration: underline;
}

.skill-icon{
    background-color:rgb(44,44,44);
    border-radius:10px;
    padding:15px;
    margin:10px
}

.skill-right-icon{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items:center;
}

@media (max-width: 959px){
  .text-box-inline {
    margin: 0px 50px;
  }
}

@media (max-width: 450px){
  .text-box-inline h2{
    color:#fff;
    font-size:29px;
    font-weight:700;
    margin-bottom:20px;
  }
}

@media (max-width:600px){
  .text-box-inline {
  margin:0px 10px;
  }
}
</style>
