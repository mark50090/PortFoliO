<template>
  <div class ="contact" id="contact">
    <v-container>
      <v-row align="center" style="margin-top:50px;">
        <v-col class="contact-top">
            <div class="contact-top-title">
              <h1>Contact.</h1>
            </div>
        </v-col>
      </v-row>
      <v-row class="contact-main" style="margin-bottom:50px;">
        <v-col cols="12" md="4">
          <div class="contact-left">
            <div class="media align-items-center">
              <div class="media-icon">
                <v-icon>mdi-email</v-icon>
              </div>
              <div class="media-body">
                <h3>Email</h3>
                <span>mark50090@gmail.com</span>
              </div>
            </div>
            <div class="media align-items-center">
              <div class="media-icon">
                <v-icon>mdi-cellphone</v-icon>
              </div>
              <div class="media-body">
                <h3>Phone</h3>
                <span>083-5154687</span>
              </div>
            </div>
            <div class="media align-items-center">
              <div class="media-icon">
                <v-icon>mdi-google-maps</v-icon>
              </div>
              <div class="media-body">
                <h3>Adress</h3>
                <span>Mueang Lampang, Thailand</span>
              </div>
            </div>
          </div>
        </v-col>
        <v-col cols="12" md="8">
          <v-form class="contact-form">
            <v-row>
              <v-col cols="12" md="5" sm="6">
                <v-text-field class="custom-label-color" outlined rounded  label="Enter your name"></v-text-field>
              </v-col>
              <v-col cols="12" md="5" sm="6">
                <v-text-field class="custom-label-color" outlined rounded  label="Your email address"></v-text-field>
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="12" md="10" >
                <v-text-field class="custom-label-color" outlined rounded  label="Enter the discussion title"></v-text-field>
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="12" md="10" >
                <v-textarea class="custom-textarea-color" outlined  label="Write your message "></v-textarea>
              </v-col>
            </v-row>
            <v-row>
              <v-btn class="btn-add" x-large depressed rounded color="rgb(24, 144, 255)">Send message now
                <v-icon class="pl-3">mdi-send</v-icon>
              </v-btn>
            </v-row>
          </v-form>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  name: 'Contact',
  data () {
    return {
      count: 0
    }
  }
}
</script>

<style>
.contact{
  background-color:rgb(31, 31, 31);
  font-family:"Montserrat",sans-serif;
  color:hsla(0,0%,82.7%,.774);
  min-height: 500px;
}
.contact .contact-top-title h1{
  color: #F9F9F9;
  font-size: 45px;
  font-weight: 700;
  position: relative;
  margin-bottom: 50px;
  line-height: 44px;
  text-align: center;
  text-decoration: underline;
}

.contact .v-icon{
    color: #fff;
}

.media{
  display: flex;
  align-items: center;
  margin-bottom: 30px;
}
.media-icon{
  width:  50px;
  height: 50px;
  font-size: 23px;
  text-align: center;
  line-height: 43px;
  border: 2px solid #1972d2;
  border-radius:50%;
}

.media-body{
  padding-left: 25px;
}

.contact .contact-form .theme--light.v-text-field--outlined:not(.v-input--is-focused):not(.v-input--has-state) > .v-input__control > .v-input__slot fieldset{
  color: #ffffff !important;
}

.contact .custom-label-color .v-label {
    color: rgb(255 255 255 / 60%) !important;
}

.contact .custom-textarea-color .v-label {
  color: rgb(255 255 255 / 60%) !important;
}

.custom-label-color input{
  color: #ffffff !important;
}

.custom-textarea-color textarea{
  color: #ffffff !important;
}

.custom-textarea-color textarea .v-label{
  color: #ffffff !important;
}

/* .btn-add{
  color: red !important;
} */
.contact span.v-btn__content  {
    color: #111;
}

.contact span.v-btn__content:hover{
  color: #fff;
}

@media (max-width: 959px){
  .contact .contact-main {
    margin: 0px 50px;
  }
}

@media (max-width:600px){
  .contact .contact-main {
    margin: 0px 10px;
  }
}
</style>
