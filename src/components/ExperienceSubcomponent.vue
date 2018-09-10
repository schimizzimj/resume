<template lang="html">

  <section class="experienceSubcomponent">
    <template v-if="orientation === 'left'">
      <div class="third float">
        <h2>{{role}}</h2>
        <h3>{{company}}</h3>
      </div>
      <div class="third float">
        <ul>
          <li v-for="bullet in text">{{bullet}}</li>
        </ul>
      </div>
      <div class="third float">
        <img :src="image">
      </div>
    </template>
    <template v-else-if="orientation === 'right'">
      <div class="third float">
        <img :src="image">
      </div>
      <div class="third float">
        <ul>
          <li v-for="bullet in text">{{bullet}}</li>
        </ul>
      </div>
      <div class="third float">
        <h2>{{role}}</h2>
        <h3>{{company}}</h3>
      </div>
    </template>
  </section>

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class ExperienceComponent extends Vue {
  @Prop() private role!: string;
  @Prop() private company!: string;
  @Prop() private text!: string;
  @Prop() private image!: string;
  @Prop() private orientation!: string;
}
</script>

<style scoped lang="scss">
  $height: 300px;
  .experienceSubcomponent {
    height: $height;
  }
  .float {
    float: left;
  }
  .third {
    width: calc(100%/3);
    height: $height;
  }
  h2 {
    font-weight: bold;
    font-size: 48px;
  }
  ul {
    list-style: none;
  }
  li {
    padding-bottom: 20px;
    font-size: 1.2em;
  }
</style>
