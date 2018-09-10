<template lang="html">

  <section id="education" class="education">
    <h1 class="section-title">Education</h1>
    <div class="third float">
      <h2>University of Notre Dame</h2>
    </div>
    <div class="third float">
      <h3>B.S. in Computer Science</h3>
      <h4>Relevant Coursework</h4>
      <ul>
        <li>Algorithms</li>
        <li>Data Structures</li>
        <li>Data Science</li>
        <li>Computer Networks</li>
        <li>Linear Algebra & Differential Equations</li>
        <li>Systems Programming</li>
        <li>Logic Design</li>
        <li>Discrete Mathematics</li>
        <li>Theory of Computing</li>
        <li>Computer Architecture</li>
        <li>Programming Paradigms</li>
        <li>Computer Graphics</li>
        <li>Web Applications</li>
        <li>Operating Systems</li>
      </ul>
    </div>
    <div class="third float">
      <img src="https://res.cloudinary.com/marcusschimizzi/image/upload/c_scale,h_300/v1536560208/nd_o31imv.png">
    </div>
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
export default class Education extends Vue {

}
</script>

<style scoped lang="scss">
  $height: 500px;
  .education {
    height: $height;
  }
  .float {
    float: left;
  }
  .third {
    width: calc(100%/3);
    height: $height;
    @media screen and (max-width: 600px) {
      width: 100%;
    }
  }
  h2 {
    font-weight: bold;
    font-size: 48px;
  }
  h3 {
    font-weight: bold;
    font-size: 36px;
  }
  h4 {
    font-size: 24px;
    color: lightgrey;
  }
  ul {
    list-style: none;
  }
  li {
    float: left;
    width: 15em;
    padding: 5px 0;
  }
</style>
