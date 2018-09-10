<template lang="html">

  <section id="projects" class="projects">
    <h1 class="section-title">Projects</h1>
    <Subcomponent
      title="Sentiment Analysis Web Application"
      text="At a hackathon hosted by Credit Suisse at their office in New York,
      my team developed a web application that performs sentiment analysis on a
      company. The project relies on node.js and python (for web scraping).
      Once a user inputs a stock ticker of their chosen company on the web app,
      it uses API requests (causes it to be quite slow) to find recent articles
      about the company. It then tallies occurrences of well-known positive and
      negative words to compute a ratio indicating recent sentiment on the company."
      image="http://res.cloudinary.com/marcusschimizzi/image/upload/c_crop,h_600,w_800,x_260,y_200/c_scale,h_300,w_400/v1518625368/10_dvdlu8.png"
      orientation="right"
    />
    <Subcomponent
      title="ND Adventure"
      text="For the final project in my Data Structures course, I worked with a
      team of students to develop an RPG/adventure based around the Notre Dame
      Campus. The player takes on the role of a Notre Dame computer science
      student and has to complete tasks for professors around campus. The game
      is built using python and the pygame library."
      image="http://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,w_400/v1504123162/871d0e5d3a57b37aa28a5b7cf867fcec_cirncl.png"
      orientation="left"
    />
    <Subcomponent
      title="Frogger Clone"
      text="Final project for my Fundamentals of Computing course during my
      sophomore year at the University of Notre Dame. I created a Frogger clone
      using C++ and a custom graphics library built by our faculty from the X11
      library. The game has a very simple menu that launches into gameplay
      closely replicating the original game. The game keeps going until the
      player loses all three lives or they make it to the end enough times to
      fill all of the lilypads."
      image="http://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,h_300,w_400/v1504125705/frogger_be25kj.jpg"
      orientation="right"
    />
    <Subcomponent
      title="GE Align Lighting Project"
      text="For the final project for my Introduction to Engineering course, I
      worked in a team to use an RGB lightbulb to replicate GE's AM and PM Align
      bulbs. We worked in association with GE and used MATLAB in order to
      program our bulb to match the Align ones provided to us. We then gave a
      demonstration of our project based on a final report we compiled."
      image="http://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,w_400/v1504125703/ge_t85ghe.jpg"
      orientation="left"
    />
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import Subcomponent from '@/components/Subcomponent.vue';

@Component({
  components: {
    Subcomponent,
  },
})
export default class Projects extends Vue {
}
</script>

<style scoped lang="scss">
  .projects {

  }
</style>
