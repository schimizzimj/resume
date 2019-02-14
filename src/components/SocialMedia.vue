<template lang="html">

  <section id="social" class="social">
    <div class="container">
        <div class="block" id="item-1">
          <a href="https://instagram.com/marcusschimizzi">
            <span class="item-content">
              <h2>Instagram</h2>
            </span>
          </a>
          <img class="footer-icon" src="https://res.cloudinary.com/marcusschimizzi/image/upload/v1488528004/icon-instagram_wig3ya.svg">
        </div>

        <div class="block" id="item-2">
          <a href="https://github.com/schimizzimj">
            <span class="item-content">
              <h2>Github</h2>
            </span>
          </a>
          <img class="footer-icon" src="http://res.cloudinary.com/marcusschimizzi/image/upload/v1488527979/icon-github_h2cpnw.svg">
        </div>

        <div class="block" id="item-3">
          <a href="https://www.linkedin.com/in/marcus-schimizzi-56a6229b">
            <span class="item-content">
              <h2>LinkedIn</h2>
            </span>
          </a>
          <img class="footer-icon" src="http://res.cloudinary.com/marcusschimizzi/image/upload/v1488527986/icon-linkedin_s1jn8k.svg">
        </div>

        <div class="block" id="item-4">
          <a href="https://facebook.com/marcus.j.schimizzi">
            <span class="item-content">
              <h2>Facebook</h2>
            </span>
          </a>
          <img class="footer-icon" src="http://res.cloudinary.com/marcusschimizzi/image/upload/v1488527974/icon-facebook_supky9.svg">
        </div>

        <div class="block" id="item-5">
          <a href="https://twitter.com/marcusschimizzi">
            <span class="item-content">
              <h2>Twitter</h2>
            </span>
          </a>
          <img class="footer-icon" src="http://res.cloudinary.com/marcusschimizzi/image/upload/v1488527989/icon-twitter_uv4qkd.svg">
        </div>

        <div class="block" id="item-6">
          <a href="mailto:mschimiz@nd.edu">
            <span class="item-content">
              <h2>Email</h2>
            </span>
          </a>
          <img class="footer-icon" src="http://res.cloudinary.com/marcusschimizzi/image/upload/v1488527982/icon-gmail_q3rpvi.svg">
        </div>
      </div>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class SocialMedia extends Vue {
}
</script>

<style scoped lang="scss">
  .social {

  }
  .social:after {
    content: "";
    display: table;
    clear: both;
  }

 .item-content h2 {
   font-size: 60px;
   display: none;
 }

 #item-1 {
   background-color: #527FA3;
 }
 #item-1:hover > a {
   background: rgba(225, 48, 108, 0.7);
 }

 #item-2 {
   background-color: #181616;
 }
 #item-2:hover > a {
   background: rgba(108, 198, 68, 0.7);
 }

 #item-3 {
   background-color: #0274B3;
 }
 #item-3:hover > a {
   background: rgba(0, 160, 220, 0.7);
 }

 #item-4 {
   background-color: #3D5A98;
 }
 #item-4:hover > a {
   background: rgba(173, 185, 211, 0.7);
 }

 #item-5 {
   background-color: #2AA9E0;
 }
 #item-5:hover > a {
   background: rgba(0, 132, 180, 0.7);
 }

 #item-6 {
   background-color: #EBF7F9;
 }
 #item-6:hover > a {
   background: rgba(230, 55, 52, 0.7);
 }

 .footer-icon {
   width: 50%;
   height: 50%;
   position: absolute;
   left: 50%;
   top: 50%;
   -o-transform: translate3d(-50%, -50%, 0) scale(1);
 	-ms-transform: translate3d(-50%, -50%, 0) scale(1);
 	-moz-transform: translate3d(-50%, -50%, 0) scale(1);
 	-webkit-transform: translate3d(-50%, -50%, 0) scale(1);
 	transform: translate3d(-50%, -50%, 0) scale(1);
  -webkit-transition: all 425ms ease;
    -moz-transition: all 425ms ease;
    transition: all 425ms ease;
 }

 .block {
   width: 33.33%;
   height: 304px;
   position: relative;
   float: left;
   -webkit-transition: width 1s ease;
 	-moz-transition: width 1s ease;
 	transition: width 1s ease;
   overflow: hidden;
 }

 .block a {
   display: block;
   position: absolute;
   left: 0;
   top: 0;
   height: 100%;
   width: 100%;
   text-align: center;
   background: transparent;
   z-index: 10;
 }

 .block a .item-content {
   color: white;
   width: 70%;
   position: absolute;
   left: 50%;
   top: 50%;
   text-transform: uppercase;
   -o-transform: translate3d(-50%, -50%, 0) scale(1);
 	-ms-transform: translate3d(-50%, -50%, 0) scale(1);
 	-moz-transform: translate3d(-50%, -50%, 0) scale(1);
 	-webkit-transform: translate3d(-50%, -50%, 0) scale(1);
 	transform: translate3d(-50%, -50%, 0) scale(1);
 }

 .block a:hover .item-content p, .block a:hover .item-content h2{
   -o-transform: translate(0, 0) scale(1);
 	-ms-transform: translate(0, 0) scale(1);
 	-moz-transform: translate(0, 0) scale(1);
 	-webkit-transform: translate(0, 0) scale(1);
 	transform: translate(0, 0) scale(1);
 	display:block;
 	-webkit-transition: all 425ms ease;
     -moz-transition: all 425ms ease;
     transition: all 425ms ease;
 }

 .block:hover .footer-icon {
   -o-transform: translate3d(-50%, -50%, 0) scale(1.5);
 	-ms-transform: translate3d(-50%, -50%, 0) scale(1.5);
 	-moz-transform: translate3d(-50%, -50%, 0) scale(1.5);
 	-webkit-transform: translate3d(-50%, -50%, 0) scale(1.5);
 	transform: translate3d(-50%, -50%, 0) scale(1.5);
 }

 @media screen and (max-width: 1300px) {
   .block {
     width: 50%;
   }
 }

 @media screen and (max-width: 1050px) {
   .block a .item-content h2 {
     border: 2px solid white;
     padding: 5%;
   }

   .block a:hover {
   	background: transparent;
   }
 }

 @media screen and (max-width: 750px) {
   .block {
     width: 100%;
     height: 250px;
   }
   .item-content h2 {
     font-size: 36px;
   }
 }

 @media screen and (max-width: 650px) {
   .block {
     height: 150px;
   }

 }
</style>
