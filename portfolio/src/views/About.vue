<template>
  <v-container fluid grid-list-md class="heh">
    <v-layout row wrap>
      <v-flex d-flex xs12 md6>
        <v-card color="red darken-3" dark>
          <v-img :src="require('../assets/me.jpg')"></v-img>
        </v-card>
      </v-flex>
      <v-flex d-flex xs12 md6>
        <v-layout row wrap>
          <v-flex d-flex sm12>
            <h1>about Edvin</h1>
          </v-flex>
          <v-flex d-flex sm12>
              <h2>competitive, ambitious and creative</h2>
              </v-flex>
              <v-flex d-flex sm12>
              <p>
                I strive to learn new skills and techniques of design to give myself more tools to play with,
                which in turn allows me to create design solutions that are more sophisticated and unique.
              </p>
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
    <div class="space"></div>
    <div class="buttons">
      <v-btn dark color="red darken-3" class="btn" href="https://www.dropbox.com/s/nt522j3nujc7qg6/CV.pdf?dl=0" target="_blank">CV</v-btn>
      <v-btn dark color="red darken-3" class="btn" href="https://www.dropbox.com/s/d3j5g7n3evelxga/business-card.pdf?dl=0" target="_blank">Business Card</v-btn>
    </div>
    <div class="contacts">
      <span class="email">e-mail: milos.edvin@gmail.com</span>
      <div class="social">
          <a href="https://www.instagram.com/milos.edvin/" target="_blank"><div class="ig"></div></a>
          <a href="https://www.linkedin.com/in/edvin-milos-07697111a/" target="_blank"><div class="in"></div></a>
      </div>
    </div>
  </v-container>
</template>

<script>
  export default {
    data() {
      return {
        
      }
    },
  }
</script>

<style scoped>
.heh{
  max-width: 1300px;
}
.img{
  height: 300px;
}
h1{
  font-family: 'gothamB';
  font-size: 1.5em;
  text-align: right;
  padding: 20px 60px;
}
h2{
  font-family: 'gothamB';
  font-size: 2.5em;
  text-align: center;
  padding: 0 60px;
}
p{
  font-family: 'gothamM';
  font-size: 1.4em;
  padding: 0 60px;
}
.space{
  height: 150px;
}
.buttons{
  text-align: center;
}
.contacts{
  text-align: center;
  padding: 30px;
}
.email{
  font-family: 'gothamB';
  font-size: 1.2em;
}
.ig, .in{
    margin: 30px 10px;
    transition: 200ms;
}
.ig{
    background: url('../assets/instagram.png');
    width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.in{
    background: url('../assets/linkedin1.png');
    width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.ig:hover{
    background: url('../assets/instagramRed.png');
        width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}
.in:hover{
    background: url('../assets/linkedinRed.png');
        width: 20px;
    height: 20px;
    background-size: contain;
    display: inline-block;
}

/* MEDIA QUERIES */
@media only screen and (min-width: 500px){
  .img {
      min-height: 400px;
    }
}
@media only screen and (min-width: 960px){
  .img {
      min-height: 400px;
    }
}
</style>