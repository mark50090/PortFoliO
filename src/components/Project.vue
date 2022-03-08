<template>
  <div class ="project" id="project">
    <v-container>
      <v-row align="center" style="margin-top:50px;">
        <v-col class="project-top">
            <div class="project-top-title">
              <h1>Project.</h1>
            </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col class="project-section">
            <div class="project-detail">
              <v-tabs color="hsla(0,0%,82.7%,.774)" background-color="rgb(31,31,31)">
                <v-tabs-slider color="white"></v-tabs-slider>
                <v-tab v-for="item in items" :key="item" >{{item}}</v-tab>
                <v-tab-item>
                  <div class="project-itemone">
                    <v-row >
                      <v-col cols="12" md="4">
                        <div class="project-itemone-detail">
                          <v-card class="pa-3 ma-2" height="335" color="rgb(42,42,42)">
                            <v-img class="white--text align-end" height="200px" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg">
                              <v-card-title>Smart Door Lock</v-card-title>
                            </v-img>
                            <v-card-text class="text--primary">
                              <p>Smart Door Lock</p>
                              <v-btn color="" dark text class="">Know more
                                <v-icon right>mdi-arrow-right</v-icon>
                              </v-btn>
                            </v-card-text>
                          </v-card>
                        </div>
                      </v-col>
                      <v-col cols="12" md="4">
                        <div class="project-itemone-detail">
                          <v-card class="pa-3 ma-2" height="335" color="rgb(42,42,42)">
                            <v-img class="white--text align-end" height="200px" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg">
                              <v-card-title>Top 10 Australian beaches</v-card-title>
                            </v-img>
                            <v-card-text class="text--primary">
                              <p>Sensor Lidar</p>
                              <v-btn color="" dark text class="">Know more
                                <v-icon right>mdi-arrow-right</v-icon>
                              </v-btn>
                            </v-card-text>
                          </v-card>
                        </div>
                      </v-col>
                      <v-col cols="12" md="4">
                        <div class="project-itemone-detail">
                          <v-card class="pa-3 ma-2" height="335" color="rgb(42,42,42)">
                            <v-img class="white--text align-end" height="200px" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg">
                              <v-card-title>Top 10 Australian beaches</v-card-title>
                            </v-img>
                            <v-card-text class="text--primary">
                              <v-btn color="" dark text class="mb-2">sensor lidar</v-btn> <br>
                              <v-btn color="" dark text class="">Know more
                                <v-icon right>mdi-arrow-right</v-icon>
                              </v-btn>
                            </v-card-text>
                          </v-card>
                        </div>
                      </v-col>
                      <v-col cols="12" md="4">
                        <div class="project-itemone-detail">
                          <v-card class="pa-3 ma-2" height="335" color="rgb(42,42,42)">
                            <v-img class="white--text align-end" height="200px" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg">
                              <v-card-title>Top 10 Australian beaches</v-card-title>
                            </v-img>
                            <v-card-text class="text--primary">
                              <p>Sensor Lidar</p>
                              <v-btn color="" dark text class="">Know more
                                <v-icon right>mdi-arrow-right</v-icon>
                              </v-btn>
                            </v-card-text>
                          </v-card>
                        </div>
                      </v-col>
                      <v-col cols="12" md="4">
                        <div class="project-itemone-detail">
                          <v-card class="pa-3 ma-2" height="335" color="rgb(42,42,42)">
                            <v-img class="white--text align-end" height="200px" src="https://cdn.vuetifyjs.com/images/cards/docks.jpg">
                              <v-card-title>Top 10 Australian beaches</v-card-title>
                            </v-img>
                            <v-card-text class="text--primary">
                              <p>Sensor Lidar</p>
                              <v-btn color="" dark text class="">Know more
                                <v-icon right>mdi-arrow-right</v-icon>
                              </v-btn>
                            </v-card-text>
                          </v-card>
                        </div>
                      </v-col>
                    </v-row>
                  </div>
                </v-tab-item>
                <v-tab-item>
                  <div class="project-detail-main">
                    <v-card flat>
                      <v-card-text>
                        <p>2Sed aliquam ultrices mauris. Donec posuere vulputate arcu. Morbi ac felis. Etiam feugiat lorem non metus. Sed a libero.</p>
                      </v-card-text>
                    </v-card>
                  </div>
                </v-tab-item>
              </v-tabs>
            </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  name: 'Project',
  data () {
    return {
      items: ['all', 'iot', 'image processing', 'Web']
    }
  }
}
</script>

<style>
.project{
  background-color:rgb(31,31,31);
  font-family:"Montserrat",sans-serif;
  color:hsla(0,0%,82.7%,.774);
}

.theme--light.v-tabs-items {
  background-color: rgb(31,31,31) !important;
}
.v-tab.v-tab {
    color: #fff !important;
}
.project .project-top-title h1{
  color: #F9F9F9;
  font-size: 45px;
  font-weight: 700;
  position: relative;
  margin-bottom: 25px;
  line-height: 44px;
  text-align: center;
  text-decoration: underline;
}

@media (max-width: 959px){
  .project-detail {
    margin: 0px 50px;
  }
}

@media (max-width:600px){
  .project-detail {
    margin: 0px 10px;
  }
}

</style>
