<template>
  <div class="home">
    <Header msg="Marcus J. Schimizzi"/>
    <!-- <Contents/> -->
    <!-- <AboutMe/> -->
    <!-- <Education/> -->
    <Projects/>
    <Experience/>
    <Skills/>
    <SocialMedia/>
    <Footer/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Header from '@/components/Header.vue'; // @ is an alias to /src
import Contents from '@/components/Contents.vue';
import AboutMe from '@/components/AboutMe.vue';
import Education from '@/components/Education.vue';
import Projects from '@/components/Projects.vue';
import Experience from '@/components/Experience.vue';
import Skills from '@/components/Skills.vue';
import SocialMedia from '@/components/SocialMedia.vue';
import Footer from '@/components/Footer.vue';




@Component({
  components: {
    Header,
    Contents,
    AboutMe,
    Education,
    Projects,
    Experience,
    Skills,
    SocialMedia,
    Footer,
  },
})
export default class Home extends Vue {}
</script>
