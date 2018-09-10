<template lang="html">

  <section id="skills" class="skills">
    <h1>Skills</h1>
    <div class="skill">
      <h3>C</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>C++</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>Java</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>Python</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>Angular</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>Vue</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>JavaScript</h3>
      <Stars :numberChecked="4"/>
    </div>
    <div class="skill">
      <h3>Node.js</h3>
      <Stars :numberChecked="3"/>
    </div>
    <div class="skill">
      <h3>React</h3>
      <Stars :numberChecked="3"/>
    </div>
    <div class="skill">
      <h3>Ionic</h3>
      <Stars :numberChecked="3"/>
    </div>
    <div class="skill">
      <h3>CSS</h3>
      <Stars :numberChecked="5"/>
    </div>
    <div class="skill">
      <h3>HTML</h3>
      <Stars :numberChecked="5"/>
    </div>
    <div class="skill">
      <h3>MATLAB</h3>
      <Stars :numberChecked="2"/>
    </div>
    <div class="skill">
      <h3>WebGL</h3>
      <Stars :numberChecked="2"/>
    </div>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import Stars from '@/components/Stars.vue';

@Component({
  components: {
    Stars,
  },
})
export default class Skills extends Vue {

}
</script>

<style scoped lang="scss">
  .skills {
    width: 60%;
    margin: 0 auto;
    min-height: 100px;
  }
  .skills:after {
    content: "";
    display: table;
    clear: both;
  }
  .skill:hover {
    h3 {
      font-size: 2.5em;
    }
  }
  .skill {
    width: 20%;
    float: left;
    min-height: 150px;
    position: relative;
    @media screen and (max-width: 1300px) {
      width: calc(100%/3);
    }
    @media screen and (max-width: 870px) {
      width: calc(100%/2);
    }
    @media screen and (max-width: 580px) {
      width: 100%;
    }
  }
  h3 {
    font-size: 2em;
    margin: 0;
    -webkit-transition: all 425ms ease;
    -moz-transition: all 425ms ease;
    transition: all 425ms ease;
  }
</style>
