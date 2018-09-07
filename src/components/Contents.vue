<template lang="html">

  <section class="contents">
    <div class="left half float">
      <div class="text-wrapper">
        <h1>Hello, I'm Marcus Schimizzi. I'm a passionate, optimistic person who loves
        to create more than anything.</h1>
      </div>
    </div>
    <div class="middle-spacer"></div>
    <div class="right half float">
      <h2>Skip to section</h2>
      <ul>
        <li><a href="#about-me">About Me</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#social">Social Media</a></li>
      </ul>
    </div>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Contents extends Vue {
}
</script>

<style scoped lang="scss">
  .contents {
    width: 80%;
    margin: 0 auto;
    height: 200px;
  }
  .half {
    width: calc(99%/2);
  }
  .middle-spacer {
    float: left;
    width: .1%;
    background-color: lightgrey;
    margin-left: calc(2%/5);
    margin-right: calc(2%/5);
    height: 200px;
  }
  .left {
    text-align: right;
  }
  .right {
    text-align: left;
  }
  .float {
    float: left;
  }
  .text-wrapper {
    width: 70%;
    padding-left: 30%;
  }
</style>
