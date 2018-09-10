<template lang="html">

  <section id="experience" class="experience">
    <h1 class="section-title">Experience</h1>
    <ExperienceComponent
      role="Software Developer Intern"
      company="Ford Motor Company"
      v-bind:text="['Worked on development of two web applications using technology stack of Java, Spring Boot, and Angular',
      'Used Agile, Continuous Integration/Continuous Delivery, Test-Driven Development, and Mobbing/Pairing development practices',
      'Won Ford’s Intern Innovation Challenge for most unique idea']"
      image="http://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,h_181/v1536547380/580b585b2edbce24c47b2c67_hpiuik.png"
      orientation="right"
    />
    <ExperienceComponent
      role="Freelance Web Developer"
      company="Self"
      v-bind:text="['Used frontend frameworks (Angular & Vue) to update/develop websites & applications',
      'Developed responsive mobile app for client using Ionic framework',
      'Worked with WordPress themes & plugins to provide customizations for clients’ websites']"
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,h_250/v1536554701/pexels-photo-270404_dgsbtx.jpg"
      orientation="left"
    />
    <ExperienceComponent

      role="Computer Science Tutor"
      company="University of Notre Dame"
      v-bind:text="['Leads group discussion sessions to facilitate students\’ understanding of course content',
      'Offers individual tutoring to provide additional help to students in need']"
      image="https://res.cloudinary.com/marcusschimizzi/image/upload/c_crop,h_500,w_800/c_scale,h_300/v1536554878/ntgr89zdyyi1tijv8rlx_ralfp0.png"
      orientation="right"
    />
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import ExperienceComponent from '@/components/ExperienceComponent.vue';

@Component({
  components: {
    ExperienceComponent,
  },
})
export default class Experience extends Vue {
}
</script>

<style scoped lang="scss">
  .experience {

  }
</style>
